# Comparing `tmp/faker_cli-0.2.0.tar.gz` & `tmp/faker_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_cli-0.2.0.tar", max compression
+gzip compressed data, was "faker_cli-0.3.0.tar", max compression
```

## Comparing `faker_cli-0.2.0.tar` & `faker_cli-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-08 20:43:16.777604 faker_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     3217 2023-06-08 20:43:16.777604 faker_cli-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/__init__.py
--rw-r--r--   0        0        0     3157 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/cli.py
--rw-r--r--   0        0        0    27694 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/templates.py
--rw-r--r--   0        0        0     1517 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/writer.py
--rw-r--r--   0        0        0      569 2023-06-08 20:43:42.865893 faker_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 faker_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-10 17:36:11.579005 faker_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3364 2023-06-10 17:36:11.579005 faker_cli-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 17:36:11.579005 faker_cli-0.3.0/faker_cli/__init__.py
+-rw-r--r--   0        0        0     3267 2023-06-10 17:36:11.579005 faker_cli-0.3.0/faker_cli/cli.py
+-rw-r--r--   0        0        0    27694 2023-06-10 17:36:11.579005 faker_cli-0.3.0/faker_cli/templates.py
+-rw-r--r--   0        0        0     1674 2023-06-10 17:36:11.579005 faker_cli-0.3.0/faker_cli/writer.py
+-rw-r--r--   0        0        0      590 2023-06-10 17:36:31.999259 faker_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3954 1970-01-01 00:00:00.000000 faker_cli-0.3.0/PKG-INFO
```

### Comparing `faker_cli-0.2.0/LICENSE` & `faker_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_cli-0.2.0/README.md` & `faker_cli-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,23 @@
 
 _youcanevenwritestraighttos3_ 🤭
 
 ```bash
 fake -n 10 pyint,user_name,date_this_year -f parquet -o s3://YOUR_BUCKET/data/sample.parquet
 ```
 
+### Delta Lake
+
+Data can be exported as a delta lake table.  
+
+```bash
+fake -n 10 pyint,user_name,date_this_year -f deltalake -o sample_data
+```
+
+
 ## Templates
 
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
 fake -t s3access -n 10
 ```
```

### Comparing `faker_cli-0.2.0/faker_cli/cli.py` & `faker_cli-0.3.0/faker_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from faker import Faker
 import click
 import sys
 from faker_cli.templates import CloudFrontWriter, S3AccessLogs, S3AccessWriter, CloudTrailLogs, CloudFrontLogs
 
-from faker_cli.writer import CSVWriter, JSONWriter, ParquetWriter
+from faker_cli.writer import CSVWriter, JSONWriter, ParquetWriter, DeltaLakeWriter
 from typing import List
 
 def infer_column_names(col_names, col_types: str) -> List[str]:
     """
     Infer column names from column types
     """
     # For now, nothing special - but eventually we need to parse things out
@@ -16,28 +16,29 @@
     
     return col_types.split(",")
 
 KLAS_MAPPER = {
     "csv": CSVWriter,
     "json": JSONWriter,
     "parquet": ParquetWriter,
+    "deltalake": DeltaLakeWriter
 }
 
 TEMPLATE_MAPPER = {
     "s3access": [S3AccessWriter, "s3_access_log"],
     "cloudfront": [CloudFrontWriter, "cloudfront_log"],
 }
 
 fake = Faker()
 fake.add_provider(S3AccessLogs)
 fake.add_provider(CloudFrontLogs)
 
 @click.command()
 @click.option("--num-rows", "-n", default=1, help="Number of rows")
-@click.option("--format", "-f", type=click.Choice(["csv", "json", "parquet"]), default="csv", help="Format of the output")
+@click.option("--format", "-f", type=click.Choice(["csv", "json", "parquet", "deltalake"]), default="csv", help="Format of the output")
 @click.option("--output", "-o", type=click.Path(writable=True))
 @click.option("--columns", "-c", help="Column names", default=None, required=False)
 @click.option("--template", "-t", help="Template to use", type=click.Choice(["s3access", "cloudfront"]), default=None)
 @click.argument("column_types", required=False)
 def main(num_rows, format, output, columns, template, column_types):
     """
     Generate fake data, easily.
@@ -53,17 +54,17 @@
         click.echo(ctx.get_help())
         ctx.exit()
         raise click.BadArgumentUsage(
             "either --template or a list of Faker property names must be provided."
         )
 
     # Parquet output requires a filename
-    if format == "parquet" and output is None:
-        raise click.BadArgumentUsage("parquet format requires --output/-o filename parameter.")
-    if output is not None and format != "parquet":
+    if format in ["parquet", "deltalake"] and output is None:
+        raise click.BadArgumentUsage("parquet | deltalake formats requires --output/-o filename parameter.")
+    if output is not None and format not in ["parquet", "deltalake"]:
         raise click.BadArgumentUsage("output files not supported for csv/json yet.")
     
     # If the user provides a template, we use that provider and writer and exit.
     # We assume a template has a custom writer that may be different than CSV or JSON
     if template:
         writer = TEMPLATE_MAPPER[template][0](sys.stdout, None)
         log_entry = TEMPLATE_MAPPER[template][1]
```

### Comparing `faker_cli-0.2.0/faker_cli/templates.py` & `faker_cli-0.3.0/faker_cli/templates.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.2.0/faker_cli/writer.py` & `faker_cli-0.3.0/faker_cli/writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import csv
 import json
 from typing import Optional
 import pyarrow as pa
 import pyarrow.parquet as pq
+import deltalake
 
 
 class Writer:
     def __init__(self, output, headers, filename: Optional[str] = None):
         self.output = output
         self.headers = headers
         self.writer = None
@@ -52,7 +53,12 @@
         if self.table is None:
             self.table = table
         else:
             self.table = pa.concat_tables([self.table, table])
 
     def close(self):
         pq.write_table(self.table, self.filename)
+
+
+class DeltaLakeWriter(ParquetWriter):
+    def close(self):
+        deltalake.write_deltalake(table_or_uri=self.filename, data=self.table)
```

### Comparing `faker_cli-0.2.0/pyproject.toml` & `faker_cli-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "faker-cli"
-version = "v0.2.0"
+version = "v0.3.0"
 description = "Command-line fake data generator"
 authors = ["Damon P. Cortesi <d.lifehacker@gmail.com>"]
 readme = "README.md"
 packages = [{include = "faker_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 faker = "^18.9.0"
 click = "^8.1.3"
 pyarrow = "^12.0.0"
+deltalake = "^0.9.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `faker_cli-0.2.0/PKG-INFO` & `faker_cli-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: faker-cli
-Version: 0.2.0
+Version: 0.3.0
 Summary: Command-line fake data generator
 Author: Damon P. Cortesi
 Author-email: d.lifehacker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: deltalake (>=0.9.0,<0.10.0)
 Requires-Dist: faker (>=18.9.0,<19.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Description-Content-Type: text/markdown
 
 # Faker CLI
 
 Faker is an awesome Python library, but I often just want a simple command I can run to generate data in a variety of formats.
@@ -96,14 +97,23 @@
 
 _youcanevenwritestraighttos3_ 🤭
 
 ```bash
 fake -n 10 pyint,user_name,date_this_year -f parquet -o s3://YOUR_BUCKET/data/sample.parquet
 ```
 
+### Delta Lake
+
+Data can be exported as a delta lake table.  
+
+```bash
+fake -n 10 pyint,user_name,date_this_year -f deltalake -o sample_data
+```
+
+
 ## Templates
 
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
 fake -t s3access -n 10
 ```
```


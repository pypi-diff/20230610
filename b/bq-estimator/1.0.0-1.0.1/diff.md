# Comparing `tmp/bq_estimator-1.0.0.tar.gz` & `tmp/bq_estimator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bq_estimator-1.0.0.tar", last modified: Fri Mar 31 02:35:17 2023, max compression
+gzip compressed data, was "bq_estimator-1.0.1.tar", last modified: Sat Jun 10 02:38:33 2023, max compression
```

## Comparing `bq_estimator-1.0.0.tar` & `bq_estimator-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jclemons  (1000) jclemons  (1000)        0 2023-03-31 02:35:17.943219 bq_estimator-1.0.0/
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     1073 2023-03-22 00:39:30.000000 bq_estimator-1.0.0/LICENSE
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     1144 2023-03-31 02:35:17.943219 bq_estimator-1.0.0/PKG-INFO
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      676 2023-03-31 02:34:39.000000 bq_estimator-1.0.0/README.md
-drwxrwxr-x   0 jclemons  (1000) jclemons  (1000)        0 2023-03-31 02:35:17.943219 bq_estimator-1.0.0/bq_estimator.egg-info/
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     1144 2023-03-31 02:35:17.000000 bq_estimator-1.0.0/bq_estimator.egg-info/PKG-INFO
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      270 2023-03-31 02:35:17.000000 bq_estimator-1.0.0/bq_estimator.egg-info/SOURCES.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)        1 2023-03-31 02:35:17.000000 bq_estimator-1.0.0/bq_estimator.egg-info/dependency_links.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       51 2023-03-31 02:35:17.000000 bq_estimator-1.0.0/bq_estimator.egg-info/entry_points.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       29 2023-03-31 02:35:17.000000 bq_estimator-1.0.0/bq_estimator.egg-info/requires.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       13 2023-03-31 02:35:17.000000 bq_estimator-1.0.0/bq_estimator.egg-info/top_level.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     2590 2023-03-31 02:25:50.000000 bq_estimator-1.0.0/bq_estimator.py
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      689 2023-03-31 02:35:17.947219 bq_estimator-1.0.0/setup.cfg
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       74 2023-03-23 01:49:28.000000 bq_estimator-1.0.0/setup.py
+drwxrwxr-x   0 jclemons  (1000) jclemons  (1000)        0 2023-06-10 02:38:33.150764 bq_estimator-1.0.1/
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     1073 2023-03-22 00:39:30.000000 bq_estimator-1.0.1/LICENSE
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     1167 2023-06-10 02:38:33.150764 bq_estimator-1.0.1/PKG-INFO
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      699 2023-06-10 02:36:17.000000 bq_estimator-1.0.1/README.md
+drwxrwxr-x   0 jclemons  (1000) jclemons  (1000)        0 2023-06-10 02:38:33.150764 bq_estimator-1.0.1/bq_estimator.egg-info/
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     1167 2023-06-10 02:38:33.000000 bq_estimator-1.0.1/bq_estimator.egg-info/PKG-INFO
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      270 2023-06-10 02:38:33.000000 bq_estimator-1.0.1/bq_estimator.egg-info/SOURCES.txt
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)        1 2023-06-10 02:38:33.000000 bq_estimator-1.0.1/bq_estimator.egg-info/dependency_links.txt
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       51 2023-06-10 02:38:33.000000 bq_estimator-1.0.1/bq_estimator.egg-info/entry_points.txt
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       45 2023-06-10 02:38:33.000000 bq_estimator-1.0.1/bq_estimator.egg-info/requires.txt
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       13 2023-06-10 02:38:33.000000 bq_estimator-1.0.1/bq_estimator.egg-info/top_level.txt
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     3355 2023-06-10 02:36:17.000000 bq_estimator-1.0.1/bq_estimator.py
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      706 2023-06-10 02:38:33.150764 bq_estimator-1.0.1/setup.cfg
+-rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       74 2023-03-23 01:49:28.000000 bq_estimator-1.0.1/setup.py
```

### Comparing `bq_estimator-1.0.0/LICENSE` & `bq_estimator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bq_estimator-1.0.0/PKG-INFO` & `bq_estimator-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq_estimator
-Version: 1.0.0
+Version: 1.0.1
 Summary: estimate BigQuery usage of sql queries
 Home-page: https://github.com/j-clemons/bq-estimator
 Author: Jonathan Clemons
 Author-email: j-clemons@tuta.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,12 +29,13 @@
 Ready to execute SQL queries.
 
 `bq-estimator query.sql [query2.sql query3.sql …]`
 
 ## Options
 ## --dbt
 
-***An installation of dbt-bigquery is required for using this functionality.***
-
 Takes any model selection command that is compatible with dbt
 
 `bq-estimator --dbt [dbt model selection]`
+
+## --verbose -v
+If errors are present the error details from BigQuery will be printed to the terminal.
```

### Comparing `bq_estimator-1.0.0/README.md` & `bq_estimator-1.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 Ready to execute SQL queries.
 
 `bq-estimator query.sql [query2.sql query3.sql …]`
 
 ## Options
 ## --dbt
 
-***An installation of dbt-bigquery is required for using this functionality.***
-
 Takes any model selection command that is compatible with dbt
 
 `bq-estimator --dbt [dbt model selection]`
+
+## --verbose -v
+If errors are present the error details from BigQuery will be printed to the terminal.
```

### Comparing `bq_estimator-1.0.0/bq_estimator.egg-info/PKG-INFO` & `bq_estimator-1.0.1/bq_estimator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq-estimator
-Version: 1.0.0
+Version: 1.0.1
 Summary: estimate BigQuery usage of sql queries
 Home-page: https://github.com/j-clemons/bq-estimator
 Author: Jonathan Clemons
 Author-email: j-clemons@tuta.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,12 +29,13 @@
 Ready to execute SQL queries.
 
 `bq-estimator query.sql [query2.sql query3.sql …]`
 
 ## Options
 ## --dbt
 
-***An installation of dbt-bigquery is required for using this functionality.***
-
 Takes any model selection command that is compatible with dbt
 
 `bq-estimator --dbt [dbt model selection]`
+
+## --verbose -v
+If errors are present the error details from BigQuery will be printed to the terminal.
```

### Comparing `bq_estimator-1.0.0/bq_estimator.py` & `bq_estimator-1.0.1/bq_estimator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,126 @@
 from __future__ import annotations
 
 import argparse
+import sys
+from io import StringIO
 from re import findall
-from subprocess import run
 from typing import Sequence
 
+from dbt.cli.main import dbtRunner
+from dbt.cli.main import dbtRunnerResult
+from google.api_core.exceptions import BadRequest
 from google.cloud import bigquery
 
 
-def bq_estimate(query_text: str) -> int:
+RED = '\033[91m'
+NORMAL = '\033[m'
+
+
+def bq_estimate(query_text: str) -> tuple[float, str]:
     client = bigquery.Client()
 
     job_config = bigquery.QueryJobConfig(dry_run=True, use_query_cache=False)
+    try:
+        query_job = client.query(query_text, job_config=job_config)
+    except BadRequest as e:
+        return -1, e
 
-    query_job = client.query(query_text, job_config=job_config)
+    return query_job.total_bytes_processed, ''
 
-    return query_job.total_bytes_processed
+
+class NullIO(StringIO):
+    def write(self, txt):
+        pass
 
 
 def dbt_process(dbt_selection: str) -> Sequence[str]:
-    list_models = run(
-        f'dbt ls --select {dbt_selection} --resource-type model',
-        shell=True,
-        capture_output=True,
-        text=True,
-    )
+    dbt = dbtRunner()
+
+    ls_args = ['ls', '--select', dbt_selection, '--resource-type', 'model']
+
+    sys.stdout = NullIO()
+    res: dbtRunnerResult = dbt.invoke(ls_args)
+
+    if res.success is False:
+        return []
 
     result = []
-    for m in list_models.stdout.split('\n'):
+    for m in res.result:
         model = findall(r'^[a-zA-Z0-9_-]+(?:\.[a-zA-Z0-9_-]+)+', m)
         if model != []:
             ele = model[0].split('.')
             result.append(
                 f'target/compiled/{ele[0]}/models/'
                 f'{"/".join(ele[1:])}.sql',
             )
 
         if 'No nodes selected' in m:
             return []
 
-    run(f'dbt compile -s {dbt_selection}', shell=True, capture_output=True)
+    dbt.invoke(['compile', '-s', dbt_selection])
+    sys.stdout = sys.__stdout__
 
     return result
 
 
 def format_data(raw_bytes: float) -> str:
-    if raw_bytes / 2**10 < 1000:
+    if raw_bytes == -1.0:
+        return 'ERROR'
+    elif raw_bytes / 2**10 < 1000:
         return f'{raw_bytes/2**10:.2f} KB'
     elif raw_bytes / 2**20 < 1000:
         return f'{raw_bytes/2**20:.2f} MB'
     elif raw_bytes / 2**30 < 1000:
         return f'{raw_bytes/2**30:.2f} GB'
     else:
         return f'{raw_bytes/2**40:.2f} TB'
 
 
 def print_result(string: str, num: str, char_width: int = 60) -> None:
     dash_count = char_width - len(string) - len(num) \
         if len(string) + len(num) < char_width else 1
-    print(f'{string} {dash_count*"-"} {num}')
+    if num == 'ERROR':
+        print(f'{RED}{string} {dash_count*"-"} {num}{NORMAL}')
+    else:
+        print(f'{string} {dash_count*"-"} {num}')
 
 
-def process_files(filenames: Sequence[str]) -> float:
+def process_files(filenames: Sequence[str], verbose: bool) -> float:
     total_est = 0.0
     for file in filenames:
         f_name = file.split('/')[-1]
         with open(file) as f:
-            est = bq_estimate(f.read())
-            print_result(f_name, format_data(est))
+            est, txt = bq_estimate(f.read())
+            if verbose:
+                print_result(f_name, format_data(est))
+                print(txt)
+            else:
+                print_result(f_name, format_data(est))
+
             total_est += est
 
     print('Total Estimated Usage: ' + format_data(total_est))
     return total_est
 
 
 def main(argv: Sequence[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('filenames', nargs='*')
     parser.add_argument('--dbt', dest='dbt', nargs='*')
+    parser.add_argument('--verbose', '-v', action='store_true', default=False)
 
     args = parser.parse_args(argv)
 
     if args.dbt is not None:
         dbt_files: list[str] = []
         for darg in args.dbt:
             dbt_files.extend(dbt_process(darg))
-        process_files(dbt_files)
+        process_files(dbt_files, args.verbose)
     else:
-        process_files(args.filenames)
+        process_files(args.filenames, args.verbose)
 
     return 0
 
 
 if __name__ == '__main__':
     raise SystemExit(main())
```


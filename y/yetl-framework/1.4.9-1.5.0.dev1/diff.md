# Comparing `tmp/yetl-framework-1.4.9.tar.gz` & `tmp/yetl-framework-1.5.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.4.9.tar", last modified: Sun Jun  4 12:05:30 2023, max compression
+gzip compressed data, was "yetl-framework-1.5.0.dev1.tar", last modified: Sat Jun 10 19:35:50 2023, max compression
```

## Comparing `yetl-framework-1.4.9.tar` & `yetl-framework-1.5.0.dev1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.286295 yetl-framework-1.4.9/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-04 12:05:30.286295 yetl-framework-1.4.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-04 12:05:30.286295 yetl-framework-1.4.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.278294 yetl-framework-1.4.9/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.278294 yetl-framework-1.4.9/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.278294 yetl-framework-1.4.9/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16007 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.282295 yetl-framework-1.4.9/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16494 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.282295 yetl-framework-1.4.9/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3991 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.282295 yetl-framework-1.4.9/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-04 12:04:29.000000 yetl-framework-1.4.9/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 12:05:30.286295 yetl-framework-1.4.9/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-04 12:05:30.000000 yetl-framework-1.4.9/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-04 12:05:30.000000 yetl-framework-1.4.9/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-04 12:05:30.000000 yetl-framework-1.4.9/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-04 12:05:30.000000 yetl-framework-1.4.9/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-04 12:05:30.000000 yetl-framework-1.4.9/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-04 12:05:30.000000 yetl-framework-1.4.9/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16007 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3143 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9236 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4094 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.4.9/PKG-INFO` & `yetl-framework-1.5.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.9
+Version: 1.5.0.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.9/README.md` & `yetl-framework-1.5.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/setup.py` & `yetl-framework-1.5.0.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.4.9",
+    version="1.5.0.dev1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.4.9/yetl/__main__.py` & `yetl-framework-1.5.0.dev1/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/cli/_init.py` & `yetl-framework-1.5.0.dev1/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/__init__.py` & `yetl-framework-1.5.0.dev1/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/_config.py` & `yetl-framework-1.5.0.dev1/yetl/config/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,23 @@
         return tables
 
     def get_table_mapping(
         self,
         stage: StageType,
         table: str = _INDEX_WILDCARD,
         database: str = _INDEX_WILDCARD,
+        create_database: bool = True,
         create_table: bool = True,
     ):
         table_mapping = self.tables.get_table_mapping(
-            stage=stage, table=table, database=database, create_table=create_table
+            stage=stage,
+            table=table,
+            database=database,
+            create_database=create_database,
+            create_table=create_table,
         )
 
         return table_mapping
 
     def set_checkpoint(
         self,
         source: Table,
```

### Comparing `yetl-framework-1.4.9/yetl/config/_decorators.py` & `yetl-framework-1.5.0.dev1/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/_logging_config.py` & `yetl-framework-1.5.0.dev1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/_project.py` & `yetl-framework-1.5.0.dev1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/_spark_context.py` & `yetl-framework-1.5.0.dev1/yetl/config/_spark_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,22 @@
 
 _logger = logging.getLogger(__name__)
 
 
 def get_spark_context(project: str, config: dict = None):
     if is_databricks():
         _logger.debug("Getting databricks spark context")
-        from databricks.sdk.runtime import spark
+        try:
+            from databricks.sdk.runtime import spark
+
+            return spark
+        except Exception:
+            _logger.info("cannot create spark context, spark not found.")
+            return None
 
-        return spark
     else:
         _logger.debug("Getting local spark context")
 
         if config is None:
             config = {
                 "spark.master": "local",
                 "spark.databricks.delta.allowArbitraryProperties.enabled": True,
```

### Comparing `yetl-framework-1.4.9/yetl/config/_tables.py` & `yetl-framework-1.5.0.dev1/yetl/config/_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 
     def lookup_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         first_match: bool = True,
+        create_database: bool = False,
         create_table: bool = False,
         **kwargs,
     ):
         index = Tables.get_index(stage, database, table)
         matches = fnmatch.filter(list(self.tables_index.keys()), index)
 
         if not matches:
@@ -187,51 +188,61 @@
             }
 
         if first_match:
             matches = matches[0]
             table = tables_index[matches]
             msg_tables = f"{table.database}.{table.table}"
             self._logger.info(f"Matched tables: {msg_tables}")
+            if create_database:
+                table.create_database()
             if create_table:
                 table.create_table()
             return table
         else:
             tables = [tables_index[i] for i in matches]
             msg_tables = "\n".join([f"{t.database}.{t.table}" for t in tables])
             self._logger.info(f"Matched tables: {msg_tables}")
-            if create_table:
+            db = ""
+            if create_table or create_database:
                 for t in tables:
-                    t.create_table()
+                    if create_database and db != t.database:
+                        db = t.database
+                        t.create_database()
+                    if create_table:
+                        t.create_table()
             return tables
 
     def get_table_mapping(
         self,
         stage: StageType,
         table=_INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
+        create_database: bool = True,
         create_table: bool = True,
     ):
         destination = self.lookup_table(
             stage=stage,
             database=database,
             table=table,
             first_match=True,
+            create_database=create_database,
             create_table=create_table,
         )
         source = {}
 
         tables = []
         try:
             for index in destination.depends_on:
                 do_stage, do_database, do_table = Tables.parse_index(index)
                 tables = tables + self.lookup_table(
                     stage=do_stage,
                     table=do_table,
                     database=do_database,
                     first_match=False,
+                    create_database=create_database,
                     create_table=create_table,
                 )
         except Exception as e:
             raise Exception(f"Error looking up dependencies for table {table}") from e
 
         for tbl in tables:
             source[tbl.table] = tbl
```

### Comparing `yetl-framework-1.4.9/yetl/config/_timeslice.py` & `yetl-framework-1.5.0.dev1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/_utils.py` & `yetl-framework-1.5.0.dev1/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/deltalake.py` & `yetl-framework-1.5.0.dev1/yetl/config/deltalake.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 from pyspark.sql import DataFrame
 import logging
 from pyspark.sql.types import StructType, StructField
 import jinja2
 from typing import List, Union, Dict
 from ._spark_context import get_spark_context
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, PrivateAttr
 from typing import Any
 from ._project import Project
 from pyspark.sql import SparkSession
 import re
 
-_logger = logging.getLogger(__name__)
-
 
 class DeltaLakeFn(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
+        self._logger = logging.getLogger(self.__class__.__name__)
         self.spark = get_spark_context(self.project.name, self.project.spark.config)
 
+    _logger: Any = PrivateAttr(default=None)
     project: Project = Field(...)
     spark: SparkSession = Field(default=None)
 
     @classmethod
     def to_regex_search_pattern(cls, py_format: str):
         """Convert python format codes to regex search pattern
            these can be used to intelligently strip timeslice from file or name
@@ -205,24 +205,25 @@
             p = f"`{k}` in ({','.join(v)})"
             predicates.append(p)
 
         predicate = " and ".join(predicates)
 
         return predicate
 
-    def table_exists(self, database: str, table: str):
-        table_exists = (
+    def table_exists(self, database: str, table: str, catalog: str = None):
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        _table_exists = (
             self.spark.sql(f"SHOW TABLES in {database};")
             .where(f"tableName='{table}' AND !isTemporary")
             .count()
             == 1
         )
         # Not whitelist on databricks.
         # table_exists = self.spark.catalog.tableExists(f"`{database}`.`{table}`")
-        return table_exists
+        return _table_exists
 
     def get_delta_properties_sql(self, delta_properties: Dict[str, Union[str, bool]]):
         sql_properties = [
             f"{k.lower()} = {v.lower()}" for k, v in delta_properties.items()
         ]
         sql_properties = ", ".join(sql_properties)
         return sql_properties
@@ -230,59 +231,73 @@
     def create_table(
         self,
         database: str,
         table: str,
         path: str = None,
         delta_properties: List[str] = None,
         sql: str = None,
+        catalog: str = None,
     ):
-        _logger.debug(f"Creating table if not exists {database}.{table} at {path}")
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        table = f"`{table}`"
+        self._logger.info(f"Creating table if not exists {database}.{table} at {path}")
         if not sql:
-            sql = f"CREATE TABLE IF NOT EXISTS `{database}`.`{table}`"
+            sql = f"CREATE TABLE IF NOT EXISTS {database}.{table}"
 
             # add in the delta properties if there are any
             sql_properties = ""
             if delta_properties:
                 sql_properties = self.get_delta_properties_sql(delta_properties)
                 sql_properties = f"TBLPROPERTIES({sql_properties})"
 
             sql_path = ""
             if path:
                 sql_path = f"USING DELTA LOCATION '{path}'"
 
                 sql = f"{sql}\n{sql_path}\n{sql_properties};"
 
-        _logger.info(f"{sql}")
+        self._logger.info(f"{sql}")
         self.spark.sql(sql)
 
         return sql
 
-    def create_database(self, database: str):
-        _logger.debug(f"Creating database if not exists `{database}`")
+    def create_database(self, database: str, catalog: str = None):
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        self._logger.debug(f"Creating database if not exists {database}")
         sql = f"CREATE DATABASE IF NOT EXISTS {database}"
-        _logger.debug(sql)
+        self._logger.debug(sql)
         self.spark.sql(sql)
         return sql
 
-    def alter_table_drop_constraint(self, database: str, table: str, name: str):
-        return f"ALTER TABLE `{database}`.`{table}` DROP CONSTRAINT {name};"
+    def alter_table_drop_constraint(
+        self, database: str, table: str, name: str, catalog: str = None
+    ):
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        return f"ALTER TABLE {database}.`{table}` DROP CONSTRAINT {name};"
 
     def alter_table_add_constraint(
-        self, database: str, table: str, name: str, constraint: str
+        self, database: str, table: str, name: str, constraint: str, catalog: str = None
     ):
-        return f"ALTER TABLE `{database}`.`{table}` ADD CONSTRAINT {name} CHECK ({constraint});"
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        return f"ALTER TABLE {database}.`{table}` ADD CONSTRAINT {name} CHECK ({constraint});"
 
-    def alter_table_set_tblproperties(self, database: str, table: str, properties: str):
-        return f"ALTER TABLE `{database}`.`{table}` SET TBLPROPERTIES ({properties});"
+    def alter_table_set_tblproperties(
+        self, database: str, table: str, properties: str, catalog: str = None
+    ):
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        return f"ALTER TABLE {database}.`{table}` SET TBLPROPERTIES ({properties});"
 
-    def get_table_properties(self, database: str, table: str):
-        _logger.debug(f"getting existing table properties for table {database}.{table}")
+    def get_table_properties(self, database: str, table: str, catalog: str = None):
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        self._logger.debug(
+            f"getting existing table properties for table {database}.`{table}`"
+        )
 
         df: DataFrame = self.spark.sql(
-            f"SHOW TBLPROPERTIES `{database}`.`{table}`"
+            f"SHOW TBLPROPERTIES {database}.`{table}`"
         ).collect()
         tbl_properties = {
             c.asDict()["key"]: c.asDict()["value"]
             for c in df
             if not c["key"].startswith("delta.constraints")
         }
         tbl_constraints = {
@@ -294,41 +309,48 @@
         properties = {
             f"{database}.{table}": {
                 "constraints": tbl_constraints,
                 "properties": tbl_properties,
             }
         }
         msg = json.dumps(properties, indent=4, default=str)
-        _logger.debug(msg)
+        self._logger.debug(msg)
         return properties
 
     def optimize(
-        self, database: str, table: str, partition_values: dict, zorder_by: list = []
+        self,
+        database: str,
+        table: str,
+        partition_values: dict,
+        zorder_by: list = [],
+        catalog: str = None,
     ):
-        sql = f"OPTIMIZE `{database}`.`{table}`"
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        sql = f"OPTIMIZE {database}.`{table}`"
 
         if partition_values:
             predicate = self.get_partition_predicate(partition_values)
             predicate = f" WHERE {predicate}"
             sql = f"{sql}{predicate}"
 
         if zorder_by:
             sql_zorderby = ",".join([f"`{z}`" for z in zorder_by])
             sql = f"{sql} ZORDER BY ({sql_zorderby})"
 
-        _logger.debug(f"optimizing table {database}.{table}\n{sql}")
+        self._logger.info(f"optimizing table {database}.{table}\n{sql}")
         self.spark.sql(sql)
 
-    def get_table_details(self, database: str, table: str):
-        _logger.debug(
+    def get_table_details(self, database: str, table: str, catalog: str = None):
+        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
+        self._logger.debug(
             f"getting existing table details and partitions for table {database}.{table}"
         )
 
         df: DataFrame = self.spark.sql(
-            f"DESCRIBE TABLE EXTENDED `{database}`.`{table}`"
+            f"DESCRIBE TABLE EXTENDED {database}.`{table}`"
         ).collect()
 
         # get the details into a dictionary
         details = {c.asDict()["col_name"]: c.asDict()["data_type"] for c in df}
 
         # pull out the columns
         columns = {}
@@ -353,15 +375,15 @@
                 "location": details.get("Location"),
                 "provider": details.get("Provider"),
                 "owner": details.get("Owner"),
             }
         }
 
         msg = json.dumps(details, indent=4, default=str)
-        _logger.debug(msg)
+        self._logger.debug(msg)
         return details
 
     def create_column_ddl(self, field: StructField):
         nullable = "" if field.nullable else "NOT NULL"
         comment = f"COMMENT {field.metadata}" if field.metadata else ""
         field_type = field.dataType.typeName()
         field_name = f"`{field.name}`"
```

### Comparing `yetl-framework-1.4.9/yetl/config/table/_deltalake.py` & `yetl-framework-1.5.0.dev1/yetl/config/table/_deltalake.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 class DeltaLake(Table):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._spark = DeltaLakeFn(project=self.project)
         self._render()
-        self._spark.create_database(self.database)
 
     @classmethod
     def in_allowed_stages(cls, stage: StageType):
         return stage in (stage.raw, stage.base, stage.curated)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
@@ -80,19 +79,23 @@
             if self.options:
                 for option, value in self.options.items():
                     if isinstance(value, str):
                         self.options[option] = render_jinja(value, self._replacements)
 
         self._rendered = True
 
+    def create_database(self):
+        self._spark.create_database(self.database)
+
     # TODO: Create or alter table
     def create_table(self):
         if self._spark.table_exists(database=self.database, table=self.table):
             pass
             # TODO: alter table
+            self._logger.info(f"table `{self.database}`.`{self.table}` already exists.")
         else:
             if self.managed:
                 self._spark.create_table(
                     database=self.database,
                     table=self.table,
                     delta_properties=self.delta_properties,
                     sql=self.sql,
```

### Comparing `yetl-framework-1.4.9/yetl/config/table/_factory.py` & `yetl-framework-1.5.0.dev1/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/table/_read.py` & `yetl-framework-1.5.0.dev1/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl/config/table/_table.py` & `yetl-framework-1.5.0.dev1/yetl/config/table/_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,7 +115,10 @@
             if self.warning_thresholds:
                 return self.warning_thresholds.select_sql()
             else:
                 return ValidationThreshold.default_select_sql()
 
     def create_table(self):
         pass
+
+    def create_database(self):
+        pass
```

### Comparing `yetl-framework-1.4.9/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.5.0.dev1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.9/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.5.0.dev1/yetl_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.9
+Version: 1.5.0.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.9/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.5.0.dev1/yetl_framework.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 yetl/config/table/_deltalake.py
 yetl/config/table/_factory.py
 yetl/config/table/_read.py
 yetl/config/table/_table.py
 yetl/config/table/_table_type.py
 yetl/config/table/_write.py
 yetl/workflow/__init__.py
+yetl/workflow/_dlt.py
 yetl/workflow/_multi_threaded.py
 yetl/workflow/_notebook.py
 yetl_framework.egg-info/PKG-INFO
 yetl_framework.egg-info/SOURCES.txt
 yetl_framework.egg-info/dependency_links.txt
 yetl_framework.egg-info/not-zip-safe
 yetl_framework.egg-info/requires.txt
```


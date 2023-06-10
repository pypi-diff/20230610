# Comparing `tmp/cuallee-0.4.4.tar.gz` & `tmp/cuallee-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuallee-0.4.4.tar", last modified: Sat Jun  3 16:14:56 2023, max compression
+gzip compressed data, was "cuallee-0.4.5.tar", last modified: Sat Jun 10 16:44:11 2023, max compression
```

## Comparing `cuallee-0.4.4.tar` & `cuallee-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/
--rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.4.4/LICENSE
--rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:14:56.499344 cuallee-0.4.4/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)    14258 2023-06-03 15:46:05.000000 cuallee-0.4.4/README.md
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/cuallee/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    20284 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     9876 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/duckdb_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/cuallee/iso/
--rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/iso/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/iso/checks.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/pandas_validation.py
--rw-rw-r--   0 herminio  (1000) herminio  (1000)        0 2022-11-26 21:58:56.000000 cuallee-0.4.4/cuallee/polars.validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-06-03 15:46:05.000000 cuallee-0.4.4/cuallee/pyspark_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.4.4/cuallee/snowpark_validation.py
--rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.4.4/cuallee/utils.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:14:56.499344 cuallee-0.4.4/cuallee.egg-info/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/SOURCES.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/dependency_links.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)      312 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/requires.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-06-03 16:14:56.000000 cuallee-0.4.4/cuallee.egg-info/top_level.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1211 2023-06-03 16:13:57.000000 cuallee-0.4.4/pyproject.toml
--rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-06-03 16:14:56.499344 cuallee-0.4.4/setup.cfg
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.4.5/LICENSE
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-10 16:44:11.188587 cuallee-0.4.5/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    14258 2023-06-03 15:46:05.000000 cuallee-0.4.5/README.md
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/cuallee/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    20708 2023-06-10 16:39:56.000000 cuallee-0.4.5/cuallee/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     9872 2023-06-10 16:39:56.000000 cuallee-0.4.5/cuallee/duckdb_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/cuallee/iso/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/iso/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/iso/checks.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/pandas_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    16162 2023-06-10 16:39:56.000000 cuallee-0.4.5/cuallee/polars_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/pyspark_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.4.5/cuallee/snowpark_validation.py
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.4.5/cuallee/utils.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/cuallee.egg-info/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/SOURCES.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/dependency_links.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      311 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/requires.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/top_level.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     1210 2023-06-10 16:41:33.000000 cuallee-0.4.5/pyproject.toml
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-06-10 16:44:11.188587 cuallee-0.4.5/setup.cfg
```

### Comparing `cuallee-0.4.4/LICENSE` & `cuallee-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.4/PKG-INFO` & `cuallee-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cuallee-0.4.4/README.md` & `cuallee-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.4/cuallee/__init__.py` & `cuallee-0.4.5/cuallee/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,21 @@
     from pandas import DataFrame as pandas_dataframe  # type: ignore
 
     logger.debug(Fore.GREEN + "[OK]" + Fore.WHITE + " Pandas")
 except:
     logger.debug(Fore.RED + "[KO]" + Fore.WHITE + " Pandas")
 
 try:
+    from polars.dataframe.frame import DataFrame as polars_dataframe  # type: ignore
+
+    logger.debug(Fore.GREEN + "[OK]" + Fore.WHITE + " Polars")
+except:
+    logger.debug(Fore.RED + "[KO]" + Fore.WHITE + " Polars")
+
+try:
     from pyspark.sql import DataFrame as pyspark_dataframe
 
     logger.debug(Fore.GREEN + "[OK]" + Fore.WHITE + " PySpark")
 
 except:
     logger.debug(Fore.RED + "[KO]" + Fore.WHITE + " PySpark")
 
@@ -552,14 +559,19 @@
             self.compute_engine = importlib.import_module("cuallee.snowpark_validation")
 
         elif "duckdb_dataframe" in globals() and isinstance(
             dataframe, duckdb_dataframe
         ):
             self.compute_engine = importlib.import_module("cuallee.duckdb_validation")
 
+        elif "polars_dataframe" in globals() and isinstance(
+            dataframe, polars_dataframe
+        ):
+            self.compute_engine = importlib.import_module("cuallee.polars_validation")
+
         assert self.compute_engine.validate_data_types(
             self.rules, dataframe
         ), "Invalid data types between rules and dataframe"
         return self.compute_engine.summary(self, dataframe)
 
     # def samples(self, dataframe: Any, rule_index: int = None) -> Any:
     #     if not rule_index:
```

### Comparing `cuallee-0.4.4/cuallee/duckdb_validation.py` & `cuallee-0.4.5/cuallee/duckdb_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,15 @@
     def is_on_saturday(self, rule: Rule) -> str:
         return f"SUM(CAST(EXTRACT(dow from {rule.column}) = 6 AS INTEGER))"
 
     def is_on_sunday(self, rule: Rule) -> str:
         return f"SUM(CAST(EXTRACT(dow from {rule.column}) = 0 AS INTEGER))"
 
     def is_on_schedule(self, rule: Rule) -> str:
-        return (
-            f"SUM(CAST(EXTRACT(hour from {rule.column}) BETWEEN {rule.value[0]} AND {rule.value[1]} AS INTEGER))"
-        )
+        return f"SUM(CAST(EXTRACT(hour from {rule.column}) BETWEEN {rule.value[0]} AND {rule.value[1]} AS INTEGER))"
 
     def is_daily(self, rule: Rule) -> str:
         """Returns the number or violations and matches on a daily schedule"""
         if rule.value is None:
             day_mask = tuple([1, 2, 3, 4, 5])
         else:
             day_mask = rule.value
@@ -150,19 +148,21 @@
         )
 
         return template.substitute(
             {"id": rule.column, "value": str(day_mask), "table": self.table_name}
         )
 
     def is_inside_interquartile_range(self, rule: Rule) -> str:
-        template = Template("""
+        template = Template(
+            """
             (select SUM(CAST(A.$id BETWEEN B.q[1] AND B.q[2] AS INTEGER)) as r from $table A,(
             select QUANTILE_CONT($id, [0.25, 0.75]) as q from $table) B)
-        """.strip())
-        return template.substitute({"id" : rule.column, "table" : self.table_name})
+        """.strip()
+        )
+        return template.substitute({"id": rule.column, "table": self.table_name})
 
     def has_workflow(self, rule: Rule) -> str:
 
         template = Template(
             """
         (select sum(A.CUALLEE_RESULT) from (
             select
```

### Comparing `cuallee-0.4.4/cuallee/iso/checks.py` & `cuallee-0.4.5/cuallee/iso/checks.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.4/cuallee/pandas_validation.py` & `cuallee-0.4.5/cuallee/pandas_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.4/cuallee/pyspark_validation.py` & `cuallee-0.4.5/cuallee/pyspark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.4/cuallee/snowpark_validation.py` & `cuallee-0.4.5/cuallee/snowpark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.4/cuallee/utils.py` & `cuallee-0.4.5/cuallee/utils.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.4/cuallee.egg-info/PKG-INFO` & `cuallee-0.4.5/cuallee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cuallee-0.4.4/pyproject.toml` & `cuallee-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuallee"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   { name="Virginie Grosboillot", email="vestalisvirginis@gmail.com" },
   { name="Herminio Vazquez", email="canimus@gmail.com"}
 ]
 description = "Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -37,15 +37,15 @@
 pandas = [
   "pandas>=2.0.1"
 ]
 duckdb = [
   "duckdb>=0.7.1"
 ]
 polars = [
-  "polars>=0.14.29"
+  "polars>=0.15.7"
 ]
 iso = [
   "lxml >= 4.9.1"
 ]
 test = [
   "pytest",
   "pytest-cov",
```


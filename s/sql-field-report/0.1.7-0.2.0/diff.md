# Comparing `tmp/sql_field_report-0.1.7.tar.gz` & `tmp/sql_field_report-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.1.7.tar", max compression
+gzip compressed data, was "sql_field_report-0.2.0.tar", max compression
```

## Comparing `sql_field_report-0.1.7.tar` & `sql_field_report-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0      676 2023-06-09 16:52:34.738729 sql_field_report-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-27 11:53:49.547739 sql_field_report-0.1.7/sql_field_report/__init__.py
--rw-r--r--   0        0        0       68 2023-04-27 13:15:20.467845 sql_field_report-0.1.7/sql_field_report/__main__.py
--rw-r--r--   0        0        0    11963 2023-06-09 16:01:59.427291 sql_field_report-0.1.7/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 sql_field_report-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      676 2023-06-10 11:18:05.099656 sql_field_report-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.2.0/README.md
+-rw-r--r--   0        0        0       82 2023-06-10 11:17:52.279652 sql_field_report-0.2.0/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.2.0/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     2724 2023-06-10 11:33:46.727213 sql_field_report-0.2.0/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.2.0/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0     7106 2023-06-10 11:35:47.875592 sql_field_report-0.2.0/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     1579 2023-06-10 10:54:46.102029 sql_field_report-0.2.0/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3221 2023-06-10 10:58:30.065756 sql_field_report-0.2.0/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 sql_field_report-0.2.0/PKG-INFO
```

### Comparing `sql_field_report-0.1.7/pyproject.toml` & `sql_field_report-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "0.1.7"
+version = "0.2.0"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `sql_field_report-0.1.7/README.md` & `sql_field_report-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.1.7/PKG-INFO` & `sql_field_report-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 0.1.7
+Version: 0.2.0
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
```


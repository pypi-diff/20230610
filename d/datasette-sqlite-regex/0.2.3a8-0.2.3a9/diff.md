# Comparing `tmp/datasette_sqlite_regex-0.2.3a8-py3-none-any.whl.zip` & `tmp/datasette_sqlite_regex-0.2.3a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2192 bytes, number of entries: 7
--rw-r--r--  2.0 unx      269 b- defN 23-Jun-10 20:51 datasette_sqlite_regex/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 20:51 datasette_sqlite_regex/version.py
--rw-r--r--  2.0 unx      569 b- defN 23-Jun-10 20:51 datasette_sqlite_regex-0.2.3a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 20:51 datasette_sqlite_regex-0.2.3a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jun-10 20:51 datasette_sqlite_regex-0.2.3a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-10 20:51 datasette_sqlite_regex-0.2.3a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-10 20:51 datasette_sqlite_regex-0.2.3a8.dist-info/RECORD
-7 files, 1737 bytes uncompressed, 998 bytes compressed:  42.5%
+Zip file size: 2191 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-10 21:31 datasette_sqlite_regex/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 21:31 datasette_sqlite_regex/version.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Jun-10 21:31 datasette_sqlite_regex-0.2.3a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 21:31 datasette_sqlite_regex-0.2.3a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-10 21:31 datasette_sqlite_regex-0.2.3a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-10 21:31 datasette_sqlite_regex-0.2.3a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-10 21:31 datasette_sqlite_regex-0.2.3a9.dist-info/RECORD
+7 files, 1737 bytes uncompressed, 997 bytes compressed:  42.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_regex/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_regex/version.py
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a8.dist-info/METADATA
+Filename: datasette_sqlite_regex-0.2.3a9.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a8.dist-info/WHEEL
+Filename: datasette_sqlite_regex-0.2.3a9.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a8.dist-info/entry_points.txt
+Filename: datasette_sqlite_regex-0.2.3a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a8.dist-info/top_level.txt
+Filename: datasette_sqlite_regex-0.2.3a9.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_regex-0.2.3a8.dist-info/RECORD
+Filename: datasette_sqlite_regex-0.2.3a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_regex/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.3-alpha.8"
+__version__ = "0.2.3-alpha.9"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_regex-0.2.3a8.dist-info/METADATA` & `datasette_sqlite_regex-0.2.3a9.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-regex
-Version: 0.2.3a8
+Version: 0.2.3a9
 Home-page: https://github.com/asg017/sqlite-regex
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-regex/issues
 Project-URL: CI, https://github.com/asg017/sqlite-regex/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-regex/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_regex-0.2.3a8.dist-info/RECORD` & `datasette_sqlite_regex-0.2.3a9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_regex/__init__.py,sha256=gAZZGeI-BnNoB0cNpqhiiUcVh-BrAfdojdzff9v0B-o,269
-datasette_sqlite_regex/version.py,sha256=nX1HTeMDHklLbUTDaeIPZW6e4NFuraFR3wilxA-ogA4,79
-datasette_sqlite_regex-0.2.3a8.dist-info/METADATA,sha256=xOkUFeh7t9G3VsB_SzPEsmCXItkZLpwNvnqWnWmtGK4,569
-datasette_sqlite_regex-0.2.3a8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_regex-0.2.3a8.dist-info/entry_points.txt,sha256=Zk3m397tATyr9K3ZSBiMtwjGslB-xitDauEcT8TTE4k,50
-datasette_sqlite_regex-0.2.3a8.dist-info/top_level.txt,sha256=B9-o0e-bXWWM2wW4Z2fCLlpdh_xevETnuqjaWZ0a5qg,23
-datasette_sqlite_regex-0.2.3a8.dist-info/RECORD,,
+datasette_sqlite_regex/version.py,sha256=0FMI8YXJMgmVrJmkIk_kpl6KEMAbMkrf2izL6iELjLM,79
+datasette_sqlite_regex-0.2.3a9.dist-info/METADATA,sha256=Yz8KqJDy_t8rO19SGdB5cvRhD2TxUrDgjITK7qZYCBM,569
+datasette_sqlite_regex-0.2.3a9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_regex-0.2.3a9.dist-info/entry_points.txt,sha256=Zk3m397tATyr9K3ZSBiMtwjGslB-xitDauEcT8TTE4k,50
+datasette_sqlite_regex-0.2.3a9.dist-info/top_level.txt,sha256=B9-o0e-bXWWM2wW4Z2fCLlpdh_xevETnuqjaWZ0a5qg,23
+datasette_sqlite_regex-0.2.3a9.dist-info/RECORD,,
```


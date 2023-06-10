# Comparing `tmp/datasette_sqlite_jsonschema-0.2.3a4-py3-none-any.whl.zip` & `tmp/datasette_sqlite_jsonschema-0.2.3a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2284 bytes, number of entries: 7
--rw-r--r--  2.0 unx      284 b- defN 23-Jun-07 18:51 datasette_sqlite_jsonschema/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 18:51 datasette_sqlite_jsonschema/version.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jun-07 18:52 datasette_sqlite_jsonschema-0.2.3a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 18:52 datasette_sqlite_jsonschema-0.2.3a4.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Jun-07 18:52 datasette_sqlite_jsonschema-0.2.3a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-07 18:52 datasette_sqlite_jsonschema-0.2.3a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      690 b- defN 23-Jun-07 18:52 datasette_sqlite_jsonschema-0.2.3a4.dist-info/RECORD
-7 files, 1832 bytes uncompressed, 1020 bytes compressed:  44.3%
+Zip file size: 2285 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-10 20:53 datasette_sqlite_jsonschema/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 20:53 datasette_sqlite_jsonschema/version.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Jun-10 20:53 datasette_sqlite_jsonschema-0.2.3a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 20:53 datasette_sqlite_jsonschema-0.2.3a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-10 20:53 datasette_sqlite_jsonschema-0.2.3a5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-10 20:53 datasette_sqlite_jsonschema-0.2.3a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      690 b- defN 23-Jun-10 20:53 datasette_sqlite_jsonschema-0.2.3a5.dist-info/RECORD
+7 files, 1832 bytes uncompressed, 1021 bytes compressed:  44.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_jsonschema/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_jsonschema/version.py
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a4.dist-info/METADATA
+Filename: datasette_sqlite_jsonschema-0.2.3a5.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a4.dist-info/WHEEL
+Filename: datasette_sqlite_jsonschema-0.2.3a5.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a4.dist-info/entry_points.txt
+Filename: datasette_sqlite_jsonschema-0.2.3a5.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a4.dist-info/top_level.txt
+Filename: datasette_sqlite_jsonschema-0.2.3a5.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a4.dist-info/RECORD
+Filename: datasette_sqlite_jsonschema-0.2.3a5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_jsonschema/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.3-alpha.4"
+__version__ = "0.2.3-alpha.5"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_jsonschema-0.2.3a4.dist-info/METADATA` & `datasette_sqlite_jsonschema-0.2.3a5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-jsonschema
-Version: 0.2.3a4
+Version: 0.2.3a5
 Home-page: https://github.com/asg017/sqlite-jsonschema
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-jsonschema/issues
 Project-URL: CI, https://github.com/asg017/sqlite-jsonschema/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-jsonschema/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_jsonschema-0.2.3a4.dist-info/RECORD` & `datasette_sqlite_jsonschema-0.2.3a5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_jsonschema/__init__.py,sha256=CkEgCNG1ogAHTmP5eAR4aQ3TdxqqmgBIs9kLzsEp29U,284
-datasette_sqlite_jsonschema/version.py,sha256=4j5-oxNd3Lqp6OW8UEJ1qO8xsk12tmgvn1RclWqs4AE,79
-datasette_sqlite_jsonschema-0.2.3a4.dist-info/METADATA,sha256=lMGfzI1Qz5QPcTvRWMTjIzi0iFOOYWqllKW5vpyHx5M,599
-datasette_sqlite_jsonschema-0.2.3a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_jsonschema-0.2.3a4.dist-info/entry_points.txt,sha256=GudkqSm13Ou5ZqFjwDzCYFo5oo9FSVgstqZWdGYOGTo,60
-datasette_sqlite_jsonschema-0.2.3a4.dist-info/top_level.txt,sha256=gGoRXv89K-JydhKqkfeF25P05Er5OkO8wqnHPcKfim0,28
-datasette_sqlite_jsonschema-0.2.3a4.dist-info/RECORD,,
+datasette_sqlite_jsonschema/version.py,sha256=o6GdM3-8whcUNqnr6UQj86FWQQbmlnj0V8Xg5Cb8FSI,79
+datasette_sqlite_jsonschema-0.2.3a5.dist-info/METADATA,sha256=uKwzA2P9g6-t2QdjLDDAjCHBQGmG8OnLbcLIJL4wDaU,599
+datasette_sqlite_jsonschema-0.2.3a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_jsonschema-0.2.3a5.dist-info/entry_points.txt,sha256=GudkqSm13Ou5ZqFjwDzCYFo5oo9FSVgstqZWdGYOGTo,60
+datasette_sqlite_jsonschema-0.2.3a5.dist-info/top_level.txt,sha256=gGoRXv89K-JydhKqkfeF25P05Er5OkO8wqnHPcKfim0,28
+datasette_sqlite_jsonschema-0.2.3a5.dist-info/RECORD,,
```


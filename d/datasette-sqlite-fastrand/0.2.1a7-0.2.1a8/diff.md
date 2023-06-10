# Comparing `tmp/datasette_sqlite_fastrand-0.2.1a7-py3-none-any.whl.zip` & `tmp/datasette_sqlite_fastrand-0.2.1a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2243 bytes, number of entries: 7
--rw-r--r--  2.0 unx      278 b- defN 23-Jun-07 19:00 datasette_sqlite_fastrand/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 19:00 datasette_sqlite_fastrand/version.py
--rw-r--r--  2.0 unx      587 b- defN 23-Jun-07 19:00 datasette_sqlite_fastrand-0.2.1a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 19:00 datasette_sqlite_fastrand-0.2.1a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-Jun-07 19:00 datasette_sqlite_fastrand-0.2.1a7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-07 19:00 datasette_sqlite_fastrand-0.2.1a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 23-Jun-07 19:00 datasette_sqlite_fastrand-0.2.1a7.dist-info/RECORD
-7 files, 1794 bytes uncompressed, 1007 bytes compressed:  43.9%
+Zip file size: 2241 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      278 b- defN 23-Jun-10 20:57 datasette_sqlite_fastrand/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 20:57 datasette_sqlite_fastrand/version.py
+-rw-r--r--  2.0 unx      587 b- defN 23-Jun-10 20:57 datasette_sqlite_fastrand-0.2.1a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 20:57 datasette_sqlite_fastrand-0.2.1a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-10 20:57 datasette_sqlite_fastrand-0.2.1a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-10 20:57 datasette_sqlite_fastrand-0.2.1a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-10 20:57 datasette_sqlite_fastrand-0.2.1a8.dist-info/RECORD
+7 files, 1794 bytes uncompressed, 1005 bytes compressed:  44.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_fastrand/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_fastrand/version.py
 Comment: 
 
-Filename: datasette_sqlite_fastrand-0.2.1a7.dist-info/METADATA
+Filename: datasette_sqlite_fastrand-0.2.1a8.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_fastrand-0.2.1a7.dist-info/WHEEL
+Filename: datasette_sqlite_fastrand-0.2.1a8.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_fastrand-0.2.1a7.dist-info/entry_points.txt
+Filename: datasette_sqlite_fastrand-0.2.1a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_fastrand-0.2.1a7.dist-info/top_level.txt
+Filename: datasette_sqlite_fastrand-0.2.1a8.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_fastrand-0.2.1a7.dist-info/RECORD
+Filename: datasette_sqlite_fastrand-0.2.1a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_fastrand/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1-alpha.7"
+__version__ = "0.2.1-alpha.8"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_fastrand-0.2.1a7.dist-info/METADATA` & `datasette_sqlite_fastrand-0.2.1a8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-fastrand
-Version: 0.2.1a7
+Version: 0.2.1a8
 Home-page: https://github.com/asg017/sqlite-fastrand
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-fastrand/issues
 Project-URL: CI, https://github.com/asg017/sqlite-fastrand/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-fastrand/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_fastrand-0.2.1a7.dist-info/RECORD` & `datasette_sqlite_fastrand-0.2.1a8.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_fastrand/__init__.py,sha256=yAxdMjiiU-78b5VxKcjW2GGc9yKD_GdSLafIjqz_Vek,278
-datasette_sqlite_fastrand/version.py,sha256=nRG6tm7IqbsXeMveG4FXxki4OGcgFKwNvfU0irh9vcA,79
-datasette_sqlite_fastrand-0.2.1a7.dist-info/METADATA,sha256=5C3bjcyHUoKqugqaWDWp2uwPUxjdrsEE0p1ET9uMyLo,587
-datasette_sqlite_fastrand-0.2.1a7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_fastrand-0.2.1a7.dist-info/entry_points.txt,sha256=UM_x4MK7MhhhUVsbun3u4-Q5qTd3X2JEz4pe2kgT-Ss,56
-datasette_sqlite_fastrand-0.2.1a7.dist-info/top_level.txt,sha256=Z0y5c1moSczEQ4TWNrS2xud6HOaTx6CYyzJioTv3jRY,26
-datasette_sqlite_fastrand-0.2.1a7.dist-info/RECORD,,
+datasette_sqlite_fastrand/version.py,sha256=jl9m1HGTn5QCjLy0YcAnz0gk8WEhw0bBKtHsfSQZlf8,79
+datasette_sqlite_fastrand-0.2.1a8.dist-info/METADATA,sha256=6AlXkl70j68-eiMHkUJJXnZae7iudgUHsrCaeqaVTmo,587
+datasette_sqlite_fastrand-0.2.1a8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_fastrand-0.2.1a8.dist-info/entry_points.txt,sha256=UM_x4MK7MhhhUVsbun3u4-Q5qTd3X2JEz4pe2kgT-Ss,56
+datasette_sqlite_fastrand-0.2.1a8.dist-info/top_level.txt,sha256=Z0y5c1moSczEQ4TWNrS2xud6HOaTx6CYyzJioTv3jRY,26
+datasette_sqlite_fastrand-0.2.1a8.dist-info/RECORD,,
```


# Comparing `tmp/datasette_sqlite_ulid-0.2.1a8-py3-none-any.whl.zip` & `tmp/datasette_sqlite_ulid-0.2.1a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2174 bytes, number of entries: 7
--rw-r--r--  2.0 unx      266 b- defN 23-Mar-11 06:09 datasette_sqlite_ulid/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-11 06:09 datasette_sqlite_ulid/version.py
--rw-r--r--  2.0 unx      563 b- defN 23-Mar-11 06:10 datasette_sqlite_ulid-0.2.1a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-11 06:10 datasette_sqlite_ulid-0.2.1a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Mar-11 06:10 datasette_sqlite_ulid-0.2.1a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Mar-11 06:10 datasette_sqlite_ulid-0.2.1a8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      648 b- defN 23-Mar-11 06:10 datasette_sqlite_ulid-0.2.1a8.dist-info/RECORD
-7 files, 1718 bytes uncompressed, 994 bytes compressed:  42.1%
+Zip file size: 2172 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      266 b- defN 23-Mar-11 06:18 datasette_sqlite_ulid/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Mar-11 06:18 datasette_sqlite_ulid/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Mar-11 06:18 datasette_sqlite_ulid-0.2.1a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-11 06:18 datasette_sqlite_ulid-0.2.1a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Mar-11 06:18 datasette_sqlite_ulid-0.2.1a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Mar-11 06:18 datasette_sqlite_ulid-0.2.1a9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      648 b- defN 23-Mar-11 06:18 datasette_sqlite_ulid-0.2.1a9.dist-info/RECORD
+7 files, 1718 bytes uncompressed, 992 bytes compressed:  42.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_ulid/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_ulid/version.py
 Comment: 
 
-Filename: datasette_sqlite_ulid-0.2.1a8.dist-info/METADATA
+Filename: datasette_sqlite_ulid-0.2.1a9.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_ulid-0.2.1a8.dist-info/WHEEL
+Filename: datasette_sqlite_ulid-0.2.1a9.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_ulid-0.2.1a8.dist-info/entry_points.txt
+Filename: datasette_sqlite_ulid-0.2.1a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_ulid-0.2.1a8.dist-info/top_level.txt
+Filename: datasette_sqlite_ulid-0.2.1a9.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_ulid-0.2.1a8.dist-info/RECORD
+Filename: datasette_sqlite_ulid-0.2.1a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_ulid/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1-alpha.8"
+__version__ = "0.2.1-alpha.9"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_ulid-0.2.1a8.dist-info/METADATA` & `datasette_sqlite_ulid-0.2.1a9.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-ulid
-Version: 0.2.1a8
+Version: 0.2.1a9
 Home-page: https://github.com/asg017/sqlite-ulid
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-ulid/issues
 Project-URL: CI, https://github.com/asg017/sqlite-ulid/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-ulid/releases
 Requires-Python: >=3.6
```

## Comparing `datasette_sqlite_ulid-0.2.1a8.dist-info/RECORD` & `datasette_sqlite_ulid-0.2.1a9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_ulid/__init__.py,sha256=BlPI-lSJzN3uUxQ2Wm9I04orjdjV9pBtYwesv44Tfog,266
-datasette_sqlite_ulid/version.py,sha256=jl9m1HGTn5QCjLy0YcAnz0gk8WEhw0bBKtHsfSQZlf8,79
-datasette_sqlite_ulid-0.2.1a8.dist-info/METADATA,sha256=Bmr-nh7xZz6-zN07PXUEJBEd0qqnZNIAlKwCKXEoKVA,563
-datasette_sqlite_ulid-0.2.1a8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datasette_sqlite_ulid-0.2.1a8.dist-info/entry_points.txt,sha256=87OYgkv9YF0IH5FlLWI4CTuhC3Ty_EdxXD2AgDwhOjo,48
-datasette_sqlite_ulid-0.2.1a8.dist-info/top_level.txt,sha256=qWangeDrWtPzSSF8jGjS_MFlD5K73__0EOMZu-ItmcU,22
-datasette_sqlite_ulid-0.2.1a8.dist-info/RECORD,,
+datasette_sqlite_ulid/version.py,sha256=hIbkUMOHRY40IOMiXLTSTkpxY60AIS_XO9LOJvYL6JE,79
+datasette_sqlite_ulid-0.2.1a9.dist-info/METADATA,sha256=Snc9YYN_EOSILHk6EV7dd7gHhIwcClzdO8D7MUzeABA,563
+datasette_sqlite_ulid-0.2.1a9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datasette_sqlite_ulid-0.2.1a9.dist-info/entry_points.txt,sha256=87OYgkv9YF0IH5FlLWI4CTuhC3Ty_EdxXD2AgDwhOjo,48
+datasette_sqlite_ulid-0.2.1a9.dist-info/top_level.txt,sha256=qWangeDrWtPzSSF8jGjS_MFlD5K73__0EOMZu-ItmcU,22
+datasette_sqlite_ulid-0.2.1a9.dist-info/RECORD,,
```


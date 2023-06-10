# Comparing `tmp/flake8_2020-1.8.0.tar.gz` & `tmp/flake8_2020-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_2020-1.8.0.tar", last modified: Sat May  6 21:06:58 2023, max compression
+gzip compressed data, was "flake8_2020-1.8.1.tar", last modified: Sat Jun 10 19:04:41 2023, max compression
```

## Comparing `flake8_2020-1.8.0.tar` & `flake8_2020-1.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 20:25:33.000000 flake8_2020-1.8.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4262 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3687 2023-05-06 20:25:33.000000 flake8_2020-1.8.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/flake8_2020.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4262 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      263 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       44 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6585 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1099 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 20:25:33.000000 flake8_2020-1.8.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 19:04:41.645342 flake8_2020-1.8.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 19:00:28.000000 flake8_2020-1.8.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4262 2023-06-10 19:04:41.645342 flake8_2020-1.8.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3687 2023-06-10 19:00:28.000000 flake8_2020-1.8.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 19:04:41.645342 flake8_2020-1.8.1/flake8_2020.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4262 2023-06-10 19:04:41.000000 flake8_2020-1.8.1/flake8_2020.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      263 2023-06-10 19:04:41.000000 flake8_2020-1.8.1/flake8_2020.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 19:04:41.000000 flake8_2020-1.8.1/flake8_2020.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       44 2023-06-10 19:04:41.000000 flake8_2020-1.8.1/flake8_2020.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-06-10 19:04:41.000000 flake8_2020-1.8.1/flake8_2020.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2023-06-10 19:04:41.000000 flake8_2020-1.8.1/flake8_2020.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6657 2023-06-10 19:04:41.000000 flake8_2020-1.8.1/flake8_2020.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1100 2023-06-10 19:04:41.645342 flake8_2020-1.8.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 19:00:28.000000 flake8_2020-1.8.1/setup.py
```

### Comparing `flake8_2020-1.8.0/LICENSE` & `flake8_2020-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_2020-1.8.0/PKG-INFO` & `flake8_2020-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_2020
-Version: 1.8.0
+Version: 1.8.1
 Summary: flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 Home-page: https://github.com/asottile/flake8-2020
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flake8_2020-1.8.0/README.md` & `flake8_2020-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8_2020-1.8.0/flake8_2020.egg-info/PKG-INFO` & `flake8_2020-1.8.1/flake8_2020.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-2020
-Version: 1.8.0
+Version: 1.8.1
 Summary: flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 Home-page: https://github.com/asottile/flake8-2020
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flake8_2020-1.8.0/flake8_2020.py` & `flake8_2020-1.8.1/flake8_2020.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,17 +95,18 @@
             self.errors.append((
                 node.left.lineno, node.left.col_offset, YTT201,
             ))
         elif (
                 self._is_sys('version', node.left) and
                 len(node.ops) == 1 and
                 isinstance(node.ops[0], (ast.Lt, ast.LtE, ast.Gt, ast.GtE)) and
-                isinstance(node.comparators[0], ast.Str)
+                isinstance(node.comparators[0], ast.Constant) and
+                isinstance(node.comparators[0].value, str)
         ):
-            if len(node.comparators[0].s) == 1:
+            if len(node.comparators[0].value) == 1:
                 code = YTT302
             else:
                 code = YTT103
             self.errors.append((
                 node.left.lineno, node.left.col_offset, code,
             ))
         elif (
```

### Comparing `flake8_2020-1.8.0/setup.cfg` & `flake8_2020-1.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = flake8_2020
-version = 1.8.0
+version = 1.8.1
 description = flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/flake8-2020
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
```


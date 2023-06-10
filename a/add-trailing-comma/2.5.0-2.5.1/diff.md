# Comparing `tmp/add_trailing_comma-2.5.0.tar.gz` & `tmp/add_trailing_comma-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "add_trailing_comma-2.5.0.tar", last modified: Sat Jun 10 20:30:39 2023, max compression
+gzip compressed data, was "add_trailing_comma-2.5.1.tar", last modified: Sat Jun 10 21:05:03 2023, max compression
```

## Comparing `add_trailing_comma-2.5.0.tar` & `add_trailing_comma-2.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4032 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/add_trailing_comma/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2307 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3227 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/_with.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1887 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1645 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/functions.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3058 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/match.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6613 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1233 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 21:05:03.167805 add_trailing_comma-2.5.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4032 2023-06-10 21:05:02.000000 add_trailing_comma-2.5.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/add_trailing_comma/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2307 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3228 2023-06-10 21:05:02.000000 add_trailing_comma-2.5.1/add_trailing_comma/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/_with.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1887 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1645 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/functions.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3058 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/match.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6613 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1233 2023-06-10 21:05:03.167805 add_trailing_comma-2.5.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/setup.py
```

### Comparing `add_trailing_comma-2.5.0/LICENSE` & `add_trailing_comma-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/PKG-INFO` & `add_trailing_comma-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add_trailing_comma
-Version: 2.5.0
+Version: 2.5.1
 Summary: Automatically add trailing commas to calls and literals
 Home-page: https://github.com/asottile/add-trailing-comma
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.5.0
+    rev: v2.5.1
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.5.0/README.md` & `add_trailing_comma-2.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.5.0
+    rev: v2.5.1
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_ast_helpers.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_data.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_data.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_main.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         '--py36-plus',
         action='store_const', dest='min_version', const=(3, 6),
     )
     args = parser.parse_args(argv)
 
     if args.min_version < (3, 6):
         print(
-            'WARNING: add-trailing-comma will only use 3.6+ mod after 3.0',
+            'WARNING: add-trailing-comma will only use 3.6+ mode after 3.0',
             file=sys.stderr,
         )
 
     ret = 0
     for filename in args.filenames:
         ret |= fix_file(filename, args)
     return ret
```

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/_with.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/_with.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/calls.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/calls.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/classes.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/classes.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/functions.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/functions.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/imports.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/imports.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/literals.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/literals.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/match.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/match.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma/_token_helpers.py` & `add_trailing_comma-2.5.1/add_trailing_comma/_token_helpers.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma.egg-info/PKG-INFO` & `add_trailing_comma-2.5.1/add_trailing_comma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add-trailing-comma
-Version: 2.5.0
+Version: 2.5.1
 Summary: Automatically add trailing commas to calls and literals
 Home-page: https://github.com/asottile/add-trailing-comma
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.5.0
+    rev: v2.5.1
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.5.0/add_trailing_comma.egg-info/SOURCES.txt` & `add_trailing_comma-2.5.1/add_trailing_comma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.0/setup.cfg` & `add_trailing_comma-2.5.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = add_trailing_comma
-version = 2.5.0
+version = 2.5.1
 description = Automatically add trailing commas to calls and literals
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/add-trailing-comma
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```


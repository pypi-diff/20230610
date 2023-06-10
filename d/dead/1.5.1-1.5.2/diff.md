# Comparing `tmp/dead-1.5.1.tar.gz` & `tmp/dead-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dead-1.5.1.tar", last modified: Sat May  6 20:35:39 2023, max compression
+gzip compressed data, was "dead-1.5.2.tar", last modified: Sat Jun 10 18:01:40 2023, max compression
```

## Comparing `dead-1.5.1.tar` & `dead-1.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:35:39.315444 dead-1.5.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 20:21:19.000000 dead-1.5.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2593 2023-05-06 20:35:39.315444 dead-1.5.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2070 2023-05-06 20:35:39.000000 dead-1.5.1/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:35:39.315444 dead-1.5.1/dead.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2593 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      214 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       35 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12050 2023-05-06 20:35:39.000000 dead-1.5.1/dead.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1030 2023-05-06 20:35:39.319444 dead-1.5.1/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 20:21:19.000000 dead-1.5.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 18:01:40.120371 dead-1.5.2/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 17:55:02.000000 dead-1.5.2/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2593 2023-06-10 18:01:40.120371 dead-1.5.2/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2070 2023-06-10 18:01:39.000000 dead-1.5.2/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 18:01:40.120371 dead-1.5.2/dead.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2593 2023-06-10 18:01:40.000000 dead-1.5.2/dead.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      214 2023-06-10 18:01:40.000000 dead-1.5.2/dead.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 18:01:40.000000 dead-1.5.2/dead.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       35 2023-06-10 18:01:40.000000 dead-1.5.2/dead.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2023-06-10 18:01:40.000000 dead-1.5.2/dead.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2023-06-10 18:01:40.000000 dead-1.5.2/dead.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12075 2023-06-10 18:01:39.000000 dead-1.5.2/dead.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1031 2023-06-10 18:01:40.120371 dead-1.5.2/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 17:55:02.000000 dead-1.5.2/setup.py
```

### Comparing `dead-1.5.1/LICENSE` & `dead-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dead-1.5.1/PKG-INFO` & `dead-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead
-Version: 1.5.1
+Version: 1.5.2
 Summary: dead simple python dead code detection
 Home-page: https://github.com/asottile/dead
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,15 +51,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/dead
-    rev: v1.5.1
+    rev: v1.5.2
     hooks:
     -   id: dead
 ```
 
 ### how it works
 
 1. find all files in a repository using `git ls-files` and filtering:
```

### Comparing `dead-1.5.1/README.md` & `dead-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/dead
-    rev: v1.5.1
+    rev: v1.5.2
     hooks:
     -   id: dead
 ```
 
 ### how it works
 
 1. find all files in a repository using `git ls-files` and filtering:
```

### Comparing `dead-1.5.1/dead.egg-info/PKG-INFO` & `dead-1.5.2/dead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead
-Version: 1.5.1
+Version: 1.5.2
 Summary: dead simple python dead code detection
 Home-page: https://github.com/asottile/dead
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,15 +51,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/dead
-    rev: v1.5.1
+    rev: v1.5.2
     hooks:
     -   id: dead
 ```
 
 ### how it works
 
 1. find all files in a repository using `git ls-files` and filtering:
```

### Comparing `dead-1.5.1/dead.py` & `dead-1.5.2/dead.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,16 +272,17 @@
             return
 
         section = parser['options.entry_points']
         for k, v in section.items():
             for line in v.strip().splitlines():
                 match = ENTRYPOINT_RE.match(line)
                 if match:
-                    node = ast.fix_missing_locations(ast.Str(match.group(1)))
-                    visitor.read(match.group(1), node)
+                    node = ast.Constant(match[1])
+                    node = ast.fix_missing_locations(node)
+                    visitor.read(match[1], node)
 
 
 def main(argv: Sequence[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '--files', default='',
         help='regex for file inclusion, default: %(default)r',
```

### Comparing `dead-1.5.1/setup.cfg` & `dead-1.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = dead
-version = 1.5.1
+version = 1.5.2
 description = dead simple python dead code detection
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/dead
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


# Comparing `tmp/setup_py_upgrade-1.3.0.tar.gz` & `tmp/setup_py_upgrade-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_py_upgrade-1.3.0.tar", last modified: Sat May  6 21:17:04 2023, max compression
+gzip compressed data, was "setup_py_upgrade-1.3.1.tar", last modified: Sat Jun 10 18:51:42 2023, max compression
```

## Comparing `setup_py_upgrade-1.3.0.tar` & `setup_py_upgrade-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 21:10:42.000000 setup_py_upgrade-1.3.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3983 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3432 2023-05-06 21:10:42.000000 setup_py_upgrade-1.3.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1064 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 21:10:42.000000 setup_py_upgrade-1.3.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:17:04.555502 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3983 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      259 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       59 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8552 2023-05-06 21:17:04.000000 setup_py_upgrade-1.3.0/setup_py_upgrade.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 18:51:42.930294 setup_py_upgrade-1.3.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 18:48:02.000000 setup_py_upgrade-1.3.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3983 2023-06-10 18:51:42.930294 setup_py_upgrade-1.3.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3432 2023-06-10 18:48:02.000000 setup_py_upgrade-1.3.1/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1065 2023-06-10 18:51:42.930294 setup_py_upgrade-1.3.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 18:48:02.000000 setup_py_upgrade-1.3.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 18:51:42.930294 setup_py_upgrade-1.3.1/setup_py_upgrade.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3983 2023-06-10 18:51:42.000000 setup_py_upgrade-1.3.1/setup_py_upgrade.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      259 2023-06-10 18:51:42.000000 setup_py_upgrade-1.3.1/setup_py_upgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 18:51:42.000000 setup_py_upgrade-1.3.1/setup_py_upgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       59 2023-06-10 18:51:42.000000 setup_py_upgrade-1.3.1/setup_py_upgrade.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2023-06-10 18:51:42.000000 setup_py_upgrade-1.3.1/setup_py_upgrade.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8556 2023-06-10 18:51:42.000000 setup_py_upgrade-1.3.1/setup_py_upgrade.py
```

### Comparing `setup_py_upgrade-1.3.0/LICENSE` & `setup_py_upgrade-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_py_upgrade-1.3.0/PKG-INFO` & `setup_py_upgrade-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup_py_upgrade
-Version: 1.3.0
+Version: 1.3.1
 Summary: upgrade a setup.py to declarative metadata
 Home-page: https://github.com/asottile/setup-py-upgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setup_py_upgrade-1.3.0/README.md` & `setup_py_upgrade-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `setup_py_upgrade-1.3.0/setup.cfg` & `setup_py_upgrade-1.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = setup_py_upgrade
-version = 1.3.0
+version = 1.3.1
 description = upgrade a setup.py to declarative metadata
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/setup-py-upgrade
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

### Comparing `setup_py_upgrade-1.3.0/setup_py_upgrade.egg-info/PKG-INFO` & `setup_py_upgrade-1.3.1/setup_py_upgrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup-py-upgrade
-Version: 1.3.0
+Version: 1.3.1
 Summary: upgrade a setup.py to declarative metadata
 Home-page: https://github.com/asottile/setup-py-upgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setup_py_upgrade-1.3.0/setup_py_upgrade.py` & `setup_py_upgrade-1.3.1/setup_py_upgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 isinstance(node.body[0].value.func.value, ast.Name) and
                 (
                     node.body[0].value.func.value.id ==
                     node.items[0].optional_vars.id
                 )
         ):
             varname = node.body[0].targets[0].id
-            filename = node.items[0].context_expr.args[0].s
+            filename = node.items[0].context_expr.args[0].value
             self._files[varname] = filename
         self.generic_visit(node)
 
     def visit_Call(self, node: ast.Call) -> None:
         if is_setuptools_attr_call(node, 'setup'):
             for kwd in node.keywords:
                 if kwd.arg in METADATA_KEYS:
```


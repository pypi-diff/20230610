# Comparing `tmp/datoso_plugin_internetarchive-0.2.3.tar.gz` & `tmp/datoso_plugin_internetarchive-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_plugin_internetarchive-0.2.3.tar", last modified: Fri May  5 04:21:18 2023, max compression
+gzip compressed data, was "datoso_plugin_internetarchive-0.3.0.tar", last modified: Sat Jun 10 20:41:44 2023, max compression
```

## Comparing `datoso_plugin_internetarchive-0.2.3.tar` & `datoso_plugin_internetarchive-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.326601 datoso_plugin_internetarchive-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/ia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:41:44.767742 datoso_plugin_internetarchive-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:41:32.000000 datoso_plugin_internetarchive-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-10 20:41:44.767742 datoso_plugin_internetarchive-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-10 20:41:32.000000 datoso_plugin_internetarchive-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-10 20:41:32.000000 datoso_plugin_internetarchive-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:41:44.767742 datoso_plugin_internetarchive-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:41:44.763742 datoso_plugin_internetarchive-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:41:44.767742 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-10 20:41:32.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-10 20:41:32.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-10 20:41:32.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive/ia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:41:44.767742 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-10 20:41:44.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-10 20:41:44.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:41:44.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-10 20:41:44.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-10 20:41:44.000000 datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive.egg-info/top_level.txt
```

### Comparing `datoso_plugin_internetarchive-0.2.3/LICENSE` & `datoso_plugin_internetarchive-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.3/PKG-INFO` & `datoso_plugin_internetarchive-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso_plugin_internetarchive
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_plugin_internetarchive
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datoso_plugin_internetarchive-0.2.3/README.md` & `datoso_plugin_internetarchive-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.3/pyproject.toml` & `datoso_plugin_internetarchive-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 requires-python = ">=3.10"
 license     = {text = "MIT License"}
 authors     = [
     {name = 'Lacides Miranda', email = 'laromicas@hotmail.com'},
 ]
 keywords = ["emulators", "roms"]
 classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.3",
+    "datoso>=0.3.1",
     "internetarchive>=3.0.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_plugin_internetarchive"
```

### Comparing `datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/fetch.py` & `datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/ia.py` & `datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive/ia.py`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/PKG-INFO` & `datoso_plugin_internetarchive-0.3.0/src/datoso_plugin_internetarchive.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso-plugin-internetarchive
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_plugin_internetarchive
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```


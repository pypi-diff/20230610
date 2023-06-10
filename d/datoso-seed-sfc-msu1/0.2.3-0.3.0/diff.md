# Comparing `tmp/datoso_seed_sfc_msu1-0.2.3.tar.gz` & `tmp/datoso_seed_sfc_msu1-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_sfc_msu1-0.2.3.tar", last modified: Fri May  5 04:32:40 2023, max compression
+gzip compressed data, was "datoso_seed_sfc_msu1-0.3.0.tar", last modified: Sat Jun 10 20:51:25 2023, max compression
```

## Comparing `datoso_seed_sfc_msu1-0.2.3.tar` & `datoso_seed_sfc_msu1-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:32:40.680545 datoso_seed_sfc_msu1-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 04:32:40.680545 datoso_seed_sfc_msu1-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:32:40.680545 datoso_seed_sfc_msu1-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:32:40.680545 datoso_seed_sfc_msu1-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:32:40.680545 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 04:32:28.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:32:40.680545 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 04:32:40.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 04:32:40.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:32:40.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 04:32:40.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 04:32:40.000000 datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:51:25.502715 datoso_seed_sfc_msu1-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-10 20:51:25.502715 datoso_seed_sfc_msu1-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:51:25.502715 datoso_seed_sfc_msu1-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:51:25.498715 datoso_seed_sfc_msu1-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:51:25.502715 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-10 20:51:11.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:51:25.502715 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-10 20:51:25.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-10 20:51:25.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:51:25.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 20:51:25.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-10 20:51:25.000000 datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1.egg-info/top_level.txt
```

### Comparing `datoso_seed_sfc_msu1-0.2.3/LICENSE` & `datoso_seed_sfc_msu1-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_sfc_msu1-0.2.3/PKG-INFO` & `datoso_seed_sfc_msu1-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso_seed_sfc_msu1
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_sfc_msu1
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

### Comparing `datoso_seed_sfc_msu1-0.2.3/README.md` & `datoso_seed_sfc_msu1-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_sfc_msu1-0.2.3/pyproject.toml` & `datoso_seed_sfc_msu1-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,24 +10,24 @@
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
-    "datoso-plugin-internetarchive>=0.2.3",
+    "datoso>=0.3.1",
+    "datoso-plugin-internetarchive>=0.3.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_sfc_msu1"
 
 [tool.setuptools]
```

### Comparing `datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/dats.py` & `datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1/rules.py` & `datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_sfc_msu1-0.2.3/src/datoso_seed_sfc_msu1.egg-info/PKG-INFO` & `datoso_seed_sfc_msu1-0.3.0/src/datoso_seed_sfc_msu1.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso-seed-sfc-msu1
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_sfc_msu1
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


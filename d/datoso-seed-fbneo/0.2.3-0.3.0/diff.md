# Comparing `tmp/datoso_seed_fbneo-0.2.3.tar.gz` & `tmp/datoso_seed_fbneo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_fbneo-0.2.3.tar", last modified: Fri May  5 04:11:38 2023, max compression
+gzip compressed data, was "datoso_seed_fbneo-0.3.0.tar", last modified: Sat Jun 10 20:43:03 2023, max compression
```

## Comparing `datoso_seed_fbneo-0.2.3.tar` & `datoso_seed_fbneo-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:11:38.302584 datoso_seed_fbneo-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-05 04:11:38.302584 datoso_seed_fbneo-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:11:38.302584 datoso_seed_fbneo-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:11:38.302584 datoso_seed_fbneo-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:11:38.302584 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-05 04:11:26.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:11:38.302584 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-05 04:11:38.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-05 04:11:38.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:11:38.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 04:11:38.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 04:11:38.000000 datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-10 20:42:51.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:43:03.935021 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-10 20:43:03.000000 datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/top_level.txt
```

### Comparing `datoso_seed_fbneo-0.2.3/LICENSE` & `datoso_seed_fbneo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.2.3/PKG-INFO` & `datoso_seed_fbneo-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso_seed_fbneo
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_fbneo
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

### Comparing `datoso_seed_fbneo-0.2.3/README.md` & `datoso_seed_fbneo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.2.3/pyproject.toml` & `datoso_seed_fbneo-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

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
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_fbneo"
 
 [tool.setuptools]
```

### Comparing `datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/actions.py` & `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/actions.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/dats.py` & `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/fetch.py` & `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo/rules.py` & `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_fbneo-0.2.3/src/datoso_seed_fbneo.egg-info/PKG-INFO` & `datoso_seed_fbneo-0.3.0/src/datoso_seed_fbneo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso-seed-fbneo
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_fbneo
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


# Comparing `tmp/heracless-0.1.0.tar.gz` & `tmp/heracless-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heracless-0.1.0.tar", last modified: Sat Jun 10 17:52:20 2023, max compression
+gzip compressed data, was "heracless-0.1.1.tar", last modified: Sat Jun 10 18:11:20 2023, max compression
```

## Comparing `heracless-0.1.0.tar` & `heracless-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 17:52:20.882801 heracless-0.1.0/
--rw-rw-r--   0 felix     (1000) felix     (1000)     1066 2023-02-14 19:23:45.000000 heracless-0.1.0/LICENSE
--rw-rw-r--   0 felix     (1000) felix     (1000)     2180 2023-06-10 17:52:20.878801 heracless-0.1.0/PKG-INFO
--rw-rw-r--   0 felix     (1000) felix     (1000)     1591 2023-03-03 02:13:37.000000 heracless-0.1.0/README.md
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 17:52:20.878801 heracless-0.1.0/heracless/
--rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-02-13 23:57:18.000000 heracless-0.1.0/heracless/__init__.py
--rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-02-13 23:02:55.000000 heracless-0.1.0/heracless/cli_tool.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     1279 2023-03-03 00:58:59.000000 heracless-0.1.0/heracless/decorator.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     2125 2023-03-03 01:01:39.000000 heracless-0.1.0/heracless/main.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 17:52:20.878801 heracless-0.1.0/heracless/tests/
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 17:52:20.878801 heracless-0.1.0/heracless/tests/config/
--rw-------   0 felix     (1000) felix     (1000)      698 2023-03-03 01:01:39.000000 heracless-0.1.0/heracless/tests/config/types.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     2049 2023-03-03 00:42:36.000000 heracless-0.1.0/heracless/tests/conftest.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      983 2023-03-02 23:41:19.000000 heracless-0.1.0/heracless/tests/load.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      955 2023-03-03 00:58:59.000000 heracless-0.1.0/heracless/tests/test_end_to_end.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      827 2023-03-03 01:01:39.000000 heracless-0.1.0/heracless/tests/test_units.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 17:52:20.878801 heracless-0.1.0/heracless/utils/
--rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-02-14 20:48:31.000000 heracless-0.1.0/heracless/utils/c_types.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     6767 2023-06-10 16:58:13.000000 heracless-0.1.0/heracless/utils/cfg_tree.py
--rw-rw-r--   0 felix     (1000) felix     (1000)      538 2023-03-01 21:15:38.000000 heracless-0.1.0/heracless/utils/exceptions.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 17:52:20.878801 heracless-0.1.0/heracless.egg-info/
--rw-rw-r--   0 felix     (1000) felix     (1000)     2180 2023-06-10 17:52:20.000000 heracless-0.1.0/heracless.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1000) felix     (1000)      532 2023-06-10 17:52:20.000000 heracless-0.1.0/heracless.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-06-10 17:52:20.000000 heracless-0.1.0/heracless.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)       40 2023-06-10 17:52:20.000000 heracless-0.1.0/heracless.egg-info/requires.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)       10 2023-06-10 17:52:20.000000 heracless-0.1.0/heracless.egg-info/top_level.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)      859 2023-06-10 17:52:07.000000 heracless-0.1.0/pyproject.toml
--rw-rw-r--   0 felix     (1000) felix     (1000)      561 2023-06-10 17:22:01.000000 heracless-0.1.0/requirements.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-06-10 17:52:20.882801 heracless-0.1.0/setup.cfg
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 18:11:20.191370 heracless-0.1.1/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1066 2023-02-14 19:23:45.000000 heracless-0.1.1/LICENSE
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2180 2023-06-10 18:11:20.191370 heracless-0.1.1/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1591 2023-03-03 02:13:37.000000 heracless-0.1.1/README.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 18:11:20.187370 heracless-0.1.1/heracless/
+-rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-02-13 23:57:18.000000 heracless-0.1.1/heracless/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-02-13 23:02:55.000000 heracless-0.1.1/heracless/cli_tool.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1279 2023-03-03 00:58:59.000000 heracless-0.1.1/heracless/decorator.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2125 2023-03-03 01:01:39.000000 heracless-0.1.1/heracless/main.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 18:11:20.191370 heracless-0.1.1/heracless/tests/
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 18:11:20.191370 heracless-0.1.1/heracless/tests/config/
+-rw-------   0 felix     (1000) felix     (1000)      698 2023-03-03 01:01:39.000000 heracless-0.1.1/heracless/tests/config/types.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2049 2023-03-03 00:42:36.000000 heracless-0.1.1/heracless/tests/conftest.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      983 2023-03-02 23:41:19.000000 heracless-0.1.1/heracless/tests/load.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      955 2023-03-03 00:58:59.000000 heracless-0.1.1/heracless/tests/test_end_to_end.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      827 2023-03-03 01:01:39.000000 heracless-0.1.1/heracless/tests/test_units.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 18:11:20.191370 heracless-0.1.1/heracless/utils/
+-rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-02-14 20:48:31.000000 heracless-0.1.1/heracless/utils/c_types.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     6767 2023-06-10 16:58:13.000000 heracless-0.1.1/heracless/utils/cfg_tree.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      538 2023-03-01 21:15:38.000000 heracless-0.1.1/heracless/utils/exceptions.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-10 18:11:20.191370 heracless-0.1.1/heracless.egg-info/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2180 2023-06-10 18:11:20.000000 heracless-0.1.1/heracless.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      532 2023-06-10 18:11:20.000000 heracless-0.1.1/heracless.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-06-10 18:11:20.000000 heracless-0.1.1/heracless.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       40 2023-06-10 18:11:20.000000 heracless-0.1.1/heracless.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       10 2023-06-10 18:11:20.000000 heracless-0.1.1/heracless.egg-info/top_level.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)      859 2023-06-10 18:09:08.000000 heracless-0.1.1/pyproject.toml
+-rw-rw-r--   0 felix     (1000) felix     (1000)      561 2023-06-10 17:22:01.000000 heracless-0.1.1/requirements.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-06-10 18:11:20.195370 heracless-0.1.1/setup.cfg
```

### Comparing `heracless-0.1.0/LICENSE` & `heracless-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/PKG-INFO` & `heracless-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heracless
-Version: 0.1.0
+Version: 0.1.1
 Summary: Yaml to Dataclass parser for Config files
 Author-email: Felix Schelling <felix.schelling@protonmail.com>
 Project-URL: Homepage, https://github.com/felixscode/heracless
 Keywords: YMAL,Dataclass,Config
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `heracless-0.1.0/README.md` & `heracless-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/decorator.py` & `heracless-0.1.1/heracless/decorator.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/main.py` & `heracless-0.1.1/heracless/main.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/tests/config/types.py` & `heracless-0.1.1/heracless/tests/config/types.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/tests/conftest.py` & `heracless-0.1.1/heracless/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/tests/load.py` & `heracless-0.1.1/heracless/tests/load.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/tests/test_end_to_end.py` & `heracless-0.1.1/heracless/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/tests/test_units.py` & `heracless-0.1.1/heracless/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/utils/cfg_tree.py` & `heracless-0.1.1/heracless/utils/cfg_tree.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless/utils/exceptions.py` & `heracless-0.1.1/heracless/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/heracless.egg-info/PKG-INFO` & `heracless-0.1.1/heracless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heracless
-Version: 0.1.0
+Version: 0.1.1
 Summary: Yaml to Dataclass parser for Config files
 Author-email: Felix Schelling <felix.schelling@protonmail.com>
 Project-URL: Homepage, https://github.com/felixscode/heracless
 Keywords: YMAL,Dataclass,Config
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `heracless-0.1.0/heracless.egg-info/SOURCES.txt` & `heracless-0.1.1/heracless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heracless-0.1.0/pyproject.toml` & `heracless-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 target-version = ['py311']
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "heracless"
-version = "0.1.0"
+version = "0.1.1"
 description = "Yaml to Dataclass parser for Config files"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{ name = "Felix Schelling", email = "felix.schelling@protonmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `heracless-0.1.0/requirements.txt` & `heracless-0.1.1/requirements.txt`

 * *Files identical despite different names*


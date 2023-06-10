# Comparing `tmp/remla23-team10-preprocessing-1.2.0.tar.gz` & `tmp/remla23-team10-preprocessing-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla23-team10-preprocessing-1.2.0.tar", last modified: Sat Jun 10 20:52:25 2023, max compression
+gzip compressed data, was "remla23-team10-preprocessing-2.0.0.tar", last modified: Sat Jun 10 20:56:57 2023, max compression
```

## Comparing `remla23-team10-preprocessing-1.2.0.tar` & `remla23-team10-preprocessing-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:52:25.690983 remla23-team10-preprocessing-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-10 20:52:16.000000 remla23-team10-preprocessing-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-10 20:52:25.690983 remla23-team10-preprocessing-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-10 20:52:16.000000 remla23-team10-preprocessing-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-10 20:52:17.000000 remla23-team10-preprocessing-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:52:25.690983 remla23-team10-preprocessing-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:52:25.690983 remla23-team10-preprocessing-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:52:25.690983 remla23-team10-preprocessing-1.2.0/src/remla23-team10-preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-10 20:52:16.000000 remla23-team10-preprocessing-1.2.0/src/remla23-team10-preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-10 20:52:16.000000 remla23-team10-preprocessing-1.2.0/src/remla23-team10-preprocessing/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-10 20:52:16.000000 remla23-team10-preprocessing-1.2.0/src/remla23-team10-preprocessing/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:52:25.690983 remla23-team10-preprocessing-1.2.0/src/remla23_team10_preprocessing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-10 20:52:25.000000 remla23-team10-preprocessing-1.2.0/src/remla23_team10_preprocessing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-10 20:52:25.000000 remla23-team10-preprocessing-1.2.0/src/remla23_team10_preprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:52:25.000000 remla23-team10-preprocessing-1.2.0/src/remla23_team10_preprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-10 20:52:25.000000 remla23-team10-preprocessing-1.2.0/src/remla23_team10_preprocessing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-10 20:52:25.000000 remla23-team10-preprocessing-1.2.0/src/remla23_team10_preprocessing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:56:57.746566 remla23-team10-preprocessing-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-10 20:56:47.000000 remla23-team10-preprocessing-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-10 20:56:57.746566 remla23-team10-preprocessing-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-10 20:56:47.000000 remla23-team10-preprocessing-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-10 20:56:47.000000 remla23-team10-preprocessing-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:56:57.746566 remla23-team10-preprocessing-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:56:57.742566 remla23-team10-preprocessing-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:56:57.746566 remla23-team10-preprocessing-2.0.0/src/remla23_team10_preprocessing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-10 20:56:57.000000 remla23-team10-preprocessing-2.0.0/src/remla23_team10_preprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-10 20:56:57.000000 remla23-team10-preprocessing-2.0.0/src/remla23_team10_preprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:56:57.000000 remla23-team10-preprocessing-2.0.0/src/remla23_team10_preprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-10 20:56:57.000000 remla23-team10-preprocessing-2.0.0/src/remla23_team10_preprocessing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 20:56:57.000000 remla23-team10-preprocessing-2.0.0/src/remla23_team10_preprocessing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:56:57.746566 remla23-team10-preprocessing-2.0.0/src/restaurant_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-10 20:56:47.000000 remla23-team10-preprocessing-2.0.0/src/restaurant_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-10 20:56:47.000000 remla23-team10-preprocessing-2.0.0/src/restaurant_preprocessing/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-10 20:56:47.000000 remla23-team10-preprocessing-2.0.0/src/restaurant_preprocessing/version_util.py
```

### Comparing `remla23-team10-preprocessing-1.2.0/LICENSE` & `remla23-team10-preprocessing-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remla23-team10-preprocessing-1.2.0/PKG-INFO` & `remla23-team10-preprocessing-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remla23-team10-preprocessing
-Version: 1.2.0
+Version: 2.0.0
 Summary: Preprocessing for the REMLA project
 Author-email: REMLA23 Team 10 <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `remla23-team10-preprocessing-1.2.0/pyproject.toml` & `remla23-team10-preprocessing-2.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "remla23-team10-preprocessing"
-version = "1.2.0"
+version = "2.0.0"
 authors = [
   { name="REMLA23 Team 10", email="author@example.com" },
 ]
 description = "Preprocessing for the REMLA project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `remla23-team10-preprocessing-1.2.0/src/remla23-team10-preprocessing/preprocessing.py` & `remla23-team10-preprocessing-2.0.0/src/restaurant_preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `remla23-team10-preprocessing-1.2.0/src/remla23_team10_preprocessing.egg-info/PKG-INFO` & `remla23-team10-preprocessing-2.0.0/src/remla23_team10_preprocessing.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remla23-team10-preprocessing
-Version: 1.2.0
+Version: 2.0.0
 Summary: Preprocessing for the REMLA project
 Author-email: REMLA23 Team 10 <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```


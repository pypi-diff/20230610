# Comparing `tmp/autogluon-0.7.1b20230609.tar.gz` & `tmp/autogluon-0.7.1b20230610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.7.1b20230609.tar", last modified: Fri Jun  9 09:04:16 2023, max compression
+gzip compressed data, was "autogluon-0.7.1b20230610.tar", last modified: Sat Jun 10 09:04:18 2023, max compression
```

## Comparing `autogluon-0.7.1b20230609.tar` & `autogluon-0.7.1b20230610.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:16.442498 autogluon-0.7.1b20230609/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-09 09:04:16.442498 autogluon-0.7.1b20230609/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:04:16.442498 autogluon-0.7.1b20230609/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-09 09:03:31.000000 autogluon-0.7.1b20230609/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:16.438497 autogluon-0.7.1b20230609/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:16.438497 autogluon-0.7.1b20230609/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:16.442498 autogluon-0.7.1b20230609/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:03:31.000000 autogluon-0.7.1b20230609/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:16.442498 autogluon-0.7.1b20230609/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-09 09:04:16.000000 autogluon-0.7.1b20230609/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 09:04:16.000000 autogluon-0.7.1b20230609/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:16.000000 autogluon-0.7.1b20230609/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:16.000000 autogluon-0.7.1b20230609/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 09:04:16.000000 autogluon-0.7.1b20230609/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:16.000000 autogluon-0.7.1b20230609/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:16.000000 autogluon-0.7.1b20230609/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:18.756293 autogluon-0.7.1b20230610/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-10 09:04:18.756293 autogluon-0.7.1b20230610/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:04:18.756293 autogluon-0.7.1b20230610/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-10 09:03:29.000000 autogluon-0.7.1b20230610/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:18.752293 autogluon-0.7.1b20230610/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:18.752293 autogluon-0.7.1b20230610/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:18.756293 autogluon-0.7.1b20230610/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:03:29.000000 autogluon-0.7.1b20230610/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:04:18.756293 autogluon-0.7.1b20230610/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-10 09:04:18.000000 autogluon-0.7.1b20230610/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-10 09:04:18.000000 autogluon-0.7.1b20230610/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:04:18.000000 autogluon-0.7.1b20230610/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 09:04:18.000000 autogluon-0.7.1b20230610/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-10 09:04:18.000000 autogluon-0.7.1b20230610/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 09:04:18.000000 autogluon-0.7.1b20230610/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:04:18.000000 autogluon-0.7.1b20230610/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.7.1b20230609/PKG-INFO` & `autogluon-0.7.1b20230610/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230609
+Version: 0.7.1b20230610
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.7.1b20230609/setup.py` & `autogluon-0.7.1b20230610/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.7.1b20230609/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.7.1b20230610/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230609
+Version: 0.7.1b20230610
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```


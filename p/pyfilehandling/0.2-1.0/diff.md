# Comparing `tmp/pyfilehandling-0.2.tar.gz` & `tmp/pyfilehandling-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfilehandling-0.2.tar", last modified: Sat Jun 10 05:23:11 2023, max compression
+gzip compressed data, was "pyfilehandling-1.0.tar", last modified: Sat Jun 10 06:19:13 2023, max compression
```

## Comparing `pyfilehandling-0.2.tar` & `pyfilehandling-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:23:11.535790 pyfilehandling-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 05:22:54.000000 pyfilehandling-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 05:23:11.535790 pyfilehandling-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 05:22:54.000000 pyfilehandling-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:23:11.531790 pyfilehandling-0.2/pyfilehandling/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-10 05:22:54.000000 pyfilehandling-0.2/pyfilehandling/FileIO.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 05:22:54.000000 pyfilehandling-0.2/pyfilehandling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:23:11.531790 pyfilehandling-0.2/pyfilehandling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 05:23:11.535790 pyfilehandling-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 05:22:54.000000 pyfilehandling-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:19:13.765364 pyfilehandling-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 06:19:02.000000 pyfilehandling-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 06:19:13.765364 pyfilehandling-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 06:19:02.000000 pyfilehandling-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:19:13.765364 pyfilehandling-1.0/pyfilehandling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-10 06:19:02.000000 pyfilehandling-1.0/pyfilehandling/FileIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 06:19:02.000000 pyfilehandling-1.0/pyfilehandling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 06:19:13.765364 pyfilehandling-1.0/pyfilehandling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 06:19:13.000000 pyfilehandling-1.0/pyfilehandling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 06:19:13.000000 pyfilehandling-1.0/pyfilehandling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 06:19:13.000000 pyfilehandling-1.0/pyfilehandling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-10 06:19:13.000000 pyfilehandling-1.0/pyfilehandling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 06:19:13.769364 pyfilehandling-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 06:19:02.000000 pyfilehandling-1.0/setup.py
```

### Comparing `pyfilehandling-0.2/LICENSE` & `pyfilehandling-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfilehandling-0.2/PKG-INFO` & `pyfilehandling-1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilehandling
-Version: 0.2
+Version: 1.0
 Summary: A Python package for file manipulation operations.
 Home-page: https://github.com/JeelDobariya38/pyfilehandling
 Author: JeelDobariya
 Author-email: dobariyaj34@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JeelDobariya38/pyfilehandling/issues
 Project-URL: Documentation, https://jeeldobariya38.github.io/pyfilehandling/
```

### Comparing `pyfilehandling-0.2/pyfilehandling.egg-info/PKG-INFO` & `pyfilehandling-1.0/pyfilehandling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilehandling
-Version: 0.2
+Version: 1.0
 Summary: A Python package for file manipulation operations.
 Home-page: https://github.com/JeelDobariya38/pyfilehandling
 Author: JeelDobariya
 Author-email: dobariyaj34@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JeelDobariya38/pyfilehandling/issues
 Project-URL: Documentation, https://jeeldobariya38.github.io/pyfilehandling/
```

### Comparing `pyfilehandling-0.2/setup.py` & `pyfilehandling-1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pyfilehandling',
-    version='0.2',
+    version='1.0',
     description='A Python package for file manipulation operations.',
     long_description='pyfilehandling is a Python package that provides functions and classes for handling file operations, including creating files and directories, reading and writing data, and more.',
     long_description_content_type='text/markdown',
     author='JeelDobariya',
     author_email='dobariyaj34@gmail.com',
     url='https://github.com/JeelDobariya38/pyfilehandling',
     packages=['pyfilehandling'],
```


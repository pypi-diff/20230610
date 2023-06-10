# Comparing `tmp/pyfilehandling-1.1.tar.gz` & `tmp/pyfilehandling-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfilehandling-1.1.tar", last modified: Sat Jun 10 09:55:45 2023, max compression
+gzip compressed data, was "pyfilehandling-1.1.1.tar", last modified: Sat Jun 10 10:11:27 2023, max compression
```

## Comparing `pyfilehandling-1.1.tar` & `pyfilehandling-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:55:45.404965 pyfilehandling-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 09:55:34.000000 pyfilehandling-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 09:55:45.404965 pyfilehandling-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 09:55:34.000000 pyfilehandling-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:55:45.404965 pyfilehandling-1.1/pyfilehandling/
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-10 09:55:34.000000 pyfilehandling-1.1/pyfilehandling/FileIO.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 09:55:34.000000 pyfilehandling-1.1/pyfilehandling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:55:45.404965 pyfilehandling-1.1/pyfilehandling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 09:55:45.000000 pyfilehandling-1.1/pyfilehandling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 09:55:45.000000 pyfilehandling-1.1/pyfilehandling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:55:45.000000 pyfilehandling-1.1/pyfilehandling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-10 09:55:45.000000 pyfilehandling-1.1/pyfilehandling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:55:45.404965 pyfilehandling-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 09:55:34.000000 pyfilehandling-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:11:27.493088 pyfilehandling-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 10:11:11.000000 pyfilehandling-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-10 10:11:27.493088 pyfilehandling-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 10:11:11.000000 pyfilehandling-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:11:27.493088 pyfilehandling-1.1.1/pyfilehandling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-10 10:11:11.000000 pyfilehandling-1.1.1/pyfilehandling/FileIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-10 10:11:11.000000 pyfilehandling-1.1.1/pyfilehandling/TypeFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 10:11:11.000000 pyfilehandling-1.1.1/pyfilehandling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:11:27.493088 pyfilehandling-1.1.1/pyfilehandling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-10 10:11:27.000000 pyfilehandling-1.1.1/pyfilehandling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-10 10:11:27.000000 pyfilehandling-1.1.1/pyfilehandling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 10:11:27.000000 pyfilehandling-1.1.1/pyfilehandling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-10 10:11:27.000000 pyfilehandling-1.1.1/pyfilehandling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 10:11:27.493088 pyfilehandling-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-10 10:11:11.000000 pyfilehandling-1.1.1/setup.py
```

### Comparing `pyfilehandling-1.1/LICENSE` & `pyfilehandling-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfilehandling-1.1/PKG-INFO` & `pyfilehandling-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilehandling
-Version: 1.1
+Version: 1.1.1
 Summary: A Python package for file manipulation operations.
 Home-page: https://github.com/JeelDobariya38/pyfilehandling
 Author: JeelDobariya
 Author-email: dobariyaj34@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JeelDobariya38/pyfilehandling/issues
 Project-URL: Documentation, https://jeeldobariya38.github.io/pyfilehandling/
```

### Comparing `pyfilehandling-1.1/pyfilehandling/FileIO.py` & `pyfilehandling-1.1.1/pyfilehandling/FileIO.py`

 * *Files identical despite different names*

### Comparing `pyfilehandling-1.1/pyfilehandling.egg-info/PKG-INFO` & `pyfilehandling-1.1.1/pyfilehandling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilehandling
-Version: 1.1
+Version: 1.1.1
 Summary: A Python package for file manipulation operations.
 Home-page: https://github.com/JeelDobariya38/pyfilehandling
 Author: JeelDobariya
 Author-email: dobariyaj34@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JeelDobariya38/pyfilehandling/issues
 Project-URL: Documentation, https://jeeldobariya38.github.io/pyfilehandling/
```

### Comparing `pyfilehandling-1.1/setup.py` & `pyfilehandling-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pyfilehandling',
-    version='1.1',
+    version='1.1.1',
     description='A Python package for file manipulation operations.',
     long_description='pyfilehandling is a Python package that provides functions and classes for handling file operations, including creating files and directories, reading and writing data, and more.',
     long_description_content_type='text/markdown',
     author='JeelDobariya',
     author_email='dobariyaj34@gmail.com',
     url='https://github.com/JeelDobariya38/pyfilehandling',
     packages=['pyfilehandling'],
```


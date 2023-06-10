# Comparing `tmp/pyfilehandling-0.1.tar.gz` & `tmp/pyfilehandling-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfilehandling-0.1.tar", last modified: Fri Jun  9 16:29:28 2023, max compression
+gzip compressed data, was "pyfilehandling-0.2.tar", last modified: Sat Jun 10 05:23:11 2023, max compression
```

## Comparing `pyfilehandling-0.1.tar` & `pyfilehandling-0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:29:28.253593 pyfilehandling-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 16:29:19.000000 pyfilehandling-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-09 16:29:28.253593 pyfilehandling-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 16:29:19.000000 pyfilehandling-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:29:28.249593 pyfilehandling-0.1/pyfilehandling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-09 16:29:28.000000 pyfilehandling-0.1/pyfilehandling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 16:29:28.000000 pyfilehandling-0.1/pyfilehandling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:29:28.000000 pyfilehandling-0.1/pyfilehandling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 16:29:28.000000 pyfilehandling-0.1/pyfilehandling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 16:29:28.253593 pyfilehandling-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-09 16:29:19.000000 pyfilehandling-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:29:28.249593 pyfilehandling-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:29:28.253593 pyfilehandling-0.1/src/pyfilehandling/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 16:29:19.000000 pyfilehandling-0.1/src/pyfilehandling/FileIO.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 16:29:19.000000 pyfilehandling-0.1/src/pyfilehandling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:23:11.535790 pyfilehandling-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 05:22:54.000000 pyfilehandling-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 05:23:11.535790 pyfilehandling-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 05:22:54.000000 pyfilehandling-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:23:11.531790 pyfilehandling-0.2/pyfilehandling/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-10 05:22:54.000000 pyfilehandling-0.2/pyfilehandling/FileIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 05:22:54.000000 pyfilehandling-0.2/pyfilehandling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:23:11.531790 pyfilehandling-0.2/pyfilehandling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-10 05:23:11.000000 pyfilehandling-0.2/pyfilehandling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 05:23:11.535790 pyfilehandling-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 05:22:54.000000 pyfilehandling-0.2/setup.py
```

### Comparing `pyfilehandling-0.1/LICENSE` & `pyfilehandling-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfilehandling-0.1/PKG-INFO` & `pyfilehandling-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilehandling
-Version: 0.1
+Version: 0.2
 Summary: A Python package for file manipulation operations.
 Home-page: https://github.com/JeelDobariya38/pyfilehandling
 Author: JeelDobariya
 Author-email: dobariyaj34@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JeelDobariya38/pyfilehandling/issues
 Project-URL: Documentation, https://jeeldobariya38.github.io/pyfilehandling/
```

### Comparing `pyfilehandling-0.1/pyfilehandling.egg-info/PKG-INFO` & `pyfilehandling-0.2/pyfilehandling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilehandling
-Version: 0.1
+Version: 0.2
 Summary: A Python package for file manipulation operations.
 Home-page: https://github.com/JeelDobariya38/pyfilehandling
 Author: JeelDobariya
 Author-email: dobariyaj34@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JeelDobariya38/pyfilehandling/issues
 Project-URL: Documentation, https://jeeldobariya38.github.io/pyfilehandling/
```

### Comparing `pyfilehandling-0.1/setup.py` & `pyfilehandling-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='pyfilehandling',
-    version='0.1',
+    version='0.2',
     description='A Python package for file manipulation operations.',
     long_description='pyfilehandling is a Python package that provides functions and classes for handling file operations, including creating files and directories, reading and writing data, and more.',
     long_description_content_type='text/markdown',
     author='JeelDobariya',
     author_email='dobariyaj34@gmail.com',
     url='https://github.com/JeelDobariya38/pyfilehandling',
-    packages=['src.pyfilehandling'],
+    packages=['pyfilehandling'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```


# Comparing `tmp/pybreaker-1.0.1.tar.gz` & `tmp/pybreaker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybreaker-1.0.1.tar", last modified: Fri Aug 12 01:35:09 2022, max compression
+gzip compressed data, was "pybreaker-1.0.2.tar", last modified: Sat Jun 10 01:16:41 2023, max compression
```

## Comparing `pybreaker-1.0.1.tar` & `pybreaker-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 danielfm  (1000) danielfm  (1000)        0 2022-08-12 01:35:09.193573 pybreaker-1.0.1/
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)     1550 2022-03-02 21:56:07.000000 pybreaker-1.0.1/LICENSE
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)     9211 2022-08-12 01:35:09.193573 pybreaker-1.0.1/PKG-INFO
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)     8553 2022-08-11 12:48:50.000000 pybreaker-1.0.1/README.rst
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)      184 2022-08-11 12:48:50.000000 pybreaker-1.0.1/pyproject.toml
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)       38 2022-08-12 01:35:09.193573 pybreaker-1.0.1/setup.cfg
--rwxr-xr-x   0 danielfm  (1000) danielfm  (1000)     1086 2022-08-12 01:34:10.000000 pybreaker-1.0.1/setup.py
-drwxr-xr-x   0 danielfm  (1000) danielfm  (1000)        0 2022-08-12 01:35:09.190573 pybreaker-1.0.1/src/
-drwxr-xr-x   0 danielfm  (1000) danielfm  (1000)        0 2022-08-12 01:35:09.192573 pybreaker-1.0.1/src/pybreaker.egg-info/
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)     9211 2022-08-12 01:35:09.000000 pybreaker-1.0.1/src/pybreaker.egg-info/PKG-INFO
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)      279 2022-08-12 01:35:09.000000 pybreaker-1.0.1/src/pybreaker.egg-info/SOURCES.txt
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)        1 2022-08-12 01:35:09.000000 pybreaker-1.0.1/src/pybreaker.egg-info/dependency_links.txt
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)        1 2021-12-14 15:05:53.000000 pybreaker-1.0.1/src/pybreaker.egg-info/not-zip-safe
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)       53 2022-08-12 01:35:09.000000 pybreaker-1.0.1/src/pybreaker.egg-info/requires.txt
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)       10 2022-08-12 01:35:09.000000 pybreaker-1.0.1/src/pybreaker.egg-info/top_level.txt
--rw-r--r--   0 danielfm  (1000) danielfm  (1000)    31362 2022-08-12 01:34:08.000000 pybreaker-1.0.1/src/pybreaker.py
+drwxr-xr-x   0 danielfm  (1000) danielfm  (1000)        0 2023-06-10 01:16:41.217962 pybreaker-1.0.2/
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)     1550 2023-06-10 01:11:25.000000 pybreaker-1.0.2/LICENSE
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)     9211 2023-06-10 01:16:41.217962 pybreaker-1.0.2/PKG-INFO
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)     8553 2023-05-23 22:05:59.000000 pybreaker-1.0.2/README.rst
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)      184 2023-06-10 01:11:05.000000 pybreaker-1.0.2/pyproject.toml
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)       38 2023-06-10 01:16:41.217962 pybreaker-1.0.2/setup.cfg
+-rwxr-xr-x   0 danielfm  (1000) danielfm  (1000)     1085 2023-06-10 01:11:36.000000 pybreaker-1.0.2/setup.py
+drwxr-xr-x   0 danielfm  (1000) danielfm  (1000)        0 2023-06-10 01:16:41.216962 pybreaker-1.0.2/src/
+drwxr-xr-x   0 danielfm  (1000) danielfm  (1000)        0 2023-06-10 01:16:41.217962 pybreaker-1.0.2/src/pybreaker.egg-info/
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)     9211 2023-06-10 01:16:41.000000 pybreaker-1.0.2/src/pybreaker.egg-info/PKG-INFO
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)      279 2023-06-10 01:16:41.000000 pybreaker-1.0.2/src/pybreaker.egg-info/SOURCES.txt
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)        1 2023-06-10 01:16:41.000000 pybreaker-1.0.2/src/pybreaker.egg-info/dependency_links.txt
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)        1 2023-06-10 01:15:53.000000 pybreaker-1.0.2/src/pybreaker.egg-info/not-zip-safe
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)       53 2023-06-10 01:16:41.000000 pybreaker-1.0.2/src/pybreaker.egg-info/requires.txt
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)       10 2023-06-10 01:16:41.000000 pybreaker-1.0.2/src/pybreaker.egg-info/top_level.txt
+-rw-r--r--   0 danielfm  (1000) danielfm  (1000)    31362 2023-06-10 01:11:05.000000 pybreaker-1.0.2/src/pybreaker.py
```

### Comparing `pybreaker-1.0.1/LICENSE` & `pybreaker-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybreaker-1.0.1/PKG-INFO` & `pybreaker-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybreaker
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python implementation of the Circuit Breaker pattern
 Home-page: http://github.com/danielfm/pybreaker
 Author: Daniel Fernandes Martins
 Author-email: daniel.tritone@gmail.com
 License: BSD
 Keywords: design,pattern,circuit,breaker,integration
 Platform: Any
```

### Comparing `pybreaker-1.0.1/README.rst` & `pybreaker-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pybreaker-1.0.1/setup.py` & `pybreaker-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pybreaker",
-    version="1.0.1",
+    version="1.0.2",
     description="Python implementation of the Circuit Breaker pattern",
     long_description=open("README.rst", "r").read(),
     keywords=["design", "pattern", "circuit", "breaker", "integration"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
@@ -22,9 +22,9 @@
     package_dir={"": "src"},
     py_modules=["pybreaker"],
     include_package_data=True,
     install_requires=["typing_extensions>=3.10.0; python_version < '3.8'"],
     zip_safe=False,
     python_requires=">=3.7",
     test_suite="tests",
-    tests_require=["mock", "fakeredis==0.16.0", "redis==2.10.6", "tornado"],
+    tests_require=["mock", "fakeredis==2.14.1", "redis==4.5.5", "tornado"],
 )
```

### Comparing `pybreaker-1.0.1/src/pybreaker.egg-info/PKG-INFO` & `pybreaker-1.0.2/src/pybreaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybreaker
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python implementation of the Circuit Breaker pattern
 Home-page: http://github.com/danielfm/pybreaker
 Author: Daniel Fernandes Martins
 Author-email: daniel.tritone@gmail.com
 License: BSD
 Keywords: design,pattern,circuit,breaker,integration
 Platform: Any
```

### Comparing `pybreaker-1.0.1/src/pybreaker.py` & `pybreaker-1.0.2/src/pybreaker.py`

 * *Files identical despite different names*


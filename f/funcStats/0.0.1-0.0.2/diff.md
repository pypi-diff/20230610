# Comparing `tmp/funcStats-0.0.1.tar.gz` & `tmp/funcStats-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.0.1.tar", last modified: Sat Jun 10 01:38:42 2023, max compression
+gzip compressed data, was "funcStats-0.0.2.tar", last modified: Sat Jun 10 01:51:36 2023, max compression
```

## Comparing `funcStats-0.0.1.tar` & `funcStats-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:38:42.291361 funcStats-0.0.1/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-06-10 01:38:42.290765 funcStats-0.0.1/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:38:42.288714 funcStats-0.0.1/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-06-10 01:38:42.000000 funcStats-0.0.1/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      202 2023-06-10 01:38:42.000000 funcStats-0.0.1/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-10 01:38:42.000000 funcStats-0.0.1/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-10 01:38:42.000000 funcStats-0.0.1/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-10 01:38:42.000000 funcStats-0.0.1/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-10 01:38:42.291532 funcStats-0.0.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      873 2023-06-10 01:36:49.000000 funcStats-0.0.1/setup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:38:42.289597 funcStats-0.0.1/utilities/
--rw-r--r--   0 tom        (501) staff       (20)      582 2023-06-10 01:33:42.000000 funcStats-0.0.1/utilities/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:51:36.074447 funcStats-0.0.2/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)      607 2023-06-10 01:51:36.073681 funcStats-0.0.2/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:51:36.071801 funcStats-0.0.2/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      607 2023-06-10 01:51:36.000000 funcStats-0.0.2/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      202 2023-06-10 01:51:36.000000 funcStats-0.0.2/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-10 01:51:36.000000 funcStats-0.0.2/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-10 01:51:36.000000 funcStats-0.0.2/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-10 01:51:36.000000 funcStats-0.0.2/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-10 01:51:36.074710 funcStats-0.0.2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      873 2023-06-10 01:51:23.000000 funcStats-0.0.2/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:51:36.072545 funcStats-0.0.2/utilities/
+-rw-r--r--   0 tom        (501) staff       (20)      582 2023-06-10 01:33:42.000000 funcStats-0.0.2/utilities/__init__.py
```

### Comparing `funcStats-0.0.1/LICENSE` & `funcStats-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.1/PKG-INFO` & `funcStats-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.1/funcStats.egg-info/PKG-INFO` & `funcStats-0.0.2/funcStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.1/setup.py` & `funcStats-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A module that helps to evaluate functions when some tests are needed'
 LONG_DESCRIPTION = ''
 
 setup(
     name="funcStats",
     version=VERSION,
     author="Elemental (Tom Neto)",
```

### Comparing `funcStats-0.0.1/utilities/__init__.py` & `funcStats-0.0.2/utilities/__init__.py`

 * *Files identical despite different names*


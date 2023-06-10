# Comparing `tmp/funcStats-0.0.3.tar.gz` & `tmp/funcStats-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.0.3.tar", last modified: Sat Jun 10 01:56:55 2023, max compression
+gzip compressed data, was "funcStats-0.0.4.tar", last modified: Sat Jun 10 02:40:01 2023, max compression
```

## Comparing `funcStats-0.0.3.tar` & `funcStats-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:56:55.172218 funcStats-0.0.3/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.3/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-06-10 01:56:55.171399 funcStats-0.0.3/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:56:55.164947 funcStats-0.0.3/funcStats/
--rw-r--r--   0 tom        (501) staff       (20)      582 2023-06-10 01:33:42.000000 funcStats-0.0.3/funcStats/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 01:56:55.170031 funcStats-0.0.3/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-06-10 01:56:55.000000 funcStats-0.0.3/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      202 2023-06-10 01:56:55.000000 funcStats-0.0.3/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-10 01:56:55.000000 funcStats-0.0.3/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-10 01:56:55.000000 funcStats-0.0.3/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-10 01:56:55.000000 funcStats-0.0.3/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-10 01:56:55.172378 funcStats-0.0.3/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      873 2023-06-10 01:56:11.000000 funcStats-0.0.3/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 02:40:01.835934 funcStats-0.0.4/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.4/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     1797 2023-06-10 02:40:01.835464 funcStats-0.0.4/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 02:40:01.830453 funcStats-0.0.4/funcStats/
+-rw-r--r--   0 tom        (501) staff       (20)      758 2023-06-10 02:26:48.000000 funcStats-0.0.4/funcStats/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-10 02:40:01.834337 funcStats-0.0.4/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     1797 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      202 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-10 02:40:01.000000 funcStats-0.0.4/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-10 02:40:01.836035 funcStats-0.0.4/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     1018 2023-06-10 02:39:53.000000 funcStats-0.0.4/setup.py
```

### Comparing `funcStats-0.0.3/LICENSE` & `funcStats-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.3/setup.py` & `funcStats-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import os.path
+
 from setuptools import setup, find_packages
+from pathlib import Path
+this_directory = Path(__file__).parent
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A module that helps to evaluate functions when some tests are needed'
-LONG_DESCRIPTION = ''
+LONG_DESCRIPTION = str(open('/Volumes/Projetos/Git/funcStats/README.MD', 'r').read())
 
 setup(
     name="funcStats",
     version=VERSION,
     author="Elemental (Tom Neto)",
     author_email="<info@elemental.run>",
     description=DESCRIPTION,
@@ -19,8 +23,8 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```


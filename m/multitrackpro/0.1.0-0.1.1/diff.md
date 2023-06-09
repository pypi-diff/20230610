# Comparing `tmp/multitrackpro-0.1.0.tar.gz` & `tmp/multitrackpro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multitrackpro-0.1.0.tar", last modified: Fri Jun  9 13:03:43 2023, max compression
+gzip compressed data, was "multitrackpro-0.1.1.tar", last modified: Fri Jun  9 22:34:21 2023, max compression
```

## Comparing `multitrackpro-0.1.0.tar` & `multitrackpro-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/
--rw-rw-r--   0 sk        (1000) sk        (1000)      165 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/AUTHORS.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     3611 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       89 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/HISTORY.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     1613 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/LICENSE
--rw-rw-r--   0 sk        (1000) sk        (1000)      262 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/MANIFEST.in
--rw-rw-r--   0 sk        (1000) sk        (1000)     2038 2023-06-09 13:03:43.280503 multitrackpro-0.1.0/PKG-INFO
--rw-rw-r--   0 sk        (1000) sk        (1000)      985 2023-06-09 13:02:50.000000 multitrackpro-0.1.0/README.rst
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/docs/
--rw-rw-r--   0 sk        (1000) sk        (1000)      614 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/Makefile
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/docs/_build/
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/docs/_build/html/
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/docs/_build/html/_static/
--rw-rw-r--   0 sk        (1000) sk        (1000)      286 2022-07-14 07:38:19.000000 multitrackpro-0.1.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2022-07-14 07:38:19.000000 multitrackpro-0.1.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2022-07-14 07:38:19.000000 multitrackpro-0.1.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/authors.rst
--rwxrwxr-x   0 sk        (1000) sk        (1000)     4868 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/conf.py
--rw-rw-r--   0 sk        (1000) sk        (1000)       33 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/contributing.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/history.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      310 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/index.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     1182 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/installation.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      811 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/make.bat
--rw-rw-r--   0 sk        (1000) sk        (1000)       27 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/readme.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/docs/usage.rst
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/multitrackpro/
--rw-rw-r--   0 sk        (1000) sk        (1000)      140 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/multitrackpro/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)       19 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/multitrackpro/multitrackpro.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/multitrackpro.egg-info/
--rw-rw-r--   0 sk        (1000) sk        (1000)     2038 2023-06-09 13:03:43.000000 multitrackpro-0.1.0/multitrackpro.egg-info/PKG-INFO
--rw-rw-r--   0 sk        (1000) sk        (1000)      645 2023-06-09 13:03:43.000000 multitrackpro-0.1.0/multitrackpro.egg-info/SOURCES.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 13:03:43.000000 multitrackpro-0.1.0/multitrackpro.egg-info/dependency_links.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 11:25:09.000000 multitrackpro-0.1.0/multitrackpro.egg-info/not-zip-safe
--rw-rw-r--   0 sk        (1000) sk        (1000)       14 2023-06-09 13:03:43.000000 multitrackpro-0.1.0/multitrackpro.egg-info/top_level.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)      385 2023-06-09 13:03:43.280503 multitrackpro-0.1.0/setup.cfg
--rw-rw-r--   0 sk        (1000) sk        (1000)     1535 2023-06-09 13:03:40.000000 multitrackpro-0.1.0/setup.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 13:03:43.276503 multitrackpro-0.1.0/tests/
--rw-rw-r--   0 sk        (1000) sk        (1000)       43 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/tests/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)      417 2023-06-09 10:59:19.000000 multitrackpro-0.1.0/tests/test_multitrackpro.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      165 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/AUTHORS.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3611 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      179 2023-06-09 20:51:56.000000 multitrackpro-0.1.1/HISTORY.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1613 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/LICENSE
+-rw-rw-r--   0 sk        (1000) sk        (1000)      262 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/MANIFEST.in
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3242 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/PKG-INFO
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1647 2023-06-09 21:56:44.000000 multitrackpro-0.1.1/README.rst
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/docs/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      614 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/Makefile
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.763862 multitrackpro-0.1.1/docs/_build/
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.763862 multitrackpro-0.1.1/docs/_build/html/
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/docs/_build/html/_static/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      286 2023-06-09 12:32:19.000000 multitrackpro-0.1.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/authors.rst
+-rwxrwxr-x   0 sk        (1000) sk        (1000)     4868 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/conf.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)       33 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/contributing.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/history.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      310 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/index.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1182 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/installation.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      811 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/make.bat
+-rw-rw-r--   0 sk        (1000) sk        (1000)       73 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/modules.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      632 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.core.io.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      645 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.core.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      374 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.qt.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      784 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       27 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/readme.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/usage.rst
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/multitracker/
+-rw-rw-r--   0 sk        (1000) sk        (1000)     4395 2023-06-09 20:50:32.000000 multitrackpro-0.1.1/multitracker/auto_annotate_pro.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/multitrackpro.egg-info/
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3242 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/PKG-INFO
+-rw-rw-r--   0 sk        (1000) sk        (1000)      819 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/SOURCES.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/dependency_links.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)       61 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/entry_points.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/not-zip-safe
+-rw-rw-r--   0 sk        (1000) sk        (1000)       65 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/requires.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/top_level.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)      407 2023-06-09 22:34:21.771862 multitrackpro-0.1.1/setup.cfg
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2235 2023-06-09 22:18:53.000000 multitrackpro-0.1.1/setup.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/tests/
+-rw-rw-r--   0 sk        (1000) sk        (1000)       43 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/tests/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)      376 2023-06-09 22:31:54.000000 multitrackpro-0.1.1/tests/test_multitrackpro.py
```

### Comparing `multitrackpro-0.1.0/CONTRIBUTING.rst` & `multitrackpro-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.0/LICENSE` & `multitrackpro-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.0/docs/Makefile` & `multitrackpro-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.0/docs/conf.py` & `multitrackpro-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.0/docs/installation.rst` & `multitrackpro-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.0/docs/make.bat` & `multitrackpro-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.0/multitrackpro.egg-info/SOURCES.txt` & `multitrackpro-0.1.1/multitrackpro.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,27 @@
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/modules.rst
+docs/multitracker.core.io.rst
+docs/multitracker.core.rst
+docs/multitracker.qt.rst
+docs/multitracker.rst
 docs/readme.rst
 docs/usage.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
-multitrackpro/__init__.py
-multitrackpro/multitrackpro.py
+multitracker/auto_annotate_pro.py
 multitrackpro.egg-info/PKG-INFO
 multitrackpro.egg-info/SOURCES.txt
 multitrackpro.egg-info/dependency_links.txt
+multitrackpro.egg-info/entry_points.txt
 multitrackpro.egg-info/not-zip-safe
+multitrackpro.egg-info/requires.txt
 multitrackpro.egg-info/top_level.txt
 tests/__init__.py
 tests/test_multitrackpro.py
```


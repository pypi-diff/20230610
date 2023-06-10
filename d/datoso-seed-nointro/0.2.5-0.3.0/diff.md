# Comparing `tmp/datoso_seed_nointro-0.2.5.tar.gz` & `tmp/datoso_seed_nointro-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_nointro-0.2.5.tar", last modified: Thu May 11 18:49:04 2023, max compression
+gzip compressed data, was "datoso_seed_nointro-0.3.0.tar", last modified: Sat Jun 10 20:47:44 2023, max compression
```

## Comparing `datoso_seed_nointro-0.2.5.tar` & `datoso_seed_nointro-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.598089 datoso_seed_nointro-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-11 18:48:45.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:49:04.602089 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 18:49:04.000000 datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:47:44.327901 datoso_seed_nointro-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-10 20:47:44.327901 datoso_seed_nointro-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:47:44.327901 datoso_seed_nointro-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:47:44.323901 datoso_seed_nointro-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:47:44.323901 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-10 20:47:30.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:47:44.327901 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-10 20:47:44.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-10 20:47:44.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:47:44.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-10 20:47:44.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 20:47:44.000000 datoso_seed_nointro-0.3.0/src/datoso_seed_nointro.egg-info/top_level.txt
```

### Comparing `datoso_seed_nointro-0.2.5/LICENSE` & `datoso_seed_nointro-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.5/PKG-INFO` & `datoso_seed_nointro-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso_seed_nointro
-Version: 0.2.5
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso_seed_nointro-0.2.5/README.md` & `datoso_seed_nointro-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.5/pyproject.toml` & `datoso_seed_nointro-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.5",
+    "datoso>=0.3.1",
     "selenium==4.8.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_nointro"
```

### Comparing `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/dats.py` & `datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/fetch.py` & `datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-import sys
 import time
 import random
 import zipfile
 
 from selenium import webdriver
 from selenium.webdriver import FirefoxOptions
 from selenium.webdriver.common.by import By
```

### Comparing `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro/rules.py` & `datoso_seed_nointro-0.3.0/src/datoso_seed_nointro/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.5/src/datoso_seed_nointro.egg-info/PKG-INFO` & `datoso_seed_nointro-0.3.0/src/datoso_seed_nointro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso-seed-nointro
-Version: 0.2.5
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```


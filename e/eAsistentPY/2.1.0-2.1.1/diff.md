# Comparing `tmp/eAsistentPY-2.1.0.tar.gz` & `tmp/eAsistentPY-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eAsistentPY-2.1.0.tar", last modified: Sat Jun 10 16:45:29 2023, max compression
+gzip compressed data, was "eAsistentPY-2.1.1.tar", last modified: Sat Jun 10 16:48:56 2023, max compression
```

## Comparing `eAsistentPY-2.1.0.tar` & `eAsistentPY-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:45:29.064655 eAsistentPY-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 16:45:14.000000 eAsistentPY-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-10 16:45:29.064655 eAsistentPY-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-10 16:45:14.000000 eAsistentPY-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-10 16:45:14.000000 eAsistentPY-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 16:45:29.064655 eAsistentPY-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:45:29.064655 eAsistentPY-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:45:29.064655 eAsistentPY-2.1.0/src/eAsisitentPY/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 16:45:14.000000 eAsistentPY-2.1.0/src/eAsisitentPY/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-06-10 16:45:14.000000 eAsistentPY-2.1.0/src/eAsisitentPY/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:45:29.064655 eAsistentPY-2.1.0/src/eAsistentPY.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-10 16:45:29.000000 eAsistentPY-2.1.0/src/eAsistentPY.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-10 16:45:29.000000 eAsistentPY-2.1.0/src/eAsistentPY.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:45:29.000000 eAsistentPY-2.1.0/src/eAsistentPY.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-10 16:45:29.000000 eAsistentPY-2.1.0/src/eAsistentPY.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 16:45:29.000000 eAsistentPY-2.1.0/src/eAsistentPY.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/src/eAsisitentPY/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/src/eAsisitentPY/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-06-10 16:48:41.000000 eAsistentPY-2.1.1/src/eAsisitentPY/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:48:56.727656 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 16:48:56.000000 eAsistentPY-2.1.1/src/eAsistentPY.egg-info/top_level.txt
```

### Comparing `eAsistentPY-2.1.0/LICENSE` & `eAsistentPY-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eAsistentPY-2.1.0/PKG-INFO` & `eAsistentPY-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eAsistentPY
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scrapes data from easistent.com/urniki/... and returns it as Python dictionary
 Home-page: https://github.com/PingIsFun/eAsistentAPI
 Author: PingIsFun
 Author-email: pingisfun@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/PingIsFun/eAsistentAPI/issues
 Project-URL: Help, https://github.com/PingIsFun/eAsistentAPI/discussions/categories/general
@@ -17,15 +17,15 @@
 License-File: LICENSE
 
 # eAsistentPY
 
 ## EN
 To install it run:
 
-    pip install eAsistent-scraper
+    pip install eAsistentPY
 
 ***
 Example usage:
 
 ```python
 import eAsistentPY
```

### Comparing `eAsistentPY-2.1.0/setup.cfg` & `eAsistentPY-2.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eAsistentPY
-version = 2.1.0
+version = 2.1.1
 author = PingIsFun
 author_email = pingisfun@protonmail.com
 description = Scrapes data from easistent.com/urniki/... and returns it as Python dictionary
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PingIsFun/eAsistentAPI
 project_urls =
```

### Comparing `eAsistentPY-2.1.0/src/eAsisitentPY/scraper.py` & `eAsistentPY-2.1.1/src/eAsisitentPY/scraper.py`

 * *Files identical despite different names*

### Comparing `eAsistentPY-2.1.0/src/eAsistentPY.egg-info/PKG-INFO` & `eAsistentPY-2.1.1/src/eAsistentPY.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eAsistentPY
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scrapes data from easistent.com/urniki/... and returns it as Python dictionary
 Home-page: https://github.com/PingIsFun/eAsistentAPI
 Author: PingIsFun
 Author-email: pingisfun@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/PingIsFun/eAsistentAPI/issues
 Project-URL: Help, https://github.com/PingIsFun/eAsistentAPI/discussions/categories/general
@@ -17,15 +17,15 @@
 License-File: LICENSE
 
 # eAsistentPY
 
 ## EN
 To install it run:
 
-    pip install eAsistent-scraper
+    pip install eAsistentPY
 
 ***
 Example usage:
 
 ```python
 import eAsistentPY
```


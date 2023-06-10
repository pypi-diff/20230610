# Comparing `tmp/needed-libs-0.4.tar.gz` & `tmp/needed-libs-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "needed-libs-0.4.tar", last modified: Sat Jun 10 18:56:18 2023, max compression
+gzip compressed data, was "needed-libs-0.5.tar", last modified: Sat Jun 10 19:05:34 2023, max compression
```

## Comparing `needed-libs-0.4.tar` & `needed-libs-0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 18:56:18.395702 needed-libs-0.4/
--rw-rw-rw-   0        0        0       56 2023-06-10 18:56:18.395702 needed-libs-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 18:56:18.389706 needed-libs-0.4/needed_libs/
--rw-rw-rw-   0        0        0        0 2023-06-10 18:56:07.000000 needed-libs-0.4/needed_libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 18:56:18.394702 needed-libs-0.4/needed_libs.egg-info/
--rw-rw-rw-   0        0        0       56 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-10 18:56:18.000000 needed-libs-0.4/needed_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      364 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-10 18:56:18.396701 needed-libs-0.4/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-06-10 18:56:15.000000 needed-libs-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:05:34.160830 needed-libs-0.5/
+-rw-rw-rw-   0        0        0       56 2023-06-10 19:05:34.160830 needed-libs-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 19:05:34.154835 needed-libs-0.5/needed_libs/
+-rw-rw-rw-   0        0        0        0 2023-06-10 18:56:07.000000 needed-libs-0.5/needed_libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:05:34.160830 needed-libs-0.5/needed_libs.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-06-10 19:05:33.000000 needed-libs-0.5/needed_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-10 19:05:33.000000 needed-libs-0.5/needed_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 19:05:33.000000 needed-libs-0.5/needed_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      320 2023-06-10 19:05:33.000000 needed-libs-0.5/needed_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-10 19:05:33.000000 needed-libs-0.5/needed_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-10 19:05:34.161830 needed-libs-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-06-10 19:05:32.000000 needed-libs-0.5/setup.py
```

### Comparing `needed-libs-0.4/setup.py` & `needed-libs-0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name = 'needed-libs',
     packages = ['needed_libs'],
-    version = '0.4',
+    version = '0.5',
     install_requires = [
         # cc
         'websocket-client',
         'python_ghost_cursor',
         'price_parser',
         'requests',
 
@@ -22,27 +22,29 @@
         'instagrapi',
         'moviepy',
         'telethon',
 
         # Scraping
         'bs4',
         'httpx',
-        'selenium-shortcurts',
-        'undetected-chromedriver',
+        # 'selenium-shortcuts',
+        # 'undetected-chromedriver',
         'requestium',
         'feedparser',
 
         # Google
         'gspread',
         'google-api-python-client',
         'google-auth-httplib2',
         'google-auth-oauthlib',
-        
-        # Misc
+
+        # Server
         'flask',
         'waitress',
+        
+        # Misc
         'python-dateutil',
         'demoji',
         'schedule',
         'ffprobe-python',
         ]
     )
```


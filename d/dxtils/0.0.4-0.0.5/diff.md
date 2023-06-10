# Comparing `tmp/dxtils-0.0.4.tar.gz` & `tmp/dxtils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxtils-0.0.4.tar", last modified: Wed May 31 23:29:09 2023, max compression
+gzip compressed data, was "dxtils-0.0.5.tar", last modified: Sat Jun 10 11:49:14 2023, max compression
```

## Comparing `dxtils-0.0.4.tar` & `dxtils-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 23:29:09.134539 dxtils-0.0.4/
--rw-rw-rw-   0        0        0      169 2023-05-31 23:29:09.132542 dxtils-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-05-31 18:05:29.000000 dxtils-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 23:29:09.077838 dxtils-0.0.4/dxtils/
--rw-rw-rw-   0        0        0     2339 2023-05-31 23:26:44.000000 dxtils-0.0.4/dxtils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:29:09.128526 dxtils-0.0.4/dxtils.egg-info/
--rw-rw-rw-   0        0        0      169 2023-05-31 23:29:07.000000 dxtils-0.0.4/dxtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-05-31 23:29:08.000000 dxtils-0.0.4/dxtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 23:29:07.000000 dxtils-0.0.4/dxtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 23:29:07.000000 dxtils-0.0.4/dxtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2023-05-31 23:27:04.000000 dxtils-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 23:29:09.135547 dxtils-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 11:49:14.266393 dxtils-0.0.5/
+-rw-rw-rw-   0        0        0      169 2023-06-10 11:49:14.263068 dxtils-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2023-05-31 18:05:29.000000 dxtils-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 11:49:14.227580 dxtils-0.0.5/dxtils/
+-rw-rw-rw-   0        0        0     2563 2023-06-09 19:26:37.000000 dxtils-0.0.5/dxtils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 11:49:14.259066 dxtils-0.0.5/dxtils.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-06-10 11:49:13.000000 dxtils-0.0.5/dxtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-06-10 11:49:14.000000 dxtils-0.0.5/dxtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 11:49:13.000000 dxtils-0.0.5/dxtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 11:49:13.000000 dxtils-0.0.5/dxtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-06-10 11:47:49.000000 dxtils-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 11:49:14.266526 dxtils-0.0.5/setup.cfg
```

### Comparing `dxtils-0.0.4/dxtils/utils.py` & `dxtils-0.0.5/dxtils/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import platform
+import subprocess
 
 import requests as rq
 import undetected_chromedriver as uc
 from bs4 import BeautifulSoup
 from selenium.webdriver import Chrome, ChromeOptions
 from selenium.webdriver.chrome.service import Service
 from webdriver_manager.chrome import ChromeDriver
@@ -50,14 +51,18 @@
     else:
         driver_binary = ChromeDriverManager().install()
         executable_path = None        
     if not undetected:
         if kwargs_only:
             return {"service": Service(driver_binary), "options": options}
         return Chrome(service=Service(driver_binary), options=options)
+    if PLATFORM != "Windows":
+        subprocess.run(("codesign", "--remove-signature", driver_binary))
+        subprocess.run(
+            ("codesign", "--force", "--deep", "-s", "-", driver_binary))
     if kwargs_only:
         return {
             "driver_executable_path": driver_binary,
             "browser_executable_path": executable_path
         }
     return uc.Chrome(
         driver_executable_path=driver_binary,
```


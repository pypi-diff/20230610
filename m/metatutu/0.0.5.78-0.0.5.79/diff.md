# Comparing `tmp/metatutu-0.0.5.78.tar.gz` & `tmp/metatutu-0.0.5.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatutu-0.0.5.78.tar", last modified: Mon Apr 24 00:58:11 2023, max compression
+gzip compressed data, was "metatutu-0.0.5.79.tar", last modified: Sat Jun 10 12:26:06 2023, max compression
```

## Comparing `metatutu-0.0.5.78.tar` & `metatutu-0.0.5.79.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:11.021542 metatutu-0.0.5.78/
--rw-rw-rw-   0        0        0     1075 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/LICENSE
--rw-rw-rw-   0        0        0     1297 2023-04-24 00:58:11.020246 metatutu-0.0.5.78/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.657614 metatutu-0.0.5.78/lib/
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.815010 metatutu-0.0.5.78/lib/metatutu/
--rw-rw-rw-   0        0        0      630 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/__init__.py
--rw-rw-rw-   0        0        0      782 2023-04-24 00:58:08.000000 metatutu-0.0.5.78/lib/metatutu/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.882156 metatutu-0.0.5.78/lib/metatutu/app/
--rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/app/__init__.py
--rw-rw-rw-   0        0        0     8159 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/app/cli.py
--rw-rw-rw-   0        0        0     5451 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/app/servicelet.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.893104 metatutu-0.0.5.78/lib/metatutu/apps3/
--rw-rw-rw-   0        0        0      219 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/apps3/__init__.py
--rw-rw-rw-   0        0        0     2565 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/apps3/caller.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.916747 metatutu-0.0.5.78/lib/metatutu/da/
--rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/da/__init__.py
--rw-rw-rw-   0        0        0     6134 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/da/figure.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.976248 metatutu-0.0.5.78/lib/metatutu/dc/
--rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/dc/__init__.py
--rw-rw-rw-   0        0        0     4602 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/dc/capturing.py
--rw-rw-rw-   0        0        0     5994 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/dc/scanning.py
--rw-rw-rw-   0        0        0    23747 2023-04-24 00:57:35.000000 metatutu-0.0.5.78/lib/metatutu/dc/scraping.py
--rw-rw-rw-   0        0        0     2239 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/debugging.py
--rw-rw-rw-   0        0        0    15429 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/fsds.py
--rw-rw-rw-   0        0        0     4703 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/images.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.998783 metatutu-0.0.5.78/lib/metatutu/jupyter/
--rw-rw-rw-   0        0        0      219 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/jupyter/__init__.py
--rw-rw-rw-   0        0        0     8032 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/jupyter/display.py
--rw-rw-rw-   0        0        0    13101 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/logging.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:11.018216 metatutu-0.0.5.78/lib/metatutu/messaging/
--rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/messaging/__init__.py
--rw-rw-rw-   0        0        0    10370 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/messaging/smtp.py
--rw-rw-rw-   0        0        0    14045 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/osys.py
--rw-rw-rw-   0        0        0    17162 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/lib/metatutu/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:58:10.843502 metatutu-0.0.5.78/lib/metatutu.egg-info/
--rw-rw-rw-   0        0        0     1297 2023-04-24 00:58:10.000000 metatutu-0.0.5.78/lib/metatutu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2023-04-24 00:58:10.000000 metatutu-0.0.5.78/lib/metatutu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 00:58:10.000000 metatutu-0.0.5.78/lib/metatutu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 00:58:10.000000 metatutu-0.0.5.78/lib/metatutu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 00:58:11.021542 metatutu-0.0.5.78/setup.cfg
--rw-rw-rw-   0        0        0     1366 2023-02-07 13:20:31.000000 metatutu-0.0.5.78/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.617362 metatutu-0.0.5.79/
+-rw-rw-rw-   0        0        0     1075 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/LICENSE
+-rw-rw-rw-   0        0        0     1297 2023-06-10 12:26:06.616367 metatutu-0.0.5.79/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.282832 metatutu-0.0.5.79/lib/
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.406199 metatutu-0.0.5.79/lib/metatutu/
+-rw-rw-rw-   0        0        0      630 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/__init__.py
+-rw-rw-rw-   0        0        0      782 2023-06-10 12:26:04.000000 metatutu-0.0.5.79/lib/metatutu/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.493451 metatutu-0.0.5.79/lib/metatutu/app/
+-rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/app/__init__.py
+-rw-rw-rw-   0        0        0     8159 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/app/cli.py
+-rw-rw-rw-   0        0        0     5451 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/app/servicelet.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.509374 metatutu-0.0.5.79/lib/metatutu/apps3/
+-rw-rw-rw-   0        0        0      219 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/apps3/__init__.py
+-rw-rw-rw-   0        0        0     2565 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/apps3/caller.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.526578 metatutu-0.0.5.79/lib/metatutu/da/
+-rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/da/__init__.py
+-rw-rw-rw-   0        0        0     6134 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/da/figure.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.582917 metatutu-0.0.5.79/lib/metatutu/dc/
+-rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/dc/__init__.py
+-rw-rw-rw-   0        0        0     4602 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/dc/capturing.py
+-rw-rw-rw-   0        0        0     5994 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/dc/scanning.py
+-rw-rw-rw-   0        0        0    23747 2023-04-24 00:57:35.000000 metatutu-0.0.5.79/lib/metatutu/dc/scraping.py
+-rw-rw-rw-   0        0        0     2239 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/debugging.py
+-rw-rw-rw-   0        0        0    15429 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/fsds.py
+-rw-rw-rw-   0        0        0     4703 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/images.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.593141 metatutu-0.0.5.79/lib/metatutu/jupyter/
+-rw-rw-rw-   0        0        0      219 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/jupyter/__init__.py
+-rw-rw-rw-   0        0        0     8032 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/jupyter/display.py
+-rw-rw-rw-   0        0        0    13101 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/logging.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.613371 metatutu-0.0.5.79/lib/metatutu/messaging/
+-rw-rw-rw-   0        0        0      221 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/messaging/__init__.py
+-rw-rw-rw-   0        0        0    10370 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/messaging/smtp.py
+-rw-rw-rw-   0        0        0    14045 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/osys.py
+-rw-rw-rw-   0        0        0    17162 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/lib/metatutu/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:26:06.448488 metatutu-0.0.5.79/lib/metatutu.egg-info/
+-rw-rw-rw-   0        0        0     1297 2023-06-10 12:26:05.000000 metatutu-0.0.5.79/lib/metatutu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2023-06-10 12:26:05.000000 metatutu-0.0.5.79/lib/metatutu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 12:26:05.000000 metatutu-0.0.5.79/lib/metatutu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 12:26:05.000000 metatutu-0.0.5.79/lib/metatutu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 12:26:06.618363 metatutu-0.0.5.79/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2023-02-07 13:20:31.000000 metatutu-0.0.5.79/setup.py
```

### Comparing `metatutu-0.0.5.78/LICENSE` & `metatutu-0.0.5.79/LICENSE`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/PKG-INFO` & `metatutu-0.0.5.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatutu
-Version: 0.0.5.78
+Version: 0.0.5.79
 Summary: metatutu library
 Home-page: https://github.com/metatutu/metatutu
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/metatutu
 Project-URL: Source Code, https://github.com/metatutu/metatutu
```

### Comparing `metatutu-0.0.5.78/README.md` & `metatutu-0.0.5.79/README.md`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/__init__.py` & `metatutu-0.0.5.79/lib/metatutu/__init__.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/__version__.py` & `metatutu-0.0.5.79/lib/metatutu/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 __PROJECT_URLS__ = {
 	"Documentation": "https://github.com/metatutu/metatutu",
 	"Source Code": "https://github.com/metatutu/metatutu",
 	"Bug Tracker": "https://github.com/metatutu/metatutu/issues",
 	"Forum": "https://github.com/metatutu/metatutu/issues",
 	"Donate": "https://github.com/metatutu/metatutu"
 }
-__BUILD__ = 78
+__BUILD__ = 79
```

### Comparing `metatutu-0.0.5.78/lib/metatutu/app/cli.py` & `metatutu-0.0.5.79/lib/metatutu/app/cli.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/app/servicelet.py` & `metatutu-0.0.5.79/lib/metatutu/app/servicelet.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/apps3/caller.py` & `metatutu-0.0.5.79/lib/metatutu/apps3/caller.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/da/figure.py` & `metatutu-0.0.5.79/lib/metatutu/da/figure.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/dc/capturing.py` & `metatutu-0.0.5.79/lib/metatutu/dc/capturing.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/dc/scanning.py` & `metatutu-0.0.5.79/lib/metatutu/dc/scanning.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/dc/scraping.py` & `metatutu-0.0.5.79/lib/metatutu/dc/scraping.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/debugging.py` & `metatutu-0.0.5.79/lib/metatutu/debugging.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/fsds.py` & `metatutu-0.0.5.79/lib/metatutu/fsds.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/images.py` & `metatutu-0.0.5.79/lib/metatutu/images.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/jupyter/display.py` & `metatutu-0.0.5.79/lib/metatutu/jupyter/display.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/logging.py` & `metatutu-0.0.5.79/lib/metatutu/logging.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/messaging/smtp.py` & `metatutu-0.0.5.79/lib/metatutu/messaging/smtp.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/osys.py` & `metatutu-0.0.5.79/lib/metatutu/osys.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu/pipeline.py` & `metatutu-0.0.5.79/lib/metatutu/pipeline.py`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/lib/metatutu.egg-info/PKG-INFO` & `metatutu-0.0.5.79/lib/metatutu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatutu
-Version: 0.0.5.78
+Version: 0.0.5.79
 Summary: metatutu library
 Home-page: https://github.com/metatutu/metatutu
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/metatutu
 Project-URL: Source Code, https://github.com/metatutu/metatutu
```

### Comparing `metatutu-0.0.5.78/lib/metatutu.egg-info/SOURCES.txt` & `metatutu-0.0.5.79/lib/metatutu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metatutu-0.0.5.78/setup.py` & `metatutu-0.0.5.79/setup.py`

 * *Files identical despite different names*


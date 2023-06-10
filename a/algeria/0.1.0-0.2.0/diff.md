# Comparing `tmp/algeria-0.1.0.tar.gz` & `tmp/algeria-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algeria-0.1.0.tar", last modified: Fri Jun  9 14:23:44 2023, max compression
+gzip compressed data, was "algeria-0.2.0.tar", last modified: Sat Jun 10 18:39:28 2023, max compression
```

## Comparing `algeria-0.1.0.tar` & `algeria-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 med       (1000) med       (1000)        0 2023-06-09 14:23:44.312607 algeria-0.1.0/
--rw-rw-r--   0 med       (1000) med       (1000)     2806 2023-06-09 14:23:44.312607 algeria-0.1.0/PKG-INFO
--rw-rw-r--   0 med       (1000) med       (1000)     2042 2023-06-09 13:52:41.000000 algeria-0.1.0/README.md
-drwxrwxr-x   0 med       (1000) med       (1000)        0 2023-06-09 14:23:44.308607 algeria-0.1.0/algeria/
--rw-rw-r--   0 med       (1000) med       (1000)        0 2023-06-09 14:19:25.000000 algeria-0.1.0/algeria/__init__.py
--rw-rw-r--   0 med       (1000) med       (1000)     1265 2023-06-09 13:17:55.000000 algeria-0.1.0/algeria/ccp.py
-drwxrwxr-x   0 med       (1000) med       (1000)        0 2023-06-09 14:23:44.312607 algeria-0.1.0/algeria.egg-info/
--rw-rw-r--   0 med       (1000) med       (1000)     2806 2023-06-09 14:23:44.000000 algeria-0.1.0/algeria.egg-info/PKG-INFO
--rw-rw-r--   0 med       (1000) med       (1000)      177 2023-06-09 14:23:44.000000 algeria-0.1.0/algeria.egg-info/SOURCES.txt
--rw-rw-r--   0 med       (1000) med       (1000)        1 2023-06-09 14:23:44.000000 algeria-0.1.0/algeria.egg-info/dependency_links.txt
--rw-rw-r--   0 med       (1000) med       (1000)        8 2023-06-09 14:23:44.000000 algeria-0.1.0/algeria.egg-info/top_level.txt
--rw-rw-r--   0 med       (1000) med       (1000)       38 2023-06-09 14:23:44.312607 algeria-0.1.0/setup.cfg
--rw-rw-r--   0 med       (1000) med       (1000)      964 2023-06-09 14:20:15.000000 algeria-0.1.0/setup.py
+drwxrwxr-x   0 med       (1000) med       (1000)        0 2023-06-10 18:39:28.265482 algeria-0.2.0/
+-rw-rw-r--   0 med       (1000) med       (1000)     4315 2023-06-10 18:39:28.265482 algeria-0.2.0/PKG-INFO
+-rw-rw-r--   0 med       (1000) med       (1000)     3551 2023-06-10 18:35:01.000000 algeria-0.2.0/README.md
+drwxrwxr-x   0 med       (1000) med       (1000)        0 2023-06-10 18:39:28.265482 algeria-0.2.0/algeria/
+-rw-rw-r--   0 med       (1000) med       (1000)        0 2023-06-09 14:19:25.000000 algeria-0.2.0/algeria/__init__.py
+-rw-rw-r--   0 med       (1000) med       (1000)     1971 2023-06-10 18:21:33.000000 algeria-0.2.0/algeria/ccp.py
+drwxrwxr-x   0 med       (1000) med       (1000)        0 2023-06-10 18:39:28.265482 algeria-0.2.0/algeria.egg-info/
+-rw-rw-r--   0 med       (1000) med       (1000)     4315 2023-06-10 18:39:28.000000 algeria-0.2.0/algeria.egg-info/PKG-INFO
+-rw-rw-r--   0 med       (1000) med       (1000)      177 2023-06-10 18:39:28.000000 algeria-0.2.0/algeria.egg-info/SOURCES.txt
+-rw-rw-r--   0 med       (1000) med       (1000)        1 2023-06-10 18:39:28.000000 algeria-0.2.0/algeria.egg-info/dependency_links.txt
+-rw-rw-r--   0 med       (1000) med       (1000)        8 2023-06-10 18:39:28.000000 algeria-0.2.0/algeria.egg-info/top_level.txt
+-rw-rw-r--   0 med       (1000) med       (1000)       38 2023-06-10 18:39:28.265482 algeria-0.2.0/setup.cfg
+-rw-rw-r--   0 med       (1000) med       (1000)      964 2023-06-10 18:38:21.000000 algeria-0.2.0/setup.py
```

### Comparing `algeria-0.1.0/setup.py` & `algeria-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="algeria",
-    version="0.1.0",
+    version="0.2.0",
     author="Mohammed BADI",
     author_email="badi.mohammed@univ-oran2.dz",
     description="Python library which gives you a (clé) and (rip) of a given (ccp) CCP number account, additional features may be added to the library in the future",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mouh2020/algeria",
     packages=["algeria"],
```


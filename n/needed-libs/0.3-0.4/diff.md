# Comparing `tmp/needed-libs-0.3.tar.gz` & `tmp/needed-libs-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "needed-libs-0.3.tar", last modified: Sat Jun 10 18:53:14 2023, max compression
+gzip compressed data, was "needed-libs-0.4.tar", last modified: Sat Jun 10 18:56:18 2023, max compression
```

## Comparing `needed-libs-0.3.tar` & `needed-libs-0.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 18:53:14.243275 needed-libs-0.3/
--rw-rw-rw-   0        0        0       56 2023-06-10 18:53:14.243275 needed-libs-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 18:53:14.242276 needed-libs-0.3/needed_libs.egg-info/
--rw-rw-rw-   0        0        0       56 2023-06-10 18:53:13.000000 needed-libs-0.3/needed_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-10 18:53:14.000000 needed-libs-0.3/needed_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 18:53:13.000000 needed-libs-0.3/needed_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      364 2023-06-10 18:53:13.000000 needed-libs-0.3/needed_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 18:53:13.000000 needed-libs-0.3/needed_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-10 18:53:14.244274 needed-libs-0.3/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-06-10 18:52:54.000000 needed-libs-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:56:18.395702 needed-libs-0.4/
+-rw-rw-rw-   0        0        0       56 2023-06-10 18:56:18.395702 needed-libs-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 18:56:18.389706 needed-libs-0.4/needed_libs/
+-rw-rw-rw-   0        0        0        0 2023-06-10 18:56:07.000000 needed-libs-0.4/needed_libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:56:18.394702 needed-libs-0.4/needed_libs.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-10 18:56:18.000000 needed-libs-0.4/needed_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      364 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-10 18:56:17.000000 needed-libs-0.4/needed_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-10 18:56:18.396701 needed-libs-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-06-10 18:56:15.000000 needed-libs-0.4/setup.py
```

### Comparing `needed-libs-0.3/setup.py` & `needed-libs-0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name = 'needed-libs',
-    packages = ['folder'],
-    version = '0.3',
+    packages = ['needed_libs'],
+    version = '0.4',
     install_requires = [
         # cc
         'websocket-client',
         'python_ghost_cursor',
         'price_parser',
         'requests',
```


# Comparing `tmp/cliopts-1.0.0.tar.gz` & `tmp/cliopts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliopts-1.0.0.tar", last modified: Sat Jun 10 06:35:49 2023, max compression
+gzip compressed data, was "cliopts-1.0.1.tar", last modified: Sat Jun 10 06:39:39 2023, max compression
```

## Comparing `cliopts-1.0.0.tar` & `cliopts-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 06:35:49.301891 cliopts-1.0.0/
--rw-rw-rw-   0        0        0    35821 2023-06-10 05:20:08.000000 cliopts-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      981 2023-06-10 06:35:49.299886 cliopts-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 06:35:49.230144 cliopts-1.0.0/cliopts/
--rw-rw-rw-   0        0        0     2256 2023-06-10 06:11:25.000000 cliopts-1.0.0/cliopts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 06:35:49.298880 cliopts-1.0.0/cliopts.egg-info/
--rw-rw-rw-   0        0        0      981 2023-06-10 06:35:49.000000 cliopts-1.0.0/cliopts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-06-10 06:35:49.000000 cliopts-1.0.0/cliopts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 06:35:49.000000 cliopts-1.0.0/cliopts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 06:35:49.000000 cliopts-1.0.0/cliopts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 06:35:49.301891 cliopts-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1570 2023-06-10 06:35:22.000000 cliopts-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 06:39:39.455366 cliopts-1.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-06-10 05:20:08.000000 cliopts-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4179 2023-06-10 06:39:39.455366 cliopts-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 06:39:39.426922 cliopts-1.0.1/cliopts/
+-rw-rw-rw-   0        0        0     2256 2023-06-10 06:11:25.000000 cliopts-1.0.1/cliopts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 06:39:39.452044 cliopts-1.0.1/cliopts.egg-info/
+-rw-rw-rw-   0        0        0     4179 2023-06-10 06:39:39.000000 cliopts-1.0.1/cliopts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-06-10 06:39:39.000000 cliopts-1.0.1/cliopts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 06:39:39.000000 cliopts-1.0.1/cliopts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 06:39:39.000000 cliopts-1.0.1/cliopts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 06:39:39.456367 cliopts-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1322 2023-06-10 06:39:34.000000 cliopts-1.0.1/setup.py
```

### Comparing `cliopts-1.0.0/LICENSE` & `cliopts-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cliopts-1.0.0/cliopts/__init__.py` & `cliopts-1.0.1/cliopts/__init__.py`

 * *Files identical despite different names*


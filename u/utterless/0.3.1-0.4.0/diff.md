# Comparing `tmp/utterless-0.3.1.tar.gz` & `tmp/utterless-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utterless-0.3.1.tar", last modified: Fri Apr 28 15:32:36 2023, max compression
+gzip compressed data, was "utterless-0.4.0.tar", last modified: Sat Jun 10 02:09:57 2023, max compression
```

## Comparing `utterless-0.3.1.tar` & `utterless-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-04-28 15:32:36.128014 utterless-0.3.1/
--rw-rw-r--   0 psc       (1000) psc       (1000)     3763 2023-04-28 15:32:36.128014 utterless-0.3.1/PKG-INFO
--rw-rw-r--   0 psc       (1000) psc       (1000)     2251 2023-03-07 23:44:52.000000 utterless-0.3.1/README.md
--rw-rw-r--   0 psc       (1000) psc       (1000)      966 2023-04-28 15:32:36.128014 utterless-0.3.1/setup.cfg
--rw-rw-r--   0 psc       (1000) psc       (1000)      161 2023-01-20 22:41:33.000000 utterless-0.3.1/setup.py
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-04-28 15:32:36.128014 utterless-0.3.1/utterless/
--rw-rw-r--   0 psc       (1000) psc       (1000)      113 2023-04-28 15:32:13.000000 utterless-0.3.1/utterless/__init__.py
--rw-rw-r--   0 psc       (1000) psc       (1000)      386 2023-02-05 14:12:40.000000 utterless-0.3.1/utterless/__main__.py
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-04-28 15:32:36.128014 utterless-0.3.1/utterless/contrib/
--rw-rw-r--   0 psc       (1000) psc       (1000)        0 2023-02-05 14:12:40.000000 utterless-0.3.1/utterless/contrib/__init__.py
--rw-rw-r--   0 psc       (1000) psc       (1000)      280 2023-02-05 14:12:40.000000 utterless-0.3.1/utterless/contrib/django.py
--rw-rw-r--   0 psc       (1000) psc       (1000)     1451 2023-04-28 15:29:15.000000 utterless-0.3.1/utterless/results.py
--rw-rw-r--   0 psc       (1000) psc       (1000)      280 2023-02-05 14:12:40.000000 utterless-0.3.1/utterless/runner.py
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-04-28 15:32:36.128014 utterless-0.3.1/utterless.egg-info/
--rw-rw-r--   0 psc       (1000) psc       (1000)     3763 2023-04-28 15:32:36.000000 utterless-0.3.1/utterless.egg-info/PKG-INFO
--rw-rw-r--   0 psc       (1000) psc       (1000)      303 2023-04-28 15:32:36.000000 utterless-0.3.1/utterless.egg-info/SOURCES.txt
--rw-rw-r--   0 psc       (1000) psc       (1000)        1 2023-04-28 15:32:36.000000 utterless-0.3.1/utterless.egg-info/dependency_links.txt
--rw-rw-r--   0 psc       (1000) psc       (1000)       10 2023-04-28 15:32:36.000000 utterless-0.3.1/utterless.egg-info/top_level.txt
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-06-10 02:09:57.915102 utterless-0.4.0/
+-rw-rw-r--   0 psc       (1000) psc       (1000)     3763 2023-06-10 02:09:57.915102 utterless-0.4.0/PKG-INFO
+-rw-rw-r--   0 psc       (1000) psc       (1000)     2251 2023-03-07 23:44:52.000000 utterless-0.4.0/README.md
+-rw-rw-r--   0 psc       (1000) psc       (1000)      966 2023-06-10 02:09:57.915102 utterless-0.4.0/setup.cfg
+-rw-rw-r--   0 psc       (1000) psc       (1000)      161 2023-01-20 22:41:33.000000 utterless-0.4.0/setup.py
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-06-10 02:09:57.911102 utterless-0.4.0/utterless/
+-rw-rw-r--   0 psc       (1000) psc       (1000)      113 2023-06-10 02:08:17.000000 utterless-0.4.0/utterless/__init__.py
+-rw-rw-r--   0 psc       (1000) psc       (1000)      386 2023-02-05 14:12:40.000000 utterless-0.4.0/utterless/__main__.py
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-06-10 02:09:57.915102 utterless-0.4.0/utterless/contrib/
+-rw-rw-r--   0 psc       (1000) psc       (1000)        0 2023-02-05 14:12:40.000000 utterless-0.4.0/utterless/contrib/__init__.py
+-rw-rw-r--   0 psc       (1000) psc       (1000)      280 2023-02-05 14:12:40.000000 utterless-0.4.0/utterless/contrib/django.py
+-rw-rw-r--   0 psc       (1000) psc       (1000)     1458 2023-06-10 02:04:14.000000 utterless-0.4.0/utterless/results.py
+-rw-rw-r--   0 psc       (1000) psc       (1000)      280 2023-02-05 14:12:40.000000 utterless-0.4.0/utterless/runner.py
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2023-06-10 02:09:57.915102 utterless-0.4.0/utterless.egg-info/
+-rw-rw-r--   0 psc       (1000) psc       (1000)     3763 2023-06-10 02:09:57.000000 utterless-0.4.0/utterless.egg-info/PKG-INFO
+-rw-rw-r--   0 psc       (1000) psc       (1000)      303 2023-06-10 02:09:57.000000 utterless-0.4.0/utterless.egg-info/SOURCES.txt
+-rw-rw-r--   0 psc       (1000) psc       (1000)        1 2023-06-10 02:09:57.000000 utterless-0.4.0/utterless.egg-info/dependency_links.txt
+-rw-rw-r--   0 psc       (1000) psc       (1000)       10 2023-06-10 02:09:57.000000 utterless-0.4.0/utterless.egg-info/top_level.txt
```

### Comparing `utterless-0.3.1/PKG-INFO` & `utterless-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utterless
-Version: 0.3.1
+Version: 0.4.0
 Summary: Extend Python's "unittest" to better handle "logging" messages
 Home-page: https://github.com/pscl4rke/utterless
 Author: P. S. Clarke
 Author-email: utterless@pscl4rke.net
 License: UNKNOWN
 Project-URL: Source Code, https://github.com/pscl4rke/utterless
 Project-URL: Issues, https://github.com/pscl4rke/utterless/issues
```

### Comparing `utterless-0.3.1/README.md` & `utterless-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `utterless-0.3.1/setup.cfg` & `utterless-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `utterless-0.3.1/utterless.egg-info/PKG-INFO` & `utterless-0.4.0/utterless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utterless
-Version: 0.3.1
+Version: 0.4.0
 Summary: Extend Python's "unittest" to better handle "logging" messages
 Home-page: https://github.com/pscl4rke/utterless
 Author: P. S. Clarke
 Author-email: utterless@pscl4rke.net
 License: UNKNOWN
 Project-URL: Source Code, https://github.com/pscl4rke/utterless
 Project-URL: Issues, https://github.com/pscl4rke/utterless/issues
```


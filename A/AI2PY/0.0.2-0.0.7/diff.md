# Comparing `tmp/AI2PY-0.0.2.tar.gz` & `tmp/AI2PY-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AI2PY-0.0.2.tar", last modified: Fri Jun  9 22:09:53 2023, max compression
+gzip compressed data, was "AI2PY-0.0.7.tar", last modified: Fri Jun  9 22:10:13 2023, max compression
```

## Comparing `AI2PY-0.0.2.tar` & `AI2PY-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 22:09:53.020789 AI2PY-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-09 22:09:52.955829 AI2PY-0.0.2/AI2PY/
--rw-rw-rw-   0        0        0       28 2023-06-09 22:00:30.000000 AI2PY-0.0.2/AI2PY/__init__.py
--rw-rw-rw-   0        0        0     3558 2023-06-09 22:00:40.000000 AI2PY-0.0.2/AI2PY/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:09:52.975818 AI2PY-0.0.2/AI2PY.egg-info/
--rw-rw-rw-   0        0        0     2643 2023-06-09 22:09:52.000000 AI2PY-0.0.2/AI2PY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-09 22:09:52.000000 AI2PY-0.0.2/AI2PY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 22:09:52.000000 AI2PY-0.0.2/AI2PY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-09 22:09:52.000000 AI2PY-0.0.2/AI2PY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 22:09:52.000000 AI2PY-0.0.2/AI2PY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2023-06-09 22:09:53.019789 AI2PY-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2076 2023-06-09 21:55:16.000000 AI2PY-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 22:09:53.020789 AI2PY-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1168 2023-06-09 22:06:01.000000 AI2PY-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:10:13.010465 AI2PY-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-09 22:10:12.985482 AI2PY-0.0.7/AI2PY/
+-rw-rw-rw-   0        0        0       28 2023-06-09 22:00:30.000000 AI2PY-0.0.7/AI2PY/__init__.py
+-rw-rw-rw-   0        0        0     3558 2023-06-09 22:00:40.000000 AI2PY-0.0.7/AI2PY/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:10:13.006468 AI2PY-0.0.7/AI2PY.egg-info/
+-rw-rw-rw-   0        0        0     2643 2023-06-09 22:10:12.000000 AI2PY-0.0.7/AI2PY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-06-09 22:10:12.000000 AI2PY-0.0.7/AI2PY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 22:10:12.000000 AI2PY-0.0.7/AI2PY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-09 22:10:12.000000 AI2PY-0.0.7/AI2PY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 22:10:12.000000 AI2PY-0.0.7/AI2PY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2023-06-09 22:10:13.009466 AI2PY-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2076 2023-06-09 21:55:16.000000 AI2PY-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 22:10:13.010465 AI2PY-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-06-09 22:10:10.000000 AI2PY-0.0.7/setup.py
```

### Comparing `AI2PY-0.0.2/AI2PY/main.py` & `AI2PY-0.0.7/AI2PY/main.py`

 * *Files identical despite different names*

### Comparing `AI2PY-0.0.2/AI2PY.egg-info/PKG-INFO` & `AI2PY-0.0.7/AI2PY.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AI2PY
-Version: 0.0.2
+Version: 0.0.7
 Summary: Integrate AI into Python projects easily.
 Author: Bertran Usher (theaihub)
 Author-email: <bjusher820@gmail.com>
 Keywords: python,openai,ai,artificial intelligence
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AI2PY-0.0.2/PKG-INFO` & `AI2PY-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AI2PY
-Version: 0.0.2
+Version: 0.0.7
 Summary: Integrate AI into Python projects easily.
 Author: Bertran Usher (theaihub)
 Author-email: <bjusher820@gmail.com>
 Keywords: python,openai,ai,artificial intelligence
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AI2PY-0.0.2/README.md` & `AI2PY-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `AI2PY-0.0.2/setup.py` & `AI2PY-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.00.02'
+VERSION = '0.00.07'
 DESCRIPTION = 'Integrate AI into Python projects easily.'
 LONG_DESCRIPTION = 'Easily integrate artificial intelligence into your Python projects with AI2PY.'
 
 # Setting up
 setup(
     name="AI2PY",
     version=VERSION,
```


# Comparing `tmp/smart_dummy-0.1.2.tar.gz` & `tmp/smart_dummy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_dummy-0.1.2.tar", last modified: Fri Jun  9 23:40:31 2023, max compression
+gzip compressed data, was "smart_dummy-0.1.3.tar", last modified: Fri Jun  9 23:48:31 2023, max compression
```

## Comparing `smart_dummy-0.1.2.tar` & `smart_dummy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 23:40:31.053506 smart_dummy-0.1.2/
--rw-rw-rw-   0        0        0     1105 2023-06-09 23:14:45.000000 smart_dummy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2634 2023-06-09 23:40:31.053506 smart_dummy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1622 2023-06-09 23:14:45.000000 smart_dummy-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 23:40:31.054505 smart_dummy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-06-09 23:40:24.000000 smart_dummy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 23:40:31.040501 smart_dummy-0.1.2/smart_dummy/
--rw-rw-rw-   0        0        0      284 2023-06-09 23:14:45.000000 smart_dummy-0.1.2/smart_dummy/__init__.py
--rw-rw-rw-   0        0        0      661 2023-06-09 23:14:45.000000 smart_dummy-0.1.2/smart_dummy/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 23:40:31.052505 smart_dummy-0.1.2/smart_dummy.egg-info/
--rw-rw-rw-   0        0        0     2634 2023-06-09 23:40:30.000000 smart_dummy-0.1.2/smart_dummy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-09 23:40:30.000000 smart_dummy-0.1.2/smart_dummy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 23:40:30.000000 smart_dummy-0.1.2/smart_dummy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-09 23:40:30.000000 smart_dummy-0.1.2/smart_dummy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 23:40:30.000000 smart_dummy-0.1.2/smart_dummy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 23:48:31.946780 smart_dummy-0.1.3/
+-rw-rw-rw-   0        0        0     1105 2023-06-09 23:14:45.000000 smart_dummy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2634 2023-06-09 23:48:31.926760 smart_dummy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1622 2023-06-09 23:14:45.000000 smart_dummy-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 23:48:31.946780 smart_dummy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-06-09 23:46:58.000000 smart_dummy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 23:48:31.913756 smart_dummy-0.1.3/smart_dummy/
+-rw-rw-rw-   0        0        0      298 2023-06-09 23:46:39.000000 smart_dummy-0.1.3/smart_dummy/__init__.py
+-rw-rw-rw-   0        0        0      661 2023-06-09 23:14:45.000000 smart_dummy-0.1.3/smart_dummy/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 23:48:31.925758 smart_dummy-0.1.3/smart_dummy.egg-info/
+-rw-rw-rw-   0        0        0     2634 2023-06-09 23:48:31.000000 smart_dummy-0.1.3/smart_dummy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-09 23:48:31.000000 smart_dummy-0.1.3/smart_dummy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 23:48:31.000000 smart_dummy-0.1.3/smart_dummy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-09 23:48:31.000000 smart_dummy-0.1.3/smart_dummy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 23:48:31.000000 smart_dummy-0.1.3/smart_dummy.egg-info/top_level.txt
```

### Comparing `smart_dummy-0.1.2/LICENSE` & `smart_dummy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_dummy-0.1.2/PKG-INFO` & `smart_dummy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_dummy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A smart and easy replacement to pandas.get_dummies() 
 Home-page: https://github.com/emmalzhang/smart_dummy
 Author: Muriel Grobler, Emma Zhang
 Author-email: muriel.grobler@gmail.com, emma.lzhang@gmail.com
 License: UNKNOWN
 Description: # smart_dummy
```

### Comparing `smart_dummy-0.1.2/README.md` & `smart_dummy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `smart_dummy-0.1.2/setup.py` & `smart_dummy-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="smart_dummy",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.24',
         'pandas>=1.0',
         'pydantic>=1.10',
         'scikit-learn>=1.0',
         'spacy>=3.5'
```

### Comparing `smart_dummy-0.1.2/smart_dummy/main.py` & `smart_dummy-0.1.3/smart_dummy/main.py`

 * *Files identical despite different names*

### Comparing `smart_dummy-0.1.2/smart_dummy.egg-info/PKG-INFO` & `smart_dummy-0.1.3/smart_dummy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-dummy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A smart and easy replacement to pandas.get_dummies() 
 Home-page: https://github.com/emmalzhang/smart_dummy
 Author: Muriel Grobler, Emma Zhang
 Author-email: muriel.grobler@gmail.com, emma.lzhang@gmail.com
 License: UNKNOWN
 Description: # smart_dummy
```


# Comparing `tmp/archs4py-0.2.3.tar.gz` & `tmp/archs4py-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.2.3.tar", last modified: Fri Jun  9 23:13:52 2023, max compression
+gzip compressed data, was "archs4py-0.2.4.tar", last modified: Fri Jun  9 23:17:37 2023, max compression
```

## Comparing `archs4py-0.2.3.tar` & `archs4py-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.154559 archs4py-0.2.3/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.3/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.3/MANIFEST.in
--rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:13:52.154361 archs4py-0.2.3/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     9022 2023-06-09 23:12:51.000000 archs4py-0.2.3/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.153340 archs4py-0.2.3/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.3/archs4py/__init__.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3659 2023-06-09 21:25:34.000000 archs4py-0.2.3/archs4py/align.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.154151 archs4py-0.2.3/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     3161 2023-06-09 20:26:38.000000 archs4py-0.2.3/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.3/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2341 2023-06-09 20:28:56.000000 archs4py-0.2.3/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.3/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.3/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.154014 archs4py-0.2.3/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      155 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 23:13:52.154610 archs4py-0.2.3/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1096 2023-06-09 23:13:30.000000 archs4py-0.2.3/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.740258 archs4py-0.2.4/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.4/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.4/MANIFEST.in
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:17:37.739899 archs4py-0.2.4/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9022 2023-06-09 23:12:51.000000 archs4py-0.2.4/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.738751 archs4py-0.2.4/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.4/archs4py/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3659 2023-06-09 21:25:34.000000 archs4py-0.2.4/archs4py/align.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.739662 archs4py-0.2.4/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3161 2023-06-09 20:26:38.000000 archs4py-0.2.4/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.4/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2341 2023-06-09 20:28:56.000000 archs4py-0.2.4/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.4/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.4/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.739524 archs4py-0.2.4/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      140 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 23:17:37.740331 archs4py-0.2.4/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1070 2023-06-09 23:17:12.000000 archs4py-0.2.4/setup.py
```

### Comparing `archs4py-0.2.3/LICENSE` & `archs4py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/PKG-INFO` & `archs4py-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.3
+Version: 0.2.4
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `archs4py-0.2.3/README.md` & `archs4py-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/archs4py/align.py` & `archs4py-0.2.4/archs4py/align.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/archs4py/data/config.json` & `archs4py-0.2.4/archs4py/data/config.json`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/archs4py/data.py` & `archs4py-0.2.4/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/archs4py/download.py` & `archs4py-0.2.4/archs4py/download.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/archs4py/meta.py` & `archs4py-0.2.4/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/archs4py/utils.py` & `archs4py-0.2.4/archs4py/utils.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.3/archs4py.egg-info/PKG-INFO` & `archs4py-0.2.4/archs4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.3
+Version: 0.2.4
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `archs4py-0.2.3/setup.py` & `archs4py-0.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.2.3",
+    version="0.2.4",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
@@ -27,14 +27,13 @@
         'numpy==1.24.3',
         'pandas==2.0.2',
         'qnorm==0.8.1',
         'setuptools==67.8.0',
         'tqdm==4.65.0',
         'wget==3.2',
         's3fs==2023.5.0',
-        'xalign==0.1.73',
         'biomart==0.9.2',
         'xalign==0.1.74'
 
     ],
     python_requires='>=3.7',
 )
```


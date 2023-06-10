# Comparing `tmp/useful_rdkit_utils-0.2.5.tar.gz` & `tmp/useful_rdkit_utils-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useful_rdkit_utils-0.2.5.tar", last modified: Sun Dec  4 17:44:01 2022, max compression
+gzip compressed data, was "useful_rdkit_utils-0.2.6.tar", last modified: Sat Jun 10 19:37:12 2023, max compression
```

## Comparing `useful_rdkit_utils-0.2.5.tar` & `useful_rdkit_utils-0.2.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2022-12-04 17:44:01.475660 useful_rdkit_utils-0.2.5/
--rw-r--r--   0 pwalters   (501) staff       (20)     3555 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 pwalters   (501) staff       (20)     1068 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/LICENSE
--rw-r--r--   0 pwalters   (501) staff       (20)      152 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/MANIFEST.in
--rw-r--r--   0 pwalters   (501) staff       (20)     1461 2022-12-04 17:44:01.475744 useful_rdkit_utils-0.2.5/PKG-INFO
--rw-r--r--   0 pwalters   (501) staff       (20)     1140 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/README.md
--rw-r--r--   0 pwalters   (501) staff       (20)      385 2022-12-04 17:44:01.476085 useful_rdkit_utils-0.2.5/setup.cfg
--rw-r--r--   0 pwalters   (501) staff       (20)     2245 2022-12-03 03:52:40.000000 useful_rdkit_utils-0.2.5/setup.py
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2022-12-04 17:44:01.476518 useful_rdkit_utils-0.2.5/useful_rdkit_utils/
--rw-r--r--   0 pwalters   (501) staff       (20)      386 2022-11-27 21:51:25.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/__init__.py
--rw-r--r--   0 pwalters   (501) staff       (20)      498 2022-12-04 17:44:01.476570 useful_rdkit_utils-0.2.5/useful_rdkit_utils/_version.py
--rw-r--r--   0 pwalters   (501) staff       (20)     1297 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/pandas_utils.py
--rw-r--r--   0 pwalters   (501) staff       (20)     4124 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/reos.py
--rw-r--r--   0 pwalters   (501) staff       (20)      834 2022-11-29 22:30:32.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_counts.csv
--rw-r--r--   0 pwalters   (501) staff       (20)      645 2022-11-28 00:30:51.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_freq_test.csv
--rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-28 02:57:29.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_systems.csv
--rwxr-xr-x   0 pwalters   (501) staff       (20)     8963 2022-12-03 18:19:39.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_systems.py
--rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-29 12:48:31.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_test.csv
--rw-r--r--   0 pwalters   (501) staff       (20)      310 2022-11-28 02:02:49.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/seaborn_utils.py
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2022-12-04 17:44:01.475503 useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/
--rw-r--r--   0 pwalters   (501) staff       (20)      113 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/__init__.py
--rw-r--r--   0 pwalters   (501) staff       (20)      566 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/test_reos.py
--rw-r--r--   0 pwalters   (501) staff       (20)     1620 2022-11-28 00:30:45.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/test_ring_systems.py
--rw-r--r--   0 pwalters   (501) staff       (20)     5151 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/test_useful_rdkit_utils.py
--rw-r--r--   0 pwalters   (501) staff       (20)    12334 2022-12-04 00:52:31.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils/useful_rdkit_utils.py
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2022-12-04 17:44:01.474653 useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/
--rw-r--r--   0 pwalters   (501) staff       (20)     1461 2022-12-04 17:44:01.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/PKG-INFO
--rw-r--r--   0 pwalters   (501) staff       (20)      841 2022-12-04 17:44:01.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/SOURCES.txt
--rw-r--r--   0 pwalters   (501) staff       (20)        1 2022-12-04 17:44:01.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/dependency_links.txt
--rw-r--r--   0 pwalters   (501) staff       (20)       70 2022-12-04 17:44:01.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/requires.txt
--rw-r--r--   0 pwalters   (501) staff       (20)       19 2022-12-04 17:44:01.000000 useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/top_level.txt
--rw-r--r--   0 pwalters   (501) staff       (20)    68611 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.5/versioneer.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.773552 useful_rdkit_utils-0.2.6/
+-rw-r--r--   0 pwalters   (501) staff       (20)     3555 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 pwalters   (501) staff       (20)     1068 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/LICENSE
+-rw-r--r--   0 pwalters   (501) staff       (20)      152 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/MANIFEST.in
+-rw-r--r--   0 pwalters   (501) staff       (20)     1459 2023-06-10 19:37:12.773614 useful_rdkit_utils-0.2.6/PKG-INFO
+-rw-r--r--   0 pwalters   (501) staff       (20)     1140 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/README.md
+-rw-r--r--   0 pwalters   (501) staff       (20)      385 2023-06-10 19:37:12.773977 useful_rdkit_utils-0.2.6/setup.cfg
+-rw-r--r--   0 pwalters   (501) staff       (20)     2245 2022-12-03 03:52:40.000000 useful_rdkit_utils-0.2.6/setup.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.774377 useful_rdkit_utils-0.2.6/useful_rdkit_utils/
+-rw-r--r--   0 pwalters   (501) staff       (20)      386 2022-11-27 21:51:25.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/__init__.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      498 2023-06-10 19:37:12.774422 useful_rdkit_utils-0.2.6/useful_rdkit_utils/_version.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     1297 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/pandas_utils.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     4124 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/reos.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      834 2022-11-29 22:30:32.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_counts.csv
+-rw-r--r--   0 pwalters   (501) staff       (20)      645 2022-11-28 00:30:51.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_freq_test.csv
+-rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-28 02:57:29.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.csv
+-rwxr-xr-x   0 pwalters   (501) staff       (20)     8963 2022-12-03 18:19:39.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-29 12:48:31.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_test.csv
+-rw-r--r--   0 pwalters   (501) staff       (20)      310 2022-11-28 02:02:49.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/seaborn_utils.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.773383 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/
+-rw-r--r--   0 pwalters   (501) staff       (20)      113 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/__init__.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      566 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_reos.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     1620 2022-11-28 00:30:45.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_ring_systems.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     5151 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_useful_rdkit_utils.py
+-rw-r--r--   0 pwalters   (501) staff       (20)    12336 2022-12-20 01:59:21.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/useful_rdkit_utils.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.772626 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/
+-rw-r--r--   0 pwalters   (501) staff       (20)     1459 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/PKG-INFO
+-rw-r--r--   0 pwalters   (501) staff       (20)      841 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)        1 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)       70 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/requires.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)       19 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/top_level.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)    68611 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/versioneer.py
```

### Comparing `useful_rdkit_utils-0.2.5/CODE_OF_CONDUCT.md` & `useful_rdkit_utils-0.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/LICENSE` & `useful_rdkit_utils-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/PKG-INFO` & `useful_rdkit_utils-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useful_rdkit_utils
-Version: 0.2.5
+Version: 0.2.6
 Summary: Some useful RDKit functions
 Author: PatWalters
 Author-email: wpwalters@gmail.com
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
@@ -56,9 +56,7 @@
 
 The code in this package is licensed under the MIT License.
 
 ### Acknowledgements
  
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.6.
-
-
```

### Comparing `useful_rdkit_utils-0.2.5/README.md` & `useful_rdkit_utils-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/setup.py` & `useful_rdkit_utils-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/pandas_utils.py` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/reos.py` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/reos.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_counts.csv` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_counts.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_freq_test.csv` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_freq_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_systems.csv` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_systems.py` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/ring_test.csv` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/test_reos.py` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_reos.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/test_ring_systems.py` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_ring_systems.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/tests/test_useful_rdkit_utils.py` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_useful_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils/useful_rdkit_utils.py` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils/useful_rdkit_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     :param name: descriptor name
     :param mol: RDKit molecule
     :return:
     """
     try:
         return FUNCS[name](mol)
     except:
-        logging.exception("function application failed (%s->%s)", name, Chem.MolToSmiles(m))
+        logging.exception("function application failed (%s->%s)", name, Chem.MolToSmiles(mol))
         return None
 
 
 class RDKitDescriptors:
     """ Calculate RDKit descriptors"""
 
     def __init__(self):
```

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/PKG-INFO` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useful-rdkit-utils
-Version: 0.2.5
+Version: 0.2.6
 Summary: Some useful RDKit functions
 Author: PatWalters
 Author-email: wpwalters@gmail.com
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
@@ -56,9 +56,7 @@
 
 The code in this package is licensed under the MIT License.
 
 ### Acknowledgements
  
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.6.
-
-
```

### Comparing `useful_rdkit_utils-0.2.5/useful_rdkit_utils.egg-info/SOURCES.txt` & `useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.5/versioneer.py` & `useful_rdkit_utils-0.2.6/versioneer.py`

 * *Files identical despite different names*


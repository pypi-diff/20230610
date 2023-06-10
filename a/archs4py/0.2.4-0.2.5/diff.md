# Comparing `tmp/archs4py-0.2.4.tar.gz` & `tmp/archs4py-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.2.4.tar", last modified: Fri Jun  9 23:17:37 2023, max compression
+gzip compressed data, was "archs4py-0.2.5.tar", last modified: Fri Jun  9 23:58:10 2023, max compression
```

## Comparing `archs4py-0.2.4.tar` & `archs4py-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.740258 archs4py-0.2.4/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.4/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.4/MANIFEST.in
--rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:17:37.739899 archs4py-0.2.4/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     9022 2023-06-09 23:12:51.000000 archs4py-0.2.4/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.738751 archs4py-0.2.4/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.4/archs4py/__init__.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3659 2023-06-09 21:25:34.000000 archs4py-0.2.4/archs4py/align.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.739662 archs4py-0.2.4/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     3161 2023-06-09 20:26:38.000000 archs4py-0.2.4/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.4/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2341 2023-06-09 20:28:56.000000 archs4py-0.2.4/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.4/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.4/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:17:37.739524 archs4py-0.2.4/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      140 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 23:17:37.000000 archs4py-0.2.4/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 23:17:37.740331 archs4py-0.2.4/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1070 2023-06-09 23:17:12.000000 archs4py-0.2.4/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.356587 archs4py-0.2.5/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.5/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.5/MANIFEST.in
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9510 2023-06-09 23:58:10.356390 archs4py-0.2.5/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9023 2023-06-09 23:57:42.000000 archs4py-0.2.5/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.355151 archs4py-0.2.5/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.5/archs4py/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3659 2023-06-09 21:25:34.000000 archs4py-0.2.5/archs4py/align.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.356087 archs4py-0.2.5/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3161 2023-06-09 20:26:38.000000 archs4py-0.2.5/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.5/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2341 2023-06-09 20:28:56.000000 archs4py-0.2.5/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.5/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.5/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.355956 archs4py-0.2.5/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9510 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      140 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 23:58:10.356641 archs4py-0.2.5/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1070 2023-06-09 23:57:53.000000 archs4py-0.2.5/setup.py
```

### Comparing `archs4py-0.2.4/LICENSE` & `archs4py-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.4/PKG-INFO` & `archs4py-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.4
+Version: 0.2.5
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -194,20 +194,20 @@
 result = a4.align.fastq("human", "data/example_1/SRR14457464.fastq", return_type="gene", identifier="symbol")
 
 ```
 
 The next example is a SRR file that extracts into a pair of paired end FASTQ files. They can be passed to ARCHS4py like this:
 
 ```python
-import xalign
+import archs4py as a4
 
 # the sample is paired-end and will result in two files (SRR15972519_1.fastq, SRR15972519_2.fastq)
 a4.align.load(["SRR15972519"], "data/example_2")
 
-result = a4.align.fastq("homo_sapiens", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
+result = a4.align.fastq("mouse", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
 
 ```
 
 ### Align FASTQ files from folder
 
 Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
```

### Comparing `archs4py-0.2.4/README.md` & `archs4py-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -180,20 +180,20 @@
 result = a4.align.fastq("human", "data/example_1/SRR14457464.fastq", return_type="gene", identifier="symbol")
 
 ```
 
 The next example is a SRR file that extracts into a pair of paired end FASTQ files. They can be passed to ARCHS4py like this:
 
 ```python
-import xalign
+import archs4py as a4
 
 # the sample is paired-end and will result in two files (SRR15972519_1.fastq, SRR15972519_2.fastq)
 a4.align.load(["SRR15972519"], "data/example_2")
 
-result = a4.align.fastq("homo_sapiens", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
+result = a4.align.fastq("mouse", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
 
 ```
 
 ### Align FASTQ files from folder
 
 Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
```

### Comparing `archs4py-0.2.4/archs4py/align.py` & `archs4py-0.2.5/archs4py/align.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.4/archs4py/data/config.json` & `archs4py-0.2.5/archs4py/data/config.json`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.4/archs4py/data.py` & `archs4py-0.2.5/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.4/archs4py/download.py` & `archs4py-0.2.5/archs4py/download.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.4/archs4py/meta.py` & `archs4py-0.2.5/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.4/archs4py/utils.py` & `archs4py-0.2.5/archs4py/utils.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.4/archs4py.egg-info/PKG-INFO` & `archs4py-0.2.5/archs4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.4
+Version: 0.2.5
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -194,20 +194,20 @@
 result = a4.align.fastq("human", "data/example_1/SRR14457464.fastq", return_type="gene", identifier="symbol")
 
 ```
 
 The next example is a SRR file that extracts into a pair of paired end FASTQ files. They can be passed to ARCHS4py like this:
 
 ```python
-import xalign
+import archs4py as a4
 
 # the sample is paired-end and will result in two files (SRR15972519_1.fastq, SRR15972519_2.fastq)
 a4.align.load(["SRR15972519"], "data/example_2")
 
-result = a4.align.fastq("homo_sapiens", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
+result = a4.align.fastq("mouse", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
 
 ```
 
 ### Align FASTQ files from folder
 
 Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
```

### Comparing `archs4py-0.2.4/setup.py` & `archs4py-0.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.2.4",
+    version="0.2.5",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
```


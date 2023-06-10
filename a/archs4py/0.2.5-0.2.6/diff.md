# Comparing `tmp/archs4py-0.2.5.tar.gz` & `tmp/archs4py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.2.5.tar", last modified: Fri Jun  9 23:58:10 2023, max compression
+gzip compressed data, was "archs4py-0.2.6.tar", last modified: Sat Jun 10 05:16:28 2023, max compression
```

## Comparing `archs4py-0.2.5.tar` & `archs4py-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.356587 archs4py-0.2.5/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.5/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.5/MANIFEST.in
--rw-r--r--   0 maayanlab   (501) staff       (20)     9510 2023-06-09 23:58:10.356390 archs4py-0.2.5/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     9023 2023-06-09 23:57:42.000000 archs4py-0.2.5/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.355151 archs4py-0.2.5/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.5/archs4py/__init__.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3659 2023-06-09 21:25:34.000000 archs4py-0.2.5/archs4py/align.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.356087 archs4py-0.2.5/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     3161 2023-06-09 20:26:38.000000 archs4py-0.2.5/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.5/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2341 2023-06-09 20:28:56.000000 archs4py-0.2.5/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.5/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.5/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:58:10.355956 archs4py-0.2.5/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     9510 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      140 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 23:58:10.000000 archs4py-0.2.5/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 23:58:10.356641 archs4py-0.2.5/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1070 2023-06-09 23:57:53.000000 archs4py-0.2.5/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-10 05:16:28.189437 archs4py-0.2.6/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.6/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.6/MANIFEST.in
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9550 2023-06-10 05:16:28.189219 archs4py-0.2.6/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9063 2023-06-10 05:15:58.000000 archs4py-0.2.6/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-10 05:16:28.187734 archs4py-0.2.6/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.6/archs4py/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3585 2023-06-10 01:54:12.000000 archs4py-0.2.6/archs4py/align.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-10 05:16:28.188872 archs4py-0.2.6/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3161 2023-06-09 20:26:38.000000 archs4py-0.2.6/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.6/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2341 2023-06-09 20:28:56.000000 archs4py-0.2.6/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.6/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.6/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-10 05:16:28.188732 archs4py-0.2.6/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9550 2023-06-10 05:16:28.000000 archs4py-0.2.6/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-10 05:16:28.000000 archs4py-0.2.6/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-10 05:16:28.000000 archs4py-0.2.6/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      140 2023-06-10 05:16:28.000000 archs4py-0.2.6/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-10 05:16:28.000000 archs4py-0.2.6/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-10 05:16:28.189491 archs4py-0.2.6/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1070 2023-06-10 05:16:17.000000 archs4py-0.2.6/setup.py
```

### Comparing `archs4py-0.2.5/LICENSE` & `archs4py-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.5/PKG-INFO` & `archs4py-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.5
+Version: 0.2.6
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -205,23 +205,23 @@
 
 result = a4.align.fastq("mouse", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
 
 ```
 
 ### Align FASTQ files from folder
 
-Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
+Align all FASTQ files in folder using the function `a4.align.folder()`. ARCHS4py will automatically matching samples if data is paired end.
 
 ```python
 
 import archs4py as a4
 
 a4.align.load(["SRR15972519", "SRR15972520", "SRR15972521"], "data/example_3")
 
-result = a4.align.fastq("mouse", "data/example_3", return_type="gene", identifier="symbol")
+result = a4.align.folder("mouse", "data/example_3", return_type="gene", identifier="symbol")
 
 ```
 
 ## List versions
 <span id="#version"></span>
 ARCHS4 has different versions to download from. Recommended is the default setting, which will download the latest data release.
```

### Comparing `archs4py-0.2.5/README.md` & `archs4py-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -191,23 +191,23 @@
 
 result = a4.align.fastq("mouse", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
 
 ```
 
 ### Align FASTQ files from folder
 
-Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
+Align all FASTQ files in folder using the function `a4.align.folder()`. ARCHS4py will automatically matching samples if data is paired end.
 
 ```python
 
 import archs4py as a4
 
 a4.align.load(["SRR15972519", "SRR15972520", "SRR15972521"], "data/example_3")
 
-result = a4.align.fastq("mouse", "data/example_3", return_type="gene", identifier="symbol")
+result = a4.align.folder("mouse", "data/example_3", return_type="gene", identifier="symbol")
 
 ```
 
 ## List versions
 <span id="#version"></span>
 ARCHS4 has different versions to download from. Recommended is the default setting, which will download the latest data release.
```

### Comparing `archs4py-0.2.5/archs4py/align.py` & `archs4py-0.2.6/archs4py/align.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,14 @@
     gene_count, transcript_count = xalign.align_folder(species, folder, release=conf["ALIGNMENT"][str(release)]["release"], t=t, noncoding=True, overwrite=overwrite)
     del gene_count
     if return_type == "transcript":
         return transcript_count
     else:
         return aggregate(transcript_count, species, release, identifier)
 
-def download(sra_ids, folder):
-    xalign.sra.load_sras(sra_ids, folder)
-
 def aggregate(transcript_count, species, release, identifier):
     if gene_mapping[species] is None:
         gene_mapping[species] = get_ensembl_mappings(species, release)
     trans = transcript_count.copy()
     trans.index = [x.split(".")[0] for x in transcript_count.index]
     trans.index = gene_mapping[species].loc[trans.index, "ensembl_gene"]
     trans = trans.groupby(trans.index).sum().astype(np.uint64)
```

### Comparing `archs4py-0.2.5/archs4py/data/config.json` & `archs4py-0.2.6/archs4py/data/config.json`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.5/archs4py/data.py` & `archs4py-0.2.6/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.5/archs4py/download.py` & `archs4py-0.2.6/archs4py/download.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.5/archs4py/meta.py` & `archs4py-0.2.6/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.5/archs4py/utils.py` & `archs4py-0.2.6/archs4py/utils.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.5/archs4py.egg-info/PKG-INFO` & `archs4py-0.2.6/archs4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.5
+Version: 0.2.6
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -205,23 +205,23 @@
 
 result = a4.align.fastq("mouse", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
 
 ```
 
 ### Align FASTQ files from folder
 
-Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
+Align all FASTQ files in folder using the function `a4.align.folder()`. ARCHS4py will automatically matching samples if data is paired end.
 
 ```python
 
 import archs4py as a4
 
 a4.align.load(["SRR15972519", "SRR15972520", "SRR15972521"], "data/example_3")
 
-result = a4.align.fastq("mouse", "data/example_3", return_type="gene", identifier="symbol")
+result = a4.align.folder("mouse", "data/example_3", return_type="gene", identifier="symbol")
 
 ```
 
 ## List versions
 <span id="#version"></span>
 ARCHS4 has different versions to download from. Recommended is the default setting, which will download the latest data release.
```

### Comparing `archs4py-0.2.5/setup.py` & `archs4py-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.2.5",
+    version="0.2.6",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
```


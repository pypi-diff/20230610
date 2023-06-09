# Comparing `tmp/archs4py-0.2.1.tar.gz` & `tmp/archs4py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archs4py-0.2.1.tar", last modified: Fri Jun  9 20:01:37 2023, max compression
+gzip compressed data, was "archs4py-0.2.3.tar", last modified: Fri Jun  9 23:13:52 2023, max compression
```

## Comparing `archs4py-0.2.1.tar` & `archs4py-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.904664 archs4py-0.2.1/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.1/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.1/MANIFEST.in
--rw-r--r--   0 maayanlab   (501) staff       (20)     6919 2023-06-09 20:01:37.904514 archs4py-0.2.1/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     6432 2023-06-05 17:48:08.000000 archs4py-0.2.1/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.903376 archs4py-0.2.1/archs4py/
--rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.1/archs4py/__init__.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3559 2023-06-09 19:02:34.000000 archs4py-0.2.1/archs4py/align.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.904214 archs4py-0.2.1/archs4py/data/
--rw-r--r--   0 maayanlab   (501) staff       (20)     3080 2023-06-08 15:38:06.000000 archs4py-0.2.1/archs4py/data/config.json
--rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.1/archs4py/data.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2053 2023-06-09 15:16:23.000000 archs4py-0.2.1/archs4py/download.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.1/archs4py/meta.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.1/archs4py/utils.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 20:01:37.904085 archs4py-0.2.1/archs4py.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     6919 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      155 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 20:01:37.000000 archs4py-0.2.1/archs4py.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 20:01:37.904721 archs4py-0.2.1/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1096 2023-06-09 20:01:26.000000 archs4py-0.2.1/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.154559 archs4py-0.2.3/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-11-01 18:40:54.000000 archs4py-0.2.3/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)      266 2023-06-09 19:56:39.000000 archs4py-0.2.3/MANIFEST.in
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:13:52.154361 archs4py-0.2.3/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9022 2023-06-09 23:12:51.000000 archs4py-0.2.3/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.153340 archs4py-0.2.3/archs4py/
+-rw-r--r--   0 maayanlab   (501) staff       (20)      401 2023-06-07 15:07:46.000000 archs4py-0.2.3/archs4py/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3659 2023-06-09 21:25:34.000000 archs4py-0.2.3/archs4py/align.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.154151 archs4py-0.2.3/archs4py/data/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3161 2023-06-09 20:26:38.000000 archs4py-0.2.3/archs4py/data/config.json
+-rw-r--r--   0 maayanlab   (501) staff       (20)    12493 2023-06-02 16:44:04.000000 archs4py-0.2.3/archs4py/data.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2341 2023-06-09 20:28:56.000000 archs4py-0.2.3/archs4py/download.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     5963 2023-06-03 02:17:54.000000 archs4py-0.2.3/archs4py/meta.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     3814 2023-06-08 19:32:52.000000 archs4py-0.2.3/archs4py/utils.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-06-09 23:13:52.154014 archs4py-0.2.3/archs4py.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)     9509 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      335 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      155 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        9 2023-06-09 23:13:52.000000 archs4py-0.2.3/archs4py.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-06-09 23:13:52.154610 archs4py-0.2.3/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1096 2023-06-09 23:13:30.000000 archs4py-0.2.3/setup.py
```

### Comparing `archs4py-0.2.1/LICENSE` & `archs4py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.1/PKG-INFO` & `archs4py-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.1
+Version: 0.2.3
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,18 @@
 
 <img title="archs4py" alt="archs4py" src="https://user-images.githubusercontent.com/32603869/243101679-c5147d56-fce0-4498-9577-a300df7d6dce.png">
 
 # archs4py - Official Python package to load and query ARCHS4 data
 
 Official ARCHS4 compagnion package. This package is a wrapper for basic H5 commands performed on the ARCHS4 data files. Some of the data access is optimized for specific query strategies and should make this implementation faster than manually querying the data. The package supports automated file download, mutithreading, and some convenience functions such as data normalization.
 
+ARCHS4py also supports the ARCHS4 alignment pipeline. When aligning FASTQ files using ARCHS4py gene and transcript counts will be compatible with the preprocessed ARCHS4 samples.
+
+[Installation](#installation) | [Download H5 Files](#usage) | [List H5 Contents](#list-data-fields-in-h5) | [Extract Counts](#data-access) | [Extract Meta Data](#meta-data) | [Normalize Samples](#normalizing-data) | [FASTQ Alignment](#sequence-alignment) | [Versions](#list-versions)
+
 ## ARCHS4 data
 
 ARCHS4 data is regularly updated to include publically available gene expression samples from RNA-seq. ARCHS4 processes the major platforms for human and mouse. As of 6/2023 ARCHS4 encompasses more than 1.5 million RNA-seq samples. All samples in ARCHS4 are homogeniously processed. ARCHS4 does currently not decern whether samples are bulk or single-cell and purely crawls GEO. Since samples are not always correctly annotated as single cell ARCHS4 uses a machine learning approach to predict single-cell samples and associated a singlecellprobability to each sample. Samples with a value larger than 0.5 can be removed from the queries if needed.
 
 ## Installation
 
 The python package can be directly installed from this GitHub repository using the following command (pip or pip3 depending on system setup)
@@ -30,37 +34,39 @@
 pip3 install archs4py
 ```
 
 ## Usage
 
 ### Download data file
 
+
 The data is stored in large HDF5 files which first need to be downloaded. HDF5 stores matrix information in a compressed datastructure that allows efficient data access to slices of the data. There are separate files for `human` and `mouse` data. The supported files are `gene counts` and `transcript counts`. As of 6/2023 the files are larger than 30GB and depending on the network speed will take some time to download.
 
 ```python
 import archs4py as a4
 
 file_path = a4.download.counts("human", path="", version="latest")
 ```
 
-### List data fields in H5
+## List data fields in H5
 
 The H5 files contain data and meta data information. To list the contents of ARCHS4 H5 files use the built in `ls` function.
 
-```
+```python
 import archs4py as a4
 
 file = "human_gene_v2.2.h5"
 a4.ls(file)
 ```
 
-### Data access
+## Data access
 
 archs4py supports several ways to load gene expression data. When querying ARCHS4 be aware that when loading too many samples the system might run out of memory. (e.g. the meta data search term is very broad). In most cases loading several thousand samples at the same time should be no problem. To find relevant samples there are 5 main functions in the `archs4py.data` module. A function to extract N random samples `archs4py.data.rand()`, a function to extract samples by index `archs4py.data.index()`, a function to extract samples based on meta data search `archs4py.data.meta()`, a function to extract samples based on a list of geo accessions `archs4py.data.samples()` and lastly a function to extract all samples belonging to a series `archs4.data.series()`.
 
+<span id="#extract-counts"></span>
 
 #### Extract a random set of samples
 
 To extract a random gene expression matrix use the `archs4py.data.rand()` function. The function will return a pandas dataframe with samples as columns and genes as rows.
 
 ```python
 import archs4py as a4
@@ -129,15 +135,17 @@
 file = "human_gene_v2.2.h5"
 
 #get sample counts
 series_counts = a4.data.series(file, "GSE64016")
 
 ```
 
-### Meta data
+## Meta data
+
+<span id="#extract-meta"></span>
 
 Additinally to the data module archs4py also supports the extraction of meta data. It supports similar endpoints to the `archs4.data` module. Meta data fields can be specified with: `meta_fields=["geo_accession", "series_id", "characteristics_ch1", "extract_protocol_ch1", "source_name_ch1", "title"]`
 
 ```python
 import archs4py as a4
 
 #path to file
@@ -150,32 +158,87 @@
 sample_meta = a4.meta.samples(file, ["GSM1158284","GSM1482938","GSM1562817"])
 
 # get series meta data
 series_meta = a4.meta.series(file, "GSE64016")
 
 ```
 
-### Normalizing data
-
+## Normalizing data
+<span id="#normalize"></span>
 The package also supports simple normalization. Currently supported are quantile normalization, log2 + quantile normalization, and cpm. In the example below we load 100 random samples and apply log quantile.
 
 ```python
 import archs4py as a4
 
 file = "human_gene_v2.2.h5"
 rand_counts = a4.data.rand(file, 100)
 
 #normalize using log quantile (method options for now = ["log_quantile", "quantile", "cpm", "tmm"])
 norm_exp = a4.normalize(rand_counts, method="log_quantile")
 
 ```
 
-### List versions
+## Sequence alignment
+<span id="#align"></span>
+The `align` module contains a replication of the ARCHS4 alignment pipeline. When used on FASTQ files the resulting gene or transcript counts are compatible with the previously aligned samples in ARCHS4. The package is highly automated and only required a path to a FASTQ file or a folder containing multiple FASTQ files. All file dependencies will downloaded automatically and index will be built when needed.
+
+### Align FASTQ file
+
+Pass either a single or paired FASTQ file. This function can return transcript count, gene counts, or transcript level TPM data.
+
+```python
+
+import archs4py as a4
+
+a4.align.load(["SRR14457464"], "data/example_1")
+
+result = a4.align.fastq("human", "data/example_1/SRR14457464.fastq", return_type="gene", identifier="symbol")
+
+```
+
+The next example is a SRR file that extracts into a pair of paired end FASTQ files. They can be passed to ARCHS4py like this:
+
+```python
+import xalign
+
+# the sample is paired-end and will result in two files (SRR15972519_1.fastq, SRR15972519_2.fastq)
+a4.align.load(["SRR15972519"], "data/example_2")
 
+result = a4.align.fastq("homo_sapiens", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
+
+```
+
+### Align FASTQ files from folder
+
+Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
+
+```python
+
+import archs4py as a4
+
+a4.align.load(["SRR15972519", "SRR15972520", "SRR15972521"], "data/example_3")
+
+result = a4.align.fastq("mouse", "data/example_3", return_type="gene", identifier="symbol")
+
+```
+
+## List versions
+<span id="#version"></span>
 ARCHS4 has different versions to download from. Recommended is the default setting, which will download the latest data release.
 
 ```python
 import archs4 as a4
 
 print(a4.versions())
 
 ```
+
+# Citation
+
+When using ARCHS4 please cite the following reference:
+
+Lachmann, Alexander, Denis Torre, Alexandra B. Keenan, Kathleen M. Jagodnik, Hoyjin J. Lee, Lily Wang, Moshe C. Silverstein, and Avi Ma’ayan. "Massive mining of publicly available RNA-seq data from human and mouse." Nature communications 9, no. 1 (2018): 1366.
+https://www.nature.com/articles/s41467-018-03751-6
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `archs4py-0.2.1/README.md` & `archs4py-0.2.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 <img title="archs4py" alt="archs4py" src="https://user-images.githubusercontent.com/32603869/243101679-c5147d56-fce0-4498-9577-a300df7d6dce.png">
 
 # archs4py - Official Python package to load and query ARCHS4 data
 
 Official ARCHS4 compagnion package. This package is a wrapper for basic H5 commands performed on the ARCHS4 data files. Some of the data access is optimized for specific query strategies and should make this implementation faster than manually querying the data. The package supports automated file download, mutithreading, and some convenience functions such as data normalization.
 
+ARCHS4py also supports the ARCHS4 alignment pipeline. When aligning FASTQ files using ARCHS4py gene and transcript counts will be compatible with the preprocessed ARCHS4 samples.
+
+[Installation](#installation) | [Download H5 Files](#usage) | [List H5 Contents](#list-data-fields-in-h5) | [Extract Counts](#data-access) | [Extract Meta Data](#meta-data) | [Normalize Samples](#normalizing-data) | [FASTQ Alignment](#sequence-alignment) | [Versions](#list-versions)
+
 ## ARCHS4 data
 
 ARCHS4 data is regularly updated to include publically available gene expression samples from RNA-seq. ARCHS4 processes the major platforms for human and mouse. As of 6/2023 ARCHS4 encompasses more than 1.5 million RNA-seq samples. All samples in ARCHS4 are homogeniously processed. ARCHS4 does currently not decern whether samples are bulk or single-cell and purely crawls GEO. Since samples are not always correctly annotated as single cell ARCHS4 uses a machine learning approach to predict single-cell samples and associated a singlecellprobability to each sample. Samples with a value larger than 0.5 can be removed from the queries if needed.
 
 ## Installation
 
 The python package can be directly installed from this GitHub repository using the following command (pip or pip3 depending on system setup)
@@ -16,37 +20,39 @@
 pip3 install archs4py
 ```
 
 ## Usage
 
 ### Download data file
 
+
 The data is stored in large HDF5 files which first need to be downloaded. HDF5 stores matrix information in a compressed datastructure that allows efficient data access to slices of the data. There are separate files for `human` and `mouse` data. The supported files are `gene counts` and `transcript counts`. As of 6/2023 the files are larger than 30GB and depending on the network speed will take some time to download.
 
 ```python
 import archs4py as a4
 
 file_path = a4.download.counts("human", path="", version="latest")
 ```
 
-### List data fields in H5
+## List data fields in H5
 
 The H5 files contain data and meta data information. To list the contents of ARCHS4 H5 files use the built in `ls` function.
 
-```
+```python
 import archs4py as a4
 
 file = "human_gene_v2.2.h5"
 a4.ls(file)
 ```
 
-### Data access
+## Data access
 
 archs4py supports several ways to load gene expression data. When querying ARCHS4 be aware that when loading too many samples the system might run out of memory. (e.g. the meta data search term is very broad). In most cases loading several thousand samples at the same time should be no problem. To find relevant samples there are 5 main functions in the `archs4py.data` module. A function to extract N random samples `archs4py.data.rand()`, a function to extract samples by index `archs4py.data.index()`, a function to extract samples based on meta data search `archs4py.data.meta()`, a function to extract samples based on a list of geo accessions `archs4py.data.samples()` and lastly a function to extract all samples belonging to a series `archs4.data.series()`.
 
+<span id="#extract-counts"></span>
 
 #### Extract a random set of samples
 
 To extract a random gene expression matrix use the `archs4py.data.rand()` function. The function will return a pandas dataframe with samples as columns and genes as rows.
 
 ```python
 import archs4py as a4
@@ -115,15 +121,17 @@
 file = "human_gene_v2.2.h5"
 
 #get sample counts
 series_counts = a4.data.series(file, "GSE64016")
 
 ```
 
-### Meta data
+## Meta data
+
+<span id="#extract-meta"></span>
 
 Additinally to the data module archs4py also supports the extraction of meta data. It supports similar endpoints to the `archs4.data` module. Meta data fields can be specified with: `meta_fields=["geo_accession", "series_id", "characteristics_ch1", "extract_protocol_ch1", "source_name_ch1", "title"]`
 
 ```python
 import archs4py as a4
 
 #path to file
@@ -136,32 +144,87 @@
 sample_meta = a4.meta.samples(file, ["GSM1158284","GSM1482938","GSM1562817"])
 
 # get series meta data
 series_meta = a4.meta.series(file, "GSE64016")
 
 ```
 
-### Normalizing data
-
+## Normalizing data
+<span id="#normalize"></span>
 The package also supports simple normalization. Currently supported are quantile normalization, log2 + quantile normalization, and cpm. In the example below we load 100 random samples and apply log quantile.
 
 ```python
 import archs4py as a4
 
 file = "human_gene_v2.2.h5"
 rand_counts = a4.data.rand(file, 100)
 
 #normalize using log quantile (method options for now = ["log_quantile", "quantile", "cpm", "tmm"])
 norm_exp = a4.normalize(rand_counts, method="log_quantile")
 
 ```
 
-### List versions
+## Sequence alignment
+<span id="#align"></span>
+The `align` module contains a replication of the ARCHS4 alignment pipeline. When used on FASTQ files the resulting gene or transcript counts are compatible with the previously aligned samples in ARCHS4. The package is highly automated and only required a path to a FASTQ file or a folder containing multiple FASTQ files. All file dependencies will downloaded automatically and index will be built when needed.
+
+### Align FASTQ file
+
+Pass either a single or paired FASTQ file. This function can return transcript count, gene counts, or transcript level TPM data.
+
+```python
+
+import archs4py as a4
+
+a4.align.load(["SRR14457464"], "data/example_1")
+
+result = a4.align.fastq("human", "data/example_1/SRR14457464.fastq", return_type="gene", identifier="symbol")
+
+```
+
+The next example is a SRR file that extracts into a pair of paired end FASTQ files. They can be passed to ARCHS4py like this:
+
+```python
+import xalign
+
+# the sample is paired-end and will result in two files (SRR15972519_1.fastq, SRR15972519_2.fastq)
+a4.align.load(["SRR15972519"], "data/example_2")
 
+result = a4.align.fastq("homo_sapiens", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
+
+```
+
+### Align FASTQ files from folder
+
+Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
+
+```python
+
+import archs4py as a4
+
+a4.align.load(["SRR15972519", "SRR15972520", "SRR15972521"], "data/example_3")
+
+result = a4.align.fastq("mouse", "data/example_3", return_type="gene", identifier="symbol")
+
+```
+
+## List versions
+<span id="#version"></span>
 ARCHS4 has different versions to download from. Recommended is the default setting, which will download the latest data release.
 
 ```python
 import archs4 as a4
 
 print(a4.versions())
 
 ```
+
+# Citation
+
+When using ARCHS4 please cite the following reference:
+
+Lachmann, Alexander, Denis Torre, Alexandra B. Keenan, Kathleen M. Jagodnik, Hoyjin J. Lee, Lily Wang, Moshe C. Silverstein, and Avi Ma’ayan. "Massive mining of publicly available RNA-seq data from human and mouse." Nature communications 9, no. 1 (2018): 1366.
+https://www.nature.com/articles/s41467-018-03751-6
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `archs4py-0.2.1/archs4py/align.py` & `archs4py-0.2.3/archs4py/align.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     if identifier == "symbol":
         gm = gene_mapping[species].copy()
         gm.index = gm.loc[:, "ensembl_gene"]
         gm = gm[~gm.index.duplicated(keep='first')]
         trans.index = gm.loc[trans.index, "symbol"]
     return trans
 
-
 def get_ensembl_mappings(species, release):  
     server = biomart.BiomartServer(conf["ALIGNMENT"][str(release)]["biomart"])
     if species == "mus_musculus":
         mart = server.datasets['mmusculus_gene_ensembl']
         attributes = ['ensembl_transcript_id', 'mgi_symbol', 'ensembl_gene_id', 'gene_biotype']
     else:
         mart = server.datasets['hsapiens_gene_ensembl']
@@ -73,8 +72,12 @@
         ensembl_ids.append(line)
     gene_map = pd.DataFrame(ensembl_ids)
     gene_map.index = gene_map.iloc[:,0]
     nn = np.where(gene_map.iloc[:,1] == "")[0]
     gene_map.iloc[nn, 1] = gene_map.iloc[nn, 2]
     gene_map.columns = ["ensembl_transcript", "symbol", "ensembl_gene", "biotype"]
     gene_map = gene_map[~gene_map.index.duplicated(keep='first')]
-    return gene_map
+    return gene_map
+
+def load(sras, outfolder):
+    xalign.sra.load_sras(sras, outfolder)
+    print("download complete")
```

### Comparing `archs4py-0.2.1/archs4py/data/config.json` & `archs4py-0.2.3/archs4py/data/config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'DOWNLOAD_URL'": "'https://maayanlab.cloud/archs4/search/downloadcounter.php'"}*

```diff
@@ -5,14 +5,15 @@
             "release": 107
         },
         "latest": {
             "biomart": "http://jul2022.archive.ensembl.org/biomart",
             "release": 107
         }
     },
+    "DOWNLOAD_URL": "https://maayanlab.cloud/archs4/search/downloadcounter.php",
     "GENE_COUNTS": {
         "HUMAN": {
             "1.11": {
                 "fallback": "https://s3.amazonaws.com/mssm-seq-matrix/human_matrix_v11.h5",
                 "primary": "https://s3.amazonaws.com/mssm-seq-matrix/human_matrix_v11.h5"
             },
             "2.1.2": {
```

### Comparing `archs4py-0.2.1/archs4py/data.py` & `archs4py-0.2.3/archs4py/data.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.1/archs4py/download.py` & `archs4py-0.2.3/archs4py/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import wget
 import sys
 import requests
-from tqdm import tqdm
 import archs4py.utils
+import requests
+import os
 
 def bar_progress(current, total, width=80, update_interval=10):
     current_gb = current / (1024**3)  # Convert current bytes to GB
     total_gb = total / (1024**3)  # Convert total bytes to GB
     
     if current % (update_interval * 1024**2) == 0:  # Update progress every 10 MB
         progress_message = "Downloading: %d%% [%.2f GB / %.2f GB]" % (current / total * 100, current_gb, total_gb)
@@ -36,13 +37,21 @@
         Supported count types:
         - GENE_COUNTS: Gene-level count files.
         - TRANSCRIPT_COUNTS: Transcript-level count files.
     """
     conf = archs4py.utils.get_config()
 
     try:
+        file_name = os.path.basename(conf[type][species.upper()][version]["primary"])
+        download_url = conf["DOWNLOAD_URL"]
+        url = f"{download_url}?&file={file_name}&version=1337"
+        response = requests.get(url)
+    except:
+        x = "just continue"
+    
+    try:
         fpath = wget.download(conf[type][species.upper()][version]["primary"], out=path, bar=bar_progress)
         print("file downloaded to", fpath)
     except Exception:
         fpath = wget.download(conf[type][species.upper()][version]["fallback"], out=path, bar=bar_progress)
         print("file downloaded to", fpath)
```

### Comparing `archs4py-0.2.1/archs4py/meta.py` & `archs4py-0.2.3/archs4py/meta.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.1/archs4py/utils.py` & `archs4py-0.2.3/archs4py/utils.py`

 * *Files identical despite different names*

### Comparing `archs4py-0.2.1/archs4py.egg-info/PKG-INFO` & `archs4py-0.2.3/archs4py.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archs4py
-Version: 0.2.1
+Version: 0.2.3
 Summary: ARCHS4 python package supporting data loading and data queries.
 Home-page: https://github.com/maayanlab/archs4py
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,18 @@
 
 <img title="archs4py" alt="archs4py" src="https://user-images.githubusercontent.com/32603869/243101679-c5147d56-fce0-4498-9577-a300df7d6dce.png">
 
 # archs4py - Official Python package to load and query ARCHS4 data
 
 Official ARCHS4 compagnion package. This package is a wrapper for basic H5 commands performed on the ARCHS4 data files. Some of the data access is optimized for specific query strategies and should make this implementation faster than manually querying the data. The package supports automated file download, mutithreading, and some convenience functions such as data normalization.
 
+ARCHS4py also supports the ARCHS4 alignment pipeline. When aligning FASTQ files using ARCHS4py gene and transcript counts will be compatible with the preprocessed ARCHS4 samples.
+
+[Installation](#installation) | [Download H5 Files](#usage) | [List H5 Contents](#list-data-fields-in-h5) | [Extract Counts](#data-access) | [Extract Meta Data](#meta-data) | [Normalize Samples](#normalizing-data) | [FASTQ Alignment](#sequence-alignment) | [Versions](#list-versions)
+
 ## ARCHS4 data
 
 ARCHS4 data is regularly updated to include publically available gene expression samples from RNA-seq. ARCHS4 processes the major platforms for human and mouse. As of 6/2023 ARCHS4 encompasses more than 1.5 million RNA-seq samples. All samples in ARCHS4 are homogeniously processed. ARCHS4 does currently not decern whether samples are bulk or single-cell and purely crawls GEO. Since samples are not always correctly annotated as single cell ARCHS4 uses a machine learning approach to predict single-cell samples and associated a singlecellprobability to each sample. Samples with a value larger than 0.5 can be removed from the queries if needed.
 
 ## Installation
 
 The python package can be directly installed from this GitHub repository using the following command (pip or pip3 depending on system setup)
@@ -30,37 +34,39 @@
 pip3 install archs4py
 ```
 
 ## Usage
 
 ### Download data file
 
+
 The data is stored in large HDF5 files which first need to be downloaded. HDF5 stores matrix information in a compressed datastructure that allows efficient data access to slices of the data. There are separate files for `human` and `mouse` data. The supported files are `gene counts` and `transcript counts`. As of 6/2023 the files are larger than 30GB and depending on the network speed will take some time to download.
 
 ```python
 import archs4py as a4
 
 file_path = a4.download.counts("human", path="", version="latest")
 ```
 
-### List data fields in H5
+## List data fields in H5
 
 The H5 files contain data and meta data information. To list the contents of ARCHS4 H5 files use the built in `ls` function.
 
-```
+```python
 import archs4py as a4
 
 file = "human_gene_v2.2.h5"
 a4.ls(file)
 ```
 
-### Data access
+## Data access
 
 archs4py supports several ways to load gene expression data. When querying ARCHS4 be aware that when loading too many samples the system might run out of memory. (e.g. the meta data search term is very broad). In most cases loading several thousand samples at the same time should be no problem. To find relevant samples there are 5 main functions in the `archs4py.data` module. A function to extract N random samples `archs4py.data.rand()`, a function to extract samples by index `archs4py.data.index()`, a function to extract samples based on meta data search `archs4py.data.meta()`, a function to extract samples based on a list of geo accessions `archs4py.data.samples()` and lastly a function to extract all samples belonging to a series `archs4.data.series()`.
 
+<span id="#extract-counts"></span>
 
 #### Extract a random set of samples
 
 To extract a random gene expression matrix use the `archs4py.data.rand()` function. The function will return a pandas dataframe with samples as columns and genes as rows.
 
 ```python
 import archs4py as a4
@@ -129,15 +135,17 @@
 file = "human_gene_v2.2.h5"
 
 #get sample counts
 series_counts = a4.data.series(file, "GSE64016")
 
 ```
 
-### Meta data
+## Meta data
+
+<span id="#extract-meta"></span>
 
 Additinally to the data module archs4py also supports the extraction of meta data. It supports similar endpoints to the `archs4.data` module. Meta data fields can be specified with: `meta_fields=["geo_accession", "series_id", "characteristics_ch1", "extract_protocol_ch1", "source_name_ch1", "title"]`
 
 ```python
 import archs4py as a4
 
 #path to file
@@ -150,32 +158,87 @@
 sample_meta = a4.meta.samples(file, ["GSM1158284","GSM1482938","GSM1562817"])
 
 # get series meta data
 series_meta = a4.meta.series(file, "GSE64016")
 
 ```
 
-### Normalizing data
-
+## Normalizing data
+<span id="#normalize"></span>
 The package also supports simple normalization. Currently supported are quantile normalization, log2 + quantile normalization, and cpm. In the example below we load 100 random samples and apply log quantile.
 
 ```python
 import archs4py as a4
 
 file = "human_gene_v2.2.h5"
 rand_counts = a4.data.rand(file, 100)
 
 #normalize using log quantile (method options for now = ["log_quantile", "quantile", "cpm", "tmm"])
 norm_exp = a4.normalize(rand_counts, method="log_quantile")
 
 ```
 
-### List versions
+## Sequence alignment
+<span id="#align"></span>
+The `align` module contains a replication of the ARCHS4 alignment pipeline. When used on FASTQ files the resulting gene or transcript counts are compatible with the previously aligned samples in ARCHS4. The package is highly automated and only required a path to a FASTQ file or a folder containing multiple FASTQ files. All file dependencies will downloaded automatically and index will be built when needed.
+
+### Align FASTQ file
+
+Pass either a single or paired FASTQ file. This function can return transcript count, gene counts, or transcript level TPM data.
+
+```python
+
+import archs4py as a4
+
+a4.align.load(["SRR14457464"], "data/example_1")
+
+result = a4.align.fastq("human", "data/example_1/SRR14457464.fastq", return_type="gene", identifier="symbol")
+
+```
+
+The next example is a SRR file that extracts into a pair of paired end FASTQ files. They can be passed to ARCHS4py like this:
+
+```python
+import xalign
+
+# the sample is paired-end and will result in two files (SRR15972519_1.fastq, SRR15972519_2.fastq)
+a4.align.load(["SRR15972519"], "data/example_2")
 
+result = a4.align.fastq("homo_sapiens", ["data/example_2/SRR15972519_1.fastq", "data/example_2/SRR15972519_2.fastq"], return_type="transcript")
+
+```
+
+### Align FASTQ files from folder
+
+Align all FASTQ files in folder. ARCHS4py will automatically matching samples if data is paired end.
+
+```python
+
+import archs4py as a4
+
+a4.align.load(["SRR15972519", "SRR15972520", "SRR15972521"], "data/example_3")
+
+result = a4.align.fastq("mouse", "data/example_3", return_type="gene", identifier="symbol")
+
+```
+
+## List versions
+<span id="#version"></span>
 ARCHS4 has different versions to download from. Recommended is the default setting, which will download the latest data release.
 
 ```python
 import archs4 as a4
 
 print(a4.versions())
 
 ```
+
+# Citation
+
+When using ARCHS4 please cite the following reference:
+
+Lachmann, Alexander, Denis Torre, Alexandra B. Keenan, Kathleen M. Jagodnik, Hoyjin J. Lee, Lily Wang, Moshe C. Silverstein, and Avi Ma’ayan. "Massive mining of publicly available RNA-seq data from human and mouse." Nature communications 9, no. 1 (2018): 1366.
+https://www.nature.com/articles/s41467-018-03751-6
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `archs4py-0.2.1/setup.py` & `archs4py-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="archs4py",
-    version="0.2.1",
+    version="0.2.3",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="ARCHS4 python package supporting data loading and data queries.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/archs4py",
     packages=setuptools.find_packages(),
```


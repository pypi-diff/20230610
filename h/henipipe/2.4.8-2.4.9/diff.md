# Comparing `tmp/henipipe-2.4.8.tar.gz` & `tmp/henipipe-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henipipe-2.4.8.tar", last modified: Sat Jun 10 03:38:29 2023, max compression
+gzip compressed data, was "henipipe-2.4.9.tar", last modified: Sat Jun 10 03:47:42 2023, max compression
```

## Comparing `henipipe-2.4.8.tar` & `henipipe-2.4.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.998678 henipipe-2.4.8/
--rwx------   0 sfurlan    (504) staff       (20)     1073 2019-09-12 05:36:58.000000 henipipe-2.4.8/LICENSE
--rwx------   0 sfurlan    (504) staff       (20)       42 2019-09-14 15:59:55.000000 henipipe-2.4.8/MANIFEST.in
--rw-r--r--   0 sfurlan    (504) staff       (20)    20743 2023-06-10 03:38:28.998467 henipipe-2.4.8/PKG-INFO
--rwxr-xr-x   0 sfurlan    (504) staff       (20)    20249 2023-06-10 03:10:15.000000 henipipe-2.4.8/README.md
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.995357 henipipe-2.4.8/henipipe/
--rwx------   0 sfurlan    (504) staff       (20)       21 2023-06-10 03:04:29.000000 henipipe-2.4.8/henipipe/__init__.py
--rwx------   0 sfurlan    (504) staff       (20)    18263 2022-12-28 21:07:38.000000 henipipe-2.4.8/henipipe/__main__.py
--rwx------   0 sfurlan    (504) staff       (20)     6183 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/auc.py
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.996671 henipipe-2.4.8/henipipe/data/
--rwx------   0 sfurlan    (504) staff       (20)     6626 2023-06-10 03:03:01.000000 henipipe-2.4.8/henipipe/data/environs.json
--rwx------   0 sfurlan    (504) staff       (20)     2405 2021-08-12 17:13:13.000000 henipipe-2.4.8/henipipe/data/genomes.json
--rwx------   0 sfurlan    (504) staff       (20)    64563 2022-12-09 01:15:59.000000 henipipe-2.4.8/henipipe/henipipe.py
--rwx------   0 sfurlan    (504) staff       (20)     1095 2019-09-13 03:55:32.000000 henipipe-2.4.8/henipipe/pyWriter.py
--rwx------   0 sfurlan    (504) staff       (20)     2480 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/samComp.py
--rwx------   0 sfurlan    (504) staff       (20)    29213 2019-09-17 13:51:36.000000 henipipe-2.4.8/henipipe/samTobed.py
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.998015 henipipe-2.4.8/henipipe/scripts/
--rwx------   0 sfurlan    (504) staff       (20)     5605 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.1.R
--rwx------   0 sfurlan    (504) staff       (20)     8016 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.1.sh
--rwx------   0 sfurlan    (504) staff       (20)     6996 2020-02-13 05:35:33.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.3.R
--rwx------   0 sfurlan    (504) staff       (20)     8310 2020-02-13 05:35:33.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.3.sh
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.996354 henipipe-2.4.8/henipipe.egg-info/
--rwx------   0 sfurlan    (504) staff       (20)    20743 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/PKG-INFO
--rwx------   0 sfurlan    (504) staff       (20)      546 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/SOURCES.txt
--rwx------   0 sfurlan    (504) staff       (20)        1 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/dependency_links.txt
--rwx------   0 sfurlan    (504) staff       (20)      170 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/entry_points.txt
--rwx------   0 sfurlan    (504) staff       (20)        7 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/requires.txt
--rwx------   0 sfurlan    (504) staff       (20)        9 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/top_level.txt
--rw-r--r--   0 sfurlan    (504) staff       (20)       38 2023-06-10 03:38:28.998739 henipipe-2.4.8/setup.cfg
--rwx------   0 sfurlan    (504) staff       (20)     3027 2022-12-28 21:08:11.000000 henipipe-2.4.8/setup.py
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:47:42.143650 henipipe-2.4.9/
+-rwx------   0 sfurlan    (504) staff       (20)     1073 2019-09-12 05:36:58.000000 henipipe-2.4.9/LICENSE
+-rwx------   0 sfurlan    (504) staff       (20)       42 2019-09-14 15:59:55.000000 henipipe-2.4.9/MANIFEST.in
+-rw-r--r--   0 sfurlan    (504) staff       (20)    20745 2023-06-10 03:47:42.143346 henipipe-2.4.9/PKG-INFO
+-rwxr-xr-x   0 sfurlan    (504) staff       (20)    20251 2023-06-10 03:46:58.000000 henipipe-2.4.9/README.md
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:47:42.140254 henipipe-2.4.9/henipipe/
+-rwx------   0 sfurlan    (504) staff       (20)       21 2023-06-10 03:46:40.000000 henipipe-2.4.9/henipipe/__init__.py
+-rwx------   0 sfurlan    (504) staff       (20)    18263 2022-12-28 21:07:38.000000 henipipe-2.4.9/henipipe/__main__.py
+-rwx------   0 sfurlan    (504) staff       (20)     6183 2020-02-10 23:29:46.000000 henipipe-2.4.9/henipipe/auc.py
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:47:42.141862 henipipe-2.4.9/henipipe/data/
+-rwx------   0 sfurlan    (504) staff       (20)     6626 2023-06-10 03:46:35.000000 henipipe-2.4.9/henipipe/data/environs.json
+-rwx------   0 sfurlan    (504) staff       (20)     2405 2021-08-12 17:13:13.000000 henipipe-2.4.9/henipipe/data/genomes.json
+-rwx------   0 sfurlan    (504) staff       (20)    64563 2022-12-09 01:15:59.000000 henipipe-2.4.9/henipipe/henipipe.py
+-rwx------   0 sfurlan    (504) staff       (20)     1095 2019-09-13 03:55:32.000000 henipipe-2.4.9/henipipe/pyWriter.py
+-rwx------   0 sfurlan    (504) staff       (20)     2480 2020-02-10 23:29:46.000000 henipipe-2.4.9/henipipe/samComp.py
+-rwx------   0 sfurlan    (504) staff       (20)    29213 2019-09-17 13:51:36.000000 henipipe-2.4.9/henipipe/samTobed.py
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:47:42.142971 henipipe-2.4.9/henipipe/scripts/
+-rwx------   0 sfurlan    (504) staff       (20)     5605 2020-02-10 23:29:46.000000 henipipe-2.4.9/henipipe/scripts/SEACR_1.1.R
+-rwx------   0 sfurlan    (504) staff       (20)     8016 2020-02-10 23:29:46.000000 henipipe-2.4.9/henipipe/scripts/SEACR_1.1.sh
+-rwx------   0 sfurlan    (504) staff       (20)     6996 2020-02-13 05:35:33.000000 henipipe-2.4.9/henipipe/scripts/SEACR_1.3.R
+-rwx------   0 sfurlan    (504) staff       (20)     8310 2020-02-13 05:35:33.000000 henipipe-2.4.9/henipipe/scripts/SEACR_1.3.sh
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:47:42.141535 henipipe-2.4.9/henipipe.egg-info/
+-rwx------   0 sfurlan    (504) staff       (20)    20745 2023-06-10 03:47:41.000000 henipipe-2.4.9/henipipe.egg-info/PKG-INFO
+-rwx------   0 sfurlan    (504) staff       (20)      546 2023-06-10 03:47:42.000000 henipipe-2.4.9/henipipe.egg-info/SOURCES.txt
+-rwx------   0 sfurlan    (504) staff       (20)        1 2023-06-10 03:47:41.000000 henipipe-2.4.9/henipipe.egg-info/dependency_links.txt
+-rwx------   0 sfurlan    (504) staff       (20)      170 2023-06-10 03:47:41.000000 henipipe-2.4.9/henipipe.egg-info/entry_points.txt
+-rwx------   0 sfurlan    (504) staff       (20)        7 2023-06-10 03:47:41.000000 henipipe-2.4.9/henipipe.egg-info/requires.txt
+-rwx------   0 sfurlan    (504) staff       (20)        9 2023-06-10 03:47:41.000000 henipipe-2.4.9/henipipe.egg-info/top_level.txt
+-rw-r--r--   0 sfurlan    (504) staff       (20)       38 2023-06-10 03:47:42.143704 henipipe-2.4.9/setup.cfg
+-rwx------   0 sfurlan    (504) staff       (20)     3228 2023-06-10 03:43:28.000000 henipipe-2.4.9/setup.py
```

### Comparing `henipipe-2.4.8/LICENSE` & `henipipe-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/PKG-INFO` & `henipipe-2.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henipipe
-Version: 2.4.8
+Version: 2.4.9
 Summary: A python wrapper for fast and parallel processing of sequencing data using CutnRun or CutnTag
 Home-page: https://github.com/scfurl/henipipe.git
 Author: Scott Furlan
 Author-email: scottfurlan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,22 +23,22 @@
 
 # henipipe
 ==========
 
 
 
 
-Version 2.4.8
+Version 2.4.9
 
 A python wrapper for processing of sequencing data generated using CutnRun or CutnTag (developed by the Henikoff lab FHCRC).  Now with a single-cell option ('SC') for processing CutnTag data generated using the iCell8 platform (Takara).
 
-## New in version 2.4
+## New in version 2.4.x
 
 1. Added a --version function
-2. In version 2.4.8 - environs.json was properly configured for PBS; see below for using a project ID with PBS
+2. In version 2.4.9 - environs.json was properly configured for PBS; see below for using a project ID with PBS
 
 ## New in version 2.3
 
 1. Henipipe adds a new function, DEDUP.  DEDUP will remove presumed PCR duplicates from the bed file but leave a record of how many were detected.  The DEDUP funciton is meant to be used after ALIGN and before other downstream functions.  It will replace the bed file with a collapsed bedfile with a new column that counts the number of presumed duplicates found.  Note that read pairs will be collapsed regardless of strand and all strand data will be changed to positive.  
 2. Henipipe adds a new function, BLACKLIST.  BLACKLIST will remove bed entries that overlap with a user-specified blacklist file designated with the '-bl' flag.
 2. Changes to MACS2 function were made in this version to allow custom parameters to be passed to MACS2 peak calling using the -M2p flag.
 3. Fixed a bug in SCALE function
```

### Comparing `henipipe-2.4.8/README.md` & `henipipe-2.4.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 # henipipe
 ==========
 
 
 
 
-Version 2.4.8
+Version 2.4.9
 
 A python wrapper for processing of sequencing data generated using CutnRun or CutnTag (developed by the Henikoff lab FHCRC).  Now with a single-cell option ('SC') for processing CutnTag data generated using the iCell8 platform (Takara).
 
-## New in version 2.4
+## New in version 2.4.x
 
 1. Added a --version function
-2. In version 2.4.8 - environs.json was properly configured for PBS; see below for using a project ID with PBS
+2. In version 2.4.9 - environs.json was properly configured for PBS; see below for using a project ID with PBS
 
 ## New in version 2.3
 
 1. Henipipe adds a new function, DEDUP.  DEDUP will remove presumed PCR duplicates from the bed file but leave a record of how many were detected.  The DEDUP funciton is meant to be used after ALIGN and before other downstream functions.  It will replace the bed file with a collapsed bedfile with a new column that counts the number of presumed duplicates found.  Note that read pairs will be collapsed regardless of strand and all strand data will be changed to positive.  
 2. Henipipe adds a new function, BLACKLIST.  BLACKLIST will remove bed entries that overlap with a user-specified blacklist file designated with the '-bl' flag.
 2. Changes to MACS2 function were made in this version to allow custom parameters to be passed to MACS2 peak calling using the -M2p flag.
 3. Fixed a bug in SCALE function
```

### Comparing `henipipe-2.4.8/henipipe/__main__.py` & `henipipe-2.4.9/henipipe/__main__.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/auc.py` & `henipipe-2.4.9/henipipe/auc.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/data/environs.json` & `henipipe-2.4.9/henipipe/data/environs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'PBS'": "{'array_script_lines': {'3': {insert: [(0, '#PBS -N <--0-->\\n#PBS -q paidq\\n#PBS -P "*

 * *          "$PROJECT')], delete: [0]}}}"}*

```diff
@@ -6,15 +6,15 @@
                 ""
             ],
             "2": [
                 "#PBS -J 1-<--0-->:1",
                 "ARRAY_COUNT"
             ],
             "3": [
-                "#PBS -n <--0-->\n#PBS -q paidq\n#PBS -P $PROJECT",
+                "#PBS -N <--0-->\n#PBS -q paidq\n#PBS -P $PROJECT",
                 "JOB_NAME"
             ],
             "4": [
                 "#PBS -l nodes=1:ppn=<--0-->",
                 "THREADS"
             ],
             "5": [
```

### Comparing `henipipe-2.4.8/henipipe/data/genomes.json` & `henipipe-2.4.9/henipipe/data/genomes.json`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/henipipe.py` & `henipipe-2.4.9/henipipe/henipipe.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/pyWriter.py` & `henipipe-2.4.9/henipipe/pyWriter.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/samComp.py` & `henipipe-2.4.9/henipipe/samComp.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/samTobed.py` & `henipipe-2.4.9/henipipe/samTobed.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/scripts/SEACR_1.1.R` & `henipipe-2.4.9/henipipe/scripts/SEACR_1.1.R`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/scripts/SEACR_1.1.sh` & `henipipe-2.4.9/henipipe/scripts/SEACR_1.1.sh`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/scripts/SEACR_1.3.R` & `henipipe-2.4.9/henipipe/scripts/SEACR_1.3.R`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe/scripts/SEACR_1.3.sh` & `henipipe-2.4.9/henipipe/scripts/SEACR_1.3.sh`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/henipipe.egg-info/PKG-INFO` & `henipipe-2.4.9/henipipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henipipe
-Version: 2.4.8
+Version: 2.4.9
 Summary: A python wrapper for fast and parallel processing of sequencing data using CutnRun or CutnTag
 Home-page: https://github.com/scfurl/henipipe.git
 Author: Scott Furlan
 Author-email: scottfurlan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,22 +23,22 @@
 
 # henipipe
 ==========
 
 
 
 
-Version 2.4.8
+Version 2.4.9
 
 A python wrapper for processing of sequencing data generated using CutnRun or CutnTag (developed by the Henikoff lab FHCRC).  Now with a single-cell option ('SC') for processing CutnTag data generated using the iCell8 platform (Takara).
 
-## New in version 2.4
+## New in version 2.4.x
 
 1. Added a --version function
-2. In version 2.4.8 - environs.json was properly configured for PBS; see below for using a project ID with PBS
+2. In version 2.4.9 - environs.json was properly configured for PBS; see below for using a project ID with PBS
 
 ## New in version 2.3
 
 1. Henipipe adds a new function, DEDUP.  DEDUP will remove presumed PCR duplicates from the bed file but leave a record of how many were detected.  The DEDUP funciton is meant to be used after ALIGN and before other downstream functions.  It will replace the bed file with a collapsed bedfile with a new column that counts the number of presumed duplicates found.  Note that read pairs will be collapsed regardless of strand and all strand data will be changed to positive.  
 2. Henipipe adds a new function, BLACKLIST.  BLACKLIST will remove bed entries that overlap with a user-specified blacklist file designated with the '-bl' flag.
 2. Changes to MACS2 function were made in this version to allow custom parameters to be passed to MACS2 peak calling using the -M2p flag.
 3. Fixed a bug in SCALE function
```

### Comparing `henipipe-2.4.8/henipipe.egg-info/SOURCES.txt` & `henipipe-2.4.9/henipipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.8/setup.py` & `henipipe-2.4.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,8 +93,15 @@
 
 #proceed with henipipe steps
 henipipe ALIGN -t 16 -r runsheet.csv -n spike_in
 henipipe SCALE -r runsheet_fixed.csv -n spike_in
 henipipe SEACR -r runsheet_fixed.csv
 
 
+## running dest data at SCRI
+cd /home/sfurla/develop/henipipe/test_data
+mkdir henipipe
+cd henipipe
+henipipe MAKERUNSHEET -fq ../fastq -c PBS -gk furlan_hg38
+henipipe ALIGN -t 4 -r runsheet.csv -c PBS
+
 """
```


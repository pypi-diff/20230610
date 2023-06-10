# Comparing `tmp/henipipe-2.4.7.tar.gz` & `tmp/henipipe-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henipipe-2.4.7.tar", last modified: Wed Dec 28 21:08:19 2022, max compression
+gzip compressed data, was "henipipe-2.4.8.tar", last modified: Sat Jun 10 03:38:29 2023, max compression
```

## Comparing `henipipe-2.4.7.tar` & `henipipe-2.4.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2022-12-28 21:08:19.766399 henipipe-2.4.7/
--rwx------   0 sfurlan    (504) staff       (20)     1073 2019-09-12 05:36:58.000000 henipipe-2.4.7/LICENSE
--rwx------   0 sfurlan    (504) staff       (20)       42 2019-09-14 15:59:55.000000 henipipe-2.4.7/MANIFEST.in
--rw-r--r--   0 sfurlan    (504) staff       (20)    20243 2022-12-28 21:08:19.766174 henipipe-2.4.7/PKG-INFO
--rwxr-xr-x   0 sfurlan    (504) staff       (20)    19749 2022-12-28 20:43:03.000000 henipipe-2.4.7/README.md
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2022-12-28 21:08:19.763846 henipipe-2.4.7/henipipe/
--rwx------   0 sfurlan    (504) staff       (20)       21 2022-12-28 21:08:00.000000 henipipe-2.4.7/henipipe/__init__.py
--rwx------   0 sfurlan    (504) staff       (20)    18263 2022-12-28 21:07:38.000000 henipipe-2.4.7/henipipe/__main__.py
--rwx------   0 sfurlan    (504) staff       (20)     6183 2020-02-10 23:29:46.000000 henipipe-2.4.7/henipipe/auc.py
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2022-12-28 21:08:19.765288 henipipe-2.4.7/henipipe/data/
--rwx------   0 sfurlan    (504) staff       (20)     6658 2022-12-09 01:17:41.000000 henipipe-2.4.7/henipipe/data/environs.json
--rwx------   0 sfurlan    (504) staff       (20)     2405 2021-08-12 17:13:13.000000 henipipe-2.4.7/henipipe/data/genomes.json
--rwx------   0 sfurlan    (504) staff       (20)    64563 2022-12-09 01:15:59.000000 henipipe-2.4.7/henipipe/henipipe.py
--rwx------   0 sfurlan    (504) staff       (20)     1095 2019-09-13 03:55:32.000000 henipipe-2.4.7/henipipe/pyWriter.py
--rwx------   0 sfurlan    (504) staff       (20)     2480 2020-02-10 23:29:46.000000 henipipe-2.4.7/henipipe/samComp.py
--rwx------   0 sfurlan    (504) staff       (20)    29213 2019-09-17 13:51:36.000000 henipipe-2.4.7/henipipe/samTobed.py
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2022-12-28 21:08:19.765939 henipipe-2.4.7/henipipe/scripts/
--rwx------   0 sfurlan    (504) staff       (20)     5605 2020-02-10 23:29:46.000000 henipipe-2.4.7/henipipe/scripts/SEACR_1.1.R
--rwx------   0 sfurlan    (504) staff       (20)     8016 2020-02-10 23:29:46.000000 henipipe-2.4.7/henipipe/scripts/SEACR_1.1.sh
--rwx------   0 sfurlan    (504) staff       (20)     6996 2020-02-13 05:35:33.000000 henipipe-2.4.7/henipipe/scripts/SEACR_1.3.R
--rwx------   0 sfurlan    (504) staff       (20)     8310 2020-02-13 05:35:33.000000 henipipe-2.4.7/henipipe/scripts/SEACR_1.3.sh
-drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2022-12-28 21:08:19.764961 henipipe-2.4.7/henipipe.egg-info/
--rwx------   0 sfurlan    (504) staff       (20)    20243 2022-12-28 21:08:19.000000 henipipe-2.4.7/henipipe.egg-info/PKG-INFO
--rwx------   0 sfurlan    (504) staff       (20)      546 2022-12-28 21:08:19.000000 henipipe-2.4.7/henipipe.egg-info/SOURCES.txt
--rwx------   0 sfurlan    (504) staff       (20)        1 2022-12-28 21:08:19.000000 henipipe-2.4.7/henipipe.egg-info/dependency_links.txt
--rwx------   0 sfurlan    (504) staff       (20)      170 2022-12-28 21:08:19.000000 henipipe-2.4.7/henipipe.egg-info/entry_points.txt
--rwx------   0 sfurlan    (504) staff       (20)        7 2022-12-28 21:08:19.000000 henipipe-2.4.7/henipipe.egg-info/requires.txt
--rwx------   0 sfurlan    (504) staff       (20)        9 2022-12-28 21:08:19.000000 henipipe-2.4.7/henipipe.egg-info/top_level.txt
--rw-r--r--   0 sfurlan    (504) staff       (20)       38 2022-12-28 21:08:19.766453 henipipe-2.4.7/setup.cfg
--rwx------   0 sfurlan    (504) staff       (20)     3027 2022-12-28 21:08:11.000000 henipipe-2.4.7/setup.py
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.998678 henipipe-2.4.8/
+-rwx------   0 sfurlan    (504) staff       (20)     1073 2019-09-12 05:36:58.000000 henipipe-2.4.8/LICENSE
+-rwx------   0 sfurlan    (504) staff       (20)       42 2019-09-14 15:59:55.000000 henipipe-2.4.8/MANIFEST.in
+-rw-r--r--   0 sfurlan    (504) staff       (20)    20743 2023-06-10 03:38:28.998467 henipipe-2.4.8/PKG-INFO
+-rwxr-xr-x   0 sfurlan    (504) staff       (20)    20249 2023-06-10 03:10:15.000000 henipipe-2.4.8/README.md
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.995357 henipipe-2.4.8/henipipe/
+-rwx------   0 sfurlan    (504) staff       (20)       21 2023-06-10 03:04:29.000000 henipipe-2.4.8/henipipe/__init__.py
+-rwx------   0 sfurlan    (504) staff       (20)    18263 2022-12-28 21:07:38.000000 henipipe-2.4.8/henipipe/__main__.py
+-rwx------   0 sfurlan    (504) staff       (20)     6183 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/auc.py
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.996671 henipipe-2.4.8/henipipe/data/
+-rwx------   0 sfurlan    (504) staff       (20)     6626 2023-06-10 03:03:01.000000 henipipe-2.4.8/henipipe/data/environs.json
+-rwx------   0 sfurlan    (504) staff       (20)     2405 2021-08-12 17:13:13.000000 henipipe-2.4.8/henipipe/data/genomes.json
+-rwx------   0 sfurlan    (504) staff       (20)    64563 2022-12-09 01:15:59.000000 henipipe-2.4.8/henipipe/henipipe.py
+-rwx------   0 sfurlan    (504) staff       (20)     1095 2019-09-13 03:55:32.000000 henipipe-2.4.8/henipipe/pyWriter.py
+-rwx------   0 sfurlan    (504) staff       (20)     2480 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/samComp.py
+-rwx------   0 sfurlan    (504) staff       (20)    29213 2019-09-17 13:51:36.000000 henipipe-2.4.8/henipipe/samTobed.py
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.998015 henipipe-2.4.8/henipipe/scripts/
+-rwx------   0 sfurlan    (504) staff       (20)     5605 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.1.R
+-rwx------   0 sfurlan    (504) staff       (20)     8016 2020-02-10 23:29:46.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.1.sh
+-rwx------   0 sfurlan    (504) staff       (20)     6996 2020-02-13 05:35:33.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.3.R
+-rwx------   0 sfurlan    (504) staff       (20)     8310 2020-02-13 05:35:33.000000 henipipe-2.4.8/henipipe/scripts/SEACR_1.3.sh
+drwxr-xr-x   0 sfurlan    (504) staff       (20)        0 2023-06-10 03:38:28.996354 henipipe-2.4.8/henipipe.egg-info/
+-rwx------   0 sfurlan    (504) staff       (20)    20743 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/PKG-INFO
+-rwx------   0 sfurlan    (504) staff       (20)      546 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/SOURCES.txt
+-rwx------   0 sfurlan    (504) staff       (20)        1 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/dependency_links.txt
+-rwx------   0 sfurlan    (504) staff       (20)      170 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/entry_points.txt
+-rwx------   0 sfurlan    (504) staff       (20)        7 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/requires.txt
+-rwx------   0 sfurlan    (504) staff       (20)        9 2023-06-10 03:38:28.000000 henipipe-2.4.8/henipipe.egg-info/top_level.txt
+-rw-r--r--   0 sfurlan    (504) staff       (20)       38 2023-06-10 03:38:28.998739 henipipe-2.4.8/setup.cfg
+-rwx------   0 sfurlan    (504) staff       (20)     3027 2022-12-28 21:08:11.000000 henipipe-2.4.8/setup.py
```

### Comparing `henipipe-2.4.7/LICENSE` & `henipipe-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/PKG-INFO` & `henipipe-2.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henipipe
-Version: 2.4.7
+Version: 2.4.8
 Summary: A python wrapper for fast and parallel processing of sequencing data using CutnRun or CutnTag
 Home-page: https://github.com/scfurl/henipipe.git
 Author: Scott Furlan
 Author-email: scottfurlan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,21 +23,22 @@
 
 # henipipe
 ==========
 
 
 
 
-Version 2.4.0
+Version 2.4.8
 
 A python wrapper for processing of sequencing data generated using CutnRun or CutnTag (developed by the Henikoff lab FHCRC).  Now with a single-cell option ('SC') for processing CutnTag data generated using the iCell8 platform (Takara).
 
 ## New in version 2.4
 
 1. Added a --version function
+2. In version 2.4.8 - environs.json was properly configured for PBS; see below for using a project ID with PBS
 
 ## New in version 2.3
 
 1. Henipipe adds a new function, DEDUP.  DEDUP will remove presumed PCR duplicates from the bed file but leave a record of how many were detected.  The DEDUP funciton is meant to be used after ALIGN and before other downstream functions.  It will replace the bed file with a collapsed bedfile with a new column that counts the number of presumed duplicates found.  Note that read pairs will be collapsed regardless of strand and all strand data will be changed to positive.  
 2. Henipipe adds a new function, BLACKLIST.  BLACKLIST will remove bed entries that overlap with a user-specified blacklist file designated with the '-bl' flag.
 2. Changes to MACS2 function were made in this version to allow custom parameters to be passed to MACS2 peak calling using the -M2p flag.
 3. Fixed a bug in SCALE function
@@ -351,10 +352,24 @@
 henipipe SC -fq fastq -o henipipe_sc -gk FH_mm10_unmasked
 ```
 
 ### Henipipe SC options and disclaimers
 
 Henipipe SC was written to accomodate iCell8 output.  As such, it should be able to parse the fastq folder and find paired fastq files.  That being said, it has not been exhaustively debugged.  Let us know if you have an issue using by submitting an issue through github.  Henipipe SC peak files will be generated using SEACR 1.3 (1.4 coming soon), but only by specifying an FDR value (See SEACR for more information).  The FDR is set using the '--SEACR_fdr' flag with a default of 0.05.  Future versions of henipipe will allow for use of this setting for bulk data but currently henipipe SEACR functionality in bulk still requires a control input file.
 
+### Using a project code
+
+Henipipe is not engineered to accept project IDs.  However for PBS job submission systems, our environs.json file will capture the global environmental variable PROJECT to run jobs with a specific project code.
+
+For example (note this code is made up)
+
+```sh
+export PROJECT=e05c3b6h-5a82-4943-uj87-2659cea32a54
+henipipe ALIGN -t 16 -r runsheet.csv -c PBS
+
+```
+
+
+
 ## Acknowledgements
 
 Written by Scott Furlan with code inspiration from Andrew Hill's cellwrapper; Henipipe includes a python script samTobed.py which takes code from a fantastic sam reader "simplesam" - https://github.com/mdshw5/simplesam.  samTobed.py uses specific sam-sorting parameters similar to those written in Jorja Henikoff's PERL script.
```

### Comparing `henipipe-2.4.7/README.md` & `henipipe-2.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 
 # henipipe
 ==========
 
 
 
 
-Version 2.4.0
+Version 2.4.8
 
 A python wrapper for processing of sequencing data generated using CutnRun or CutnTag (developed by the Henikoff lab FHCRC).  Now with a single-cell option ('SC') for processing CutnTag data generated using the iCell8 platform (Takara).
 
 ## New in version 2.4
 
 1. Added a --version function
+2. In version 2.4.8 - environs.json was properly configured for PBS; see below for using a project ID with PBS
 
 ## New in version 2.3
 
 1. Henipipe adds a new function, DEDUP.  DEDUP will remove presumed PCR duplicates from the bed file but leave a record of how many were detected.  The DEDUP funciton is meant to be used after ALIGN and before other downstream functions.  It will replace the bed file with a collapsed bedfile with a new column that counts the number of presumed duplicates found.  Note that read pairs will be collapsed regardless of strand and all strand data will be changed to positive.  
 2. Henipipe adds a new function, BLACKLIST.  BLACKLIST will remove bed entries that overlap with a user-specified blacklist file designated with the '-bl' flag.
 2. Changes to MACS2 function were made in this version to allow custom parameters to be passed to MACS2 peak calling using the -M2p flag.
 3. Fixed a bug in SCALE function
@@ -337,10 +338,24 @@
 henipipe SC -fq fastq -o henipipe_sc -gk FH_mm10_unmasked
 ```
 
 ### Henipipe SC options and disclaimers
 
 Henipipe SC was written to accomodate iCell8 output.  As such, it should be able to parse the fastq folder and find paired fastq files.  That being said, it has not been exhaustively debugged.  Let us know if you have an issue using by submitting an issue through github.  Henipipe SC peak files will be generated using SEACR 1.3 (1.4 coming soon), but only by specifying an FDR value (See SEACR for more information).  The FDR is set using the '--SEACR_fdr' flag with a default of 0.05.  Future versions of henipipe will allow for use of this setting for bulk data but currently henipipe SEACR functionality in bulk still requires a control input file.
 
+### Using a project code
+
+Henipipe is not engineered to accept project IDs.  However for PBS job submission systems, our environs.json file will capture the global environmental variable PROJECT to run jobs with a specific project code.
+
+For example (note this code is made up)
+
+```sh
+export PROJECT=e05c3b6h-5a82-4943-uj87-2659cea32a54
+henipipe ALIGN -t 16 -r runsheet.csv -c PBS
+
+```
+
+
+
 ## Acknowledgements
 
 Written by Scott Furlan with code inspiration from Andrew Hill's cellwrapper; Henipipe includes a python script samTobed.py which takes code from a fantastic sam reader "simplesam" - https://github.com/mdshw5/simplesam.  samTobed.py uses specific sam-sorting parameters similar to those written in Jorja Henikoff's PERL script.
```

### Comparing `henipipe-2.4.7/henipipe/__main__.py` & `henipipe-2.4.8/henipipe/__main__.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/auc.py` & `henipipe-2.4.8/henipipe/auc.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/data/environs.json` & `henipipe-2.4.8/henipipe/data/environs.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9774782509157509%*

 * *Differences: {"'PBS'": "{'script_lines': {'1': {insert: [(0, '#PBS -S /bin/bash\\n#PBS -o out\\n#PBS -e err')], "*

 * *          "delete: [0]}, '2': {insert: [(0, '#PBS -n <--0-->\\n#PBS -q paidq\\n#PBS -P "*

 * *          "$PROJECT')], delete: [0]}, '3': {insert: [(0, '#PBS -l nodes=1:ppn=<--0-->')], delete: "*

 * *          "[0]}, '4': {insert: [(0, '#PBS -l mem=<--0-->gb')], delete: [0]}}, "*

 * *          "'array_script_lines': {'1': {insert: [(0, '#PBS -S /bin/bash\\n#PBS -o out\\n#PBS -e "*

 * *          "err')], delete: [0]}, '2': {inser […]*

```diff
@@ -1,31 +1,31 @@
 {
     "PBS": {
         "array_script_lines": {
             "1": [
-                "#!/bin/bash\n#PBS --output=outarr\n#PBS --error=errarr",
+                "#PBS -S /bin/bash\n#PBS -o out\n#PBS -e err",
                 ""
             ],
             "2": [
-                "#PBS --array=1-<--0-->",
+                "#PBS -J 1-<--0-->:1",
                 "ARRAY_COUNT"
             ],
             "3": [
-                "#PBS --job-name=<--0-->",
+                "#PBS -n <--0-->\n#PBS -q paidq\n#PBS -P $PROJECT",
                 "JOB_NAME"
             ],
             "4": [
-                "#PBS --ntasks=1\n#PBS --cpus-per-task=<--0-->",
+                "#PBS -l nodes=1:ppn=<--0-->",
                 "THREADS"
             ],
             "5": [
-                "#PBS --mem-per-cpu=<--0-->000",
+                "#PBS -l mem=<--0-->gb",
                 "RAM"
             ],
-            "7": [
+            "6": [
                 "\n<--0-->\n<--1-->",
                 "MODULES|COMMAND"
             ]
         },
         "popen": "qsub",
         "resources": {
             "HENIPIPE_ALIGN": {
@@ -35,15 +35,15 @@
             },
             "HENIPIPE_AUC": {
                 "modules": "module load bedtools\nmodule load R\nmodule load htslib/1.9",
                 "ram": "8",
                 "threads": "1"
             },
             "HENIPIPE_BIGWIG": {
-                "modules": "module load Kent_tools/20201201-linux.x86_64",
+                "modules": "module load ucsc_kent_utils/3.6.4",
                 "ram": "8",
                 "threads": "1"
             },
             "HENIPIPE_BLACKLIST": {
                 "modules": "module load BEDTools/2.30.0-GCC-11.2.0",
                 "ram": "8",
                 "threads": "1"
@@ -92,27 +92,27 @@
                 "modules": "module load Trimmomatic",
                 "ram": "8",
                 "threads": "1"
             }
         },
         "script_lines": {
             "1": [
-                "#!/bin/bash\n#PBS --output=out\n#PBS --error=err",
+                "#PBS -S /bin/bash\n#PBS -o out\n#PBS -e err",
                 ""
             ],
             "2": [
-                "#PBS --job-name=<--0-->",
+                "#PBS -n <--0-->\n#PBS -q paidq\n#PBS -P $PROJECT",
                 "JOB_NAME"
             ],
             "3": [
-                "#PBS --ntasks=1\n#PBS --cpus-per-task=<--0-->",
+                "#PBS -l nodes=1:ppn=<--0-->",
                 "THREADS"
             ],
             "4": [
-                "#PBS --mem-per-cpu=<--0-->000",
+                "#PBS -l mem=<--0-->gb",
                 "RAM"
             ],
             "5": [
                 "{\n<--0-->\n<--1-->} 2>&1 | tee <--2-->",
                 "MODULES|COMMAND|TEMP_LOG_FILE"
             ],
             "6": [
```

### Comparing `henipipe-2.4.7/henipipe/data/genomes.json` & `henipipe-2.4.8/henipipe/data/genomes.json`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/henipipe.py` & `henipipe-2.4.8/henipipe/henipipe.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/pyWriter.py` & `henipipe-2.4.8/henipipe/pyWriter.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/samComp.py` & `henipipe-2.4.8/henipipe/samComp.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/samTobed.py` & `henipipe-2.4.8/henipipe/samTobed.py`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/scripts/SEACR_1.1.R` & `henipipe-2.4.8/henipipe/scripts/SEACR_1.1.R`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/scripts/SEACR_1.1.sh` & `henipipe-2.4.8/henipipe/scripts/SEACR_1.1.sh`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/scripts/SEACR_1.3.R` & `henipipe-2.4.8/henipipe/scripts/SEACR_1.3.R`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe/scripts/SEACR_1.3.sh` & `henipipe-2.4.8/henipipe/scripts/SEACR_1.3.sh`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/henipipe.egg-info/PKG-INFO` & `henipipe-2.4.8/henipipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henipipe
-Version: 2.4.7
+Version: 2.4.8
 Summary: A python wrapper for fast and parallel processing of sequencing data using CutnRun or CutnTag
 Home-page: https://github.com/scfurl/henipipe.git
 Author: Scott Furlan
 Author-email: scottfurlan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,21 +23,22 @@
 
 # henipipe
 ==========
 
 
 
 
-Version 2.4.0
+Version 2.4.8
 
 A python wrapper for processing of sequencing data generated using CutnRun or CutnTag (developed by the Henikoff lab FHCRC).  Now with a single-cell option ('SC') for processing CutnTag data generated using the iCell8 platform (Takara).
 
 ## New in version 2.4
 
 1. Added a --version function
+2. In version 2.4.8 - environs.json was properly configured for PBS; see below for using a project ID with PBS
 
 ## New in version 2.3
 
 1. Henipipe adds a new function, DEDUP.  DEDUP will remove presumed PCR duplicates from the bed file but leave a record of how many were detected.  The DEDUP funciton is meant to be used after ALIGN and before other downstream functions.  It will replace the bed file with a collapsed bedfile with a new column that counts the number of presumed duplicates found.  Note that read pairs will be collapsed regardless of strand and all strand data will be changed to positive.  
 2. Henipipe adds a new function, BLACKLIST.  BLACKLIST will remove bed entries that overlap with a user-specified blacklist file designated with the '-bl' flag.
 2. Changes to MACS2 function were made in this version to allow custom parameters to be passed to MACS2 peak calling using the -M2p flag.
 3. Fixed a bug in SCALE function
@@ -351,10 +352,24 @@
 henipipe SC -fq fastq -o henipipe_sc -gk FH_mm10_unmasked
 ```
 
 ### Henipipe SC options and disclaimers
 
 Henipipe SC was written to accomodate iCell8 output.  As such, it should be able to parse the fastq folder and find paired fastq files.  That being said, it has not been exhaustively debugged.  Let us know if you have an issue using by submitting an issue through github.  Henipipe SC peak files will be generated using SEACR 1.3 (1.4 coming soon), but only by specifying an FDR value (See SEACR for more information).  The FDR is set using the '--SEACR_fdr' flag with a default of 0.05.  Future versions of henipipe will allow for use of this setting for bulk data but currently henipipe SEACR functionality in bulk still requires a control input file.
 
+### Using a project code
+
+Henipipe is not engineered to accept project IDs.  However for PBS job submission systems, our environs.json file will capture the global environmental variable PROJECT to run jobs with a specific project code.
+
+For example (note this code is made up)
+
+```sh
+export PROJECT=e05c3b6h-5a82-4943-uj87-2659cea32a54
+henipipe ALIGN -t 16 -r runsheet.csv -c PBS
+
+```
+
+
+
 ## Acknowledgements
 
 Written by Scott Furlan with code inspiration from Andrew Hill's cellwrapper; Henipipe includes a python script samTobed.py which takes code from a fantastic sam reader "simplesam" - https://github.com/mdshw5/simplesam.  samTobed.py uses specific sam-sorting parameters similar to those written in Jorja Henikoff's PERL script.
```

### Comparing `henipipe-2.4.7/henipipe.egg-info/SOURCES.txt` & `henipipe-2.4.8/henipipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `henipipe-2.4.7/setup.py` & `henipipe-2.4.8/setup.py`

 * *Files identical despite different names*


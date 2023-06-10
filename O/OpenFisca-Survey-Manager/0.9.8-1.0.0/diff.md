# Comparing `tmp/OpenFisca-Survey-Manager-0.9.8.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OpenFisca-Survey-Manager-0.9.8.tar", last modified: Tue Mar 20 10:27:23 2018, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.0.0.tar", last modified: Sat Jun 10 06:15:36 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-0.9.8.tar` & `OpenFisca-Survey-Manager-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,63 @@
-drwxr-xr-x   0 benjello  (1000) benjello  (1000)        0 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/
-drwxr-xr-x   0 benjello  (1000) benjello  (1000)        0 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/
--rw-------   0 benjello  (1000) benjello  (1000)     3289 2015-07-16 08:02:54.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     1104 2017-01-06 13:14:15.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/config.py
-drwxr-xr-x   0 benjello  (1000) benjello  (1000)        0 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/scripts/
--rw-------   0 benjello  (1000) benjello  (1000)      925 2015-07-16 08:02:54.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 benjello  (1000) benjello  (1000)     8759 2018-03-19 17:59:30.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)      966 2018-03-08 12:40:55.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/variables.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)      150 2017-01-06 13:14:15.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/__init__.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     9667 2017-12-08 11:01:08.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/surveys.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     1278 2016-10-20 17:34:08.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/read_spss.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     5052 2018-01-26 14:46:32.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     5760 2017-06-16 08:49:57.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/tables.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)    45024 2018-02-19 15:26:26.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/scenarios.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     8709 2017-12-15 15:31:54.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/utils.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     4425 2017-12-15 15:31:54.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/temporary.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     8384 2018-02-19 15:26:26.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     4430 2017-01-06 13:14:15.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/matching.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     7945 2016-10-20 17:34:08.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/calmar.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     9614 2017-12-15 15:31:54.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/calibration.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)     1114 2016-10-20 17:34:08.000000 OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)      682 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/PKG-INFO
-drwxr-xr-x   0 benjello  (1000) benjello  (1000)        0 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/
--rw-------   0 benjello  (1000) benjello  (1000)      171 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-------   0 benjello  (1000) benjello  (1000)       25 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-------   0 benjello  (1000) benjello  (1000)      682 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 benjello  (1000) benjello  (1000)       93 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-------   0 benjello  (1000) benjello  (1000)        1 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-------   0 benjello  (1000) benjello  (1000)     1068 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-------   0 benjello  (1000) benjello  (1000)        2 2015-07-16 08:02:54.000000 OpenFisca-Survey-Manager-0.9.8/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 benjello  (1000) benjello  (1000)      135 2018-03-20 10:27:23.000000 OpenFisca-Survey-Manager-0.9.8/setup.cfg
--rw-r--r--   0 benjello  (1000) benjello  (1000)     1934 2018-03-19 18:01:57.000000 OpenFisca-Survey-Manager-0.9.8/setup.py
--rw-r--r--   0 benjello  (1000) benjello  (1000)       66 2018-03-19 16:53:25.000000 OpenFisca-Survey-Manager-0.9.8/MANIFEST.in
+drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    16295 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/CHANGELOG.md
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    34499 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/LICENSE.AGPL.txt
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      192 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/MANIFEST.in
+drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    14274 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     2469 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)        1 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)       92 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)        1 2022-08-11 23:28:29.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      734 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)       25 2023-06-10 06:15:36.000000 OpenFisca-Survey-Manager-1.0.0/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    14274 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/PKG-INFO
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    13360 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/README.md
+drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     2170 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/__init__.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    17292 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/aggregates.py
+drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     3551 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      451 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1571 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    12096 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     6262 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    10517 2022-09-02 13:23:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calibration.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     9929 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calmar.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     3150 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/coicop.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      741 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/config.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      836 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/google_colab.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    12877 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/input_dataframe_generator.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     4591 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/matching.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1386 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_dbf.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      653 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_sas.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      493 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/read_spss.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    79386 2023-06-10 04:35:43.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scenarios.py
+drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.302305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)        0 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/__init__.py
+-rwxrwxr-x   0 benjello  (1001) benjello  (1001)    10047 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/build_collection.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    11312 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/statshelpers.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     5323 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/survey_collections.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    10119 2022-09-02 13:23:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/surveys.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     9552 2022-09-02 13:23:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tables.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     3302 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/temporary.py
+drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)        0 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/__init__.py
+drwxrwxr-x   0 benjello  (1001) benjello  (1001)        0 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/data_files/
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      381 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1100 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     2457 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_calmar.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1694 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     4147 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      989 2022-09-02 13:33:56.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     3556 2022-12-02 09:34:57.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_matching.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     4373 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_quantile.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1495 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_read_sas.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)    13724 2023-06-09 05:38:14.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_scenario.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      716 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1064 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_surveys.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1671 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)      386 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     8319 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/utils.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     2850 2022-04-26 22:48:28.000000 OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/variables.py
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     1084 2023-06-10 06:15:36.306305 OpenFisca-Survey-Manager-1.0.0/setup.cfg
+-rw-rw-r--   0 benjello  (1001) benjello  (1001)     3155 2023-06-10 06:13:01.000000 OpenFisca-Survey-Manager-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-# -*- coding: utf-8 -*-
-
-
 import os
-import ConfigParser
+import configparser
 
 
-class Config(ConfigParser.SafeConfigParser):
-    config_local_ini = None
+class Config(configparser.ConfigParser):
     config_ini = None
 
     def __init__(self, config_files_directory = None):
-        ConfigParser.SafeConfigParser.__init__(self)
+        configparser.ConfigParser.__init__(self)
         if config_files_directory is not None:
-            config_local_ini = os.path.join(config_files_directory, 'config_local.ini')
-            if os.path.exists(config_local_ini):
-                self.config_local_ini = config_local_ini
             config_ini = os.path.join(config_files_directory, 'config.ini')
-            if os.path.exists(config_ini):
-                self.config_ini = config_ini
-            self.read([config_ini, config_local_ini])
+            assert os.path.exists(config_ini), "{} is not a valid path".format(config_ini)
+            self.config_ini = config_ini
+            self.read([config_ini])
 
     def save(self):
-        assert self.config_local_ini or self.config_ini, "configuration file paths are not defined"
-        if self.config_local_ini and os.path.exists(self.config_local_ini):
-            config_file = open(self.config_local_ini, 'w')
-        else:
-            config_file = open(self.config_ini, 'w')
+        assert self.config_ini, "configuration file path is not defined"
+        assert os.path.exists(self.config_ini)
+        config_file = open(self.config_ini, 'w')
         self.write(config_file)
         config_file.close()
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/scripts/build_collection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,158 @@
 #! /usr/bin/env python
-# -*- coding: utf-8 -*-
 
 
-"""Build or update a collection from raw surveys data/"""
+"""Build or update a collection from raw surveys data."""
 
 
 import argparse
-import ConfigParser
+import configparser
 import datetime
 import logging
 import os
+import pdb
 import pkg_resources
 import shutil
 import sys
-from xdg import BaseDirectory
 
 
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.surveys import Survey
-
-
-config_files_directory = BaseDirectory.save_config_path('openfisca-survey-manager')
-
+from openfisca_survey_manager import default_config_files_directory
 
 app_name = os.path.splitext(os.path.basename(__file__))[0]
 log = logging.getLogger(app_name)
 
 
-def add_survey_to_collection(survey_name = None, survey_collection = None, sas_files = [], stata_files = []):
+def add_survey_to_collection(survey_name = None, survey_collection = None, sas_files = None, stata_files = None, csv_files = None):
+    if sas_files is None:
+        sas_files = []
+    if stata_files is None:
+        stata_files = []
+    if csv_files is None:
+        csv_files = []
+
     assert survey_collection is not None
     overwrite = True
     label = survey_name
 
     for test_survey in survey_collection.surveys:
         if test_survey.name == survey_name:
             survey = survey_collection.get_survey(survey_name)
     if overwrite:
         survey = Survey(
             name = survey_name,
             label = label,
+            csv_files = csv_files,
             sas_files = sas_files,
             stata_files = stata_files,
             survey_collection = survey_collection,
             )
     else:
         survey = survey_collection.get(survey_name)
         survey.label = label
         survey.informations.update({
+            "csv_files": csv_files,
             "sas_files": sas_files,
             "stata_files": stata_files,
             })
     survey_collection.surveys = [
         kept_survey for kept_survey in survey_collection.surveys if kept_survey.name != survey_name
         ]
     survey_collection.surveys.append(survey)
 
 
 def create_data_file_by_format(directory_path = None):
-    '''
-    Browse subdirectories to extract stata and sas files
-    '''
+    """Browse subdirectories to extract stata and sas files."""
     stata_files = []
     sas_files = []
+    csv_files = []
 
-    for root, subdirs, files in os.walk(directory_path):
+    for root, _subdirs, files in os.walk(directory_path):
         for file_name in files:
             file_path = os.path.join(root, file_name)
+            if os.path.basename(file_name).endswith(".csv"):
+                log.info("Found csv file {}".format(file_path))
+                csv_files.append(file_path)
             if os.path.basename(file_name).endswith(".dta"):
                 log.info("Found stata file {}".format(file_path))
                 stata_files.append(file_path)
             if os.path.basename(file_name).endswith(".sas7bdat"):
                 log.info("Found sas file {}".format(file_path))
                 sas_files.append(file_path)
-    return {'stata': stata_files, 'sas': sas_files}
+    return {'csv': csv_files, 'stata': stata_files, 'sas': sas_files}
 
 
-def build_survey_collection(collection_name = None, replace_metadata = False, replace_data = False,
-        data_directory_path_by_survey_suffix = None, source_format = 'sas'):
+def build_survey_collection(
+        config_files_directory: str,
+        collection_name = None,
+        replace_metadata = False,
+        replace_data = False,
+        data_directory_path_by_survey_suffix = None,
+        source_format = 'sas',
+        ):
 
     assert collection_name is not None
     assert data_directory_path_by_survey_suffix is not None
-    surveys_name = data_directory_path_by_survey_suffix.keys()
+    surveys_name = list(data_directory_path_by_survey_suffix.keys())
     assert surveys_name is not None, "A list of surveys to process is needed"
 
     if replace_metadata:
         survey_collection = SurveyCollection(
             name = collection_name, config_files_directory = config_files_directory)
     else:
         try:
             survey_collection = SurveyCollection.load(
                 collection = collection_name, config_files_directory = config_files_directory)
-        except ConfigParser.NoOptionError:
+        except configparser.NoOptionError:
             survey_collection = SurveyCollection(
                 name = collection_name, config_files_directory = config_files_directory)
 
-    for survey_suffix, data_directory_path in data_directory_path_by_survey_suffix.iteritems():
+    for survey_suffix, data_directory_path in data_directory_path_by_survey_suffix.items():
         assert os.path.isdir(data_directory_path), '{} is not a valid directory path'.format(data_directory_path)
 
         data_file_by_format = create_data_file_by_format(data_directory_path)
         survey_name = '{}_{}'.format(collection_name, survey_suffix)
         add_survey_to_collection(
             survey_name = survey_name,
             survey_collection = survey_collection,
+            csv_files = data_file_by_format.get('csv'),
             sas_files = data_file_by_format.get('sas'),
             stata_files = data_file_by_format.get('stata'),
             )
 
         valid_source_format = [
-            _format for _format in data_file_by_format.keys()
+            _format for _format in list(data_file_by_format.keys())
             if data_file_by_format.get((_format))
             ]
         log.info("Valid source formats are: {}".format(valid_source_format))
         source_format = valid_source_format[0]
         log.info("Using the following format: {}".format(source_format))
         collections_directory = survey_collection.config.get('collections', 'collections_directory')
-        assert os.path.isdir(collections_directory), """{} who should be the collections' directory does not exist.
-Fix the option collections_directory in the collections section of your config file.""".format(collections_directory)
+        if os.path.isdir(collections_directory) is False:
+            log.info(
+                "{} who should be the collections' directory does not exist. Creating directory.".format(
+                    collections_directory))
+            os.mkdir(collections_directory)
         collection_json_path = os.path.join(collections_directory, "{}.json".format(collection_name))
         survey_collection.dump(json_file_path = collection_json_path)
         surveys = [survey for survey in survey_collection.surveys if survey.name.endswith(str(survey_suffix))]
         survey_collection.fill_hdf(source_format = source_format, surveys = surveys, overwrite = replace_data)
     return survey_collection
 
 
-def check_template_config_files():
+def check_template_config_files(config_files_directory: str):
     raw_data_ini_path = os.path.join(config_files_directory, 'raw_data.ini')
     config_ini_path = os.path.join(config_files_directory, 'config.ini')
     raw_data_template_ini_path = os.path.join(config_files_directory, 'raw_data_template.ini')
     config_template_ini_path = os.path.join(config_files_directory, 'config_template.ini')
 
     if os.path.exists(config_files_directory):
-        config_files_do_not_exist = not(os.path.exists(raw_data_ini_path) and os.path.exists(config_ini_path))
-        templates_config_files_do_not_exist = not(
+        config_files_do_not_exist = not (os.path.exists(raw_data_ini_path) and os.path.exists(config_ini_path))
+        templates_config_files_do_not_exist = not (
             os.path.exists(raw_data_template_ini_path) and os.path.exists(config_template_ini_path))
 
         if config_files_do_not_exist:
             if templates_config_files_do_not_exist:
                 log.info("Creating configuration template files in {}".format(config_files_directory))
                 template_files = [
                     'raw_data_template.ini', 'config_template.ini'
@@ -146,52 +163,71 @@
                     'config_files_templates'
                     )
                 for template_file in template_files:
                     shutil.copy(
                         os.path.join(templates_config_files_directory, template_file),
                         os.path.join(config_files_directory, template_file),
                         )
-            print("Rename and fill the template files in {}".format(config_files_directory))
+            print("Rename and fill the template files in {}".format(config_files_directory))  # noqa analysis:ignore
             return False
     else:
         os.makedirs(config_files_directory)
-        return check_template_config_files()
+        return check_template_config_files(config_files_directory)
 
     return True
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--collection', help = "name of collection to build or update", required = True)
     parser.add_argument('-d', '--replace-data', action = 'store_true', default = False,
         help = "erase existing survey data HDF5 file (instead of failing when HDF5 file already exists)")
     parser.add_argument('-m', '--replace-metadata', action = 'store_true', default = False,
         help = "erase existing collection metadata JSON file (instead of just adding new surveys)")
+    parser.add_argument('-p', '--path', help = f'path to the config files directory (default = {default_config_files_directory})')
     parser.add_argument('-s', '--survey', help = 'name of survey to build or update (default = all)')
     parser.add_argument('-v', '--verbose', action = 'store_true', default = False, help = "increase output verbosity")
     args = parser.parse_args()
     logging.basicConfig(level = logging.DEBUG if args.verbose else logging.WARNING, stream = sys.stdout)
-    if not check_template_config_files():
+
+    if args.path:
+        config_files_directory = args.path
+    else:
+        config_files_directory = default_config_files_directory
+
+    if not check_template_config_files(config_files_directory = config_files_directory):
         return
 
-    config_parser = ConfigParser.SafeConfigParser()
+    config_parser = configparser.ConfigParser()
     config_parser.read(os.path.join(config_files_directory, 'raw_data.ini'))
-    assert config_parser.has_section(args.collection), 'Unkwnown collection'
+    assert config_parser.has_section(args.collection), '{} is an unkown collection. Please add a section to raw_data.ini configuration file'.format(
+        args.collection)
     data_directory_path_by_survey_suffix = dict(config_parser.items(args.collection))
     if args.survey is not None:
         assert args.survey in data_directory_path_by_survey_suffix, 'Unknown survey data directory for {}'.format(
             args.collection)
         data_directory_path_by_survey_suffix = {
             args.survey: data_directory_path_by_survey_suffix[args.survey],
             }
 
     start_time = datetime.datetime.now()
-    build_survey_collection(collection_name = args.collection,
-        data_directory_path_by_survey_suffix = data_directory_path_by_survey_suffix,
-        replace_metadata = args.replace_metadata, replace_data = args.replace_data, source_format = 'sas')
+
+    try:
+        build_survey_collection(
+            collection_name = args.collection,
+            data_directory_path_by_survey_suffix = data_directory_path_by_survey_suffix,
+            replace_metadata = args.replace_metadata,
+            replace_data = args.replace_data,
+            source_format = 'sas',
+            config_files_directory = config_files_directory,
+            )
+    except Exception as e:
+        log.info(e)
+        pdb.post_mortem(sys.exc_info()[2])
+        raise e
 
     log.info("The program has been executed in {}".format(datetime.datetime.now() - start_time))
 
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/surveys.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,48 @@
 #! /usr/bin/env python
-# -*- coding: utf-8 -*-
 
 
-# OpenFisca -- A versatile microsimulation software
-# By: OpenFisca Team <contact@openfisca.fr>
-#
-# Copyright (C) 2011, 2012, 2013, 2014, 2015 OpenFisca Team
-# https://github.com/openfisca
-#
-# This file is part of OpenFisca.
-#
-# OpenFisca is free software; you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# OpenFisca is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-
 import collections
 import os
 import re
 
 import logging
 import pandas
 import yaml
 
 
 from .tables import Table
 
 
-ident_re = re.compile(u"(?i)ident\d{2,4}$")
+ident_re = re.compile(u"(?i)ident\d{2,4}$")  # noqa
 
 log = logging.getLogger(__name__)
 
 
 source_format_by_extension = dict(
+    csv = 'csv',
     sas7bdat = "sas",
     dta = 'stata',
-    Rdata = 'Rdata',  # TODO: badly named
+    Rdata = 'Rdata',
     spss = 'sav'
     )
 
 
 class Survey(object):
-    """
-    An object to describe survey data
-    """
+    """An object to describe survey data"""
     hdf5_file_path = None
     informations = dict()
     label = None
     name = None
     tables = collections.OrderedDict()
     tables_index = dict()
     survey_collection = None
 
     def __init__(self, name = None, label = None, hdf5_file_path = None,
-                 survey_collection = None, **kwargs):
+            survey_collection = None, **kwargs):
         assert name is not None, "A survey should have a name"
         self.name = name
         self.tables = dict()
 
         if label is not None:
             self.label = label
 
@@ -78,15 +54,15 @@
 
         self.informations = kwargs
 
     def __repr__(self):
         header = """{} : survey data {}
 Contains the following tables : \n""".format(self.name, self.label)
         tables = yaml.safe_dump(
-            self.tables.keys(),
+            list(self.tables.keys()),
             default_flow_style = False)
         informations = yaml.safe_dump(self.informations, default_flow_style = False)
         return header + tables + informations
 
     @classmethod
     def create_from_json(cls, survey_json):
         self = cls(
@@ -106,24 +82,23 @@
         assert self.survey_collection is not None
         assert isinstance(overwrite, bool) or isinstance(overwrite, list)
         survey = self
         if survey.hdf5_file_path is None:
             config = survey.survey_collection.config
             directory_path = config.get("data", "output_directory")
             if not os.path.isdir(directory_path):
-                print("{} who should be the HDF5 data directory does not exist: we create the directory".format(
+                log.warn("{} who should be the HDF5 data directory does not exist: we create the directory".format(
                     directory_path))
                 os.makedirs(directory_path)
 
             survey.hdf5_file_path = os.path.join(directory_path, survey.name + '.h5')
         if source_format is None:
-            source_formats = ['stata', 'sas', 'spss', 'Rdata']
+            source_formats = ['csv', 'stata', 'sas', 'spss', 'Rdata']
         else:
             source_formats = [source_format]
-
         for source_format in source_formats:
             files = "{}_files".format(source_format)
             for data_file in survey.informations.get(files, []):
                 path_name, extension = os.path.splitext(data_file)
                 name = os.path.basename(path_name)
                 if tables is None or name in tables:
                     table = Table(
@@ -144,131 +119,150 @@
 
         assert variable is not None
 
         if tables is None:
             tables = self.tables
         tables_index = self.tables_index
         for table in tables:
-            if table not in tables_index.keys():
+            if table not in tables_index:
                 tables_index[table] = self.get_columns(table)
             if variable in tables_index[table]:
                 container_tables.append(table)
         return container_tables
 
     def get_columns(self, table = None, rename_ident = True):
         assert table is not None
         store = pandas.HDFStore(self.hdf5_file_path)
         if table in store:
-            log.info("Building columns index for table {}".format(table))
+            log.debug("Building columns index for table {}".format(table))
             data_frame = store[table]
             if rename_ident is True:
                 for column_name in data_frame:
                     if ident_re.match(column_name) is not None:
                         data_frame.rename(columns = {column_name: "ident"}, inplace = True)
                         log.info("{} column have been replaced by ident".format(column_name))
                         break
+            store.close()
             return list(data_frame.columns)
         else:
-            print 'table {} was not found in {}'.format(table, store.filename)
+            log.info('table {} was not found in {}'.format(table, store.filename))
+            store.close()
             return list()
 
-    def get_value(self, variable = None, table = None):
-        """
-        Get value
+    def get_value(self, variable, table, lowercase = False, ignorecase = False):
+        """Get variable value from a survey table.
 
-        Parameters
-        ----------
-        variable : string
-                  name of the variable
-        table : string, default None
-                name of the table hosting the variable
-        Returns
-        -------
-        df : DataFrame, default None
-             A DataFrame containing the variable
-        """
-        assert variable is not None, "A variable is needed"
-        if table not in self.tables:
-            log.error("Table {} is not found in survey tables".format(table))
-        df = self.get_values([variable], table)
-        return df
+        Args:
+          variable: variable to retrieve
+          table(str): name of the table
+          lowercase(bool, optional, optional): lowercase variable names, defaults to False
+          ignorecase: ignore case of table name, defaults to False
+
+        Returns:
+          pd.DataFrame: dataframe containing the variable
 
-    def get_values(self, variables = None, table = None, lowercase = True, rename_ident = True):
         """
-        Get values
+        return self.get_values([variable], table)
+
+    def get_values(self, variables = None, table = None, lowercase = False, ignorecase = False, rename_ident = True):
+        """Get variables values from a survey table.
+
+        Args:
+          variables(list, optional, optional): variables to retrieve, defaults to None (retrieve all variables)
+          table(str, optional, optional): name of the table, defaults to None
+          ignorecase: ignore case of table name, defaults to False
+          lowercase(bool, optional, optional): lowercase variable names, defaults to False
+          rename_ident(bool, optional, optional): rename ident+yr (e.g. ident08) into ident, defaults to True
+
+        Returns:
+          pd.DataFrame: dataframe containing the variables
+
+        Raises:
+          Exception:
 
-        Parameters
-        ----------
-        variables : list of strings, default None
-                    list of variables names, if None return the whole table
-        table : string, default None
-                name of the table hosting the variables
-        lowercase : boolean, deflault True
-                    put variables of the table into lowercase
-        rename_ident :  boolean, deflault True
-                        rename variables ident+yr (e.g. ident08) into ident
-        Returns
-        -------
-        df : DataFrame, default None
-             A DataFrame containing the variables
         """
         assert self.hdf5_file_path is not None
-        assert os.path.exists(self.hdf5_file_path), '{} is not a valid path'.format(
+        assert os.path.exists(self.hdf5_file_path), '{} is not a valid path. This could happen because your data were not builded yet. Please consider using a rebuild option in your code.'.format(
             self.hdf5_file_path)
         store = pandas.HDFStore(self.hdf5_file_path)
 
+        if ignorecase:
+            keys = store.keys()
+            eligible_tables = []
+            for string in keys:
+                match = re.findall(table, string, re.IGNORECASE)
+                if match:
+                    eligible_tables.append(match[0])
+            if len(eligible_tables) > 1:
+                raise ValueError(f"{table} is ambiguious since the following tables are available: {eligible_tables}")
+            elif len(eligible_tables) == 0:
+                raise ValueError(f"No eligible available table in {keys}")
+            else:
+                table = eligible_tables[0]
         try:
             df = store.select(table)
         except KeyError:
+            log.error(f'No table {table} in the file {self.hdf5_file_path}')
+            log.error(f'This could happen because your data were not builded yet. Available tables are: {store.keys()}')
             store.close()
-            log.error('No table {} in the file {}'.format(table, self.hdf5_file_path))
             raise
 
+        store.close()
         if lowercase:
             columns = dict((column_name, column_name.lower()) for column_name in df)
             df.rename(columns = columns, inplace = True)
 
         if rename_ident is True:
             for column_name in df:
-                if ident_re.match(column_name) is not None:
+                if ident_re.match(str(column_name)) is not None:
                     df.rename(columns = {column_name: "ident"}, inplace = True)
                     log.info("{} column have been replaced by ident".format(column_name))
                     break
 
         if variables is None:
             return df
         else:
             diff = set(variables) - set(df.columns)
             if diff:
                 raise Exception("The following variable(s) {} are missing".format(diff))
             variables = list(set(variables).intersection(df.columns))
             df = df[variables]
             return df
 
-    def insert_table(self, name = None, **kwargs):
-        """
-        Insert a table in the Survey object
-        """
+    def insert_table(self, label = None, name = None, **kwargs):
+        """Inserts a table in the Survey object"""
 
         data_frame = kwargs.pop('data_frame', None)
+        variables = kwargs.pop('variables', None)
+        if data_frame is None:
+            data_frame = kwargs.pop('dataframe', None)
+
+        to_hdf_kwargs = kwargs.pop('to_hdf_kwargs', dict())
         if data_frame is not None:
             assert isinstance(data_frame, pandas.DataFrame)
+            if variables is not None:
+                assert set(variables) < set(data_frame.columns)
+            else:
+                variables = list(data_frame.columns)
 
         if data_frame is not None:
-            table = Table(label = name, name = name, survey = self)
+            if label is None:
+                label = name
+            table = Table(label = label, name = name, survey = self, variables = variables)
             assert table.survey.hdf5_file_path is not None
-            table.save_data_frame(data_frame)
+            log.debug("Saving table {} in {}".format(name, table.survey.hdf5_file_path))
+            table.save_data_frame(data_frame, **to_hdf_kwargs)
 
         if name not in self.tables:
             self.tables[name] = dict()
-        for key, val in kwargs.iteritems():
+        for key, val in kwargs.items():
             self.tables[name][key] = val
 
     def to_json(self):
         self_json = collections.OrderedDict((
             ))
         self_json['hdf5_file_path'] = self.hdf5_file_path
         self_json['label'] = self.label
         self_json['name'] = self.name
         self_json['tables'] = self.tables
-        self_json['informations'] = collections.OrderedDict(sorted(self.informations.iteritems()))
+        self_json['informations'] = collections.OrderedDict(sorted(self.informations.items()))
         return self_json
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/survey_collections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,57 @@
-# -*- coding: utf-8 -*-
-
-
-from . import default_config_files_directory
-
 
 import codecs
 import collections
 import json
 import os
 
 import logging
 
-from .surveys import Survey
-from .config import Config
+
+from openfisca_survey_manager import default_config_files_directory
+from openfisca_survey_manager.surveys import Survey
+from openfisca_survey_manager.config import Config
 
 
 log = logging.getLogger(__name__)
 
 
 class SurveyCollection(object):
-    """
-    A collection of Surveys
-    """
+    """A collection of Surveys"""
     config = None
     json_file_path = None
     label = None
     name = None
     surveys = list()
 
-    def __init__(self, config_files_directory = None, label = None, name = None, json_file_path = None):
-        if config_files_directory is None:
-            config_files_directory = default_config_files_directory
+    def __init__(self, config_files_directory = default_config_files_directory, label = None, name = None, json_file_path = None):
 
-        log.info("Initializing SurveyCollection from config file found in {} ..".format(config_files_directory))
-        self.config = Config(config_files_directory = config_files_directory)
+        log.debug("Initializing SurveyCollection from config file found in {} ..".format(config_files_directory))
+        config = Config(config_files_directory = config_files_directory)
         if label is not None:
             self.label = label
         if name is not None:
             self.name = name
         if json_file_path is not None:
             self.json_file_path = json_file_path
-            self.config.set("collections", self.name, self.json_file_path)
-            self.config.save()
-        elif self.config is not None:
-            if self.config.has_option("collections", self.name):
-                self.json_file_path = self.config.get("collections", self.name)
-            elif self.config.get("collections", 'collections_directory') is not None:
+            if 'collections' not in config.sections():
+                config["collections"] = dict()
+            config.set("collections", self.name, self.json_file_path)
+            config.save()
+        elif config is not None:
+            if config.has_option("collections", self.name):
+                self.json_file_path = config.get("collections", self.name)
+            elif config.get("collections", 'collections_directory') is not None:
                 self.json_file_path = os.path.join(
-                    self.config.get("collections", 'collections_directory'),
+                    config.get("collections", 'collections_directory'),
                     name + '.json',
                     )
 
+        self.config = config
+
     def __repr__(self):
         header = """{}
 Survey collection of {}
 Contains the following surveys :
 """.format(self.name, self.label)
         surveys = ["       {} : {} \n".format(survey.name, survey.label) for survey in self.surveys]
         return header + "".join(surveys)
@@ -71,22 +68,22 @@
 
         if json_file_path is None:
             assert self.json_file_path is not None, 'A json_file_path shoud be provided'
         else:
             self.json_file_path = json_file_path
 
         config.set("collections", self.name, self.json_file_path)
+        config.save
         config.save()
-
         with codecs.open(self.json_file_path, 'w', encoding = 'utf-8') as _file:
-            json.dump(self.to_json(), _file, encoding = "utf-8", ensure_ascii = False, indent = 2)
+            json.dump(self.to_json(), _file, ensure_ascii = False, indent = 2)
 
     def fill_hdf(self, source_format = None, surveys = None, tables = None, overwrite = False):
         if source_format is not None:
-            assert source_format in ["Rdata", "sas", "spss", "stata"], \
+            assert source_format in ["csv", "Rdata", "sas", "spss", "stata"], \
                 "Data source format {} is unknown".format(source_format)
         if surveys is None:
             surveys = self.surveys
         for survey in surveys:
             survey.fill_hdf(source_format = source_format, tables = tables, overwrite = overwrite)
         self.dump()
 
@@ -96,33 +93,38 @@
             'Survey {} cannot be found for survey collection {}.\nAvailable surveys are :{}'.format(
                 survey_name, self.name, available_surveys_names)
         return [survey for survey in self.surveys if survey.name == survey_name].pop()
 
     @classmethod
     def load(cls, json_file_path = None, collection = None, config_files_directory = default_config_files_directory):
         assert os.path.exists(config_files_directory)
+        config = Config(config_files_directory = config_files_directory)
         if json_file_path is None:
-            assert collection is not None
-            config = Config(config_files_directory = config_files_directory)
-            json_file_path = config.get("collections", collection)
+            assert collection is not None, "A collection is needed"
+            try:
+                json_file_path = config.get("collections", collection)
+            except Exception as error:
+                log.debug("Looking for congi file in {}".format(config_files_directory))
+                log.error(error)
+                raise
 
         with open(json_file_path, 'r') as _file:
             self_json = json.load(_file)
             name = self_json.get('name')
 
         self = cls(name = name)
         self.config = config
         with open(json_file_path, 'r') as _file:
             self_json = json.load(_file)
             self.json_file_path = json_file_path
             self.label = self_json.get('label')
             self.name = self_json.get('name')
 
         surveys = self_json.get('surveys')
-        for survey_name, survey_json in surveys.iteritems():
+        for survey_name, survey_json in surveys.items():
             survey = Survey(name = survey_name)
             self.surveys.append(survey.create_from_json(survey_json))
         return self
 
     def to_json(self):
         self_json = collections.OrderedDict((
             ))
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/statshelpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-# -*- coding: utf-8 -*-
 
 
-from __future__ import division
-
 from numpy import argsort, asarray, cumsum, linspace, logical_and as and_, ones, repeat, zeros
-from pandas import DataFrame
-
-
+import pandas as pd
 import weighted
+import weightedcalcs as wc
+import numpy as np
 
 
-def gini(values, weights = None, bin_size = None):
-    '''
-    Gini coefficient (normalized to 1)
-    Using fastgini formula :
-
-
-                      i=N      j=i
-                      SUM W_i*(SUM W_j*X_j - W_i*X_i/2)
-                      i=1      j=1
-          G = 1 - 2* ----------------------------------
-                           i=N             i=N
-                           SUM W_i*X_i  *  SUM W_i
-                           i=1             i=1
-
-
-        where observations are sorted in ascending order of X.
-
-    From http://fmwww.bc.edu/RePec/bocode/f/fastgini.html
-    '''
+def gini(values, weights = None):
+    """Computes Gini coefficient (normalized to 1).
+    # Using fastgini formula :
+    #             i=N      j=i
+    #             SUM W_i*(SUM W_j*X_j - W_i*X_i/2)
+    #             i=1      j=1
+    # G = 1 - 2* ----------------------------------
+    #                 i=N             i=N
+    #                 SUM W_i*X_i  *  SUM W_i
+    #                 i=1             i=1
+    # where observations are sorted in ascending order of X.
+    # From http://fmwww.bc.edu/RePec/bocode/f/fastgini.html
+
+    Args:
+      values: Vector of values
+      weights: Weights vector (Default value = None)
+
+    Returns:
+        float: Gini
+    """
     if weights is None:
         weights = ones(len(values))
 
-    df = DataFrame({'x': values, 'w': weights})
+    df = pd.DataFrame({'x': values, 'w': weights})
     df = df.sort_values(by='x')
     x = df['x']
     w = df['w']
     wx = w * x
 
     cdf = cumsum(wx) - 0.5 * wx
     numerator = (w * cdf).sum()
     denominator = ((wx).sum()) * (w.sum())
     gini = 1 - 2 * (numerator / denominator)
 
     return gini
 
 
 def kakwani(values, ineq_axis, weights = None):
-    '''
-    Computes the Kakwani index
-    '''
+    """Computes the Kakwani index
+
+    Args:
+      values: Vector of values
+      ineq_axis: Inequality axis
+      weights: Weights vector (Default value = None)
+
+    Returns:
+        float: Kakwani index
+    """
     from scipy.integrate import simps
 
     if weights is None:
         weights = ones(len(values))
 
-#    sign = -1
-#    if tax == True:
-#        sign = -1
-#    else:
-#        sign = 1
-
     PLCx, PLCy = pseudo_lorenz(values, ineq_axis, weights)
     LCx, LCy = lorenz(ineq_axis, weights)
 
     del PLCx
 
     return simps((LCy - PLCy), LCx)
 
 
 def lorenz(values, weights = None):
-    '''
-    Computes Lorenz Curve coordinates
-    '''
+    """Computes Lorenz curve coordinates (x, y)
+
+    Args:
+      values: Vector of values
+      weights: Weights vector (Default value = None)
+
+    Returns:
+        (np.array, np.array): Lorenz curve coordinates
+    """
     if weights is None:
         weights = ones(len(values))
 
-    df = DataFrame({'v': values, 'w': weights})
+    df = pd.DataFrame({'v': values, 'w': weights})
     df = df.sort_values(by = 'v')
     x = cumsum(df['w'])
     x = x / float(x[-1:])
     y = cumsum(df['v'] * df['w'])
     y = y / float(y[-1:])
 
     return x, y
 
 
-def weighted_quantiles(data, labels, weights, return_quantiles = False):
-
-    num_categories = len(labels)
-    breaks = linspace(0, 1, num_categories + 1)
-    quantiles = [
-        weighted.quantile_1D(data, weights, mybreak) for mybreak in breaks[1:]
-        ]
-    ret = zeros(len(data))
-    for i in range(0, len(quantiles) - 1):
-        lower = quantiles[i]
-        upper = quantiles[i + 1]
-        ret[and_(data >= lower, data < upper)] = labels[i]
+def mark_weighted_percentiles(a, labels, weights, method, return_quantiles=False):
+    """
 
-    if return_quantiles:
-        return ret + 1, quantiles
-    else:
-        return ret + 1
+    Args:
+      a:
+      labels:
+      weights:
+      method:
+      return_quantiles:  (Default value = False)
 
+    Returns:
 
-def mark_weighted_percentiles(a, labels, weights, method, return_quantiles=False):
+    """
     # from http://pastebin.com/KTLip9ee
     # a is an input array of values.
     # weights is an input array of weights, so weights[i] goes with a[i]
     # labels are the names you want to give to the xtiles
     # method refers to which weighted algorithm.
     #      1 for wikipedia, 2 for the stackexchange post.
 
     # The code outputs an array the same shape as 'a', but with
     # labels[i] inserted into spot j if a[j] falls in x-tile i.
     # The number of xtiles requested is inferred from the length of 'labels'.
 
+    np.random.seed(42)
+
     # First method, "vanilla" weights from Wikipedia article.
     if method == 1:
 
         # Sort the values and apply the same sort to the weights.
         N = len(a)
         sort_indx = argsort(a)
         tmp_a = a[sort_indx].copy()
@@ -134,15 +134,15 @@
 
         # Compute the percentile values at each explicit data point in a.
         cu_weights = cumsum(tmp_weights)
         p_vals = (1.0 / cu_weights[-1]) * (cu_weights - 0.5 * tmp_weights)
 
         # Set up the output array.
         ret = repeat(0, len(a))
-        if(len(a) < num_categories):
+        if len(a) < num_categories:
             return ret
 
         # Set up the array for the values at the breakpoints.
         quantiles = []
 
         # Find the two indices that bracket the breakpoint percentiles.
         # then do interpolation on the two a_vals for those indices, using
@@ -160,16 +160,19 @@
                         i_low = ii
                         i_high = ii + 1
 
             if i_low == i_high:
                 v = tmp_a[i_low]
             else:
                 # If there are two brackets, then apply the formula as per Wikipedia.
-                v = (tmp_a[i_low] +
-                    ((brk - p_vals[i_low]) / (p_vals[i_high] - p_vals[i_low])) * (tmp_a[i_high] - tmp_a[i_low]))
+                v = (
+                    tmp_a[i_low]
+                    + (
+                        (brk - p_vals[i_low]) / (p_vals[i_high] - p_vals[i_low])) * (tmp_a[i_high] - tmp_a[i_low])
+                    )
 
             # Append the result.
             quantiles.append(v)
 
         # Now that the weighted breakpoints are set, just categorize
         # the elements of a with logical indexing.
         for i in range(0, len(quantiles) - 1):
@@ -203,15 +206,15 @@
         s_vals = asarray(s_vals)
 
         # Normalized s_vals for comapring with the breakpoint.
         norm_s_vals = (1.0 / s_vals[-1]) * s_vals
 
         # Set up the output variable.
         ret = repeat(0, N)
-        if(N < num_categories):
+        if N < num_categories:
             return ret
 
         # Set up space for the values at the breakpoints.
         quantiles = []
 
         # Find the two indices that bracket the breakpoint percentiles.
         # then do interpolation on the two a_vals for those indices, using
@@ -229,17 +232,21 @@
                         i_low = ii
                         i_high = ii + 1
 
             if i_low == i_high:
                 v = tmp_a[i_low]
             else:
                 # Interpolate as in the method 1 method, but using the s_vals instead.
-                v = (tmp_a[i_low] +
-                    (((brk * s_vals[-1]) - s_vals[i_low]) /
-                        (s_vals[i_high] - s_vals[i_low])) * (tmp_a[i_high] - tmp_a[i_low]))
+                v = (
+                    tmp_a[i_low]
+                    + (
+                        ((brk * s_vals[-1]) - s_vals[i_low])
+                        / (s_vals[i_high] - s_vals[i_low])
+                        ) * (tmp_a[i_high] - tmp_a[i_low])
+                    )
             quantiles.append(v)
 
         # Now that the weighted breakpoints are set, just categorize
         # the elements of a as usual.
         for i in range(0, len(quantiles) - 1):
             lower = quantiles[i]
             upper = quantiles[i + 1]
@@ -252,20 +259,130 @@
         if return_quantiles:
             return ret, quantiles
         else:
             return ret
 
 
 def pseudo_lorenz(values, ineq_axis, weights = None):
-    '''
-    Computes The pseudo Lorenz Curve coordinates
-    '''
+    """Computes The pseudo Lorenz Curve coordinates
+
+    Args:
+      values:
+      ineq_axis:
+      weights:  (Default value = None)
+
+    Returns:
+
+    """
     if weights is None:
         weights = ones(len(values))
-    df = DataFrame({'v': values, 'a': ineq_axis, 'w': weights})
+    df = pd.DataFrame({'v': values, 'a': ineq_axis, 'w': weights})
     df = df.sort_values(by = 'a')
     x = cumsum(df['w'])
     x = x / float(x[-1:])
     y = cumsum(df['v'] * df['w'])
     y = y / float(y[-1:])
 
     return x, y
+
+
+def bottom_share(values, rank_from_bottom, weights = None):
+    """
+
+    Args:
+      values(np.array): Vector of values
+      rank_from_bottom(float): Rank from bottom (bottom is 0 and top is 1)
+      weights(np.array): Weights vector (Default value = None)
+
+    Returns:
+
+    """
+    if weights is None:
+        weights = ones(len(values))
+
+    calc = wc.Calculator("weights")
+    data_frame = pd.DataFrame({
+        'weights': weights,
+        'data': values,
+        })
+    quantile = calc.quantile(data_frame, 'data', rank_from_bottom)
+
+    return (
+        (data_frame["data"] < quantile)
+        * data_frame["data"]
+        * data_frame["weights"]
+        ).sum() / (
+            data_frame["data"]
+            * data_frame["weights"]
+            ).sum()
+
+
+def top_share(values, rank_from_top, weights = None):
+    """
+
+    Args:
+      values(np.array): Vector of values
+      rank_from_top(float): Rank from top (bottom is 1 and top is 0)
+      weights(np.array): Weights vector (Default value = None)
+
+    Returns:
+
+    """
+    if weights is None:
+        weights = ones(len(values))
+
+    calc = wc.Calculator("weights")
+    data_frame = pd.DataFrame({
+        'weights': weights,
+        'data': values,
+        })
+    quantile = calc.quantile(data_frame, 'data', 1 - rank_from_top)
+    return (
+        (data_frame["data"] >= quantile)
+        * data_frame["data"]
+        * data_frame["weights"]
+        ).sum() / (
+            data_frame["data"]
+            * data_frame["weights"]
+            ).sum()
+
+
+def weighted_quantiles(data, labels, weights, return_quantiles = False):
+    num_categories = len(labels)
+    breaks = linspace(0, 1, num_categories + 1)
+    quantiles = [
+        weighted.quantile_1D(data, weights, mybreak) for mybreak in breaks[1:]
+        ]
+    ret = zeros(len(data))
+    for i in range(0, len(quantiles) - 1):
+        lower = quantiles[i]
+        upper = quantiles[i + 1]
+        ret[and_(data >= lower, data < upper)] = labels[i]
+
+    if return_quantiles:
+        return ret + 1, quantiles
+    else:
+        return ret + 1
+
+
+def weightedcalcs_quantiles(data, labels, weights, return_quantiles = False):
+    calc = wc.Calculator("weights")
+    num_categories = len(labels)
+    breaks = linspace(0, 1, num_categories + 1)
+    data_frame = pd.DataFrame({
+        'weights': weights,
+        'data': data,
+        })
+    quantiles = [
+        calc.quantile(data_frame, 'data', mybreak) for mybreak in breaks[1:]
+        ]
+
+    ret = zeros(len(data))
+    for i in range(0, len(quantiles) - 1):
+        lower = quantiles[i]
+        upper = quantiles[i + 1]
+        ret[and_(data > lower, data <= upper)] = labels[i]
+
+    if return_quantiles:
+        return ret + 1, quantiles
+    else:
+        return ret + 1
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/matching.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 
 
 import logging
 import os
 import pkg_resources
 
 import pandas as pd
@@ -25,16 +24,15 @@
 
     temporary_directory_path = os.path.join(config_files_directory, 'tmp')
     assert os.path.exists(temporary_directory_path)
     receiver_path = os.path.join(temporary_directory_path, 'receiver.feather')
     donor_path = os.path.join(temporary_directory_path, 'donor.feather')
     feather.write_dataframe(receiver, receiver_path)
     feather.write_dataframe(donor, donor_path)
-
-    if isinstance(matching_variables, basestring):
+    if isinstance(matching_variables, str):
         match_vars = '"{}"'.format(matching_variables)
     elif len(matching_variables) == 1:
         match_vars = '"{}"'.format(matching_variables[0])
     else:
         match_vars = '"{}"'.format('todo')
 
     r_script = """
@@ -71,15 +69,15 @@
 summary(fused.nnd.m)
 """.format(
         receiver_path = receiver_path,
         donor_path = donor_path,
         match_vars = match_vars,
         z_variables = z_variables,
         )
-    print(r_script)
+    print(r_script)  # noqa analysis:ignore
 
 
 def nnd_hotdeck_using_rpy2(receiver = None, donor = None, matching_variables = None,
         z_variables = None, donor_classes = None):
     from rpy2.robjects.packages import importr
     from rpy2.robjects import pandas2ri
 
@@ -105,21 +103,21 @@
             out_NND = StatMatch.NND_hotdeck(
                 data_rec = receiver,
                 data_don = donor,
                 match_vars = pd.Series(matching_variables),
                 # don_class = pd.Series(donor_classes)
                 )
     except Exception as e:
-        print(1)
-        print(receiver)
-        print(2)
-        print(donor)
-        print(3)
-        print(pd.Series(matching_variables))
-        print e
+        print(1)  # noqa analysis:ignore
+        print(receiver)  # noqa analysis:ignore
+        print(2)  # noqa analysis:ignore
+        print(donor)  # noqa analysis:ignore
+        print(3)  # noqa analysis:ignore
+        print(pd.Series(matching_variables))  # noqa analysis:ignore
+        print(e)  # noqa analysis:ignore
 
     # create synthetic data.set, without the
     # duplication of the matching variables
 
     fused_0 = pandas2ri.ri2py(
         StatMatch.create_fused(
             data_rec = receiver,
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calmar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,140 +1,212 @@
-# -*- coding: utf-8 -*-
-
-
-from __future__ import division
+"""CALMAR: Calibrates weights to satisfy margins constraints."""
 
 import logging
 import operator
 
 from numpy import exp, ones, zeros, unique, array, dot, float64
 
 
 log = logging.getLogger(__name__)
 
 
 def linear(u):
+    """
+
+    Args:
+      u:
+
+    Returns:
+
+    """
     return 1 + u
 
 
 def linear_prime(u):
+    """
+
+    Args:
+      u:
+
+    Returns:
+
+    """
     return ones(u.shape, dtype = float)
 
 
 def raking_ratio(u):
+    """
+
+    Args:
+      u:
+
+    Returns:
+
+    """
     return exp(u)
 
 
 def raking_ratio_prime(u):
+    """
+
+    Args:
+      u:
+
+    Returns:
+
+    """
     return exp(u)
 
 
 def logit(u, low, up):
+    """
+
+    Args:
+      u:
+      low:
+      up:
+
+    Returns:
+
+    """
     a = (up - low) / ((1 - low) * (up - 1))
     return (low * (up - 1) + up * (1 - low) * exp(a * u)) / (up - 1 + (1 - low) * exp(a * u))
 
 
 def logit_prime(u, low, up):
+    """
+
+    Args:
+      u:
+      low:
+      up:
+
+    Returns:
+
+    """
     a = (up - low) / ((1 - low) * (up - 1))
-    return ((a * up * (1 - low) * exp(a * u)) * (up - 1 + (1 - low) * exp(a * u)) -
-        (low * (up - 1) + up * (1 - low) * exp(a * u)) * (1 - low) * a * exp(a * u)) \
-        / (up - 1 + (1 - low) * exp(a * u)) ** 2
+    return (
+        (a * up * (1 - low) * exp(a * u)) * (up - 1 + (1 - low) * exp(a * u))
+        - (low * (up - 1) + up * (1 - low) * exp(a * u)) * (1 - low) * a * exp(a * u)
+        ) / (up - 1 + (1 - low) * exp(a * u)) ** 2
 
 
 def build_dummies_dict(data):
-    '''
-    return a dict with unique values as keys and vectors as values
-    '''
+    """
+
+    Args:
+      data:
+
+    Returns:
+
+
+    """
     unique_val_list = unique(data)
     output = {}
     for val in unique_val_list:
         output[val] = (data == val)
     return output
 
 
-def calmar(data_in, margins, parameters = {}, pondini='wprm_init'):
-    '''
-    Calibraters weights according to some margins
-      - data_in is a dict containing individual data
-      - pondini (char) is the inital weight
-     margins is a dict containing for each var:
-      - a scalar var numeric variables
-      - a dict with categories key and population
-      - eventually a key named total_population : total population. If absent initialized to actual total population
-     parameters is a dict containing the following keys
-      - method : 'linear', 'raking ratio', 'logit'
-      - lo     : lower bound on weights ratio  <1
-      - up     : upper bound on weights ration >1
-      - use_proportions : default FALSE; if TRUE use proportions if total population from margins doesn't match total
-        population
-      - param xtol  : relative precision on lagrangian multipliers. By default xtol = 1.49012e-08 (default fsolve xtol)
-      - param maxfev :  maximum number of function evaluation TODO
-    '''
-
+def calmar(data_in, margins, initial_weight = 'wprm_init', method = 'linear', lo = None, up = None, use_proportions = False,
+        xtol = 1.49012e-08, maxfev = 256):
+    """Calibrates weights to satisfy margins constraints.
+
+    Args:
+        data_in (pd.DataFrame): The observations data
+        margins (dict): Margins is a dictionnary containing for each variable as key the following values
+          - a scalar for numeric variables
+          - a dictionnary with categories as key and populations as values
+          - eventually a key named `total_population` with value the total population. If absent it is initialized to the actual total population
+
+        initial_weight (str, optional): Initial weight variable. Defaults to 'wprm_init'.
+        method (str, optional): Calibration method. Should be 'linear', 'raking ratio' or 'logit'. Defaults to 'linear'.
+        lo (float, optional): Lower bound on weights ratio. Mandatory when using logit method. Should be < 1. Defaults to None.
+        up (float, optional): Upper bound on weights ratio. Mandatory when using logit method. Should be > 1. Defaults to None.
+        use_proportions (bool, optional): When True use proportions if total population from margins doesn't match total population. Defaults to False.
+        xtol (float, optional): Relative precision on lagrangian multipliers.  Defaults to 1.49012e-08 (fsolve xtol).
+        maxfev (int, optional): Maximum number of function evaluation. Defaults to 256.
+
+    Raises:
+        Exception: [description]
+        Exception: [description]
+        Exception: [description]
+
+    Returns:
+        np.array: Margins adjusting weights
+        float: Lagrangian parameter
+        dict: Updated margins
+    """
     from scipy.optimize import fsolve
 
     # remove null weights and keep original data
+    null_weight_observations = data_in[initial_weight].isnull().sum()
+    if null_weight_observations > 0:
+        log.info("{} observations have a NaN weight. Not used in the calibration.".format(null_weight_observations))
+
+    is_non_zero_weight = (data_in[initial_weight].fillna(0) > 0)
+    if is_non_zero_weight.sum() > null_weight_observations:
+        log.info("{} observations have a zero weight. Not used in the calibration.".format(
+            (data_in[initial_weight].fillna(0) <= 0).sum() - null_weight_observations))
+
+    variables = set(margins.keys()).intersection(set(data_in.columns))
+    for variable in variables:
+        null_value_observations = data_in[variable].isnull().sum()
+        if null_value_observations > 0:
+            log.info("For variable {}, {} observations have a NaN value. Not used in the calibration.".format(
+                variable, null_value_observations))
+            is_non_zero_weight = is_non_zero_weight & data_in[variable].notnull()
+
+    if not is_non_zero_weight.all():
+        log.info("We drop {} observations.".format((~is_non_zero_weight).sum()))
+
     data = dict()
-    is_weight_not_null = (data_in[pondini] > 0)
-    for a in data_in:
-        data[a] = data_in[a][is_weight_not_null]
+    for a in data_in.columns:
+        data[a] = data_in.loc[is_non_zero_weight, a].copy()
 
     if not margins:
         raise Exception("Calmar requires non empty dict of margins")
 
-    # choice of method
-    if 'method' not in parameters:
-        parameters['method'] = 'linear'
-
-    if parameters['method'] == 'linear':
+    # choose method
+    assert method in ['linear', 'raking ratio', 'logit'], "method should be 'linear', 'raking ratio' or 'logit'"
+    if method == 'linear':
         F = linear
         F_prime = linear_prime
-    elif parameters['method'] == 'raking ratio':
+    elif method == 'raking ratio':
         F = raking_ratio
         F_prime = raking_ratio_prime
-    elif parameters['method'] == 'logit':
-        if 'up' not in parameters:
-            raise Exception("When method is 'logit', 'up' parameter is needed in parameters")
-        if 'lo' not in parameters:
-            raise Exception("When method is 'logit', 'lo' parameter is needed in parameters")
-        if parameters['up'] <= 1:
-            raise Exception("When method is 'logit', 'up' should be strictly greater than 1")
-        if parameters['lo'] >= 1:
-            raise Exception("When method is 'logit', 'lo' should be strictly less than 1")
+    elif method == 'logit':
+        assert up is not None, "When method == 'logit', a value > 1 for up is mandatory"
+        assert up > 1, "up should be > 1"
+        assert lo is not None, "When method == 'logit', a value < 1 for lo is mandatory"
+        assert lo < 1, "lo should be < 1"
 
         def F(x):
-            return logit(x, parameters['lo'], parameters['up'])
+            return logit(x, lo, up)
 
         def F_prime(x):
-            return logit_prime(x, parameters['lo'], parameters['up'])
-    else:
-        raise Exception("method should be 'linear', 'raking ratio' or 'logit'")
-    # construction observations matrix
+            return logit_prime(x, lo, up)
+
+    # Construction observations matrix
     if 'total_population' in margins:
         total_population = margins.pop('total_population')
     else:
-        total_population = data[pondini].sum()
-
-    if 'use_proportions' in parameters:
-        use_proportions = parameters['use_proportions']
-    else:
-        use_proportions = False
-
-    nk = len(data[pondini])
+        total_population = data[initial_weight].fillna(0).sum()
 
+    nk = len(data[initial_weight])
     # number of Lagrange parameters (at least total population)
     nj = 1
 
     margins_new = {}
     margins_new_dict = {}
-    for var, val in margins.iteritems():
+    for var, val in margins.items():
         if isinstance(val, dict):
             dummies_dict = build_dummies_dict(data[var])
             k, pop = 0, 0
-            for cat, nb in val.iteritems():
+            for cat, nb in val.items():
                 cat_varname = var + '_' + str(cat)
                 data[cat_varname] = dummies_dict[cat]
                 margins_new[cat_varname] = nb
                 if var not in margins_new_dict:
                     margins_new_dict[var] = {}
                 margins_new_dict[var][cat] = nb
                 pop += nb
@@ -144,20 +216,21 @@
             if pop != total_population:
                 if use_proportions:
                     log.info(
                         'calmar: categorical variable {} is inconsistent with population; using proportions'.format(
                             var
                             )
                         )
-                    for cat, nb in val.iteritems():
+                    for cat, nb in val.items():
                         cat_varname = var + '_' + str(cat)
                         margins_new[cat_varname] = nb * total_population / pop
                         margins_new_dict[var][cat] = nb * total_population / pop
                 else:
-                    raise Exception('calmar: categorical variable ', var, ' is inconsistent with population')
+                    raise Exception('calmar: categorical variable {} weights sums up to {} != {}'.format(
+                        var, pop, total_population))
         else:
             margins_new[var] = val
             margins_new_dict[var] = val
             nj += 1
 
     # On conserve systematiquement la population
     if hasattr(data, 'dummy_is_in_pop'):
@@ -166,66 +239,79 @@
     data['dummy_is_in_pop'] = ones(nk)
     margins_new['dummy_is_in_pop'] = total_population
 
     # paramètres de Lagrange initialisés à zéro
     lambda0 = zeros(nj)
 
     # initial weights
-    d = data[pondini]
+    d = data[initial_weight].values
     x = zeros((nk, nj))  # nb obs x nb constraints
     xmargins = zeros(nj)
     margins_dict = {}
     j = 0
-    for var, val in margins_new.iteritems():
+    for var, val in margins_new.items():
         x[:, j] = data[var]
         xmargins[j] = val
         margins_dict[var] = val
         j += 1
 
     # Résolution des équations du premier ordre
-    def constraint(l):
-        return dot(d * F(dot(x, l)), x) - xmargins
+    def constraint(lambda_):
+        return dot(d * F(dot(x, lambda_)), x) - xmargins
 
-    def constraint_prime(l):
-        return dot(d * (x.T * F_prime(dot(x, l))), x)
-    # le jacobien celui ci-dessus est constraintprime = @(l) x*(d.*Fprime(x'*l)*x');
+    def constraint_prime(lambda_):
+        return dot(d * (x.T * F_prime(dot(x, lambda_))), x)
+        # le jacobien ci-dessus est constraintprime = @(lambda) x*(d.*Fprime(x'*lambda)*x');
 
     tries, ier = 0, 2
-    if 'xtol' in parameters:
-        xtol = parameters['xtol']
-    else:
-        xtol = 1.49012e-08
-
     err_max = 1
     conv = 1
     while (ier == 2 or ier == 5 or ier == 4) and not (tries >= 10 or (err_max < 1e-6 and conv < 1e-8)):
         lambdasol, infodict, ier, mesg = fsolve(
             constraint,
             lambda0,
             fprime = constraint_prime,
-            maxfev = 256,
+            maxfev = maxfev,
             xtol = xtol,
-            full_output = 1)
+            full_output = 1,
+            )
         lambda0 = 1 * lambdasol
         tries += 1
 
         pondfin = d * F(dot(x, lambdasol))
         rel_error = {}
-        for var, val in margins_new.iteritems():
+        for var, val in margins_new.items():  # noqa analysis:ignore
             rel_error[var] = abs((data[var] * pondfin).sum() - margins_dict[var]) / margins_dict[var]
-        sorted_err = sorted(rel_error.iteritems(), key = operator.itemgetter(1), reverse = True)
+        sorted_err = sorted(rel_error.items(), key = operator.itemgetter(1), reverse = True)
 
         conv = abs(err_max - sorted_err[0][1])
         err_max = sorted_err[0][1]
 
     if (ier == 2 or ier == 5 or ier == 4):
-        log.info("calmar: stopped after {} tries".format(tries))
+        log.debug("optimization converged after {} tries".format(tries))
+
     # rebuilding a weight vector with the same size of the initial one
-    pondfin_out = array(data_in[pondini], dtype = float64)
-    pondfin_out[is_weight_not_null] = pondfin
+    pondfin_out = array(data_in[initial_weight], dtype = float64)
+    pondfin_out[is_non_zero_weight] = pondfin
+
+    del infodict, mesg  # TODO better exploit this information
+
     return pondfin_out, lambdasol, margins_new_dict
 
 
-def check_calmar(data_in, margins, pondini='wprm_init', pondfin_out = None, lambdasol = None, margins_new_dict = None):
-    for variable, margin in margins.iteritems():
+def check_calmar(data_in, margins, initial_weight='wprm_init', pondfin_out = None, lambdasol = None, margins_new_dict = None):
+    """
+
+    Args:
+      data_in:
+      margins:
+      initial_weight:  (Default value = 'wprm_init')
+      pondfin_out:  (Default value = None)
+      lambdasol:  (Default value = None)
+      margins_new_dict:  (Default value = None)
+
+    Returns:
+
+    """
+    for variable, margin in margins.items():
         if variable != 'total_population':
-            print variable, margin, abs(margin - margins_new_dict[variable]) / abs(margin)
+            print(variable, margin, abs(margin - margins_new_dict[variable]) / abs(margin))  # noqa analysis:ignore
```

### Comparing `OpenFisca-Survey-Manager-0.9.8/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.0.0/openfisca_survey_manager/calibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-# -*- coding: utf-8 -*-
-
-
 import logging
 
 import numpy
 from numpy import logical_not
-from pandas import DataFrame
+import pandas as pd
 
-from openfisca_core.columns import AgeCol, BoolCol, EnumCol
+from openfisca_core.model_api import Enum
 from openfisca_survey_manager.calmar import calmar
 
 
 log = logging.getLogger(__name__)
 
 
 class Calibration(object):
-    """
-    An object to calibrate survey data of a SurveySimulation
-    """
+    """An object to calibrate survey data of a SurveySimulation"""
     filter_by_name = None
     initial_total_population = None
+    initial_weight_name = None
     margins_by_variable = dict()
     parameters = {
         'use_proportions': True,
-        'pondini': None,
+        'initial_weight': None,
         'method': None,  # 'linear', 'raking ratio', 'logit'
         'up': None,
         'lo': None
         }
+    period = None
     survey_scenario = None
     total_population = None
     weight_name = None
-    initial_weight_name = None
 
-    def __init__(self, survey_scenario = None):
-        self.filter_by_name = "menage_ordinaire"  # TODO should migrate this to france
-        assert survey_scenario is not None
+    def __init__(self, survey_scenario):
+        # TODO should migrate this to france
+        self.filter_by_name = "menage_ordinaire"
+        self.period = survey_scenario.period
         self._set_survey_scenario(survey_scenario)
 
     def reset(self):
-        """
-        Reset the calibration to it initial state
-        """
+        """Reset the calibration to its initial state"""
         simulation = self.survey_scenario.simulation
-        holder = simulation.get_or_new_holder(self.weight_name)
+        holder = simulation.get_holder(self.weight_name)
         holder.array = numpy.array(self.initial_weight, dtype = holder.variable.dtype)
 
     def _set_survey_scenario(self, survey_scenario):
-        """
-        Set simulation
+        """Sets the survey scenario
+
+        Args:
+          survey_scenario: the survey scenario
         """
         self.survey_scenario = survey_scenario
         # TODO deal with baseline if reform is present
         if survey_scenario.simulation is None:
             survey_scenario.simulation = survey_scenario.new_simulation()
-        period = self.simulation.period
+        period = self.period
         self.filter_by = filter_by = survey_scenario.calculate_variable(
             variable = self.filter_by_name, period = period)
         # TODO: shoud not be france specific
-        self.weight_name = weight_name = self.survey_scenario.weight_column_name_by_entity['menage']
+        self.weight_name = weight_name = self.survey_scenario.weight_variable_by_entity['menage']
         self.initial_weight_name = weight_name + "_ini"
         self.initial_weight = initial_weight = survey_scenario.calculate_variable(
             variable = weight_name, period = period)
         self.initial_total_population = sum(initial_weight * filter_by)
         self.weight = survey_scenario.calculate_variable(variable = weight_name, period = period)
 
     def set_parameters(self, parameter, value):
-        """
-        Set parameter
+        """Sets a parameter value
+
+        Args:
+          parameter: the parameter to be set
+          value: the value used to set the parameter
         """
         if parameter == 'lo':
             self.parameters['lo'] = 1 / value
         else:
             self.parameters[parameter] = value
 
 #    def set_margins_target_from_file(self, filename, year, source):
 #        """
-#        Sets margins for inputs variable from file
+#            Sets margins for inputs variable from file
 #        """
 #        # TODO read from h5 files
 #        with open(filename) as f_tot:
 #            totals = read_csv(f_tot, index_col = (0, 1))
 #        # if data for the configured year is not availbale leave margins empty
 #        year = str(year)
 #        if year not in totals:
@@ -92,141 +92,178 @@
 #            self.output_margins_data_frame = totals.rename(columns = {year: 'target'}, inplace = False)
 #
 #        for var, mod in totals.index:
 #            if var not in margins:
 #                margins[var] = {}
 #            margins[var][mod] = totals.get_value((var, mod), year)
 #
-#        for var in margins.keys():
+#        for var in margins:
 #            if var == 'total_population':
 #                if source == "input" or source == "config":
 #                    total_population = margins.pop('total_population')[0]
 #                    margins['total_population'] = total_population
 #                    self.total_population = total_population
 #            else:
 #                self.add_var2(var, margins[var], source = source)
 
-    def get_parameters(self):
+    def get_parameters(self) -> dict:
+        """Gets the parameters
+
+        Returns:
+            dict: Parameters
+        """
+
         p = {}
         p['method'] = self.parameters.get('method', 'linear')
         if self.parameters.get('invlo') is not None:
             p['lo'] = 1 / self.parameters.get('invlo')
         p['up'] = self.parameters.get('up')
         if p['method'] == 'logit':
             assert self.parameters.get('invlo') is not None and self.parameters.get('up') is not None
             p['lo'] = 1 / self.parameters.get('invlo')
             p['up'] = self.parameters.get('up')
         p['use_proportions'] = self.parameters.get('use_proportions', True)
-        p['pondini'] = self.weight_name + ""
+        p['initial_weight'] = self.weight_name + ""
         return p
 
-    def _build_calmar_data(self):
-        """
-        Builds the data dictionnary used as calmar input argument
+    def _build_calmar_data(self) -> pd.DataFrame:
+        """Builds the data dictionnary used as calmar input argument
+
+        Returns:
+            pd.DataFrame: Data used by calmar
         """
+
         # Select only filtered entities
         assert self.initial_weight_name is not None
-        data = {self.initial_weight_name: self.initial_weight * self.filter_by}
+        data = pd.DataFrame()
+        data[self.initial_weight_name] = self.initial_weight * self.filter_by
         for variable in self.margins_by_variable:
             if variable == 'total_population':
                 continue
-            assert variable in self.survey_scenario.tax_benefit_system.variables.keys()
-            period = self.survey_scenario.simulation.period
+            assert variable in self.survey_scenario.tax_benefit_system.variables
+            period = self.period
             data[variable] = self.survey_scenario.calculate_variable(variable = variable, period = period)
 
         return data
 
-    def _update_weights(self, margins, parameters = {}):
-        """
-        Runs calmar, stores new weights and returns adjusted margins
+    def _update_weights(self, margins, parameters = None):
+        """Runs calmar, stores new weights and returns adjusted margins
+
+        Args:
+          margins: margins
+          parameters:  Parameters (Default value = {})
+
+        Returns:
+            dict: Updated margins
+
         """
+        if parameters is None:
+            parameters = dict()
+
         data = self._build_calmar_data()
         assert self.initial_weight_name is not None
+        parameters['initial_weight'] = self.initial_weight_name
         val_pondfin, lambdasol, updated_margins = calmar(
-            data, margins, parameters = parameters, pondini = self.initial_weight_name
-            )
+            data, margins, **parameters)
         # Updating only afetr filtering weights
         self.weight = val_pondfin * self.filter_by + self.weight * (logical_not(self.filter_by))
         return updated_margins
 
     def calibrate(self):
+        """Applies the calibrations by updating weights and margins
+        """
         margins_by_variable = self.margins_by_variable
         parameters = self.get_parameters()
 
         if margins_by_variable is not None:
             simple_margins_by_variable = dict([
                 (variable, margins_by_type['target'])
-                for variable, margins_by_type in margins_by_variable.iteritems()])
+                for variable, margins_by_type in margins_by_variable.items()])
         else:
             simple_margins_by_variable = dict()
 
         if self.total_population:
             simple_margins_by_variable['total_population'] = self.total_population
 
         self._update_weights(simple_margins_by_variable, parameters = parameters)
         self._update_margins()
 
     def set_calibrated_weights(self):
-        """
-        Modify the weights to use the calibrated weights
-        """
+        """Modify the weights to use the calibrated weights"""
+        period = self.period
         survey_scenario = self.survey_scenario
         assert survey_scenario.simulation is not None
         for simulation in [survey_scenario.simulation, survey_scenario.baseline_simulation]:
             if simulation is None:
                 continue
-            holder = simulation.get_or_new_holder(self.weight_name)
-            holder.array = numpy.array(self.weight, dtype = holder.variable.dtype)
+            simulation.set_input(self.weight_name, period, self.weight)
             # TODO: propagation to other weights
 
-    def set_target_margins(self, target_margin_by_variable):
-        for variable, target in target_margin_by_variable.iteritems():
+    def set_target_margins(self, target_margin_by_variable: dict):
+        """[summary]
+
+        Args:
+            target_margin_by_variable (dict): Targets margins
+        """
+        for variable, target in target_margin_by_variable.items():
             self.set_target_margin(variable, target)
 
     def set_target_margin(self, variable, target):
+        """Sets variable target margin
+
+        Args:
+          variable: Targett variable
+          target: Target value
+        """
         survey_scenario = self.survey_scenario
-        period = survey_scenario.simulation.period
+        period = self.period
         assert variable in survey_scenario.tax_benefit_system.variables
-        column = survey_scenario.tax_benefit_system.variables[variable]
+        variable_instance = survey_scenario.tax_benefit_system.variables[variable]
 
         filter_by = self.filter_by
         target_by_category = None
-        if column.__class__ in [AgeCol, BoolCol, EnumCol]:
+        categorical_variable = (
+            (variable_instance.value_type in [bool, Enum])
+            or (variable_instance.unit == 'years')
+            or (variable_instance.unit == 'months')
+            )
+        if categorical_variable:
             value = survey_scenario.calculate_variable(variable = variable, period = period)
-            categories = numpy.sort(numpy.unique(value[filter_by]))
+            filtered_value = value if all(filter_by) else value[filter_by.astype(bool)]
+            categories = numpy.sort(numpy.unique(filtered_value))
             target_by_category = dict(zip(categories, target))
 
-        # assert len(atrget) = len
         if not self.margins_by_variable:
             self.margins_by_variable = dict()
         if variable not in self.margins_by_variable:
             self.margins_by_variable[variable] = dict()
         self.margins_by_variable[variable]['target'] = target_by_category or target
         self._update_margins()
 
     def _update_margins(self):
+        """Updates margins
+        """
         for variable in self.margins_by_variable:
             survey_scenario = self.survey_scenario
-            period = survey_scenario.simulation.period
+            period = self.period
             assert variable in survey_scenario.tax_benefit_system.variables
             column = survey_scenario.tax_benefit_system.variables[variable]
             weight = self.weight
             filter_by = self.filter_by
             initial_weight = self.initial_weight
 
             value = survey_scenario.calculate_variable(variable, period = period)
             margin_items = [
                 ('actual', weight[filter_by]),
                 ('initial', initial_weight[filter_by]),
                 ]
 
-            if column.__class__ in [AgeCol, BoolCol, EnumCol]:
+            if column.value_type in [bool, Enum]:
                 margin_items.append(('category', value[filter_by]))
-                # TODO: should not use DataFrame for that ...
-                margins_data_frame = DataFrame.from_items(margin_items)
+                margins_data_frame = pd.DataFrame.from_items(margin_items)
                 margins_data_frame = margins_data_frame.groupby('category', sort = True).sum()
                 margin_by_type = margins_data_frame.to_dict()
             else:
                 margin_by_type = dict(
                     actual = (weight[filter_by] * value[filter_by]).sum(),
                     initial = (initial_weight[filter_by] * value[filter_by]).sum(),
                     )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


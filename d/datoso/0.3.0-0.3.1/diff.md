# Comparing `tmp/datoso-0.3.0.tar.gz` & `tmp/datoso-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.3.0.tar", last modified: Fri Jun  2 05:14:32 2023, max compression
+gzip compressed data, was "datoso-0.3.1.tar", last modified: Sat Jun 10 20:36:18 2023, max compression
```

## Comparing `datoso-0.3.0.tar` & `datoso-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.865323 datoso-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 05:14:20.000000 datoso-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 05:14:20.000000 datoso-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-02 05:14:32.865323 datoso-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-02 05:14:20.000000 datoso-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-02 05:14:20.000000 datoso-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 05:14:32.865323 datoso-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.853323 datoso-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.857323 datoso-0.3.0/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.861323 datoso-0.3.0/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.865323 datoso-0.3.0/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42565 2023-06-02 05:14:20.000000 datoso-0.3.0/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:14:32.857323 datoso-0.3.0/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 05:14:32.000000 datoso-0.3.0/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.563238 datoso-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:36:06.000000 datoso-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 20:36:06.000000 datoso-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-10 20:36:18.563238 datoso-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-10 20:36:06.000000 datoso-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-10 20:36:06.000000 datoso-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:36:18.563238 datoso-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.555238 datoso-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.563238 datoso-0.3.1/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.563238 datoso-0.3.1/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-06-10 20:36:06.000000 datoso-0.3.1/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:36:18.559238 datoso-0.3.1/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-10 20:36:18.000000 datoso-0.3.1/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-10 20:36:18.000000 datoso-0.3.1/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:36:18.000000 datoso-0.3.1/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-10 20:36:18.000000 datoso-0.3.1/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-10 20:36:18.000000 datoso-0.3.1/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 20:36:18.000000 datoso-0.3.1/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.3.0/LICENSE` & `datoso-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/PKG-INFO` & `datoso-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Provides-Extra: nointro
 Provides-Extra: pleasuredome
 Provides-Extra: redump
 Provides-Extra: sfc_enhancedcolors
 Provides-Extra: sfc_msu1
 Provides-Extra: sfc_speedhacks
 Provides-Extra: translatedenglish
+Provides-Extra: vpinmame
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Datoso](/bearlogo.png)
 
 # Datoso
```

### Comparing `datoso-0.3.0/README.md` & `datoso-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/pyproject.toml` & `datoso-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,41 +24,44 @@
 ]
 dependencies = [
     "tinydb>=4.7.1",
     "pydantic>=1.10.7",
     "python-dateutil>=2.8.2",
     "xmltodict>=0.13.0",
     "tabulate>=0.9.0",
+    "requests>=2.28.1",
 ]
 dynamic = ["version"]
 
 
 [project.optional-dependencies]
 all = [
-    "datoso_seed_fbneo>=0.2.3",
-    "datoso_seed_md_enhanced>=0.2.3",
-    "datoso_seed_nointro>=0.2.3",
-    "datoso_seed_pleasuredome>=0.2.3",
-    "datoso_seed_redump>=0.2.3",
-    "datoso_seed_sfc_enhancedcolors>=0.2.3",
-    "datoso_seed_sfc_msu1>=0.2.3",
-    "datoso_seed_sfc_speedhacks>=0.2.3",
-    "datoso_seed_translatedenglish>=0.2.3",
+    "datoso_seed_fbneo>=0.3.0",
+    "datoso_seed_md_enhanced>=0.3.0",
+    "datoso_seed_nointro>=0.3.0",
+    "datoso_seed_pleasuredome>=0.3.0",
+    "datoso_seed_redump>=0.3.0",
+    "datoso_seed_sfc_enhancedcolors>=0.3.0",
+    "datoso_seed_sfc_msu1>=0.3.0",
+    "datoso_seed_sfc_speedhacks>=0.3.0",
+    "datoso_seed_translatedenglish>=0.3.0",
+    "datoso_seed_vpinmame>=0.3.0",
     ]
-fbneo = [ "datoso_seed_fbneo>=0.2.3" ]
-md_enhanced = [ "datoso_seed_md_enhanced>=0.2.3" ]
-nointro = [ "datoso_seed_nointro>=0.2.3" ]
-pleasuredome = [ "datoso_seed_pleasuredome>=0.2.3" ]
-redump = [ "datoso_seed_redump>=0.2.3" ]
-sfc_enhancedcolors = [ "datoso_seed_sfc_enhancedcolors>=0.2.3" ]
-sfc_msu1 = [ "datoso_seed_sfc_msu1>=0.2.3" ]
-sfc_speedhacks = [ "datoso_seed_sfc_speedhacks>=0.2.3" ]
-translatedenglish = [ "datoso_seed_translatedenglish>=0.2.3" ]
+fbneo = [ "datoso_seed_fbneo>=0.3.0" ]
+md_enhanced = [ "datoso_seed_md_enhanced>=0.3.0" ]
+nointro = [ "datoso_seed_nointro>=0.3.0" ]
+pleasuredome = [ "datoso_seed_pleasuredome>=0.3.0" ]
+redump = [ "datoso_seed_redump>=0.3.0" ]
+sfc_enhancedcolors = [ "datoso_seed_sfc_enhancedcolors>=0.3.0" ]
+sfc_msu1 = [ "datoso_seed_sfc_msu1>=0.3.0" ]
+sfc_speedhacks = [ "datoso_seed_sfc_speedhacks>=0.3.0" ]
+translatedenglish = [ "datoso_seed_translatedenglish>=0.3.0" ]
+vpinmame = [ "datoso_seed_vpinmame>=0.3.0" ]
 dev = [
-    "ruff>=0.0.263",
+    "ruff>=0.0.272",
     "line_profiler==4.0.3"
     ]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso"
 
 [project.scripts]
```

### Comparing `datoso-0.3.0/src/datoso/__main__.py` & `datoso-0.3.1/src/datoso/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 from venv import logger
 from tabulate import tabulate
 from datoso.configuration.configuration import get_seed_name
 from datoso.configuration.logger import enable_logging, set_verbosity
 from datoso.database.models.datfile import Dat
 
 from datoso import __version__, __app_name__, ROOT_FOLDER
-from datoso.helpers import Bcolors
+from datoso.helpers import Bcolors, FileUtils
 from datoso.configuration import config
 
 from datoso.helpers.plugins import installed_seeds, seed_description
 from datoso.commands.doctor import check_module, check_seed
 from datoso.commands.seed import Seed
 from datoso.repositories.dedupe import Dedupe
 from datoso.seeds.rules import Rules
 from datoso.seeds.unknown_seed import detect_seed
 
 #---------Boilerplate to check python version ----------
-if sys.version_info[0] < 3 or sys.version_info.minor < 9:
+if sys.version_info < (3, 10):
     print("This is a Python 3 script. Please run it with Python 3.9 or above")
     sys.exit(1)
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command line arguments
 
@@ -38,14 +38,17 @@
     """
     #pylint: disable=too-many-locals,too-many-statements
     parser = argparse.ArgumentParser(description='Update dats from different sources.')
     subparser = parser.add_subparsers(help='sub-command help')
 
     parser.add_argument('-v', '--version', action='store_true', help='show version')
 
+    parser_log = subparser.add_parser('log', help='Show log')
+    parser_log.set_defaults(func=command_log)
+
     parser_save = subparser.add_parser('config', help='Show configuration')
     parser_save.add_argument('-s', '--save', action='store_true', help='Save configuration to .datosorc')
     parser_save.add_argument('-d', '--directory', default='~', choices=['~', '.'], help='Directory to save .datosorc')
     parser_save.set_defaults(func=command_config)
     parser_save.add_argument('-ru', '--rules-update', action='store_true', help='Update system rules from GoogleSheets Url')
 
     group_save = parser_save.add_mutually_exclusive_group()
@@ -97,18 +100,20 @@
 
 
     # Seed commands
     for seed, _ in list(installed_seeds().items()) + [('all', 'All seeds')]:
         seed = get_seed_name(seed)
         parser_command = subparser.add_parser(seed, help=f'Update seed {seed}')
         parser_command.set_defaults(func=command_seed, seed=seed)
-        parser_command.add_argument('-f', '--fetch', action='store_true', help='Fetch seed')
-        parser_command.add_argument('-p', '--process', action='store_true', help='Process dats from seed')
         parser_command.add_argument('-d', '--details', action='store_true', help='Show details of seed')
-        parser_command.add_argument('-fd', '--filter', help='Filter dats to process')
+        parser_command.add_argument('-f', '--fetch', action='store_true', help='Fetch seed')
+        parser_command_process = parser_command.add_argument_group('process')
+        parser_command_process.add_argument('-p', '--process', action='store_true', help='Process dats from seed')
+        parser_command_process.add_argument('-a', '--actions', action="append", help='Action to execute')
+        parser_command_process.add_argument('-fd', '--filter', help='Filter dats to process')
         if seed == 'all':
             parser_command.add_argument('-e', '--exclude', action='append', help='Exclude seed or seeds (only work with all)')
             parser_command.add_argument('-o', '--only', action='append', help='Only seed or seeds (only work with all)')
 
     # Common arguments
     subparsers = [subparser, subparser_seed]
     for subpars in subparsers:
@@ -286,14 +291,19 @@
     print(f'  * Version: {module.__version__}')
     print(f'  * Author: {module.__author__}')
     print(f'  * Description: {module.__description__}')
 
 
 def command_seed(args) -> None:
     """ Commands with the seed (must be installed) """
+    def parse_actions(args):
+        if args.actions:
+            if len(args.actions) == 1:
+                args.actions = args.actions[0].split(',')
+    parse_actions(args)
     if args.seed == 'all':
         for seed, _ in installed_seeds().items():
             seed = get_seed_name(seed)
             if args.exclude and seed in args.exclude:
                 continue
             if args.only and seed not in args.only:
                 continue
@@ -319,15 +329,15 @@
             sys.exit(1)
         print(f'{Bcolors.OKBLUE}Finished fetching {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}')
     if getattr(args, 'process', False):
         message = f'{Bcolors.OKCYAN}Processing seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}'
         print('='*(len(message)-14))
         print(message)
         print('='*(len(message)-14))
-        if seed.process_dats(fltr=getattr(args, 'filter', None)):
+        if seed.process_dats(fltr=getattr(args, 'filter', None), actions_to_execute=args.actions):
             print(f'Errors processing {Bcolors.FAIL}{args.seed}{Bcolors.ENDC}')
             print('Please enable logs for more information or use -v parameter')
             command_doctor(args)
             sys.exit(1)
         print(f'{Bcolors.OKBLUE}Finished processing {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}')
 
 
@@ -428,14 +438,19 @@
         seeds = {seed: None}
     else:
         seeds = installed_seeds()
     for seed, module in seeds.items():
         print(f'Checking seed {Bcolors.OKCYAN}{seed}{Bcolors.ENDC}')
         check_module(seed, module, args.repair)
 
+def command_log(args):
+    log_path = FileUtils.parse_folder(config.get('PATHS','DatosoPath', fallback='~/.datoso'))
+    logfile = os.path.join(log_path, config['LOG'].get('LogFile', 'datoso.log'))
+    os.system(f'cat {logfile}')
+
 def main():
     """ Main function """
     from datoso.database.seeds.dat_rules import detect_first_run
     detect_first_run()
     args = parse_args()
     args.func(args)
```

### Comparing `datoso-0.3.0/src/datoso/actions/processor.py` & `datoso-0.3.1/src/datoso/actions/processor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/commands/doctor.py` & `datoso-0.3.1/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/commands/seed.py` & `datoso-0.3.1/src/datoso/commands/seed.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         for action in actions:
             for action_name, action_value in action.items():
                 if isinstance(action_value, str):
                     action[action_name] = action_value.format(**data)
         return actions
 
 
-    def process_dats(self, fltr=None):
+    def process_dats(self, fltr=None, actions_to_execute=None):
         """ Process dats."""
         def delete_line(line):
             # pylint: disable=expression-not-assigned
             [print('\b \b', end='') for x in range(0, len(line))]
             print(' ' * (len(line)), end='')
             print('\r', end='')
         def get_preffix(name) -> str:
@@ -49,14 +49,16 @@
             return seed.__preffix__ if seed else name
         tmp_path = config['PATHS'].get('DownloadPath', 'tmp')
         dat_origin = os.path.join(FileUtils.parse_folder(tmp_path), get_preffix(self.name), 'dats')
         line = ''
         for path, actions in self.actions.items():
             new_path = path.format(dat_origin=dat_origin)
             actions = self.format_actions(actions, data={'dat_destination': config['PATHS'].get('DatPath', 'DatRoot')})
+            if actions_to_execute:
+                actions = [x for x in actions if x['action'] in actions_to_execute]
             for file in os.listdir(new_path) if os.path.isdir(new_path) else []:
                 if config['PROCESS'].get('DatIgnoreRegEx'):
                     ignore_regex = re.compile(config['PROCESS']['DatIgnoreRegEx'])
                     if ignore_regex.match(file):
                         continue
 
                 if (not file.endswith(('.dat', '.xml')) \
```

### Comparing `datoso-0.3.0/src/datoso/configuration/folder_helper.py` & `datoso-0.3.1/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/configuration/logger.py` & `datoso-0.3.1/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/database/__init__.py` & `datoso-0.3.1/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/database/models/datfile.py` & `datoso-0.3.1/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/database/seeds/dat_repos.py` & `datoso-0.3.1/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/database/seeds/dat_rules.py` & `datoso-0.3.1/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/datoso.ini` & `datoso-0.3.1/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/helpers/__init__.py` & `datoso-0.3.1/src/datoso/helpers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Helpers
 """
 from contextlib import suppress
+from enum import Enum
 import re
 import os
 from pathlib import Path
 from dateutil import parser
 import shutil
 
 class Bcolors:
@@ -130,8 +131,12 @@
         os.makedirs(os.path.dirname(destination), exist_ok=True)
         try:
             shutil.move(origin, destination)
         except shutil.Error:
             FileUtils.remove(origin)
 
 class RequestUtils:
-    pass
+    pass
+
+class FileHeaders(Enum):
+    XML = '<?xml'
+    CLRMAMEPRO = 'clrma'
```

### Comparing `datoso-0.3.0/src/datoso/helpers/executor.py` & `datoso-0.3.1/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/helpers/plugins.py` & `datoso-0.3.1/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/repositories/dat.py` & `datoso-0.3.1/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/repositories/dedupe.py` & `datoso-0.3.1/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/seeds/unknown_seed.py` & `datoso-0.3.1/src/datoso/seeds/unknown_seed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """ Unknown seed, detects version and type of dat already in DatRoot. """
 import re
+import logging
+from datoso.helpers import FileHeaders
 from datoso.repositories.dat import ClrMameProDatFile, XMLDatFile
 
 def detect_xml(dat_file: str, rules):
     """ Detect the seed for a XML dat file. """
     dat = XMLDatFile(file=dat_file)
     for rule_details in rules:
         found = True
@@ -31,14 +33,26 @@
                 break
         if found:
             return rule_details['seed'], rule_details['_class']
     return None, None
 
 def detect_seed(dat_file: str, rules):
     """ Detect the seed for a dat file. """
+    # Read first 5 chars of file to determine type
+    with open(file, 'r', encoding='utf-8') as file:
+        file_header = file.read(5)
+    try:
+        if file_header == FileHeaders.XML.value:
+            return detect_xml(dat_file, rules)
+        if file_header == FileHeaders.CLRMAMEPRO.value:
+            return detect_clrmame(dat_file, rules)
+        raise Exception('Unknown file header', dat_file, file_header)
+    except Exception as e:
+        logging.exception('Error detecting seed type', e)
+
     try:
         return detect_xml(dat_file, rules)
     except Exception:
         try:
             return detect_clrmame(dat_file, rules)
         except Exception:
             return None, None
```

### Comparing `datoso-0.3.0/src/datoso/seeds.txt` & `datoso-0.3.1/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso/systems.json` & `datoso-0.3.1/src/datoso/systems.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990636704119851%*

 * *Differences: {'148': "{'override': OrderedDict([('system', 'Nintendo 64'), ('suffix', 'Mario no Photopi "*

 * *        "SmartMedia')])}"}*

```diff
@@ -1070,14 +1070,18 @@
     {
         "company": "Nintendo",
         "system": "Kiosk Video Compact Flash",
         "system_type": "Console"
     },
     {
         "company": "Nintendo",
+        "override": {
+            "suffix": "Mario no Photopi SmartMedia",
+            "system": "Nintendo 64"
+        },
         "system": "Mario no Photopi SmartMedia",
         "system_type": "Console"
     },
     {
         "company": "Nintendo",
         "system": "New Nintendo 3DS",
         "system_type": "Handheld"
```

### Comparing `datoso-0.3.0/src/datoso.egg-info/PKG-INFO` & `datoso-0.3.1/src/datoso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Provides-Extra: nointro
 Provides-Extra: pleasuredome
 Provides-Extra: redump
 Provides-Extra: sfc_enhancedcolors
 Provides-Extra: sfc_msu1
 Provides-Extra: sfc_speedhacks
 Provides-Extra: translatedenglish
+Provides-Extra: vpinmame
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Datoso](/bearlogo.png)
 
 # Datoso
```

### Comparing `datoso-0.3.0/src/datoso.egg-info/SOURCES.txt` & `datoso-0.3.1/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.3.0/src/datoso.egg-info/requires.txt` & `datoso-0.3.1/src/datoso.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 tinydb>=4.7.1
 pydantic>=1.10.7
 python-dateutil>=2.8.2
 xmltodict>=0.13.0
 tabulate>=0.9.0
+requests>=2.28.1
 
 [all]
-datoso_seed_fbneo>=0.2.3
-datoso_seed_md_enhanced>=0.2.3
-datoso_seed_nointro>=0.2.3
-datoso_seed_pleasuredome>=0.2.3
-datoso_seed_redump>=0.2.3
-datoso_seed_sfc_enhancedcolors>=0.2.3
-datoso_seed_sfc_msu1>=0.2.3
-datoso_seed_sfc_speedhacks>=0.2.3
-datoso_seed_translatedenglish>=0.2.3
+datoso_seed_fbneo>=0.3.0
+datoso_seed_md_enhanced>=0.3.0
+datoso_seed_nointro>=0.3.0
+datoso_seed_pleasuredome>=0.3.0
+datoso_seed_redump>=0.3.0
+datoso_seed_sfc_enhancedcolors>=0.3.0
+datoso_seed_sfc_msu1>=0.3.0
+datoso_seed_sfc_speedhacks>=0.3.0
+datoso_seed_translatedenglish>=0.3.0
+datoso_seed_vpinmame>=0.3.0
 
 [dev]
-ruff>=0.0.263
+ruff>=0.0.272
 line_profiler==4.0.3
 
 [fbneo]
-datoso_seed_fbneo>=0.2.3
+datoso_seed_fbneo>=0.3.0
 
 [md_enhanced]
-datoso_seed_md_enhanced>=0.2.3
+datoso_seed_md_enhanced>=0.3.0
 
 [nointro]
-datoso_seed_nointro>=0.2.3
+datoso_seed_nointro>=0.3.0
 
 [pleasuredome]
-datoso_seed_pleasuredome>=0.2.3
+datoso_seed_pleasuredome>=0.3.0
 
 [redump]
-datoso_seed_redump>=0.2.3
+datoso_seed_redump>=0.3.0
 
 [sfc_enhancedcolors]
-datoso_seed_sfc_enhancedcolors>=0.2.3
+datoso_seed_sfc_enhancedcolors>=0.3.0
 
 [sfc_msu1]
-datoso_seed_sfc_msu1>=0.2.3
+datoso_seed_sfc_msu1>=0.3.0
 
 [sfc_speedhacks]
-datoso_seed_sfc_speedhacks>=0.2.3
+datoso_seed_sfc_speedhacks>=0.3.0
 
 [translatedenglish]
-datoso_seed_translatedenglish>=0.2.3
+datoso_seed_translatedenglish>=0.3.0
+
+[vpinmame]
+datoso_seed_vpinmame>=0.3.0
```


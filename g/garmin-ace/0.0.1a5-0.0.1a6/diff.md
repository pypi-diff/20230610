# Comparing `tmp/garmin_ace-0.0.1a5.tar.gz` & `tmp/garmin_ace-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+DOS/MBR boot sector; partition 1 : ID=0xee, active 0xf0, start-CHS (0x1b5,183,58), end-CHS (0xf9,254,57), startsector 531624835, 4237903599 sectors; partition 3 : ID=0xca, active 0xf0, start-CHS (0x352,3,42), end-CHS (0x3f5,179,46), startsector 265264560, 3469524191 sectors
```

## Comparing `garmin_ace-0.0.1a5.tar` & `garmin_ace-0.0.1a6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/Makefile
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/Pipfile
--rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/Pipfile.lock
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/data/checklist.ace
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/data/test.org
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/constants.py
--rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/convert.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/decoder.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/encoder.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/models.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/tests.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/src/garmin_ace/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/.gitignore
--rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/LICENSE
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/Makefile
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/Pipfile
+-rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/Pipfile.lock
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/data/checklist.ace
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/data/test.org
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/constants.py
+-rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/convert.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/decoder.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/encoder.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/models.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/tests.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/src/garmin_ace/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/.gitignore
+-rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/LICENSE
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a6/PKG-INFO
```

### Comparing `garmin_ace-0.0.1a5/Pipfile.lock` & `garmin_ace-0.0.1a6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/src/garmin_ace/convert.py` & `garmin_ace-0.0.1a6/src/garmin_ace/convert.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/src/garmin_ace/decoder.py` & `garmin_ace-0.0.1a6/src/garmin_ace/decoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/src/garmin_ace/encoder.py` & `garmin_ace-0.0.1a6/src/garmin_ace/encoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/src/garmin_ace/models.py` & `garmin_ace-0.0.1a6/src/garmin_ace/models.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/src/garmin_ace/tests.py` & `garmin_ace-0.0.1a6/src/garmin_ace/tests.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/src/garmin_ace/utils.py` & `garmin_ace-0.0.1a6/src/garmin_ace/utils.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/LICENSE` & `garmin_ace-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/README.md` & `garmin_ace-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a5/pyproject.toml` & `garmin_ace-0.0.1a6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "garmin_ace"
-version = "0.0.1a5"
+version = "0.0.1a6"
 authors = [
   { name="Xavier Antoviaque", email="xavier@antoviaque.org" },
 ]
 description = "Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
-include = ["garmin_ace/**/*"]
+dependencies = [
+    "orgparse",
+]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/antoviaque/garmin-ace"
 "Bug Tracker" = "https://gitlab.com/antoviaque/garmin-ace/-/issues"
 
 [project.scripts]
 ace-convert = "garmin_ace.convert:main"
```

### Comparing `garmin_ace-0.0.1a5/PKG-INFO` & `garmin_ace-0.0.1a6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: garmin_ace
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python
 Project-URL: Homepage, https://gitlab.com/antoviaque/garmin-ace
 Project-URL: Bug Tracker, https://gitlab.com/antoviaque/garmin-ace/-/issues
 Author-email: Xavier Antoviaque <xavier@antoviaque.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: orgparse
 Description-Content-Type: text/markdown
 
 Garmin Aviation Checklist Editor (ACE) - Python Module
 ======================================================
 
 Parse and write ACE files from Python.
```


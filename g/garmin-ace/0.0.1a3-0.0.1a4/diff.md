# Comparing `tmp/garmin_ace-0.0.1a3.tar.gz` & `tmp/garmin_ace-0.0.1a4.tar.gz`

## Comparing `garmin_ace-0.0.1a3.tar` & `garmin_ace-0.0.1a4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/constants.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/convert.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/decoder.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/encoder.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/models.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/tests.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/utils.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/data/checklist.ace
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/data/test.org
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/.gitignore
--rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/LICENSE
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/README.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/Makefile
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/Pipfile
+-rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/Pipfile.lock
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/data/checklist.ace
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/data/test.org
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/constants.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/convert.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/decoder.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/encoder.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/models.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/tests.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/src/garmin_ace/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/README.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a4/PKG-INFO
```

### Comparing `garmin_ace-0.0.1a3/convert.py` & `garmin_ace-0.0.1a4/src/garmin_ace/convert.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/decoder.py` & `garmin_ace-0.0.1a4/src/garmin_ace/decoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/encoder.py` & `garmin_ace-0.0.1a4/src/garmin_ace/encoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/models.py` & `garmin_ace-0.0.1a4/src/garmin_ace/models.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/tests.py` & `garmin_ace-0.0.1a4/src/garmin_ace/tests.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/utils.py` & `garmin_ace-0.0.1a4/src/garmin_ace/utils.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/LICENSE` & `garmin_ace-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/README.md` & `garmin_ace-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a3/pyproject.toml` & `garmin_ace-0.0.1a4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "garmin_ace"
-version = "0.0.1a3"
+version = "0.0.1a4"
 authors = [
   { name="Xavier Antoviaque", email="xavier@antoviaque.org" },
 ]
 description = "Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -21,13 +21,7 @@
 [project.urls]
 "Homepage" = "https://gitlab.com/antoviaque/garmin-ace"
 "Bug Tracker" = "https://gitlab.com/antoviaque/garmin-ace/-/issues"
 
 [project.scripts]
 ace-convert = "garmin_ace.convert:main"
 
-[tool.hatch.build]
-include = [
-  "*.py",
-  "data/",
-  "LICENSE",
-]
```

### Comparing `garmin_ace-0.0.1a3/PKG-INFO` & `garmin_ace-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin_ace
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python
 Project-URL: Homepage, https://gitlab.com/antoviaque/garmin-ace
 Project-URL: Bug Tracker, https://gitlab.com/antoviaque/garmin-ace/-/issues
 Author-email: Xavier Antoviaque <xavier@antoviaque.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```


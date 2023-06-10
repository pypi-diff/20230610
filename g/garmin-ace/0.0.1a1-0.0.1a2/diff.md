# Comparing `tmp/garmin_ace-0.0.1a1.tar.gz` & `tmp/garmin_ace-0.0.1a2.tar.gz`

## Comparing `garmin_ace-0.0.1a1.tar` & `garmin_ace-0.0.1a2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/Makefile
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/Pipfile
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/Pipfile.lock
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/constants.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/decoder.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/encoder.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/models.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/tests.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/utils.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/data/checklist.ace
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/.gitignore
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/Makefile
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/Pipfile
+-rw-r--r--   0        0        0    30622 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/Pipfile.lock
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/constants.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/convert.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/decoder.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/encoder.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/models.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/tests.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/utils.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/data/checklist.ace
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/data/test.org
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0    34493 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/README.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 garmin_ace-0.0.1a2/PKG-INFO
```

### Comparing `garmin_ace-0.0.1a1/decoder.py` & `garmin_ace-0.0.1a2/decoder.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a1/encoder.py` & `garmin_ace-0.0.1a2/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         elif item.type == 'plaintext':
             self.encode_string("p", data)
             self.encode_indent(item.indent, data)
             self.encode_string(item.text, data, newline=True)
         elif item.type == 'challenge_response':
             self.encode_string("r", data)
             self.encode_indent(item.indent, data)
-            self.encode_string(item.challenge, data)
+            self.encode_string(item.text, data)
             self.encode_string(constants.CHALLENGE_RESPONSE_SEPARATOR, data)
             self.encode_string(item.response, data, newline=True)
         elif item.type == 'blank':
             self.encode_string("", data, newline=True)
         else:
             raise ValueError(f"Unexpected item type: {type(item)}")
```

### Comparing `garmin_ace-0.0.1a1/tests.py` & `garmin_ace-0.0.1a2/tests.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a1/utils.py` & `garmin_ace-0.0.1a2/utils.py`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a1/README.md` & `garmin_ace-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `garmin_ace-0.0.1a1/pyproject.toml` & `garmin_ace-0.0.1a2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "garmin_ace"
-version = "0.0.1a1"
+version = "0.0.1a2"
 authors = [
   { name="Xavier Antoviaque", email="xavier@antoviaque.org" },
 ]
 description = "Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,7 +16,11 @@
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/antoviaque/garmin-ace"
 "Bug Tracker" = "https://gitlab.com/antoviaque/garmin-ace/-/issues"
+
+[project.scripts]
+my-client = "garmin_ace.convert:main"
+
```

### Comparing `garmin_ace-0.0.1a1/PKG-INFO` & `garmin_ace-0.0.1a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: garmin_ace
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Garmin Aviation Checklist Editor (ACE) - Parse and write ACE files from Python
 Project-URL: Homepage, https://gitlab.com/antoviaque/garmin-ace
 Project-URL: Bug Tracker, https://gitlab.com/antoviaque/garmin-ace/-/issues
 Author-email: Xavier Antoviaque <xavier@antoviaque.org>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 Garmin Aviation Checklist Editor (ACE) - Python Module
```


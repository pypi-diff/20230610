# Comparing `tmp/signway_sdk-0.1.1.tar.gz` & `tmp/signway_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signway_sdk-0.1.1.tar", max compression
+gzip compressed data, was "signway_sdk-0.1.2.tar", max compression
```

## Comparing `signway_sdk-0.1.1.tar` & `signway_sdk-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      428 2023-06-10 17:21:05.475214 signway_sdk-0.1.1/README.md
--rw-r--r--   0        0        0      404 2023-06-10 17:21:19.827099 signway_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/__init__.py
--rw-r--r--   0        0        0     1471 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/sign_url.py
--rw-r--r--   0        0        0     3292 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/signing_functions.py
--rw-r--r--   0        0        0      839 2023-06-10 17:21:05.479214 signway_sdk-0.1.1/signway_sdk/test_sing_url.py
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 signway_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/LICENSE
+-rw-r--r--   0        0        0      428 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0      404 2023-06-10 17:26:22.987849 signway_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/__init__.py
+-rw-r--r--   0        0        0     1471 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/sign_url.py
+-rw-r--r--   0        0        0     3292 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/signing_functions.py
+-rw-r--r--   0        0        0      839 2023-06-10 17:26:10.683803 signway_sdk-0.1.2/signway_sdk/test_sing_url.py
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 signway_sdk-0.1.2/PKG-INFO
```

### Comparing `signway_sdk-0.1.1/signway_sdk/sign_url.py` & `signway_sdk-0.1.2/signway_sdk/sign_url.py`

 * *Files identical despite different names*

### Comparing `signway_sdk-0.1.1/signway_sdk/signing_functions.py` & `signway_sdk-0.1.2/signway_sdk/signing_functions.py`

 * *Files identical despite different names*

### Comparing `signway_sdk-0.1.1/signway_sdk/test_sing_url.py` & `signway_sdk-0.1.2/signway_sdk/test_sing_url.py`

 * *Files identical despite different names*

### Comparing `signway_sdk-0.1.1/PKG-INFO` & `signway_sdk-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signway-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create signed URLs for Signway
 Author: gabotechs
 Author-email: gb.mt.me@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


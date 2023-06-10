# Comparing `tmp/bhoelhelper-1.3.3.tar.gz` & `tmp/bhoelhelper-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhoelhelper-1.3.3.tar", max compression
+gzip compressed data, was "bhoelhelper-1.3.4.tar", max compression
```

## Comparing `bhoelhelper-1.3.3.tar` & `bhoelhelper-1.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1080 2020-04-25 16:59:11.898368 bhoelhelper-1.3.3/LICENSE
--rw-r--r--   0        0        0      543 2022-07-30 17:11:18.936016 bhoelhelper-1.3.3/README.rst
--rw-r--r--   0        0        0      565 2021-12-11 16:51:35.688345 bhoelhelper-1.3.3/berhoel/__init__.py
--rw-r--r--   0        0        0     3727 2022-07-30 16:29:33.037561 bhoelhelper-1.3.3/berhoel/helper/__init__.py
--rw-r--r--   0        0        0     3722 2023-03-25 14:30:09.317249 bhoelhelper-1.3.3/berhoel/helper/check_args.py
--rw-r--r--   0        0        0     9433 2022-07-30 17:09:34.056079 bhoelhelper-1.3.3/berhoel/helper/machar.py
--rw-r--r--   0        0        0     2132 2022-09-24 11:01:39.920122 bhoelhelper-1.3.3/berhoel/helper/set_version.py
--rw-r--r--   0        0        0     3853 2022-07-19 16:28:02.493426 bhoelhelper-1.3.3/berhoel/helper/tests/test_berhoel_helper.py
--rw-r--r--   0        0        0     1749 2023-03-25 14:33:33.269208 bhoelhelper-1.3.3/berhoel/helper/tests/test_check_args.py
--rw-r--r--   0        0        0     1334 2022-07-19 16:22:58.433560 bhoelhelper-1.3.3/berhoel/helper/tests/test_machar.py
--rw-r--r--   0        0        0     2227 2023-03-25 15:18:16.104414 bhoelhelper-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 bhoelhelper-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-04-25 16:59:11.898368 bhoelhelper-1.3.4/LICENSE
+-rw-r--r--   0        0        0      543 2022-07-30 17:11:18.936016 bhoelhelper-1.3.4/README.rst
+-rw-r--r--   0        0        0      574 2023-06-10 19:19:49.645062 bhoelhelper-1.3.4/berhoel/__init__.py
+-rw-r--r--   0        0        0     3727 2022-07-30 16:29:33.037561 bhoelhelper-1.3.4/berhoel/helper/__init__.py
+-rw-r--r--   0        0        0     3722 2023-03-25 14:30:09.317249 bhoelhelper-1.3.4/berhoel/helper/check_args.py
+-rw-r--r--   0        0        0     9433 2022-07-30 17:09:34.056079 bhoelhelper-1.3.4/berhoel/helper/machar.py
+-rw-r--r--   0        0        0     2132 2022-09-24 11:01:39.920122 bhoelhelper-1.3.4/berhoel/helper/set_version.py
+-rw-r--r--   0        0        0     3853 2022-07-19 16:28:02.493426 bhoelhelper-1.3.4/berhoel/helper/tests/test_berhoel_helper.py
+-rw-r--r--   0        0        0     1749 2023-03-25 14:33:33.269208 bhoelhelper-1.3.4/berhoel/helper/tests/test_check_args.py
+-rw-r--r--   0        0        0     1334 2022-07-19 16:22:58.433560 bhoelhelper-1.3.4/berhoel/helper/tests/test_machar.py
+-rw-r--r--   0        0        0     2227 2023-06-10 19:19:49.165062 bhoelhelper-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 bhoelhelper-1.3.4/PKG-INFO
```

### Comparing `bhoelhelper-1.3.3/LICENSE` & `bhoelhelper-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/README.rst` & `bhoelhelper-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/berhoel/helper/__init__.py` & `bhoelhelper-1.3.4/berhoel/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/berhoel/helper/check_args.py` & `bhoelhelper-1.3.4/berhoel/helper/check_args.py`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/berhoel/helper/machar.py` & `bhoelhelper-1.3.4/berhoel/helper/machar.py`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/berhoel/helper/set_version.py` & `bhoelhelper-1.3.4/berhoel/helper/set_version.py`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/berhoel/helper/tests/test_berhoel_helper.py` & `bhoelhelper-1.3.4/berhoel/helper/tests/test_berhoel_helper.py`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/berhoel/helper/tests/test_check_args.py` & `bhoelhelper-1.3.4/berhoel/helper/tests/test_check_args.py`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/berhoel/helper/tests/test_machar.py` & `bhoelhelper-1.3.4/berhoel/helper/tests/test_machar.py`

 * *Files identical despite different names*

### Comparing `bhoelhelper-1.3.3/pyproject.toml` & `bhoelhelper-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bhoelHelper"
-version = "1.3.3"
+version = "1.3.4"
 
 description = "Misc helper functionalities."
 
 packages = [{ include = "berhoel" }]
 exclude = ["**/.#*.py", "**/#*.py#"]
 
 authors = ["Berthold Höllmann <berhoel@gmail.com>"]
```

### Comparing `bhoelhelper-1.3.3/PKG-INFO` & `bhoelhelper-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhoelhelper
-Version: 1.3.3
+Version: 1.3.4
 Summary: Misc helper functionalities.
 Home-page: https://python.xn--hllmanns-n4a.de/bhoelHelper/
 License: MIT
 Author: Berthold Höllmann
 Author-email: berhoel@gmail.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


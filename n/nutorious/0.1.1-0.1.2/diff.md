# Comparing `tmp/nutorious-0.1.1.tar.gz` & `tmp/nutorious-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutorious-0.1.1.tar", max compression
+gzip compressed data, was "nutorious-0.1.2.tar", max compression
```

## Comparing `nutorious-0.1.1.tar` & `nutorious-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      707 2023-06-10 16:33:43.932367 nutorious-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1173 2023-06-10 10:15:22.825528 nutorious-0.1.1/src/nutorious/__main__.py
--rw-r--r--   0        0        0      754 2023-06-10 06:58:58.615523 nutorious-0.1.1/src/nutorious/cli/__init__.py
--rw-r--r--   0        0        0     1187 2023-06-10 09:57:17.178116 nutorious-0.1.1/src/nutorious/config/__init__.py
--rw-r--r--   0        0        0      376 2023-06-10 07:21:17.796093 nutorious-0.1.1/src/nutorious/config/default.yml
--rw-r--r--   0        0        0      204 2023-05-14 19:04:26.158982 nutorious-0.1.1/src/nutorious/context/__init__.py
--rw-r--r--   0        0        0     4436 2023-06-10 07:36:33.567713 nutorious-0.1.1/src/nutorious/journal/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-10 10:17:37.406707 nutorious-0.1.1/src/nutorious/model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:14:08.499582 nutorious-0.1.1/src/nutorious/report/__init__.py
--rw-r--r--   0        0        0      830 2023-06-10 10:23:35.991727 nutorious-0.1.1/src/nutorious/report/base.py
--rw-r--r--   0        0        0     2556 2023-06-10 10:16:29.071744 nutorious-0.1.1/src/nutorious/report/daily.py
--rw-r--r--   0        0        0        0 2023-05-08 19:14:08.499582 nutorious-0.1.1/src/nutorious/report/diff.py
--rw-r--r--   0        0        0     1094 2023-06-10 07:17:40.526810 nutorious-0.1.1/src/nutorious/ui/__init__.py
--rw-r--r--   0        0        0      503 2023-05-14 17:29:59.038374 nutorious-0.1.1/src/nutorious/ui/ui.py
--rw-r--r--   0        0        0      337 2023-06-09 14:46:48.334199 nutorious-0.1.1/src/nutorious/utils/collections.py
--rw-r--r--   0        0        0      197 2023-06-10 07:13:01.064789 nutorious-0.1.1/src/nutorious/utils/commons.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 nutorious-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      707 2023-06-10 17:01:08.764467 nutorious-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1173 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/__main__.py
+-rw-r--r--   0        0        0      754 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/cli/__init__.py
+-rw-r--r--   0        0        0     1187 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/config/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/config/default.yml
+-rw-r--r--   0        0        0      204 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/context/__init__.py
+-rw-r--r--   0        0        0     4436 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/journal/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/base.py
+-rw-r--r--   0        0        0     2556 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/daily.py
+-rw-r--r--   0        0        0        0 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/diff.py
+-rw-r--r--   0        0        0     1094 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/ui/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/ui/ui.py
+-rw-r--r--   0        0        0      337 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/utils/collections.py
+-rw-r--r--   0        0        0      197 2023-06-10 17:01:08.768467 nutorious-0.1.2/src/nutorious/utils/commons.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 nutorious-0.1.2/PKG-INFO
```

### Comparing `nutorious-0.1.1/pyproject.toml` & `nutorious-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutorious"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Dzmitry Paulenka <paulenka.dk@gmail.com>"]
 # readme = "README.md"
 # packages = [{include = "nutorious"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nutorious-0.1.1/src/nutorious/__main__.py` & `nutorious-0.1.2/src/nutorious/__main__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/src/nutorious/cli/__init__.py` & `nutorious-0.1.2/src/nutorious/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/src/nutorious/config/__init__.py` & `nutorious-0.1.2/src/nutorious/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/src/nutorious/journal/__init__.py` & `nutorious-0.1.2/src/nutorious/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/src/nutorious/model/__init__.py` & `nutorious-0.1.2/src/nutorious/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/src/nutorious/report/base.py` & `nutorious-0.1.2/src/nutorious/report/base.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/src/nutorious/report/daily.py` & `nutorious-0.1.2/src/nutorious/report/daily.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/src/nutorious/ui/__init__.py` & `nutorious-0.1.2/src/nutorious/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.1/PKG-INFO` & `nutorious-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutorious
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Dzmitry Paulenka
 Author-email: paulenka.dk@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


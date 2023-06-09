# Comparing `tmp/velesresearch-0.0.4.tar.gz` & `tmp/velesresearch-0.0.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velesresearch-0.0.4.tar", max compression
+gzip compressed data, was "velesresearch-0.0.4.post1.tar", max compression
```

## Comparing `velesresearch-0.0.4.tar` & `velesresearch-0.0.4.post1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-09 21:53:20.015152 velesresearch-0.0.4/LICENSE
--rw-r--r--   0        0        0     1261 2023-06-09 15:14:07.859737 velesresearch-0.0.4/README.md
--rw-r--r--   0        0        0      102 2023-06-09 22:03:56.416947 velesresearch-0.0.4/VelesResearch/__init__.py
--rw-r--r--   0        0        0     1544 2023-06-09 22:03:56.606946 velesresearch-0.0.4/VelesResearch/options.py
--rw-r--r--   0        0        0     1915 2023-06-09 22:03:56.593613 velesresearch-0.0.4/VelesResearch/question_types.py
--rw-r--r--   0        0        0     4472 2023-06-09 22:03:56.636946 velesresearch-0.0.4/VelesResearch/structure.py
--rw-r--r--   0        0        0     1660 2023-06-09 22:03:56.610279 velesresearch-0.0.4/VelesResearch/survey_tools.py
--rw-r--r--   0        0        0      399 2023-06-09 21:43:01.250069 velesresearch-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 velesresearch-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 21:53:20.015152 velesresearch-0.0.4.post1/LICENSE
+-rw-r--r--   0        0        0     1261 2023-06-09 15:14:07.859737 velesresearch-0.0.4.post1/README.md
+-rw-r--r--   0        0        0      102 2023-06-09 22:03:56.416947 velesresearch-0.0.4.post1/VelesResearch/__init__.py
+-rw-r--r--   0        0        0     1544 2023-06-09 22:03:56.606946 velesresearch-0.0.4.post1/VelesResearch/options.py
+-rw-r--r--   0        0        0     1915 2023-06-09 22:03:56.593613 velesresearch-0.0.4.post1/VelesResearch/question_types.py
+-rw-r--r--   0        0        0     4472 2023-06-09 22:03:56.636946 velesresearch-0.0.4.post1/VelesResearch/structure.py
+-rw-r--r--   0        0        0     1660 2023-06-09 22:03:56.610279 velesresearch-0.0.4.post1/VelesResearch/survey_tools.py
+-rw-r--r--   0        0        0      501 2023-06-09 22:31:59.878380 velesresearch-0.0.4.post1/pyproject.toml
+-rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 velesresearch-0.0.4.post1/PKG-INFO
```

### Comparing `velesresearch-0.0.4/LICENSE` & `velesresearch-0.0.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.4/README.md` & `velesresearch-0.0.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.4/VelesResearch/options.py` & `velesresearch-0.0.4.post1/VelesResearch/options.py`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.4/VelesResearch/question_types.py` & `velesresearch-0.0.4.post1/VelesResearch/question_types.py`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.4/VelesResearch/structure.py` & `velesresearch-0.0.4.post1/VelesResearch/structure.py`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.4/VelesResearch/survey_tools.py` & `velesresearch-0.0.4.post1/VelesResearch/survey_tools.py`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.4/PKG-INFO` & `velesresearch-0.0.4.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: velesresearch
-Version: 0.0.4
-Summary: 
+Version: 0.0.4.post1
+Summary: Veles is a free and open source python survey tool for researchers.
+License: GPL-3.0-or-later
 Author: Jakub Jędrusiak
 Author-email: kuba23031999@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>
```


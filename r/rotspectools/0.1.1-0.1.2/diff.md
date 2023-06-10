# Comparing `tmp/rotspectools-0.1.1.tar.gz` & `tmp/rotspectools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.1.tar", max compression
+gzip compressed data, was "rotspectools-0.1.2.tar", max compression
```

## Comparing `rotspectools-0.1.1.tar` & `rotspectools-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 21:43:42.410686 rotspectools-0.1.1/LICENSE
--rw-r--r--   0        0        0      974 2023-06-09 21:43:42.429020 rotspectools-0.1.1/README.md
--rw-r--r--   0        0        0      438 2023-06-09 22:33:29.942262 rotspectools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      146 2023-06-09 21:43:42.444253 rotspectools-0.1.1/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 21:43:42.446141 rotspectools-0.1.1/rotspectools/cli.py
--rw-r--r--   0        0        0       19 2023-06-09 21:43:42.446758 rotspectools-0.1.1/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 rotspectools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.2/LICENSE
+-rw-r--r--   0        0        0      974 2023-06-09 22:48:57.252972 rotspectools-0.1.2/README.rst
+-rw-r--r--   0        0        0      439 2023-06-10 00:32:53.804098 rotspectools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.2/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-06-09 22:48:57.256906 rotspectools-0.1.2/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.2/rotspectools/cli.py
+-rw-r--r--   0        0        0    19389 2023-06-09 20:41:27.276958 rotspectools-0.1.2/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 rotspectools-0.1.2/PKG-INFO
```

### Comparing `rotspectools-0.1.1/LICENSE` & `rotspectools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.1/README.md` & `rotspectools-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.1/PKG-INFO` & `rotspectools-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotspectools
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: Dairen Jean
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SciencePlots (>=2.1.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 
 =============================
 Rotational Spectroscopy Tools
 =============================
 
 
 .. image:: https://img.shields.io/pypi/v/rotspectools.svg
```


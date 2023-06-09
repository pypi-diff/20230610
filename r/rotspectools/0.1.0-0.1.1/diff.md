# Comparing `tmp/rotspectools-0.1.0.tar.gz` & `tmp/rotspectools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.0.tar", last modified: Fri Jun  9 20:43:52 2023, max compression
+gzip compressed data, was "rotspectools-0.1.1.tar", max compression
```

## Comparing `rotspectools-0.1.0.tar` & `rotspectools-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,7 @@
--rw-r--r--   0        0        0      155 2023-06-08 13:31:59.790879 rotspectools-0.1.0/AUTHORS.rst
--rw-r--r--   0        0        0     1070 2023-06-08 13:31:59.779863 rotspectools-0.1.0/LICENSE
--rw-r--r--   0        0        0      991 2023-06-08 13:31:59.794143 rotspectools-0.1.0/README.rst
--rw-r--r--   0        0        0     1112 2023-06-09 20:43:52.261289 rotspectools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-09 20:25:32.769200 rotspectools-0.1.0/rotspectools/.DS_Store
--rw-r--r--   0        0        0      138 2023-06-08 13:31:59.806223 rotspectools-0.1.0/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-08 13:31:59.807757 rotspectools-0.1.0/rotspectools/cli.py
--rw-r--r--   0        0        0    19389 2023-06-09 20:41:27.276958 rotspectools-0.1.0/rotspectools/rotspectools.py
--rw-r--r--   0        0        0       42 2023-06-08 13:31:59.798936 rotspectools-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1004 2023-06-08 13:31:59.798410 rotspectools-0.1.0/tests/test_rotspectools.py
--rw-r--r--   0        0        0     1964 1970-01-01 00:00:00.000000 rotspectools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 21:43:42.410686 rotspectools-0.1.1/LICENSE
+-rw-r--r--   0        0        0      974 2023-06-09 21:43:42.429020 rotspectools-0.1.1/README.md
+-rw-r--r--   0        0        0      438 2023-06-09 22:33:29.942262 rotspectools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-06-09 21:43:42.444253 rotspectools-0.1.1/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 21:43:42.446141 rotspectools-0.1.1/rotspectools/cli.py
+-rw-r--r--   0        0        0       19 2023-06-09 21:43:42.446758 rotspectools-0.1.1/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 rotspectools-0.1.1/PKG-INFO
```

### Comparing `rotspectools-0.1.0/LICENSE` & `rotspectools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.0/README.rst` & `rotspectools-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-=====================
-Rotational Spec Tools
-=====================
+=============================
+Rotational Spectroscopy Tools
+=============================
 
 
 .. image:: https://img.shields.io/pypi/v/rotspectools.svg
         :target: https://pypi.python.org/pypi/rotspectools
 
 .. image:: https://img.shields.io/travis/djean032/rotspectools.svg
         :target: https://travis-ci.com/djean032/rotspectools
@@ -12,15 +12,15 @@
 .. image:: https://readthedocs.org/projects/rotspectools/badge/?version=latest
         :target: https://rotspectools.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
 
-Project used to automate the data analysis and presentation of rotational spectroscopy datasets.
+Package for automating data analysis and visualization.
 
 
 * Free software: MIT license
 * Documentation: https://rotspectools.readthedocs.io.
 
 
 Features
```


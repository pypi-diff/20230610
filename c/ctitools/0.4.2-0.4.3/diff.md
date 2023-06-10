# Comparing `tmp/ctitools-0.4.2.tar.gz` & `tmp/ctitools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctitools-0.4.2.tar", max compression
+gzip compressed data, was "ctitools-0.4.3.tar", max compression
```

## Comparing `ctitools-0.4.2.tar` & `ctitools-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1524 2022-07-16 09:18:40.161474 ctitools-0.4.2/LICENSE
--rw-r--r--   0        0        0      899 2022-08-09 11:58:58.277412 ctitools-0.4.2/README.rst
--rw-r--r--   0        0        0      577 2022-07-16 20:31:33.760948 ctitools-0.4.2/berhoel/__init__.py
--rw-r--r--   0        0        0     8379 2022-12-02 19:55:13.119268 ctitools-0.4.2/berhoel/ctitools/__init__.py
--rw-r--r--   0        0        0      569 2022-07-30 19:39:33.591163 ctitools-0.4.2/berhoel/ctitools/__main__.py
--rw-r--r--   0        0        0     5926 2023-05-12 18:47:25.437032 ctitools-0.4.2/berhoel/ctitools/ct.py
--rw-r--r--   0        0        0     3498 2022-12-15 19:51:37.432703 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__init__.py
--rw-r--r--   0        0        0      571 2022-07-30 19:36:58.727250 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__main__.py
--rw-r--r--   0        0        0     1959 2022-10-20 19:16:43.373498 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_base.py
--rw-r--r--   0        0        0     2685 2022-12-15 19:17:59.996999 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_generate.py
--rw-r--r--   0        0        0     1260 2022-09-08 09:57:16.786064 ctitools-0.4.2/berhoel/ctitools/ctientry.py
--rw-r--r--   0        0        0     2772 2022-08-01 15:08:30.320285 ctitools-0.4.2/berhoel/ctitools/ix.py
--rw-r--r--   0        0        0     1502 2023-05-12 18:48:31.253040 ctitools-0.4.2/berhoel/ctitools/tests/test_ct.py
--rw-r--r--   0        0        0     1171 2022-08-01 14:00:56.594637 ctitools-0.4.2/berhoel/ctitools/tests/test_ctitools.py
--rw-r--r--   0        0        0     5561 2022-09-08 10:05:11.577264 ctitools-0.4.2/berhoel/ctitools/tests/test_processing.py
--rw-r--r--   0        0        0     3569 2023-05-12 18:56:05.717101 ctitools-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 ctitools-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1524 2022-07-16 09:18:40.161474 ctitools-0.4.3/LICENSE
+-rw-r--r--   0        0        0      899 2022-08-09 11:58:58.277412 ctitools-0.4.3/README.rst
+-rw-r--r--   0        0        0      586 2023-06-10 19:51:29.125002 ctitools-0.4.3/berhoel/__init__.py
+-rw-r--r--   0        0        0     8379 2022-12-02 19:55:13.119268 ctitools-0.4.3/berhoel/ctitools/__init__.py
+-rw-r--r--   0        0        0      569 2022-07-30 19:39:33.591163 ctitools-0.4.3/berhoel/ctitools/__main__.py
+-rw-r--r--   0        0        0     5926 2023-05-12 18:47:25.437032 ctitools-0.4.3/berhoel/ctitools/ct.py
+-rw-r--r--   0        0        0     3498 2022-12-15 19:51:37.432703 ctitools-0.4.3/berhoel/ctitools/cti2bibtex/__init__.py
+-rw-r--r--   0        0        0      571 2022-07-30 19:36:58.727250 ctitools-0.4.3/berhoel/ctitools/cti2bibtex/__main__.py
+-rw-r--r--   0        0        0     1959 2022-10-20 19:16:43.373498 ctitools-0.4.3/berhoel/ctitools/cti2bibtex/tests/test_base.py
+-rw-r--r--   0        0        0     2685 2022-12-15 19:17:59.996999 ctitools-0.4.3/berhoel/ctitools/cti2bibtex/tests/test_generate.py
+-rw-r--r--   0        0        0     1260 2022-09-08 09:57:16.786064 ctitools-0.4.3/berhoel/ctitools/ctientry.py
+-rw-r--r--   0        0        0     2772 2022-08-01 15:08:30.320285 ctitools-0.4.3/berhoel/ctitools/ix.py
+-rw-r--r--   0        0        0     1502 2023-05-12 18:48:31.253040 ctitools-0.4.3/berhoel/ctitools/tests/test_ct.py
+-rw-r--r--   0        0        0     1171 2022-08-01 14:00:56.594637 ctitools-0.4.3/berhoel/ctitools/tests/test_ctitools.py
+-rw-r--r--   0        0        0     5561 2022-09-08 10:05:11.577264 ctitools-0.4.3/berhoel/ctitools/tests/test_processing.py
+-rw-r--r--   0        0        0     3569 2023-06-10 19:51:49.988999 ctitools-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1969 1970-01-01 00:00:00.000000 ctitools-0.4.3/PKG-INFO
```

### Comparing `ctitools-0.4.2/LICENSE` & `ctitools-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/README.rst` & `ctitools-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/__init__.py` & `ctitools-0.4.3/berhoel/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """Initialization for berhoel python namespace packages.
 """
 
-__date__ = "2022/07/16 22:31:33 hoel"
+__date__ = "2023/06/10 21:51:28 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2017, 2022 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
 
-__import__("pkg_resources").declare_namespace(__name__)
+__path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 # Local Variables:
 # mode: python
 # compile-command: "cd ../ && python setup.py test"
 # time-stamp-pattern: "30/__date__ = \"%:y/%02m/%02d %02H:%02M:%02S %u\""
 # End:
```

### Comparing `ctitools-0.4.2/berhoel/ctitools/__init__.py` & `ctitools-0.4.3/berhoel/ctitools/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/__main__.py` & `ctitools-0.4.3/berhoel/ctitools/__main__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/ct.py` & `ctitools-0.4.3/berhoel/ctitools/ct.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__init__.py` & `ctitools-0.4.3/berhoel/ctitools/cti2bibtex/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__main__.py` & `ctitools-0.4.3/berhoel/ctitools/cti2bibtex/__main__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_base.py` & `ctitools-0.4.3/berhoel/ctitools/cti2bibtex/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_generate.py` & `ctitools-0.4.3/berhoel/ctitools/cti2bibtex/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/ctientry.py` & `ctitools-0.4.3/berhoel/ctitools/ctientry.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/ix.py` & `ctitools-0.4.3/berhoel/ctitools/ix.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/tests/test_ct.py` & `ctitools-0.4.3/berhoel/ctitools/tests/test_ct.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/tests/test_ctitools.py` & `ctitools-0.4.3/berhoel/ctitools/tests/test_ctitools.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/berhoel/ctitools/tests/test_processing.py` & `ctitools-0.4.3/berhoel/ctitools/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.2/pyproject.toml` & `ctitools-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctitools"
-version = "0.4.2"
+version = "0.4.3"
 description = "Work with cti index files for the Heise papers c't and iX"
 packages = [{ include = "berhoel" }]
 exclude = ["**/.#*.py", "**/#*.py#"]
 authors = ["Berthold Höllmann <berthold@xn--hllmanns-n4a.de>"]
 license = "BSD 3"
 repository = "https://gitlab.com/berhoel/python/ctitools.git"
 homepage = "https://python.xn--hllmanns-n4a.de/ctitools/"
```

### Comparing `ctitools-0.4.2/PKG-INFO` & `ctitools-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctitools
-Version: 0.4.2
+Version: 0.4.3
 Summary: Work with cti index files for the Heise papers c't and iX
 Home-page: https://python.xn--hllmanns-n4a.de/ctitools/
 License: BSD 3
 Author: Berthold Höllmann
 Author-email: berthold@xn--hllmanns-n4a.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -14,15 +14,14 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: German
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Dist: setuptools (>=65.3.0,<66.0.0)
 Project-URL: Documentation, https://python.xn--hllmanns-n4a.de/ctitools/
 Project-URL: Repository, https://gitlab.com/berhoel/python/ctitools.git
 Description-Content-Type: text/x-rst
 
 Ctitools
```


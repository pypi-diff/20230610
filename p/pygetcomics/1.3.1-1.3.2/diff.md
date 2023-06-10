# Comparing `tmp/pygetcomics-1.3.1.tar.gz` & `tmp/pygetcomics-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygetcomics-1.3.1.tar", max compression
+gzip compressed data, was "pygetcomics-1.3.2.tar", max compression
```

## Comparing `pygetcomics-1.3.1.tar` & `pygetcomics-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.3.1/LICENSE
--rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.3.1/README.rst
--rw-r--r--   0        0        0      629 2022-05-28 11:14:42.643154 pygetcomics-1.3.1/berhoel/__init__.py
--rw-r--r--   0        0        0     1362 2023-03-18 17:04:23.687285 pygetcomics-1.3.1/berhoel/get_comics/__init__.py
--rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.3.1/berhoel/get_comics/garfield/__init__.py
--rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.3.1/berhoel/get_comics/gen_pdf/__init__.py
--rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.3.1/berhoel/get_comics/gen_pdf/template/book.tex
--rw-r--r--   0        0        0     9026 2023-03-19 18:37:43.323433 pygetcomics-1.3.1/berhoel/get_comics/gocomics/__init__.py
--rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.3.1/berhoel/get_comics/peanuts/__init__.py
--rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.3.1/berhoel/get_comics/peanuts/clean_up.py
--rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.3.1/berhoel/get_comics/peanuts/gen_book.py
--rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.3.1/berhoel/get_comics/tests/test_get_comics.py
--rw-r--r--   0        0        0     2491 2023-03-19 18:37:27.935433 pygetcomics-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 pygetcomics-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.3.2/LICENSE
+-rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.3.2/README.rst
+-rw-r--r--   0        0        0      638 2023-06-10 19:44:37.513034 pygetcomics-1.3.2/berhoel/__init__.py
+-rw-r--r--   0        0        0     1362 2023-03-18 17:04:23.687285 pygetcomics-1.3.2/berhoel/get_comics/__init__.py
+-rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.3.2/berhoel/get_comics/garfield/__init__.py
+-rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.3.2/berhoel/get_comics/gen_pdf/__init__.py
+-rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.3.2/berhoel/get_comics/gen_pdf/template/book.tex
+-rw-r--r--   0        0        0     9026 2023-03-19 18:37:43.323433 pygetcomics-1.3.2/berhoel/get_comics/gocomics/__init__.py
+-rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.3.2/berhoel/get_comics/peanuts/__init__.py
+-rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.3.2/berhoel/get_comics/peanuts/clean_up.py
+-rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.3.2/berhoel/get_comics/peanuts/gen_book.py
+-rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.3.2/berhoel/get_comics/tests/test_get_comics.py
+-rw-r--r--   0        0        0     2491 2023-06-10 19:44:50.533034 pygetcomics-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 pygetcomics-1.3.2/PKG-INFO
```

### Comparing `pygetcomics-1.3.1/LICENSE` & `pygetcomics-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/__init__.py` & `pygetcomics-1.3.2/berhoel/get_comics/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/garfield/__init__.py` & `pygetcomics-1.3.2/berhoel/get_comics/garfield/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/gen_pdf/__init__.py` & `pygetcomics-1.3.2/berhoel/get_comics/gen_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/gen_pdf/template/book.tex` & `pygetcomics-1.3.2/berhoel/get_comics/gen_pdf/template/book.tex`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/gocomics/__init__.py` & `pygetcomics-1.3.2/berhoel/get_comics/gocomics/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/peanuts/__init__.py` & `pygetcomics-1.3.2/berhoel/get_comics/peanuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/peanuts/clean_up.py` & `pygetcomics-1.3.2/berhoel/get_comics/peanuts/clean_up.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/peanuts/gen_book.py` & `pygetcomics-1.3.2/berhoel/get_comics/peanuts/gen_book.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/berhoel/get_comics/tests/test_get_comics.py` & `pygetcomics-1.3.2/berhoel/get_comics/tests/test_get_comics.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.1/pyproject.toml` & `pygetcomics-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGetComics"
-version = "1.3.1"
+version = "1.3.2"
 
 description = "Download various daily comics."
 
 packages = [
     { include = "berhoel" },
 ]
```

### Comparing `pygetcomics-1.3.1/PKG-INFO` & `pygetcomics-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygetcomics
-Version: 1.3.1
+Version: 1.3.2
 Summary: Download various daily comics.
 Home-page: https://gitlab.com/berhoel/python/pyGetComics.git
 License: BSD-2-Clause
 Author: Berthold Höllmann
 Author-email: berhoel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```


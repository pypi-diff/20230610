# Comparing `tmp/typepy-1.3.0.tar.gz` & `tmp/typepy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typepy-1.3.0.tar", last modified: Mon Sep 20 14:50:14 2021, max compression
+gzip compressed data, was "typepy-1.3.1.tar", last modified: Sat Jun 10 13:28:00 2023, max compression
```

## Comparing `typepy-1.3.0.tar` & `typepy-1.3.1.tar`

### file list

```diff
@@ -1,104 +1,105 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.710000 typepy-1.3.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-09-20 14:49:59.000000 typepy-1.3.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2021-09-20 14:49:59.000000 typepy-1.3.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     8806 2021-09-20 14:50:14.700000 typepy-1.3.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     7197 2021-09-20 14:49:59.000000 typepy-1.3.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.690000 typepy-1.3.0/docs/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.690000 typepy-1.3.0/docs/pages/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.690000 typepy-1.3.0/docs/pages/introduction/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-09-20 14:49:59.000000 typepy-1.3.0/docs/pages/introduction/summary.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1067 2021-09-20 14:49:59.000000 typepy-1.3.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.690000 typepy-1.3.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2021-09-20 14:49:59.000000 typepy-1.3.0/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       23 2021-09-20 14:49:59.000000 typepy-1.3.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       23 2021-09-20 14:49:59.000000 typepy-1.3.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2021-09-20 14:50:14.710000 typepy-1.3.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     3039 2021-09-20 14:49:59.000000 typepy-1.3.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.690000 typepy-1.3.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-09-20 14:49:59.000000 typepy-1.3.0/test/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.700000 typepy-1.3.0/test/checker/
--rw-r--r--   0 toor      (1000) toor      (1000)     1406 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_bool.py
--rw-r--r--   0 toor      (1000) toor      (1000)      994 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_bytes.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2321 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_datetime.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1337 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_dictionary.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1195 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_infinite.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2667 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_integer.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1800 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_ipaddress.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1005 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_list.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1108 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_nan.py
--rw-r--r--   0 toor      (1000) toor      (1000)      875 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_none.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2881 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_realnumber.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1903 2021-09-20 14:49:59.000000 typepy-1.3.0/test/checker/test_checker_string.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.700000 typepy-1.3.0/test/converter/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-09-20 14:49:59.000000 typepy-1.3.0/test/converter/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      276 2021-09-20 14:49:59.000000 typepy-1.3.0/test/converter/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2806 2021-09-20 14:49:59.000000 typepy-1.3.0/test/converter/test_bool.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6169 2021-09-20 14:49:59.000000 typepy-1.3.0/test/converter/test_integer.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6229 2021-09-20 14:49:59.000000 typepy-1.3.0/test/converter/test_realnumber.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4565 2021-09-20 14:49:59.000000 typepy-1.3.0/test/converter/test_string.py
--rw-r--r--   0 toor      (1000) toor      (1000)      594 2021-09-20 14:49:59.000000 typepy-1.3.0/test/test_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1926 2021-09-20 14:49:59.000000 typepy-1.3.0/test/test_function.py
--rw-r--r--   0 toor      (1000) toor      (1000)      910 2021-09-20 14:49:59.000000 typepy-1.3.0/test/test_str_function.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2985 2021-09-20 14:49:59.000000 typepy-1.3.0/test/test_type.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1467 2021-09-20 14:49:59.000000 typepy-1.3.0/tox.ini
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.700000 typepy-1.3.0/typepy/
--rw-r--r--   0 toor      (1000) toor      (1000)      662 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      401 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)      312 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1096 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/_function.py
--rw-r--r--   0 toor      (1000) toor      (1000)      397 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/_typecode.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.700000 typepy-1.3.0/typepy/checker/
--rw-r--r--   0 toor      (1000) toor      (1000)      621 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1198 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_bool.py
--rw-r--r--   0 toor      (1000) toor      (1000)      646 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_bytes.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2485 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_checker.py
--rw-r--r--   0 toor      (1000) toor      (1000)      539 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1159 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_datetime.py
--rw-r--r--   0 toor      (1000) toor      (1000)      885 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_dictionary.py
--rw-r--r--   0 toor      (1000) toor      (1000)      916 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_infinity.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2002 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_integer.py
--rw-r--r--   0 toor      (1000) toor      (1000)      315 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_interface.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1070 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_ipaddress.py
--rw-r--r--   0 toor      (1000) toor      (1000)      985 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_list.py
--rw-r--r--   0 toor      (1000) toor      (1000)      826 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_nan.py
--rw-r--r--   0 toor      (1000) toor      (1000)      617 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_none.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1905 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_realnumber.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2055 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/checker/_string.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.700000 typepy-1.3.0/typepy/converter/
--rw-r--r--   0 toor      (1000) toor      (1000)      519 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1306 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_bool.py
--rw-r--r--   0 toor      (1000) toor      (1000)      291 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_bytes.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5174 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_datetime.py
--rw-r--r--   0 toor      (1000) toor      (1000)      655 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_dictionary.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1015 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_integer.py
--rw-r--r--   0 toor      (1000) toor      (1000)      661 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_interface.py
--rw-r--r--   0 toor      (1000) toor      (1000)      843 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_ipaddress.py
--rw-r--r--   0 toor      (1000) toor      (1000)      426 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_list.py
--rw-r--r--   0 toor      (1000) toor      (1000)      222 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_nop.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1265 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_realnumber.py
--rw-r--r--   0 toor      (1000) toor      (1000)      498 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/converter/_string.py
--rw-r--r--   0 toor      (1000) toor      (1000)      178 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.700000 typepy-1.3.0/typepy/type/
--rw-r--r--   0 toor      (1000) toor      (1000)      497 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3552 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_base.py
--rw-r--r--   0 toor      (1000) toor      (1000)      794 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_binary.py
--rw-r--r--   0 toor      (1000) toor      (1000)      844 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_bool.py
--rw-r--r--   0 toor      (1000) toor      (1000)      792 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_bytes.py
--rw-r--r--   0 toor      (1000) toor      (1000)      835 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_datetime.py
--rw-r--r--   0 toor      (1000) toor      (1000)      849 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_dictionary.py
--rw-r--r--   0 toor      (1000) toor      (1000)      829 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_infinity.py
--rw-r--r--   0 toor      (1000) toor      (1000)      864 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_integer.py
--rw-r--r--   0 toor      (1000) toor      (1000)      843 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_ipaddress.py
--rw-r--r--   0 toor      (1000) toor      (1000)      807 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_list.py
--rw-r--r--   0 toor      (1000) toor      (1000)      804 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_nan.py
--rw-r--r--   0 toor      (1000) toor      (1000)      859 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_none.py
--rw-r--r--   0 toor      (1000) toor      (1000)      913 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_realnumber.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1505 2021-09-20 14:49:59.000000 typepy-1.3.0/typepy/type/_string.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-09-20 14:50:14.700000 typepy-1.3.0/typepy.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     8806 2021-09-20 14:50:14.000000 typepy-1.3.0/typepy.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     2335 2021-09-20 14:50:14.000000 typepy-1.3.0/typepy.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2021-09-20 14:50:14.000000 typepy-1.3.0/typepy.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      172 2021-09-20 14:50:14.000000 typepy-1.3.0/typepy.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        7 2021-09-20 14:50:14.000000 typepy-1.3.0/typepy.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.657168 typepy-1.3.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-06-10 13:27:44.000000 typepy-1.3.1/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-06-10 13:27:44.000000 typepy-1.3.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     8809 2023-06-10 13:28:00.657168 typepy-1.3.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     7218 2023-06-10 13:27:44.000000 typepy-1.3.1/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.637168 typepy-1.3.1/docs/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.637168 typepy-1.3.1/docs/pages/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.637168 typepy-1.3.1/docs/pages/introduction/
+-rw-r--r--   0 toor      (1000) toor      (1000)       88 2023-06-10 13:27:44.000000 typepy-1.3.1/docs/pages/introduction/summary.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1164 2023-06-10 13:27:44.000000 typepy-1.3.1/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.637168 typepy-1.3.1/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-06-10 13:27:44.000000 typepy-1.3.1/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       23 2023-06-10 13:27:44.000000 typepy-1.3.1/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       23 2023-06-10 13:27:44.000000 typepy-1.3.1/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-10 13:28:00.657168 typepy-1.3.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     3112 2023-06-10 13:27:44.000000 typepy-1.3.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.637168 typepy-1.3.1/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-10 13:27:44.000000 typepy-1.3.1/test/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.647168 typepy-1.3.1/test/checker/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1406 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_bool.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      994 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_bytes.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2321 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_datetime.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1337 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_dictionary.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1195 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_infinite.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2667 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_integer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1800 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_ipaddress.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1005 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_list.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1108 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_nan.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      875 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_none.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2881 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_realnumber.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1903 2023-06-10 13:27:44.000000 typepy-1.3.1/test/checker/test_checker_string.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.647168 typepy-1.3.1/test/converter/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-10 13:27:44.000000 typepy-1.3.1/test/converter/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      274 2023-06-10 13:27:44.000000 typepy-1.3.1/test/converter/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2806 2023-06-10 13:27:44.000000 typepy-1.3.1/test/converter/test_bool.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6169 2023-06-10 13:27:44.000000 typepy-1.3.1/test/converter/test_integer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6229 2023-06-10 13:27:44.000000 typepy-1.3.1/test/converter/test_realnumber.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4565 2023-06-10 13:27:44.000000 typepy-1.3.1/test/converter/test_string.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      594 2023-06-10 13:27:44.000000 typepy-1.3.1/test/test_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1926 2023-06-10 13:27:44.000000 typepy-1.3.1/test/test_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      910 2023-06-10 13:27:44.000000 typepy-1.3.1/test/test_str_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2985 2023-06-10 13:27:44.000000 typepy-1.3.1/test/test_type.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1398 2023-06-10 13:27:44.000000 typepy-1.3.1/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.647168 typepy-1.3.1/typepy/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1129 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      401 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      312 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1096 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      397 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/_typecode.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.647168 typepy-1.3.1/typepy/checker/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1000 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1198 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_bool.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      646 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_bytes.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2485 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_checker.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      539 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1159 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_datetime.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      885 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_dictionary.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      916 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_infinity.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2002 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_integer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      315 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1070 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_ipaddress.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      985 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_list.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      826 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_nan.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      617 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_none.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1905 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_realnumber.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2055 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/checker/_string.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.647168 typepy-1.3.1/typepy/converter/
+-rw-r--r--   0 toor      (1000) toor      (1000)      824 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1306 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_bool.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      291 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_bytes.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5169 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_datetime.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      655 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_dictionary.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1015 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_integer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      661 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_interface.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      843 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_ipaddress.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      426 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_list.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      222 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_nop.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1265 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_realnumber.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      498 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/converter/_string.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      178 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.657168 typepy-1.3.1/typepy/type/
+-rw-r--r--   0 toor      (1000) toor      (1000)      743 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3552 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      794 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_binary.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      844 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_bool.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      792 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_bytes.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      835 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_datetime.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      849 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_dictionary.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      829 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_infinity.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      864 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_integer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      843 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_ipaddress.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      807 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_list.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      804 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_nan.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      859 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_none.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      913 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_realnumber.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1505 2023-06-10 13:27:44.000000 typepy-1.3.1/typepy/type/_string.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-10 13:28:00.647168 typepy-1.3.1/typepy.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     8809 2023-06-10 13:28:00.000000 typepy-1.3.1/typepy.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     2364 2023-06-10 13:28:00.000000 typepy-1.3.1/typepy.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-10 13:28:00.000000 typepy-1.3.1/typepy.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-10 13:27:53.000000 typepy-1.3.1/typepy.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      172 2023-06-10 13:28:00.000000 typepy-1.3.1/typepy.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        7 2023-06-10 13:28:00.000000 typepy-1.3.1/typepy.egg-info/top_level.txt
```

### Comparing `typepy-1.3.0/LICENSE` & `typepy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/PKG-INFO` & `typepy-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: typepy
-Version: 1.3.0
+Version: 1.3.1
 Summary: typepy is a Python library for variable type checker/validator/converter at a run time.
 Home-page: https://github.com/thombashi/typepy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://typepy.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/typepy
 Project-URL: Tracker, https://github.com/thombashi/typepy/issues
-Project-URL: Changes, https://github.com/thombashi/typepy/releases
+Project-URL: Changlog, https://github.com/thombashi/typepy/releases
 Keywords: library,type-checking,type-conversion,validator
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: datetime
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **typepy**
    :backlinks: top
@@ -62,23 +61,23 @@
     :target: https://github.com/thombashi/typepy/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
 .. image:: https://coveralls.io/repos/github/thombashi/typepy/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/typepy?branch=master
     :alt: Test coverage
 
-.. image:: https://github.com/thombashi/typepy/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/typepy/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/typepy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/typepy/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Features
 ==========
 - checking a value type
 - validate a value for a type
-- convert a value from a type to the other type
+- convert a value from one type to the other type
 
 The correspondence between Python types and ``typepy`` classes are as follows:
 
 .. table:: Supported Types
 
     ================================================  =======================================================================================================
     Python Type                                       typepy: Type Class
@@ -125,18 +124,18 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-typepy
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/typepy/network/dependencies>`__
 
-Optioal dependencies
+Optional dependencies
 ----------------------------------
 These packages can be installed via ``pip install typepy[datetime]``:
 
 - `python-dateutil <https://dateutil.readthedocs.io/en/stable/>`__
 - `pytz <https://pypi.org/project/pytz/>`__
 
 Usage
@@ -208,26 +207,24 @@
         >>> Integer("1").force_convert()  # force_convert() forcibly convert the value
         1
         >>> Integer(1.1).force_convert()
         1
         >>> try:
         ...     Integer("abc").force_convert()
         ... except TypeConversionError as e:
-        ...     # force_convert() raised TypeConversionError when the value not convertible
+        ...     # force_convert() raised TypeConversionError when the value was not convertible
         ...     print(e)
         ...
         failed to force_convert to int: type=<class 'str'>
 
 
 For more information
 --------------------------------------------
 Type check/validate/convert results differed according to
-``strict_level`` value which can pass to typepy classes constructors as an argument.
+``strict_level`` value which can pass to typepy class constructors as an argument.
 More information can be found in the
 `API reference <https://typepy.rtfd.io/en/latest/pages/reference/index.html>`__.
 
 Documentation
 ===============
 https://typepy.rtfd.io/
 
-
-
```

### Comparing `typepy-1.3.0/README.rst` & `typepy-1.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     :target: https://github.com/thombashi/typepy/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
 .. image:: https://coveralls.io/repos/github/thombashi/typepy/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/typepy?branch=master
     :alt: Test coverage
 
-.. image:: https://github.com/thombashi/typepy/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/typepy/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/typepy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/typepy/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Features
 ==========
 - checking a value type
 - validate a value for a type
-- convert a value from a type to the other type
+- convert a value from one type to the other type
 
 The correspondence between Python types and ``typepy`` classes are as follows:
 
 .. table:: Supported Types
 
     ================================================  =======================================================================================================
     Python Type                                       typepy: Type Class
@@ -89,18 +89,18 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-typepy
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/typepy/network/dependencies>`__
 
-Optioal dependencies
+Optional dependencies
 ----------------------------------
 These packages can be installed via ``pip install typepy[datetime]``:
 
 - `python-dateutil <https://dateutil.readthedocs.io/en/stable/>`__
 - `pytz <https://pypi.org/project/pytz/>`__
 
 Usage
@@ -172,24 +172,24 @@
         >>> Integer("1").force_convert()  # force_convert() forcibly convert the value
         1
         >>> Integer(1.1).force_convert()
         1
         >>> try:
         ...     Integer("abc").force_convert()
         ... except TypeConversionError as e:
-        ...     # force_convert() raised TypeConversionError when the value not convertible
+        ...     # force_convert() raised TypeConversionError when the value was not convertible
         ...     print(e)
         ...
         failed to force_convert to int: type=<class 'str'>
 
 
 For more information
 --------------------------------------------
 Type check/validate/convert results differed according to
-``strict_level`` value which can pass to typepy classes constructors as an argument.
+``strict_level`` value which can pass to typepy class constructors as an argument.
 More information can be found in the
 `API reference <https://typepy.rtfd.io/en/latest/pages/reference/index.html>`__.
 
 Documentation
 ===============
 https://typepy.rtfd.io/
```

### Comparing `typepy-1.3.0/pyproject.toml` & `typepy-1.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
@@ -14,14 +15,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
 known_third_party = [
     'dateutil',
     'logbook',
     'pytablewriter',
     'pytest',
@@ -55,14 +57,14 @@
     'abstractproperty',
     'abstractclassmethod',
     'warnings.warn',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `typepy-1.3.0/setup.py` & `typepy-1.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "typepy"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -51,42 +51,48 @@
     name=MODULE_NAME,
     version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description=summary,
     include_package_data=True,
-    keywords=["library", "type-checking", "type-conversion", "validator"],
+    keywords=[
+        "library",
+        "type-checking",
+        "type-conversion",
+        "validator",
+    ],
     license=pkg_info["__license__"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Documentation": f"https://{MODULE_NAME:s}.rtfd.io/",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
-        "Changes": f"{REPOSITORY_URL:s}/releases",
+        "Changlog": f"{REPOSITORY_URL:s}/releases",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=install_requires,
     extras_require={"datetime": DATETIME_REQUIRES, "test": tests_requires + DATETIME_REQUIRES},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     cmdclass=get_release_command_class(),
+    zip_safe=False,
 )
```

### Comparing `typepy-1.3.0/test/checker/test_checker_bool.py` & `typepy-1.3.1/test/checker/test_checker_bool.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_bytes.py` & `typepy-1.3.1/test/checker/test_checker_bytes.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_datetime.py` & `typepy-1.3.1/test/checker/test_checker_datetime.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_dictionary.py` & `typepy-1.3.1/test/checker/test_checker_dictionary.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_infinite.py` & `typepy-1.3.1/test/checker/test_checker_infinite.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_integer.py` & `typepy-1.3.1/test/checker/test_checker_integer.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_ipaddress.py` & `typepy-1.3.1/test/checker/test_checker_ipaddress.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_list.py` & `typepy-1.3.1/test/checker/test_checker_list.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_nan.py` & `typepy-1.3.1/test/checker/test_checker_nan.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_none.py` & `typepy-1.3.1/test/checker/test_checker_none.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_realnumber.py` & `typepy-1.3.1/test/checker/test_checker_realnumber.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/checker/test_checker_string.py` & `typepy-1.3.1/test/checker/test_checker_string.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/converter/test_bool.py` & `typepy-1.3.1/test/converter/test_bool.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/converter/test_integer.py` & `typepy-1.3.1/test/converter/test_integer.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/converter/test_realnumber.py` & `typepy-1.3.1/test/converter/test_realnumber.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/converter/test_string.py` & `typepy-1.3.1/test/converter/test_string.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/test_common.py` & `typepy-1.3.1/test/test_common.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/test_function.py` & `typepy-1.3.1/test/test_function.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/test_str_function.py` & `typepy-1.3.1/test/test_str_function.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/test/test_type.py` & `typepy-1.3.1/test/test_type.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/tox.ini` & `typepy-1.3.1/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 [tox]
 envlist =
-    py{36,37,38,39,310}
+    py{37,38,39,310,311}
     pypy3
     build
-    clean
     cov
     docs
     lint
     readme
 
 [testenv]
-deps =
-    .[test]
+passenv = *
+extras =
+    test
 commands =
     pytest {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
     twine
     wheel
 commands =
     python setup.py sdist bdist_wheel
     twine check dist/*.whl dist/*.tar.gz
     python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.3
+    cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:cov]
+extras =
+    test
 deps =
-    .[test]
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:docs]
-basepython = python3.8
 deps =
     -r{toxinidir}/requirements/docs_requirements.txt
 commands =
     python setup.py build_sphinx --source-dir=docs/ --build-dir=docs/_build --all-files
 
 [testenv:fmt]
-basepython = python3.8
 skip_install = true
 deps =
-    autoflake
-    black
+    autoflake>=2
+    black>=23.1
     isort>=5
 commands =
     black make_test_cases.py setup.py test typepy
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
 
 [testenv:lint]
-basepython = python3.8
 skip_install = true
 deps =
-    codespell
-    pylama
-    mypy>=0.902
+    codespell>=2
+    mypy>=1
+    pylama>=8.4.1
     types-python-dateutil
     types-pytz
 commands =
     python setup.py check
     codespell typepy docs/pages test -q2 --check-filenames
     mypy typepy setup.py
     pylama
 
 [testenv:readme]
 skip_install = true
 changedir = docs
 deps =
-    readmemaker>=1.0.0
+    readmemaker>=1.1.0
 commands =
     python make_readme.py
```

### Comparing `typepy-1.3.0/typepy/_function.py` & `typepy-1.3.1/typepy/_function.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_bool.py` & `typepy-1.3.1/typepy/checker/_bool.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_bytes.py` & `typepy-1.3.1/typepy/checker/_bytes.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_checker.py` & `typepy-1.3.1/typepy/checker/_checker.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_common.py` & `typepy-1.3.1/typepy/checker/_common.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_datetime.py` & `typepy-1.3.1/typepy/checker/_datetime.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_dictionary.py` & `typepy-1.3.1/typepy/checker/_dictionary.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_infinity.py` & `typepy-1.3.1/typepy/checker/_infinity.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_integer.py` & `typepy-1.3.1/typepy/checker/_integer.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_ipaddress.py` & `typepy-1.3.1/typepy/checker/_ipaddress.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_list.py` & `typepy-1.3.1/typepy/checker/_list.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_nan.py` & `typepy-1.3.1/typepy/checker/_nan.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_none.py` & `typepy-1.3.1/typepy/checker/_none.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_realnumber.py` & `typepy-1.3.1/typepy/checker/_realnumber.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/checker/_string.py` & `typepy-1.3.1/typepy/checker/_string.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/converter/__init__.py` & `typepy-1.3.1/typepy/type/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,37 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-from ._bool import BoolConverter
-from ._bytes import BytesConverter
-from ._datetime import DateTimeConverter
-from ._dictionary import DictionaryConverter
-from ._integer import IntegerConverter
-from ._interface import ValueConverterInterface
-from ._ipaddress import IpAddressConverter
-from ._list import ListConverter
-from ._nop import NopConverter
-from ._realnumber import FloatConverter
-from ._string import NullStringConverter, StringConverter
+from ._base import AbstractType
+from ._binary import Binary
+from ._bool import Bool
+from ._bytes import Bytes
+from ._datetime import DateTime
+from ._dictionary import Dictionary
+from ._infinity import Infinity
+from ._integer import Integer
+from ._ipaddress import IpAddress
+from ._list import List
+from ._nan import Nan
+from ._none import NoneType
+from ._realnumber import RealNumber
+from ._string import NullString, String
+
+
+__all__ = (
+    "AbstractType",
+    "Binary",
+    "Bool",
+    "Bytes",
+    "DateTime",
+    "Dictionary",
+    "Infinity",
+    "Integer",
+    "IpAddress",
+    "List",
+    "Nan",
+    "NoneType",
+    "NullString",
+    "RealNumber",
+    "String",
+)
```

### Comparing `typepy-1.3.0/typepy/converter/_bool.py` & `typepy-1.3.1/typepy/converter/_bool.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/converter/_datetime.py` & `typepy-1.3.1/typepy/converter/_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 from .._common import strip_ansi_escape
 from .._const import DefaultValue, ParamKey
 from ..error import TypeConversionError
 from ._interface import AbstractValueConverter
 
 
 class DateTimeConverter(AbstractValueConverter):
-
-    __DAYS_TO_SECONDS_COEF = 60 ** 2 * 24
-    __MICROSECONDS_TO_SECONDS_COEF = 1000 ** 2
+    __DAYS_TO_SECONDS_COEF = 60**2 * 24
+    __MICROSECONDS_TO_SECONDS_COEF = 1000**2
     __COMMON_DST_TIMEZONE_TABLE = {
         -36000: "America/Adak",  # -1000
         -32400: "US/Alaska",  # -0900
         -28800: "US/Pacific",  # -0800
         -25200: "US/Mountain",  # -0700
         -21600: "US/Central",  # -0600
         -18000: "US/Eastern",  # -0500
```

### Comparing `typepy-1.3.0/typepy/converter/_dictionary.py` & `typepy-1.3.1/typepy/converter/_dictionary.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/converter/_integer.py` & `typepy-1.3.1/typepy/converter/_integer.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/converter/_interface.py` & `typepy-1.3.1/typepy/converter/_interface.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/converter/_ipaddress.py` & `typepy-1.3.1/typepy/converter/_ipaddress.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/converter/_realnumber.py` & `typepy-1.3.1/typepy/converter/_realnumber.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_base.py` & `typepy-1.3.1/typepy/type/_base.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_binary.py` & `typepy-1.3.1/typepy/type/_binary.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_bool.py` & `typepy-1.3.1/typepy/type/_bool.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_bytes.py` & `typepy-1.3.1/typepy/type/_bytes.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_datetime.py` & `typepy-1.3.1/typepy/type/_datetime.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_dictionary.py` & `typepy-1.3.1/typepy/type/_dictionary.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_infinity.py` & `typepy-1.3.1/typepy/type/_infinity.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_integer.py` & `typepy-1.3.1/typepy/type/_integer.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_ipaddress.py` & `typepy-1.3.1/typepy/type/_ipaddress.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_list.py` & `typepy-1.3.1/typepy/type/_list.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_nan.py` & `typepy-1.3.1/typepy/type/_nan.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_none.py` & `typepy-1.3.1/typepy/type/_none.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_realnumber.py` & `typepy-1.3.1/typepy/type/_realnumber.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy/type/_string.py` & `typepy-1.3.1/typepy/type/_string.py`

 * *Files identical despite different names*

### Comparing `typepy-1.3.0/typepy.egg-info/PKG-INFO` & `typepy-1.3.1/typepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: typepy
-Version: 1.3.0
+Version: 1.3.1
 Summary: typepy is a Python library for variable type checker/validator/converter at a run time.
 Home-page: https://github.com/thombashi/typepy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://typepy.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/typepy
 Project-URL: Tracker, https://github.com/thombashi/typepy/issues
-Project-URL: Changes, https://github.com/thombashi/typepy/releases
+Project-URL: Changlog, https://github.com/thombashi/typepy/releases
 Keywords: library,type-checking,type-conversion,validator
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: datetime
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **typepy**
    :backlinks: top
@@ -62,23 +61,23 @@
     :target: https://github.com/thombashi/typepy/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
 .. image:: https://coveralls.io/repos/github/thombashi/typepy/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/typepy?branch=master
     :alt: Test coverage
 
-.. image:: https://github.com/thombashi/typepy/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/typepy/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/typepy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/typepy/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Features
 ==========
 - checking a value type
 - validate a value for a type
-- convert a value from a type to the other type
+- convert a value from one type to the other type
 
 The correspondence between Python types and ``typepy`` classes are as follows:
 
 .. table:: Supported Types
 
     ================================================  =======================================================================================================
     Python Type                                       typepy: Type Class
@@ -125,18 +124,18 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-typepy
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/typepy/network/dependencies>`__
 
-Optioal dependencies
+Optional dependencies
 ----------------------------------
 These packages can be installed via ``pip install typepy[datetime]``:
 
 - `python-dateutil <https://dateutil.readthedocs.io/en/stable/>`__
 - `pytz <https://pypi.org/project/pytz/>`__
 
 Usage
@@ -208,26 +207,24 @@
         >>> Integer("1").force_convert()  # force_convert() forcibly convert the value
         1
         >>> Integer(1.1).force_convert()
         1
         >>> try:
         ...     Integer("abc").force_convert()
         ... except TypeConversionError as e:
-        ...     # force_convert() raised TypeConversionError when the value not convertible
+        ...     # force_convert() raised TypeConversionError when the value was not convertible
         ...     print(e)
         ...
         failed to force_convert to int: type=<class 'str'>
 
 
 For more information
 --------------------------------------------
 Type check/validate/convert results differed according to
-``strict_level`` value which can pass to typepy classes constructors as an argument.
+``strict_level`` value which can pass to typepy class constructors as an argument.
 More information can be found in the
 `API reference <https://typepy.rtfd.io/en/latest/pages/reference/index.html>`__.
 
 Documentation
 ===============
 https://typepy.rtfd.io/
 
-
-
```

### Comparing `typepy-1.3.0/typepy.egg-info/SOURCES.txt` & `typepy-1.3.1/typepy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 typepy/_function.py
 typepy/_typecode.py
 typepy/error.py
 typepy/py.typed
 typepy.egg-info/PKG-INFO
 typepy.egg-info/SOURCES.txt
 typepy.egg-info/dependency_links.txt
+typepy.egg-info/not-zip-safe
 typepy.egg-info/requires.txt
 typepy.egg-info/top_level.txt
 typepy/checker/__init__.py
 typepy/checker/_bool.py
 typepy/checker/_bytes.py
 typepy/checker/_checker.py
 typepy/checker/_common.py
```


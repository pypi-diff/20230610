# Comparing `tmp/tokenize_rt-5.0.0.tar.gz` & `tmp/tokenize_rt-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenize_rt-5.0.0.tar", last modified: Mon Oct  3 23:27:48 2022, max compression
+gzip compressed data, was "tokenize_rt-5.1.0.tar", last modified: Sat Jun 10 20:35:48 2023, max compression
```

## Comparing `tokenize_rt-5.0.0.tar` & `tokenize_rt-5.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-03 23:27:48.406928 tokenize_rt-5.0.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-10-03 22:36:13.000000 tokenize_rt-5.0.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4290 2022-10-03 23:27:48.406928 tokenize_rt-5.0.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3666 2022-10-03 22:36:13.000000 tokenize_rt-5.0.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1141 2022-10-03 23:27:48.406928 tokenize_rt-5.0.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-10-03 22:36:13.000000 tokenize_rt-5.0.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-03 23:27:48.406928 tokenize_rt-5.0.0/tokenize_rt.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4290 2022-10-03 23:27:48.000000 tokenize_rt-5.0.0/tokenize_rt.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      229 2022-10-03 23:27:48.000000 tokenize_rt-5.0.0/tokenize_rt.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-10-03 23:27:48.000000 tokenize_rt-5.0.0/tokenize_rt.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       49 2022-10-03 23:27:48.000000 tokenize_rt-5.0.0/tokenize_rt.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2022-10-03 23:27:48.000000 tokenize_rt-5.0.0/tokenize_rt.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5702 2022-10-03 23:27:47.000000 tokenize_rt-5.0.0/tokenize_rt.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:12:24.000000 tokenize_rt-5.1.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4062 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3438 2023-06-10 20:12:24.000000 tokenize_rt-5.1.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1114 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:12:24.000000 tokenize_rt-5.1.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/tokenize_rt.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4062 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      229 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       49 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5702 2023-06-10 20:31:42.000000 tokenize_rt-5.1.0/tokenize_rt.py
```

### Comparing `tokenize_rt-5.0.0/LICENSE` & `tokenize_rt-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenize_rt-5.0.0/PKG-INFO` & `tokenize_rt-5.1.0/tokenize_rt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: tokenize_rt
-Version: 5.0.0
+Name: tokenize-rt
+Version: 5.1.0
 Summary: A wrapper around the stdlib `tokenize` which roundtrips.
 Home-page: https://github.com/asottile/tokenize-rt
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.tokenize-rt?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=25&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/25/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=25&branchName=main)
+[![build status](https://github.com/asottile/tokenize-rt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/tokenize-rt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/tokenize-rt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/tokenize-rt/main)
 
 tokenize-rt
 ===========
 
 The stdlib `tokenize` module does not properly roundtrip.  This wrapper
 around the stdlib provides two additional tokens `ESCAPED_NL` and
```

### Comparing `tokenize_rt-5.0.0/README.md` & `tokenize_rt-5.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.tokenize-rt?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=25&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/25/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=25&branchName=main)
+[![build status](https://github.com/asottile/tokenize-rt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/tokenize-rt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/tokenize-rt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/tokenize-rt/main)
 
 tokenize-rt
 ===========
 
 The stdlib `tokenize` module does not properly roundtrip.  This wrapper
 around the stdlib provides two additional tokens `ESCAPED_NL` and
```

### Comparing `tokenize_rt-5.0.0/setup.cfg` & `tokenize_rt-5.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [metadata]
 name = tokenize_rt
-version = 5.0.0
+version = 5.1.0
 description = A wrapper around the stdlib `tokenize` which roundtrips.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/tokenize-rt
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = tokenize_rt
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	tokenize-rt = tokenize_rt:main
 
 [bdist_wheel]
 universal = True
@@ -31,15 +31,14 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

### Comparing `tokenize_rt-5.0.0/tokenize_rt.egg-info/PKG-INFO` & `tokenize_rt-5.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: tokenize-rt
-Version: 5.0.0
+Name: tokenize_rt
+Version: 5.1.0
 Summary: A wrapper around the stdlib `tokenize` which roundtrips.
 Home-page: https://github.com/asottile/tokenize-rt
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.tokenize-rt?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=25&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/25/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=25&branchName=main)
+[![build status](https://github.com/asottile/tokenize-rt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/tokenize-rt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/tokenize-rt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/tokenize-rt/main)
 
 tokenize-rt
 ===========
 
 The stdlib `tokenize` module does not properly roundtrip.  This wrapper
 around the stdlib provides two additional tokens `ESCAPED_NL` and
```

### Comparing `tokenize_rt-5.0.0/tokenize_rt.py` & `tokenize_rt-5.1.0/tokenize_rt.py`

 * *Files identical despite different names*


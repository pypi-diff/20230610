# Comparing `tmp/add_trailing_comma-2.4.0.tar.gz` & `tmp/add_trailing_comma-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "add_trailing_comma-2.4.0.tar", last modified: Mon Dec 12 20:11:04 2022, max compression
+gzip compressed data, was "add_trailing_comma-2.5.0.tar", last modified: Sat Jun 10 20:30:39 2023, max compression
```

## Comparing `add_trailing_comma-2.4.0.tar` & `add_trailing_comma-2.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-12 20:11:04.484072 add_trailing_comma-2.4.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4887 2022-12-12 20:11:04.484072 add_trailing_comma-2.4.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4250 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-12 20:11:04.484072 add_trailing_comma-2.4.0/add_trailing_comma/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2307 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3227 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/add_trailing_comma/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-12 20:11:04.484072 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/_with.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1887 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1645 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/functions.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3244 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_plugins/match.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6613 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/add_trailing_comma/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-12-12 20:11:04.484072 add_trailing_comma-2.4.0/add_trailing_comma.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4887 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/add_trailing_comma.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/add_trailing_comma.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/add_trailing_comma.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/add_trailing_comma.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/add_trailing_comma.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2022-12-12 20:11:04.000000 add_trailing_comma-2.4.0/add_trailing_comma.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1232 2022-12-12 20:11:04.484072 add_trailing_comma-2.4.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-12-12 19:32:54.000000 add_trailing_comma-2.4.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4032 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/add_trailing_comma/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2307 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3227 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/_with.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1887 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1645 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/functions.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3058 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_plugins/match.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6613 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/add_trailing_comma/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.0/add_trailing_comma.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1233 2023-06-10 20:30:39.812250 add_trailing_comma-2.5.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.0/setup.py
```

### Comparing `add_trailing_comma-2.4.0/LICENSE` & `add_trailing_comma-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/PKG-INFO` & `add_trailing_comma-2.5.0/add_trailing_comma.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: add_trailing_comma
-Version: 2.4.0
+Name: add-trailing-comma
+Version: 2.5.0
 Summary: Automatically add trailing commas to calls and literals
 Home-page: https://github.com/asottile/add-trailing-comma
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
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.add-trailing-comma?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=3&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/3/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=3&branchName=main)
+[![build status](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/add-trailing-comma/main.svg)](https://results.pre-commit.ci/latest/github/asottile/add-trailing-comma/main)
 
 add-trailing-comma
 ==================
 
 A tool (and pre-commit hook) to automatically add trailing commas to calls and
 literals.
@@ -35,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.4.0
+    rev: v2.5.0
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.4.0/README.md` & `add_trailing_comma-2.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.add-trailing-comma?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=3&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/3/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=3&branchName=main)
+[![build status](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/add-trailing-comma/main.svg)](https://results.pre-commit.ci/latest/github/asottile/add-trailing-comma/main)
 
 add-trailing-comma
 ==================
 
 A tool (and pre-commit hook) to automatically add trailing commas to calls and
 literals.
@@ -18,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.4.0
+    rev: v2.5.0
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_ast_helpers.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_data.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_data.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_main.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_main.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_plugins/_with.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/_with.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_plugins/calls.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/calls.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_plugins/classes.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/classes.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_plugins/functions.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/functions.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_plugins/imports.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/imports.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_plugins/literals.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import ast
 import functools
-import sys
 from typing import Iterable
 
 from tokenize_rt import NON_CODING_TOKENS
 from tokenize_rt import Offset
 from tokenize_rt import Token
 
 from add_trailing_comma._ast_helpers import ast_to_offset
@@ -110,17 +109,13 @@
 @register(ast.Tuple)
 def visit_Tuple(
         state: State,
         node: ast.Tuple,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if node.elts:
         is_one_el = len(node.elts) == 1
-        if (
-                ast_to_offset(node) == ast_to_offset(node.elts[0]) or
-                # in < py38 tuples lie about offset -- later we must backtrack
-                sys.version_info < (3, 8)
-        ):
+        if ast_to_offset(node) == ast_to_offset(node.elts[0]):
             func = functools.partial(_fix_tuple, one_el_tuple=is_one_el)
             yield ast_to_offset(node), func
-        else:  # pragma: >=3.8 cover
+        else:
             func = functools.partial(_fix_tuple_py38, one_el_tuple=is_one_el)
             yield ast_to_offset(node), func
```

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_plugins/match.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_plugins/match.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma/_token_helpers.py` & `add_trailing_comma-2.5.0/add_trailing_comma/_token_helpers.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma.egg-info/PKG-INFO` & `add_trailing_comma-2.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: add-trailing-comma
-Version: 2.4.0
+Name: add_trailing_comma
+Version: 2.5.0
 Summary: Automatically add trailing commas to calls and literals
 Home-page: https://github.com/asottile/add-trailing-comma
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
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.add-trailing-comma?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=3&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/3/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=3&branchName=main)
+[![build status](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/add-trailing-comma/main.svg)](https://results.pre-commit.ci/latest/github/asottile/add-trailing-comma/main)
 
 add-trailing-comma
 ==================
 
 A tool (and pre-commit hook) to automatically add trailing commas to calls and
 literals.
@@ -35,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.4.0
+    rev: v2.5.0
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.4.0/add_trailing_comma.egg-info/SOURCES.txt` & `add_trailing_comma-2.5.0/add_trailing_comma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.4.0/setup.cfg` & `add_trailing_comma-2.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [metadata]
 name = add_trailing_comma
-version = 2.4.0
+version = 2.5.0
 description = Automatically add trailing commas to calls and literals
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/add-trailing-comma
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
 packages = find:
 install_requires = 
 	tokenize-rt>=3.0.1
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
 
 [options.entry_points]
```


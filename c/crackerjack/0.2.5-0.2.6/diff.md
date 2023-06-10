# Comparing `tmp/crackerjack-0.2.5.tar.gz` & `tmp/crackerjack-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.2.5.tar", last modified: Sat Jun 10 16:59:02 2023, max compression
+gzip compressed data, was "crackerjack-0.2.6.tar", last modified: Sat Jun 10 17:21:00 2023, max compression
```

## Comparing `crackerjack-0.2.5.tar` & `crackerjack-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.5/LICENSE
--rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-06-10 16:58:33.090106 crackerjack-0.2.5/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      163 2023-06-10 16:58:33.038512 crackerjack-0.2.5/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-06-10 16:58:33.073814 crackerjack-0.2.5/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     1723 2023-06-10 16:58:33.053914 crackerjack-0.2.5/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.5/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.5/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.5/crackerjack/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-10 14:55:58.374530 crackerjack-0.2.5/crackerjack/__main__.py
--rw-r--r--   0        0        0     5370 2023-06-10 16:43:42.483425 crackerjack-0.2.5/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1644 2023-06-10 16:58:33.805909 crackerjack-0.2.5/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     1644 2023-06-10 16:59:02.502818 crackerjack-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 crackerjack-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 17:20:28.681060 crackerjack-0.2.6/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      163 2023-06-10 17:20:28.622409 crackerjack-0.2.6/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-06-10 17:20:28.663949 crackerjack-0.2.6/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     1723 2023-06-10 17:20:28.643455 crackerjack-0.2.6/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.6/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.6/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.6/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-10 14:55:58.374530 crackerjack-0.2.6/crackerjack/__main__.py
+-rw-r--r--   0        0        0     5370 2023-06-10 16:43:42.483425 crackerjack-0.2.6/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1595 2023-06-10 17:20:29.654708 crackerjack-0.2.6/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     1595 2023-06-10 17:21:00.939500 crackerjack-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 crackerjack-0.2.6/PKG-INFO
```

### Comparing `crackerjack-0.2.5/LICENSE` & `crackerjack-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.5/README.md` & `crackerjack-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.5/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.2.6/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.5/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.2.6/crackerjack/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.5/crackerjack/__main__.py` & `crackerjack-0.2.6/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.5/crackerjack/crackerjack.py` & `crackerjack-0.2.6/crackerjack/crackerjack.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.5/crackerjack/pyproject.toml` & `crackerjack-0.2.6/crackerjack/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.0",
     "icecream>=2.1.3",
     "pre-commit>=3.2.2",
-    "-e file:///${PROJECT_ROOT}/../acb#egg=acb",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -36,15 +35,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.5"
+version = "0.2.6"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -60,15 +59,15 @@
 dependencies = [
     "click>=8.1.3",
     "pdoc3>=0.10.0",
     "pdm-bump>=0.7.0",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
     "pydantic>=2.0b2",
-    "acb>=0.1.5",
+    "acb>=0.1.6",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.2.5/pyproject.toml` & `crackerjack-0.2.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.0",
     "icecream>=2.1.3",
     "pre-commit>=3.2.2",
-    "-e file:///${PROJECT_ROOT}/../acb#egg=acb",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -36,15 +35,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.5"
+version = "0.2.6"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -60,15 +59,15 @@
 dependencies = [
     "click>=8.1.3",
     "pdoc3>=0.10.0",
     "pdm-bump>=0.7.0",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
     "pydantic>=2.0b2",
-    "acb>=0.1.5",
+    "acb>=0.1.6",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.2.5/PKG-INFO` & `crackerjack-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.2.5
+Version: 0.2.6
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -17,15 +17,15 @@
 Requires-Python: >=3.11
 Requires-Dist: click>=8.1.3
 Requires-Dist: pdoc3>=0.10.0
 Requires-Dist: pdm-bump>=0.7.0
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: aioconsole>=0.6.1
 Requires-Dist: pydantic>=2.0b2
-Requires-Dist: acb>=0.1.5
+Requires-Dist: acb>=0.1.6
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
 [![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
```


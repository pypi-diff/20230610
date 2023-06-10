# Comparing `tmp/yesqa-1.4.0.tar.gz` & `tmp/yesqa-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yesqa-1.4.0.tar", last modified: Tue Aug  2 00:03:51 2022, max compression
+gzip compressed data, was "yesqa-1.5.0.tar", last modified: Sat Jun 10 20:33:04 2023, max compression
```

## Comparing `yesqa-1.4.0.tar` & `yesqa-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-02 00:03:51.874245 yesqa-1.4.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-08-01 23:36:17.000000 yesqa-1.4.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2187 2022-08-02 00:03:51.874245 yesqa-1.4.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1359 2022-08-02 00:03:50.000000 yesqa-1.4.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1314 2022-08-02 00:03:51.874245 yesqa-1.4.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-08-01 23:36:17.000000 yesqa-1.4.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-02 00:03:51.874245 yesqa-1.4.0/yesqa.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2187 2022-08-02 00:03:51.000000 yesqa-1.4.0/yesqa.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      221 2022-08-02 00:03:51.000000 yesqa-1.4.0/yesqa.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-08-02 00:03:51.000000 yesqa-1.4.0/yesqa.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2022-08-02 00:03:51.000000 yesqa-1.4.0/yesqa.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2022-08-02 00:03:51.000000 yesqa-1.4.0/yesqa.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        6 2022-08-02 00:03:51.000000 yesqa-1.4.0/yesqa.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5213 2022-08-02 00:03:50.000000 yesqa-1.4.0/yesqa.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:33:04.931297 yesqa-1.5.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:29:14.000000 yesqa-1.5.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1742 2023-06-10 20:33:04.931297 yesqa-1.5.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1135 2023-06-10 20:33:04.000000 yesqa-1.5.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1130 2023-06-10 20:33:04.931297 yesqa-1.5.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:29:14.000000 yesqa-1.5.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:33:04.927297 yesqa-1.5.0/yesqa.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1742 2023-06-10 20:33:04.000000 yesqa-1.5.0/yesqa.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      221 2023-06-10 20:33:04.000000 yesqa-1.5.0/yesqa.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 20:33:04.000000 yesqa-1.5.0/yesqa.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2023-06-10 20:33:04.000000 yesqa-1.5.0/yesqa.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       29 2023-06-10 20:33:04.000000 yesqa-1.5.0/yesqa.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        6 2023-06-10 20:33:04.000000 yesqa-1.5.0/yesqa.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5213 2023-06-10 20:29:14.000000 yesqa-1.5.0/yesqa.py
```

### Comparing `yesqa-1.4.0/LICENSE` & `yesqa-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yesqa-1.4.0/PKG-INFO` & `yesqa-1.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 Metadata-Version: 2.1
 Name: yesqa
-Version: 1.4.0
+Version: 1.5.0
 Summary: Automatically remove unnecessary `# noqa` comments.
 Home-page: https://github.com/asottile/yesqa
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.yesqa?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=53&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/53/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=53&branchName=main)
+[![build status](https://github.com/asottile/yesqa/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/yesqa/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/yesqa/main.svg)](https://results.pre-commit.ci/latest/github/asottile/yesqa/main)
 
 yesqa
 =====
 
 A tool (and pre-commit hook) to automatically remove unnecessary `# noqa`
 comments, for example: a check that's no longer applicable (say you increased your
 max line length), a mistake (`# noqa` added to a line that wasn't failing),
 or other code in the file caused it to no longer need a `# noqa` (such as an unused import).
 
 ## Installation
 
-`pip install yesqa`
+```bash
+pip install yesqa
+```
 
 
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
     -   id: yesqa
 ```
 
 If you need to select a specific version of flake8 and/or run with specific
 flake8 plugins, add them to [`additional_dependencies`][0].
 
 [0]: http://pre-commit.com/#pre-commit-configyaml---hooks
-
-
```

### Comparing `yesqa-1.4.0/README.md` & `yesqa-1.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.yesqa?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=53&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/53/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=53&branchName=main)
+[![build status](https://github.com/asottile/yesqa/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/yesqa/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/yesqa/main.svg)](https://results.pre-commit.ci/latest/github/asottile/yesqa/main)
 
 yesqa
 =====
 
 A tool (and pre-commit hook) to automatically remove unnecessary `# noqa`
 comments, for example: a check that's no longer applicable (say you increased your
 max line length), a mistake (`# noqa` added to a line that wasn't failing),
 or other code in the file caused it to no longer need a `# noqa` (such as an unused import).
 
 ## Installation
 
-`pip install yesqa`
+```bash
+pip install yesqa
+```
 
 
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
     -   id: yesqa
 ```
 
 If you need to select a specific version of flake8 and/or run with specific
 flake8 plugins, add them to [`additional_dependencies`][0].
```

### Comparing `yesqa-1.4.0/setup.cfg` & `yesqa-1.5.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 [metadata]
 name = yesqa
-version = 1.4.0
+version = 1.5.0
 description = Automatically remove unnecessary `# noqa` comments.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/yesqa
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = yesqa
 install_requires = 
 	flake8>=3.9
 	tokenize-rt>=2.1
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	yesqa = yesqa:main
 
 [bdist_wheel]
 universal = True
@@ -38,15 +34,14 @@
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

### Comparing `yesqa-1.4.0/yesqa.egg-info/PKG-INFO` & `yesqa-1.5.0/yesqa.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 Metadata-Version: 2.1
 Name: yesqa
-Version: 1.4.0
+Version: 1.5.0
 Summary: Automatically remove unnecessary `# noqa` comments.
 Home-page: https://github.com/asottile/yesqa
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.yesqa?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=53&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/53/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=53&branchName=main)
+[![build status](https://github.com/asottile/yesqa/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/yesqa/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/yesqa/main.svg)](https://results.pre-commit.ci/latest/github/asottile/yesqa/main)
 
 yesqa
 =====
 
 A tool (and pre-commit hook) to automatically remove unnecessary `# noqa`
 comments, for example: a check that's no longer applicable (say you increased your
 max line length), a mistake (`# noqa` added to a line that wasn't failing),
 or other code in the file caused it to no longer need a `# noqa` (such as an unused import).
 
 ## Installation
 
-`pip install yesqa`
+```bash
+pip install yesqa
+```
 
 
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
     -   id: yesqa
 ```
 
 If you need to select a specific version of flake8 and/or run with specific
 flake8 plugins, add them to [`additional_dependencies`][0].
 
 [0]: http://pre-commit.com/#pre-commit-configyaml---hooks
-
-
```

### Comparing `yesqa-1.4.0/yesqa.py` & `yesqa-1.5.0/yesqa.py`

 * *Files identical despite different names*


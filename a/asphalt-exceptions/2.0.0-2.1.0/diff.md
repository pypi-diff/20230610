# Comparing `tmp/asphalt-exceptions-2.0.0.tar.gz` & `tmp/asphalt-exceptions-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asphalt-exceptions-2.0.0.tar", last modified: Mon May 16 20:46:05 2022, max compression
+gzip compressed data, was "asphalt-exceptions-2.1.0.tar", last modified: Sat Jun 10 17:57:11 2023, max compression
```

## Comparing `asphalt-exceptions-2.0.0.tar` & `asphalt-exceptions-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.435852 asphalt-exceptions-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.435852 asphalt-exceptions-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.435852 asphalt-exceptions-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/modules/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/modules/component.rst
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/modules/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/docs/modules/reporters/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/modules/reporters/raygun.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/modules/reporters/sentry.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.435852 asphalt-exceptions-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.435852 asphalt-exceptions-2.0.0/src/asphalt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/src/asphalt/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/src/asphalt/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/src/asphalt/exceptions/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3831 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/src/asphalt/exceptions/component.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/src/asphalt/exceptions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/src/asphalt/exceptions/reporters/
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/src/asphalt/exceptions/reporters/raygun.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/src/asphalt/exceptions/reporters/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-05-16 20:46:04.000000 asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-05-16 20:46:05.000000 asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-16 20:46:04.000000 asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-05-16 20:46:05.000000 asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-05-16 20:46:05.000000 asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-16 20:46:05.000000 asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 20:46:05.439852 asphalt-exceptions-2.0.0/tests/reporters/
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/tests/reporters/test_raygun.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/tests/reporters/test_sentry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-05-16 20:45:52.000000 asphalt-exceptions-2.0.0/tests/test_report_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.298842 asphalt-exceptions-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.290841 asphalt-exceptions-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-10 17:57:11.298842 asphalt-exceptions-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/modules/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/modules/component.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/modules/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/docs/modules/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/modules/reporters/raygun.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/modules/reporters/sentry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:57:11.298842 asphalt-exceptions-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.290841 asphalt-exceptions-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.290841 asphalt-exceptions-2.1.0/src/asphalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/src/asphalt/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/src/asphalt/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/src/asphalt/exceptions/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/src/asphalt/exceptions/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/src/asphalt/exceptions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/src/asphalt/exceptions/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/src/asphalt/exceptions/reporters/raygun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/src/asphalt/exceptions/reporters/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-10 17:57:11.000000 asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-10 17:57:11.000000 asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:57:11.000000 asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-10 17:57:11.000000 asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-10 17:57:11.000000 asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 17:57:11.000000 asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:57:11.294842 asphalt-exceptions-2.1.0/tests/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/tests/reporters/test_raygun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/tests/reporters/test_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-10 17:56:57.000000 asphalt-exceptions-2.1.0/tests/test_report_exception.py
```

### Comparing `asphalt-exceptions-2.0.0/.pre-commit-config.yaml` & `asphalt-exceptions-2.1.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,33 @@
 # This is the configuration file for pre-commit (https://pre-commit.com/).
 # To use:
 # * Install pre-commit (https://pre-commit.com/#installation)
 # * Copy this file as ".pre-commit-config.yaml"
 # * Run "pre-commit install".
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.1
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.272
     hooks:
-      - id: pyupgrade
-        args: [ "--py37-plus", "--keep-runtime-typing" ]
+      - id: ruff
+        args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-
-  - repo: https://github.com/csachs/pyproject-flake8
-    rev: v0.0.1a4
-    hooks:
-      - id: pyproject-flake8
-
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.950
+    rev: v1.3.0
     hooks:
       - id: mypy
-
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
-    hooks:
-      - id: python-check-blanket-noqa
-      - id: python-check-blanket-type-ignore
-      - id: python-no-eval
-      - id: rst-backticks
-      - id: rst-directive-colons
-      - id: rst-inline-touching-normal
+        additional_dependencies: ["pytest"]
```

### Comparing `asphalt-exceptions-2.0.0/LICENSE` & `asphalt-exceptions-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/PKG-INFO` & `asphalt-exceptions-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: asphalt-exceptions
-Version: 2.0.0
+Version: 2.1.0
 Summary: Exception reporter component for the Asphalt framework
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/asphalt-framework/asphalt-exceptions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: sentry
 Provides-Extra: raygun
 License-File: LICENSE
```

### Comparing `asphalt-exceptions-2.0.0/README.rst` & `asphalt-exceptions-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/docs/conf.py` & `asphalt-exceptions-2.1.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 from packaging.version import parse
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.extlinks",
     "sphinx_autodoc_typehints",
-    "sphinxcontrib.asyncio",
 ]
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "asphalt-exceptions"
 author = "Alex Grönholm"
 copyright = "2017, " + author
 
 v = parse(version(project))
 version = v.base_version
 release = v.public
 
-language = None
+language = "en"
 
 exclude_patterns = ["_build"]
 pygments_style = "sphinx"
 highlight_language = "python3"
 todo_include_todos = False
 
 html_theme = "sphinx_rtd_theme"
```

### Comparing `asphalt-exceptions-2.0.0/docs/configuration.rst` & `asphalt-exceptions-2.1.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/docs/extending.rst` & `asphalt-exceptions-2.1.0/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/docs/usage.rst` & `asphalt-exceptions-2.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/pyproject.toml` & `asphalt-exceptions-2.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 [build-system]
 requires = [
-    "setuptools >= 61",
-    "wheel >= 0.29.0",
-    "setuptools_scm[toml] >= 3.4"
+    "setuptools >= 64",
+    "setuptools_scm >= 6.4"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asphalt-exceptions"
 description = "Exception reporter component for the Asphalt framework"
 readme = "README.rst"
 authors = [{name = "Alex Grönholm", email = "alex.gronholm@nextday.fi"}]
 license = {text = "Apache License 2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
+requires-python = ">=3.7"
 dependencies = [
     "asphalt ~= 4.6",
-    "typeguard ~= 2.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/asphalt-framework/asphalt-exceptions"
 
 [project.optional-dependencies]
 test = [
+    "asphalt-exceptions[sentry,raygun]",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
 ]
 doc = [
+    "asphalt-exceptions[sentry,raygun]",
     "Sphinx >= 1.5",
     "sphinx_rtd_theme",
     "sphinx-autodoc-typehints >= 1.2.0",
     "sphinxcontrib-asyncio >= 0.2.0",
 ]
 sentry = ["sentry-sdk >= 1.5"]
 raygun = ["raygun4py >= 4.3"]
@@ -56,21 +59,26 @@
 sentry = "asphalt.exceptions.reporters.sentry:SentryExceptionReporter"
 raygun = "asphalt.exceptions.reporters.raygun:RaygunExceptionReporter"
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
-[tool.isort]
-src_paths = ["src"]
-skip_gitignore = true
-profile = "black"
+[tool.ruff]
+line-length = 99
+select = [
+    "E", "F", "W",  # default flake-8
+    "I",            # isort
+    "PGH",          # pygrep-hooks
+    "UP",           # pyupgrade
+]
+target-version = "py37"
 
-[tool.flake8]
-max-line-length = 99
+[tool.ruff.isort]
+known-first-party = ["asphalt.exceptions"]
 
 [tool.pytest.ini_options]
 addopts = "-rsx --tb=short"
 asyncio_mode = "strict"
 testpaths = ["tests"]
 
 [tool.mypy]
@@ -84,23 +92,21 @@
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37, py38, py39, py310, py311, pypy3
+envlist = py37, py38, py39, py310, py311, py312, pypy3
 skip_missing_interpreters = true
-isolated_build = true
+minversion = 4.4.3
 
 [testenv]
 extras = test
-    sentry
-    raygun
 commands = python -m pytest {posargs}
+package = editable
 
 [testenv:docs]
 extras = doc
-    sentry
-    raygun
 commands = sphinx-build docs build/sphinx
+package = editable
 """
```

### Comparing `asphalt-exceptions-2.0.0/src/asphalt/exceptions/__init__.py` & `asphalt-exceptions-2.1.0/src/asphalt/exceptions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 module_logger = logging.getLogger(__name__)
 
 
 def report_exception(
     ctx: Context,
     message: str,
-    exception: BaseException = None,
+    exception: BaseException | None = None,
     *,
     logger: logging.Logger | str | bool = True,
 ) -> None:
     """
     Report an exception to all exception reporters in the given context (and optionally log it too)
 
     :param ctx: context object to use for adding tags and other contextual information to the
```

### Comparing `asphalt-exceptions-2.0.0/src/asphalt/exceptions/api.py` & `asphalt-exceptions-2.1.0/src/asphalt/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/src/asphalt/exceptions/component.py` & `asphalt-exceptions-2.1.0/src/asphalt/exceptions/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 import logging
-from asyncio import AbstractEventLoop
+from asyncio import AbstractEventLoop, get_running_loop
 from functools import partial
-from typing import Any, AsyncIterator, Dict, Optional
+from typing import Any, AsyncIterator
 
 from asphalt.core import (
     Component,
     Context,
     PluginContainer,
     context_teardown,
     merge_config,
     qualified_name,
 )
-from typeguard import check_argument_types
 
 from asphalt.exceptions import report_exception
 from asphalt.exceptions.api import ExceptionReporter
 
 reporter_backends = PluginContainer("asphalt.exceptions.reporters", ExceptionReporter)
 logger = logging.getLogger(__name__)
 
@@ -58,19 +57,18 @@
     :param install_default_handler: ``True`` to install a new default exception handler for the
         event loop when the component starts
     :param default_args: default values for constructor keyword arguments
     """
 
     def __init__(
         self,
-        reporters: Dict[str, Optional[Dict[str, Any]]] = None,
+        reporters: dict[str, dict[str, Any] | None] | None = None,
         install_default_handler: bool = True,
         **default_args,
     ) -> None:
-        check_argument_types()
         self.install_default_handler = install_default_handler
         if not reporters:
             reporters = {"default": default_args}
 
         self.reporters: list[tuple] = []
         for resource_name, config in reporters.items():
             merged_config = merge_config(default_args, config or {})
@@ -87,14 +85,14 @@
                 "Configured exception reporter (%s; class=%s)",
                 resource_name,
                 qualified_name(reporter),
             )
 
         if self.install_default_handler:
             handler = partial(default_exception_handler, ctx=ctx)
-            ctx.loop.set_exception_handler(handler)
+            get_running_loop().set_exception_handler(handler)
             logger.info("Installed default event loop exception handler")
 
             yield
 
-            ctx.loop.set_exception_handler(None)
+            get_running_loop().set_exception_handler(None)
             logger.info("Uninstalled default event loop exception handler")
```

### Comparing `asphalt-exceptions-2.0.0/src/asphalt/exceptions/reporters/raygun.py` & `asphalt-exceptions-2.1.0/src/asphalt/exceptions/reporters/raygun.py`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/src/asphalt/exceptions/reporters/sentry.py` & `asphalt-exceptions-2.1.0/src/asphalt/exceptions/reporters/sentry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import logging
-from typing import Any, Dict, Sequence, Union
+from typing import Any, Sequence
 
 import sentry_sdk
 from asphalt.core import Context, resolve_reference
 from sentry_sdk.integrations import Integration
-from typeguard import check_argument_types
 
 from asphalt.exceptions.api import ExceptionReporter
 
 logger = logging.getLogger(__name__)
 
 
 class SentryExceptionReporter(ExceptionReporter):
@@ -37,17 +36,16 @@
     For more information, see the `Sentry SDK documentation`_.
 
     .. _Sentry: https://sentry.io/
     .. _Sentry SDK documentation: https://docs.sentry.io/platforms/python/
     """
 
     def __init__(
-        self, integrations: Sequence[Union[Integration, Dict[str, Any]]] = (), **options
+        self, integrations: Sequence[Integration | dict[str, Any]] = (), **options
     ) -> None:
-        check_argument_types()
         options.setdefault("environment", "development" if __debug__ else "production")
 
         integrations_: list[Integration] = []
         for integration in integrations:
             if isinstance(integration, dict):
                 integration_class = resolve_reference(integration["type"])
                 integration = integration_class(
```

### Comparing `asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/PKG-INFO` & `asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: asphalt-exceptions
-Version: 2.0.0
+Version: 2.1.0
 Summary: Exception reporter component for the Asphalt framework
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/asphalt-framework/asphalt-exceptions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: sentry
 Provides-Extra: raygun
 License-File: LICENSE
```

### Comparing `asphalt-exceptions-2.0.0/src/asphalt_exceptions.egg-info/SOURCES.txt` & `asphalt-exceptions-2.1.0/src/asphalt_exceptions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/conf.py
 docs/configuration.rst
 docs/extending.rst
 docs/index.rst
 docs/usage.rst
```

### Comparing `asphalt-exceptions-2.0.0/tests/reporters/test_raygun.py` & `asphalt-exceptions-2.1.0/tests/reporters/test_raygun.py`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/tests/reporters/test_sentry.py` & `asphalt-exceptions-2.1.0/tests/reporters/test_sentry.py`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/tests/test_component.py` & `asphalt-exceptions-2.1.0/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `asphalt-exceptions-2.0.0/tests/test_report_exception.py` & `asphalt-exceptions-2.1.0/tests/test_report_exception.py`

 * *Files identical despite different names*


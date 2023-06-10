# Comparing `tmp/hyperfast_python_template-0.8.6.tar.gz` & `tmp/hyperfast_python_template-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.8.6.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.8.7.tar", max compression
```

## Comparing `hyperfast_python_template-0.8.6.tar` & `hyperfast_python_template-0.8.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-06-09 23:36:57.366561 hyperfast_python_template-0.8.6/LICENSE
--rw-r--r--   0        0        0     5518 2023-06-09 23:36:57.366561 hyperfast_python_template-0.8.6/README.md
--rw-r--r--   0        0        0     2991 2023-06-09 23:37:12.162742 hyperfast_python_template-0.8.6/pyproject.toml
--rw-r--r--   0        0        0      323 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-06-09 23:37:12.106742 hyperfast_python_template-0.8.6/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-06-09 23:37:12.110741 hyperfast_python_template-0.8.6/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     6184 1970-01-01 00:00:00.000000 hyperfast_python_template-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-10 05:27:52.129438 hyperfast_python_template-0.8.7/LICENSE
+-rw-r--r--   0        0        0     5756 2023-06-10 05:27:52.129438 hyperfast_python_template-0.8.7/README.md
+-rw-r--r--   0        0        0     2991 2023-06-10 05:28:07.761412 hyperfast_python_template-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-06-10 05:27:52.133438 hyperfast_python_template-0.8.7/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-06-10 05:27:52.133438 hyperfast_python_template-0.8.7/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-10 05:28:07.709412 hyperfast_python_template-0.8.7/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-06-10 05:28:07.713412 hyperfast_python_template-0.8.7/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-06-10 05:27:52.133438 hyperfast_python_template-0.8.7/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-06-10 05:27:52.133438 hyperfast_python_template-0.8.7/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-06-10 05:27:52.133438 hyperfast_python_template-0.8.7/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     6422 1970-01-01 00:00:00.000000 hyperfast_python_template-0.8.7/PKG-INFO
```

### Comparing `hyperfast_python_template-0.8.6/LICENSE` & `hyperfast_python_template-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.8.6/README.md` & `hyperfast_python_template-0.8.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Hyperfast Python Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![jupyter-book-image]][docs-url]
+[![codecov][codecov-image]][codecov-url]
 
 <!-- Links: -->
 
+[codecov-image]: https://codecov.io/gh/entelecheia/hyperfast-python-template/branch/main/graph/badge.svg?token=29NXUNQUBU
+[codecov-url]: https://codecov.io/gh/entelecheia/hyperfast-python-template
 [pypi-image]: https://img.shields.io/pypi/v/hyperfast-python-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyperfast-python-template
 [license-url]: https://github.com/entelecheia/hyperfast-python-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyperfast-python-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyperfast-python-template
 [release-url]: https://github.com/entelecheia/hyperfast-python-template/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```

### Comparing `hyperfast_python_template-0.8.6/pyproject.toml` & `hyperfast_python_template-0.8.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.8.6"
+version = "0.8.7"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.8.6/PKG-INFO` & `hyperfast_python_template-0.8.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.8.6
+Version: 0.8.7
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -18,17 +18,20 @@
 # Hyperfast Python Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![jupyter-book-image]][docs-url]
+[![codecov][codecov-image]][codecov-url]
 
 <!-- Links: -->
 
+[codecov-image]: https://codecov.io/gh/entelecheia/hyperfast-python-template/branch/main/graph/badge.svg?token=29NXUNQUBU
+[codecov-url]: https://codecov.io/gh/entelecheia/hyperfast-python-template
 [pypi-image]: https://img.shields.io/pypi/v/hyperfast-python-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyperfast-python-template
 [license-url]: https://github.com/entelecheia/hyperfast-python-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyperfast-python-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyperfast-python-template
 [release-url]: https://github.com/entelecheia/hyperfast-python-template/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
```


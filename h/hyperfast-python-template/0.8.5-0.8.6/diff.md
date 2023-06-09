# Comparing `tmp/hyperfast_python_template-0.8.5.tar.gz` & `tmp/hyperfast_python_template-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.8.5.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.8.6.tar", max compression
```

## Comparing `hyperfast_python_template-0.8.5.tar` & `hyperfast_python_template-0.8.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-06-07 05:34:22.244173 hyperfast_python_template-0.8.5/LICENSE
--rw-r--r--   0        0        0     5518 2023-06-07 05:34:22.244173 hyperfast_python_template-0.8.5/README.md
--rw-r--r--   0        0        0     2991 2023-06-07 05:34:38.928588 hyperfast_python_template-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      323 2023-06-07 05:34:22.248173 hyperfast_python_template-0.8.5/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-06-07 05:34:22.248173 hyperfast_python_template-0.8.5/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-06-07 05:34:38.876587 hyperfast_python_template-0.8.5/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-06-07 05:34:38.876587 hyperfast_python_template-0.8.5/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-06-07 05:34:22.248173 hyperfast_python_template-0.8.5/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-06-07 05:34:22.248173 hyperfast_python_template-0.8.5/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-06-07 05:34:22.248173 hyperfast_python_template-0.8.5/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     6184 1970-01-01 00:00:00.000000 hyperfast_python_template-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-09 23:36:57.366561 hyperfast_python_template-0.8.6/LICENSE
+-rw-r--r--   0        0        0     5518 2023-06-09 23:36:57.366561 hyperfast_python_template-0.8.6/README.md
+-rw-r--r--   0        0        0     2991 2023-06-09 23:37:12.162742 hyperfast_python_template-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-09 23:37:12.106742 hyperfast_python_template-0.8.6/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-06-09 23:37:12.110741 hyperfast_python_template-0.8.6/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-06-09 23:36:57.370561 hyperfast_python_template-0.8.6/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     6184 1970-01-01 00:00:00.000000 hyperfast_python_template-0.8.6/PKG-INFO
```

### Comparing `hyperfast_python_template-0.8.5/LICENSE` & `hyperfast_python_template-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.8.5/README.md` & `hyperfast_python_template-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.8.5/pyproject.toml` & `hyperfast_python_template-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.8.5"
+version = "0.8.6"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.8.5/PKG-INFO` & `hyperfast_python_template-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.8.5
+Version: 0.8.6
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```


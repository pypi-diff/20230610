# Comparing `tmp/jsonschema_spec-0.1.4.tar.gz` & `tmp/jsonschema_spec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_spec-0.1.4.tar", max compression
+gzip compressed data, was "jsonschema_spec-0.1.5.tar", max compression
```

## Comparing `jsonschema_spec-0.1.4.tar` & `jsonschema_spec-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/LICENSE
--rw-r--r--   0        0        0     3123 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/README.rst
--rw-r--r--   0        0        0      301 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/__init__.py
--rw-r--r--   0        0        0     1362 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/accessors.py
--rw-r--r--   0        0        0      761 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/handlers/__init__.py
--rw-r--r--   0        0        0     1557 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/handlers/file.py
--rw-r--r--   0        0        0      395 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/handlers/protocols.py
--rw-r--r--   0        0        0      747 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/handlers/requests.py
--rw-r--r--   0        0        0      587 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/handlers/urllib.py
--rw-r--r--   0        0        0      361 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/handlers/utils.py
--rw-r--r--   0        0        0     1392 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/loaders.py
--rw-r--r--   0        0        0     1559 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/paths.py
--rw-r--r--   0        0        0        0 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/py.typed
--rw-r--r--   0        0        0     1082 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/readers.py
--rw-r--r--   0        0        0      247 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/jsonschema_spec/utils.py
--rw-r--r--   0        0        0     1797 2023-03-17 05:21:28.565620 jsonschema_spec-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 jsonschema_spec-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3123 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/README.rst
+-rw-r--r--   0        0        0      301 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/__init__.py
+-rw-r--r--   0        0        0     1362 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/accessors.py
+-rw-r--r--   0        0        0      761 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/__init__.py
+-rw-r--r--   0        0        0     1557 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/file.py
+-rw-r--r--   0        0        0      395 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/protocols.py
+-rw-r--r--   0        0        0      747 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/requests.py
+-rw-r--r--   0        0        0      587 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/urllib.py
+-rw-r--r--   0        0        0      361 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/handlers/utils.py
+-rw-r--r--   0        0        0     1392 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/loaders.py
+-rw-r--r--   0        0        0     1559 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/paths.py
+-rw-r--r--   0        0        0        0 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/py.typed
+-rw-r--r--   0        0        0     1082 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/readers.py
+-rw-r--r--   0        0        0      247 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/jsonschema_spec/utils.py
+-rw-r--r--   0        0        0     2001 2023-06-10 19:10:38.652299 jsonschema_spec-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4359 1970-01-01 00:00:00.000000 jsonschema_spec-0.1.5/PKG-INFO
```

### Comparing `jsonschema_spec-0.1.4/LICENSE` & `jsonschema_spec-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/README.rst` & `jsonschema_spec-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/accessors.py` & `jsonschema_spec-0.1.5/jsonschema_spec/accessors.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/handlers/__init__.py` & `jsonschema_spec-0.1.5/jsonschema_spec/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/handlers/file.py` & `jsonschema_spec-0.1.5/jsonschema_spec/handlers/file.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/handlers/requests.py` & `jsonschema_spec-0.1.5/jsonschema_spec/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/handlers/urllib.py` & `jsonschema_spec-0.1.5/jsonschema_spec/handlers/urllib.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/loaders.py` & `jsonschema_spec-0.1.5/jsonschema_spec/loaders.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/paths.py` & `jsonschema_spec-0.1.5/jsonschema_spec/paths.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/jsonschema_spec/readers.py` & `jsonschema_spec-0.1.5/jsonschema_spec/readers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.4/pyproject.toml` & `jsonschema_spec-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [[tool.mypy.overrides]]
 module = "jsonschema.validators"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "jsonschema-spec"
-version = "0.1.4"
+version = "0.1.5"
 description = "JSONSchema Spec with object-oriented paths"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/p1c2u/jsonschema-spec"
 keywords = ["jsonschema", "swagger", "spec"]
 classifiers = [
@@ -32,35 +32,38 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
 ]
 
 [tool.poetry.dependencies]
 jsonschema = ">=4.0.0,<4.18.0"
 pathable = "^0.4.1"
 python = "^3.7.0"
 PyYAML = ">=5.1"
-typing-extensions = "^4.3.0"
+typing-extensions = "<4.6.0" # See https://github.com/p1c2u/jsonschema-spec/issues/14
+requests = {version = "^2.31.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
-pytest = "^6.2.5"
-pytest-flake8 = "=1.0.7"
-pytest-cov = "^3.0.0"
+pytest = "^7.3.1"
+pytest-flake8 = "=1.1.0"
+pytest-cov = "^4.1.0"
 isort = "^5.0.0"
-black = "^22.0.0"
+black = "^23.3.0"
 flynt = "0.76"
 mypy = "^0.971"
 types-PyYAML = "^6.0.11"
 types-requests = "^2.28.9"
+deptry = { version = "^0.11.0", python = ">=3.8" }
 
 [tool.pytest.ini_options]
 addopts = """
 --capture=no
 --verbose
 --showlocals
 --junitxml=reports/junit.xml
```

### Comparing `jsonschema_spec-0.1.4/PKG-INFO` & `jsonschema_spec-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-spec
-Version: 0.1.4
+Version: 0.1.5
 Summary: JSONSchema Spec with object-oriented paths
 Home-page: https://github.com/p1c2u/jsonschema-spec
 License: Apache-2.0
 Keywords: jsonschema,swagger,spec
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -14,25 +14,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=5.1)
 Requires-Dist: jsonschema (>=4.0.0,<4.18.0)
 Requires-Dist: pathable (>=0.4.1,<0.5.0)
-Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: typing-extensions (<4.6.0)
 Project-URL: Repository, https://github.com/p1c2u/jsonschema-spec
 Description-Content-Type: text/x-rst
 
 ***************
 JSONSchema Spec
 ***************
```


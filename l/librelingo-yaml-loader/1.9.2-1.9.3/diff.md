# Comparing `tmp/librelingo_yaml_loader-1.9.2.tar.gz` & `tmp/librelingo_yaml_loader-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librelingo_yaml_loader-1.9.2.tar", max compression
+gzip compressed data, was "librelingo_yaml_loader-1.9.3.tar", max compression
```

## Comparing `librelingo_yaml_loader-1.9.2.tar` & `librelingo_yaml_loader-1.9.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      261 2022-01-23 17:55:20.661482 librelingo_yaml_loader-1.9.2/README.md
--rw-r--r--   0        0        0      188 2021-11-03 21:41:09.706314 librelingo_yaml_loader-1.9.2/librelingo_yaml_loader/__init__.py
--rw-r--r--   0        0        0     3302 2022-01-22 15:27:02.153034 librelingo_yaml_loader-1.9.2/librelingo_yaml_loader/_spelling.py
--rw-r--r--   0        0        0    14016 2022-01-22 15:27:02.163034 librelingo_yaml_loader-1.9.2/librelingo_yaml_loader/yaml_loader.py
--rw-r--r--   0        0        0      851 2022-01-29 17:14:21.828106 librelingo_yaml_loader-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     1290 2022-01-29 17:14:29.431332 librelingo_yaml_loader-1.9.2/setup.py
--rw-r--r--   0        0        0     1200 2022-01-29 17:14:29.431526 librelingo_yaml_loader-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0      261 2022-01-23 17:55:20.661482 librelingo_yaml_loader-1.9.3/README.md
+-rw-r--r--   0        0        0      188 2021-11-03 21:41:09.706314 librelingo_yaml_loader-1.9.3/librelingo_yaml_loader/__init__.py
+-rw-r--r--   0        0        0     3302 2022-01-22 15:27:02.153034 librelingo_yaml_loader-1.9.3/librelingo_yaml_loader/_spelling.py
+-rw-r--r--   0        0        0    14016 2022-01-22 15:27:02.163034 librelingo_yaml_loader-1.9.3/librelingo_yaml_loader/yaml_loader.py
+-rw-r--r--   0        0        0      851 2022-01-30 09:24:34.501918 librelingo_yaml_loader-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1290 2022-01-30 09:24:45.699948 librelingo_yaml_loader-1.9.3/setup.py
+-rw-r--r--   0        0        0     1200 2022-01-30 09:24:45.700142 librelingo_yaml_loader-1.9.3/PKG-INFO
```

### Comparing `librelingo_yaml_loader-1.9.2/librelingo_yaml_loader/_spelling.py` & `librelingo_yaml_loader-1.9.3/librelingo_yaml_loader/_spelling.py`

 * *Files identical despite different names*

### Comparing `librelingo_yaml_loader-1.9.2/librelingo_yaml_loader/yaml_loader.py` & `librelingo_yaml_loader-1.9.3/librelingo_yaml_loader/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `librelingo_yaml_loader-1.9.2/pyproject.toml` & `librelingo_yaml_loader-1.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "librelingo_yaml_loader"
-version = "1.9.2"  # Do not edit before merge to 'main'
+version = "1.9.3"  # Do not edit before merge to 'main'
 description = "Load YAML-based LibreLingo courses in your Python project."
 authors = ["Dániel Kántor <git@daniel-kantor.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyfakefs = "^4.3.3"
 pyyaml = "^5.3.1"
 snapshottest = "^0.6.0"
-click = "^8.0.0"
+click = "^7.0.0"
 librelingo-types = "^3.3.0"
 Markdown = "^3.3.4"
 html2markdown = "^0.1.7"
 bleach = "^4.0.0"
 bleach-whitelist = "^0.0.11"
 hunspell = { version = "^0.5.5", optional = true }
```

### Comparing `librelingo_yaml_loader-1.9.2/setup.py` & `librelingo_yaml_loader-1.9.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Markdown>=3.3.4,<4.0.0',
  'bleach-whitelist>=0.0.11,<0.0.12',
  'bleach>=4.0.0,<5.0.0',
- 'click>=8.0.0,<9.0.0',
+ 'click>=7.0.0,<8.0.0',
  'html2markdown>=0.1.7,<0.2.0',
  'librelingo-types>=3.3.0,<4.0.0',
  'pyfakefs>=4.3.3,<5.0.0',
  'pyyaml>=5.3.1,<6.0.0',
  'snapshottest>=0.6.0,<0.7.0']
 
 extras_require = \
 {'hunspell': ['hunspell>=0.5.5,<0.6.0']}
 
 setup_kwargs = {
     'name': 'librelingo-yaml-loader',
-    'version': '1.9.2',
+    'version': '1.9.3',
     'description': 'Load YAML-based LibreLingo courses in your Python project.',
     'long_description': '<a id="librelingo_yaml_loader.yaml_loader"></a>\n\n# librelingo\\_yaml\\_loader.yaml\\_loader\n\n<a id="librelingo_yaml_loader.yaml_loader.load_course"></a>\n\n#### load\\_course\n\n```python\ndef load_course(path: str)\n```\n\nLoad a YAML-based course into a Course() object\n\n',
     'author': 'Dániel Kántor',
     'author_email': 'git@daniel-kantor.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `librelingo_yaml_loader-1.9.2/PKG-INFO` & `librelingo_yaml_loader-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: librelingo-yaml-loader
-Version: 1.9.2
+Version: 1.9.3
 Summary: Load YAML-based LibreLingo courses in your Python project.
 Author: Dániel Kántor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: hunspell
 Requires-Dist: Markdown (>=3.3.4,<4.0.0)
 Requires-Dist: bleach (>=4.0.0,<5.0.0)
 Requires-Dist: bleach-whitelist (>=0.0.11,<0.0.12)
-Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: click (>=7.0.0,<8.0.0)
 Requires-Dist: html2markdown (>=0.1.7,<0.2.0)
 Requires-Dist: hunspell (>=0.5.5,<0.6.0); extra == "hunspell"
 Requires-Dist: librelingo-types (>=3.3.0,<4.0.0)
 Requires-Dist: pyfakefs (>=4.3.3,<5.0.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
 Requires-Dist: snapshottest (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
```


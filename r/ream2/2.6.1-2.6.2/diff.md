# Comparing `tmp/ream2-2.6.1.tar.gz` & `tmp/ream2-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.6.1.tar", max compression
+gzip compressed data, was "ream2-2.6.2.tar", max compression
```

## Comparing `ream2-2.6.1.tar` & `ream2-2.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-06-07 23:26:17.540756 ream2-2.6.1/LICENSE
--rw-r--r--   0        0        0     5267 2023-06-07 23:26:17.540756 ream2-2.6.1/README.md
--rw-r--r--   0        0        0      752 2023-06-07 23:26:17.540756 ream2-2.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/__init__.py
--rw-r--r--   0        0        0    13032 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actor_graph.py
--rw-r--r--   0        0        0     2197 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actor_version.py
--rw-r--r--   0        0        0        0 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/__init__.py
--rw-r--r--   0        0        0     3815 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/base.py
--rw-r--r--   0        0        0     1155 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/dsid.py
--rw-r--r--   0        0        0      976 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/enum.py
--rw-r--r--   0        0        0      363 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/interface.py
--rw-r--r--   0        0        0    37569 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/cli_helper.py
--rw-r--r--   0        0        0    34210 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/data_model_helper.py
--rw-r--r--   0        0        0    14434 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/dataset_helper.py
--rw-r--r--   0        0        0     9838 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/fs.py
--rw-r--r--   0        0        0     6636 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/helper.py
--rw-r--r--   0        0        0     5684 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/params_helper.py
--rw-r--r--   0        0        0     1090 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/prelude.py
--rw-r--r--   0        0        0     2248 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/workspace.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-10 04:15:44.178252 ream2-2.6.2/LICENSE
+-rw-r--r--   0        0        0     5267 2023-06-10 04:15:44.178252 ream2-2.6.2/README.md
+-rw-r--r--   0        0        0      763 2023-06-10 04:15:44.178252 ream2-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/__init__.py
+-rw-r--r--   0        0        0    13032 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actor_graph.py
+-rw-r--r--   0        0        0     2197 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/__init__.py
+-rw-r--r--   0        0        0     3815 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/base.py
+-rw-r--r--   0        0        0     1155 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/dsid.py
+-rw-r--r--   0        0        0      976 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/actors/interface.py
+-rw-r--r--   0        0        0    37569 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/cli_helper.py
+-rw-r--r--   0        0        0    34210 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/data_model_helper.py
+-rw-r--r--   0        0        0    14434 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/dataset_helper.py
+-rw-r--r--   0        0        0     9838 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/helper.py
+-rw-r--r--   0        0        0     5684 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/params_helper.py
+-rw-r--r--   0        0        0     1090 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/prelude.py
+-rw-r--r--   0        0        0     2248 2023-06-10 04:15:44.178252 ream2-2.6.2/ream/workspace.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.6.2/PKG-INFO
```

### Comparing `ream2-2.6.1/LICENSE` & `ream2-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/README.md` & `ream2-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/pyproject.toml` & `ream2-2.6.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.6.1"
+version = "2.6.2"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
@@ -14,15 +14,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 t2-yada = "^1.2.0"
 timer4 = ">= 1.0.4, < 2.0.0"
 loguru = "^0.6.0"
 graph-wrapper = "^1.5.0"
 filelock = "^3.8.0"
-orjson = "^3.8.2"
+orjson = ">= 3.9.0, < 4.0.0"
 python-slugify = "^6.1.2"
 serde2 = "^1.6.0"
 hugedict = "^2.9.2"
 pyarrow = "^11.0.0"
 nptyping = "^2.5.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `ream2-2.6.1/ream/actor_graph.py` & `ream2-2.6.2/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/actor_state.py` & `ream2-2.6.2/ream/actor_state.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/actor_version.py` & `ream2-2.6.2/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/actors/base.py` & `ream2-2.6.2/ream/actors/base.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/actors/dsid.py` & `ream2-2.6.2/ream/actors/dsid.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/actors/enum.py` & `ream2-2.6.2/ream/actors/enum.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/cache_helper.py` & `ream2-2.6.2/ream/cache_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/cli_helper.py` & `ream2-2.6.2/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/data_model_helper.py` & `ream2-2.6.2/ream/data_model_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/dataset_helper.py` & `ream2-2.6.2/ream/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/fs.py` & `ream2-2.6.2/ream/fs.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/helper.py` & `ream2-2.6.2/ream/helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/params_helper.py` & `ream2-2.6.2/ream/params_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/prelude.py` & `ream2-2.6.2/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/ream/workspace.py` & `ream2-2.6.2/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.1/PKG-INFO` & `ream2-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 2.6.1
+Version: 2.6.2
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: filelock (>=3.8.0,<4.0.0)
 Requires-Dist: graph-wrapper (>=1.5.0,<2.0.0)
 Requires-Dist: hugedict (>=2.9.2,<3.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
-Requires-Dist: orjson (>=3.8.2,<4.0.0)
+Requires-Dist: orjson (>=3.9.0,<4.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
 Requires-Dist: serde2 (>=1.6.0,<2.0.0)
 Requires-Dist: t2-yada (>=1.2.0,<2.0.0)
 Requires-Dist: timer4 (>=1.0.4,<2.0.0)
 Project-URL: Repository, https://github.com/binh-vu/ream
 Description-Content-Type: text/markdown
```


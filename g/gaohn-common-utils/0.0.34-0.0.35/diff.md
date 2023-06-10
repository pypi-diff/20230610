# Comparing `tmp/gaohn-common-utils-0.0.34.tar.gz` & `tmp/gaohn-common-utils-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.34.tar", last modified: Fri Jun  9 07:54:07 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.35.tar", last modified: Sat Jun 10 09:13:31 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.34.tar` & `gaohn-common-utils-0.0.35.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.476327 gaohn-common-utils-0.0.34/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 07:54:07.476327 gaohn-common-utils-0.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.472327 gaohn-common-utils-0.0.34/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.472327 gaohn-common-utils-0.0.34/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.472327 gaohn-common-utils-0.0.34/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.476327 gaohn-common-utils-0.0.34/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.476327 gaohn-common-utils-0.0.34/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.472327 gaohn-common-utils-0.0.34/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.476327 gaohn-common-utils-0.0.34/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:54:07.476327 gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 07:54:07.000000 gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 07:54:07.000000 gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:54:07.000000 gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 07:54:07.000000 gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 07:54:07.000000 gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 07:53:37.000000 gaohn-common-utils-0.0.34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:54:07.476327 gaohn-common-utils-0.0.34/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.297543 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.297543 gaohn-common-utils-0.0.35/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 09:13:31.000000 gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-10 09:13:09.000000 gaohn-common-utils-0.0.35/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:13:31.301543 gaohn-common-utils-0.0.35/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.34/LICENSE` & `gaohn-common-utils-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/PKG-INFO` & `gaohn-common-utils-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.34
+Version: 0.0.35
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.34/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.35/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.35/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.35/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/common_utils/core/common.py` & `gaohn-common-utils-0.0.35/common_utils/core/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This module contains common utility functions for various purposes.
 """
 import json
 import logging
 import os
 import random
+import uuid
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import numpy as np
 import rich
 import torch
 import yaml
@@ -79,14 +80,25 @@
 
     def load_to_dict(self, filepath: str, **kwargs: Dict[str, Any]) -> Dict[str, Any]:
         with open(filepath, "r", encoding="utf-8") as f:
             data = yaml.load(f, Loader=FullLoader, **kwargs)
         return data
 
 
+def generate_uuid() -> str:
+    """Generate a UUID.
+
+    Returns
+    -------
+    str
+        UUID1 as a string.
+    """
+    return str(uuid.uuid1())
+
+
 def seed_all(seed: Optional[int] = 1992, seed_torch: bool = True) -> None:
     """
     Seed all random number generators.
 
     Parameters
     ----------
     seed : int, optional
```

### Comparing `gaohn-common-utils-0.0.34/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.35/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.35/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/common_utils/core/logger.py` & `gaohn-common-utils-0.0.35/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.35/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.34
+Version: 0.0.35
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.34/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.35/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 common_utils/core/__init__.py
 common_utils/core/artifacts.py
 common_utils/core/base.py
 common_utils/core/common.py
 common_utils/core/decorators.py
 common_utils/core/file_system_utils.py
 common_utils/core/logger.py
+common_utils/orchestrator/base.py
 common_utils/versioning/dvc/base.py
 gaohn_common_utils.egg-info/PKG-INFO
 gaohn_common_utils.egg-info/SOURCES.txt
 gaohn_common_utils.egg-info/dependency_links.txt
 gaohn_common_utils.egg-info/requires.txt
 gaohn_common_utils.egg-info/top_level.txt
```

### Comparing `gaohn-common-utils-0.0.34/pyproject.toml` & `gaohn-common-utils-0.0.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.34"
+version = "0.0.35"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


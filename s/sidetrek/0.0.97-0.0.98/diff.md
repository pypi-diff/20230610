# Comparing `tmp/sidetrek-0.0.97.tar.gz` & `tmp/sidetrek-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.97.tar", max compression
+gzip compressed data, was "sidetrek-0.0.98.tar", max compression
```

## Comparing `sidetrek-0.0.97.tar` & `sidetrek-0.0.98.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.97/README.md
--rw-r--r--   0        0        0      747 2023-06-09 22:28:04.485901 sidetrek-0.0.97/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.97/sidetrek/__init__.py
--rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.97/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.97/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.97/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.97/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     4836 2023-06-09 02:10:49.422608 sidetrek-0.0.97/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.97/sidetrek/collect_env.py
--rw-r--r--   0        0        0       80 2023-06-05 14:27:08.634241 sidetrek-0.0.97/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.97/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.97/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.97/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0     3007 2023-06-08 15:16:50.143147 sidetrek-0.0.97/sidetrek/global_fns.py
--rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.97/sidetrek/helpers.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.97/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.97/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.97/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.97/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.98/README.md
+-rw-r--r--   0        0        0      747 2023-06-10 02:30:13.484032 sidetrek-0.0.98/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.98/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.98/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.98/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.98/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.98/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.98/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.98/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.98/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.98/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     4836 2023-06-09 02:10:49.422608 sidetrek-0.0.98/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.98/sidetrek/collect_env.py
+-rw-r--r--   0        0        0      127 2023-06-10 02:16:10.111028 sidetrek-0.0.98/sidetrek/constants.py
+-rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.98/sidetrek/datapipes.py
+-rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.98/sidetrek/dataset.py
+-rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.98/sidetrek/flyte/__init__.py
+-rw-r--r--   0        0        0     3050 2023-06-10 02:16:49.060748 sidetrek-0.0.98/sidetrek/global_fns.py
+-rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.98/sidetrek/helpers.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.98/sidetrek/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.98/sidetrek/types/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.98/sidetrek/types/dataset.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.98/PKG-INFO
```

### Comparing `sidetrek-0.0.97/pyproject.toml` & `sidetrek-0.0.98/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.97"
+version = "0.0.98"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
```

### Comparing `sidetrek-0.0.97/sidetrek/__init__.py` & `sidetrek-0.0.98/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/cli.py` & `sidetrek-0.0.98/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.98/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.98/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.98/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.98/sidetrek/cli_commands/workflow.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/collect_env.py` & `sidetrek-0.0.98/sidetrek/collect_env.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/datapipes.py` & `sidetrek-0.0.98/sidetrek/datapipes.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/dataset.py` & `sidetrek-0.0.98/sidetrek/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/global_fns.py` & `sidetrek-0.0.98/sidetrek/global_fns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from sidetrek.constants import USER_REPO_DATA_DIRNAME, USER_DATA_BUCKET
+from sidetrek.constants import USER_DATA_S3_BUCKET, GENERATED_SIDETREK_DIRNAME
 from typing import Any, Optional, Dict
 from s3fs import S3FileSystem
 import cloudpickle
 import flytekit
 from sidetrek.helpers import get_flyte_exec_id
 
 
@@ -39,15 +39,15 @@
     # Construct bucket prefix
     flyte_exec_ctx = flytekit.current_context()
     flyte_exec_id = flyte_exec_ctx.execution_id.name
     user_prefix = test_prefix if test_prefix is not None else flyte_exec_id
     bucket_prefix = f"/custom_objects/{user_prefix}"
 
     s3 = S3FileSystem(anon=False)
-    with s3.open(f"{USER_DATA_BUCKET}{bucket_prefix}/{key}", "wb") as f:
+    with s3.open(f"{USER_DATA_S3_BUCKET}{bucket_prefix}/{key}", "wb") as f:
         f.write(pickled_val)
 
 
 def load_custom_objects(bentoml_model_tag: str, key: str, test_prefix: Optional[str]) -> Dict[str, Any]:
     """
     Load cloudpickle serialized python code from save_custom_objects
     - bentoml_model_tag: bentoml model tag
@@ -55,18 +55,18 @@
     - test_prefix: ONLY used for testing - if provided in save_custom_objects, must be supplied here (overrides bentoml_model_tag)
     """
     # Get bucket prefix
     user_prefix = test_prefix if test_prefix is not None else get_flyte_exec_id(bentoml_model_tag)
     # bucket_prefix = f"/custom_objects/{user_prefix}"
 
     # s3 = S3FileSystem(anon=False)
-    # with s3.open(f"{USER_DATA_BUCKET}{bucket_prefix}/{key}", "rb") as f:
+    # with s3.open(f"{USER_DATA_S3_BUCKET}{bucket_prefix}/{key}", "rb") as f:
     #     pickled_val = f.read()
     #     val = cloudpickle.loads(pickled_val)
     #     return val
 
     # Load the custom_objects locally (saved locally from s3 during model build)
-    custom_objects_local_path = Path.cwd() / "src/custom_objects" / f"{user_prefix}.cpkl"
+    custom_objects_local_path = Path.cwd() / f"src/{GENERATED_SIDETREK_DIRNAME}/custom_objects" / f"{user_prefix}.cpkl"
     with open(custom_objects_local_path, "rb") as f:
         pickled_val = f.read()
         val = cloudpickle.loads(pickled_val)
         return val
```

### Comparing `sidetrek-0.0.97/sidetrek/helpers.py` & `sidetrek-0.0.98/sidetrek/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/loggers.py` & `sidetrek-0.0.98/sidetrek/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/sidetrek/types/dataset.py` & `sidetrek-0.0.98/sidetrek/types/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.97/PKG-INFO` & `sidetrek-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.97
+Version: 0.0.98
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


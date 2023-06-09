# Comparing `tmp/sidetrek-0.0.96.tar.gz` & `tmp/sidetrek-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.96.tar", max compression
+gzip compressed data, was "sidetrek-0.0.97.tar", max compression
```

## Comparing `sidetrek-0.0.96.tar` & `sidetrek-0.0.97.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.96/README.md
--rw-r--r--   0        0        0      661 2023-06-06 02:32:02.301541 sidetrek-0.0.96/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.96/sidetrek/__init__.py
--rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.96/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.96/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.96/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.96/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.96/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.96/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.96/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.96/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     4811 2023-05-29 16:57:11.110851 sidetrek-0.0.96/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.96/sidetrek/collect_env.py
--rw-r--r--   0        0        0       80 2023-06-05 14:27:08.634241 sidetrek-0.0.96/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.96/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.96/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.96/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0     2675 2023-06-06 02:31:59.005199 sidetrek-0.0.96/sidetrek/global_fns.py
--rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.96/sidetrek/helpers.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.96/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.96/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.96/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.96/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.97/README.md
+-rw-r--r--   0        0        0      747 2023-06-09 22:28:04.485901 sidetrek-0.0.97/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.97/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.97/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.97/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0    12711 2023-05-29 16:56:31.562946 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     3485 2023-05-29 16:57:15.777556 sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.97/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0    14143 2023-05-29 16:58:01.660580 sidetrek-0.0.97/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     4836 2023-06-09 02:10:49.422608 sidetrek-0.0.97/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.97/sidetrek/collect_env.py
+-rw-r--r--   0        0        0       80 2023-06-05 14:27:08.634241 sidetrek-0.0.97/sidetrek/constants.py
+-rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.97/sidetrek/datapipes.py
+-rw-r--r--   0        0        0     4354 2023-05-27 15:54:43.543881 sidetrek-0.0.97/sidetrek/dataset.py
+-rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.97/sidetrek/flyte/__init__.py
+-rw-r--r--   0        0        0     3007 2023-06-08 15:16:50.143147 sidetrek-0.0.97/sidetrek/global_fns.py
+-rw-r--r--   0        0        0      923 2023-06-05 21:50:39.414912 sidetrek-0.0.97/sidetrek/helpers.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.97/sidetrek/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.97/sidetrek/types/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.97/sidetrek/types/dataset.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sidetrek-0.0.97/PKG-INFO
```

### Comparing `sidetrek-0.0.96/pyproject.toml` & `sidetrek-0.0.97/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.96"
+version = "0.0.97"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
@@ -12,15 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 typer = {extras = ["all"], version = "^0.7.0"}
 requests = "^2.28.2"
 pylint = "^2.17.0"
 torchdata = "^0.6.0"
 fsspec = "^2023.4.0"
-s3fs = "^2023.4.0"
+s3fs = "^2023.4.0,<2023.6.0" # must pin below 2023.6.0 for now because of flytekit's gcsfs pinned at 5.0
 bentoml = "^1.0.20"
 mlflow = "^2.3.2"
 flytekit = "^1.6.1"
 aiohttp = "^3.8.4"
 cloudpickle = "^2.2.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `sidetrek-0.0.96/sidetrek/__init__.py` & `sidetrek-0.0.97/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/cli.py` & `sidetrek-0.0.97/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.97/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.97/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.97/sidetrek/cli_commands/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,29 +59,30 @@
         print("generated_local_sidetrek_dir_path", get_generated_local_sidetrek_dir_path())
 
         # Get current user
         auth_step = progress.add_task(description="Authenticating...", total=None)
         current_user = get_current_user()
         print(f"current_user={current_user}")
 
-        # Get aws credentials and set it as env var for execution (grants temporary local s3 access for datasets)
+        # Get temporary aws credentials and set it as env var for execution (grants temporary local s3 access for datasets)
         aws_creds = get_aws_creds()
         if aws_creds is None:
             raise Exception("Failed to get aws credentials")
         aws_env = {**os.environ, "AWS_ACCESS_KEY_ID": aws_creds["AccessKeyId"], "AWS_SECRET_ACCESS_KEY": aws_creds["SecretKey"], "AWS_SESSION_TOKEN": aws_creds["SessionToken"]}
 
         progress.remove_task(auth_step)
         time_elapsed = round(time.time() - start_time, 2)
         print(f"[green]✔️ [white]Authenticated [grey89]({time_elapsed}s)")
 
         # Always use the draft version for testing
         wf_generation_step = progress.add_task(description="Generating the workflow...", total=None)
         workflow_version = get_workflow_draft_version(workflow_id=workflow_id)
         # print(f"workflow_version={workflow_version}")
 
+        # TODO
         # Check dataset auth - i.e. make sure this user has access to the dataset they're trying to access
         wf_ui = json.loads(workflow_version["ui"])
         dataset_ids = [node.get("data", {}).get("datasetId") for node in wf_ui["nodes"] if node["type"] == "dataset"]
         ds_collab_roles = await get_dataset_collaborator_roles(dataset_ids)
         print(f"ds_collab_roles={ds_collab_roles}")
 
         return
```

### Comparing `sidetrek-0.0.96/sidetrek/collect_env.py` & `sidetrek-0.0.97/sidetrek/collect_env.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/datapipes.py` & `sidetrek-0.0.97/sidetrek/datapipes.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/dataset.py` & `sidetrek-0.0.97/sidetrek/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/global_fns.py` & `sidetrek-0.0.97/sidetrek/global_fns.py`

 * *Files 24% similar despite different names*

```diff
@@ -52,14 +52,21 @@
     Load cloudpickle serialized python code from save_custom_objects
     - bentoml_model_tag: bentoml model tag
     - key: unique key for custom_objects
     - test_prefix: ONLY used for testing - if provided in save_custom_objects, must be supplied here (overrides bentoml_model_tag)
     """
     # Get bucket prefix
     user_prefix = test_prefix if test_prefix is not None else get_flyte_exec_id(bentoml_model_tag)
-    bucket_prefix = f"/custom_objects/{user_prefix}"
+    # bucket_prefix = f"/custom_objects/{user_prefix}"
 
-    s3 = S3FileSystem(anon=False)
-    with s3.open(f"{USER_DATA_BUCKET}{bucket_prefix}/{key}", "rb") as f:
+    # s3 = S3FileSystem(anon=False)
+    # with s3.open(f"{USER_DATA_BUCKET}{bucket_prefix}/{key}", "rb") as f:
+    #     pickled_val = f.read()
+    #     val = cloudpickle.loads(pickled_val)
+    #     return val
+
+    # Load the custom_objects locally (saved locally from s3 during model build)
+    custom_objects_local_path = Path.cwd() / "src/custom_objects" / f"{user_prefix}.cpkl"
+    with open(custom_objects_local_path, "rb") as f:
         pickled_val = f.read()
         val = cloudpickle.loads(pickled_val)
         return val
```

### Comparing `sidetrek-0.0.96/sidetrek/helpers.py` & `sidetrek-0.0.97/sidetrek/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/loggers.py` & `sidetrek-0.0.97/sidetrek/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/sidetrek/types/dataset.py` & `sidetrek-0.0.97/sidetrek/types/dataset.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.96/PKG-INFO` & `sidetrek-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.96
+Version: 0.0.97
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 Requires-Dist: bentoml (>=1.0.20,<2.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: flytekit (>=1.6.1,<2.0.0)
 Requires-Dist: fsspec (>=2023.4.0,<2024.0.0)
 Requires-Dist: mlflow (>=2.3.2,<3.0.0)
 Requires-Dist: pylint (>=2.17.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: s3fs (>=2023.4.0,<2024.0.0)
+Requires-Dist: s3fs (>=2023.4.0,<2023.6.0)
 Requires-Dist: torchdata (>=0.6.0,<0.7.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Sidetrek Python SDK/CLI
```


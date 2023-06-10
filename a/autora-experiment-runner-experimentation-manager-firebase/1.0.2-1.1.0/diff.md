# Comparing `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.2.tar.gz` & `tmp/autora-experiment-runner-experimentation-manager-firebase-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.2.tar", last modified: Mon Jun  5 15:20:13 2023, max compression
+gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.1.0.tar", last modified: Sat Jun 10 17:17:39 2023, max compression
```

## Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2.tar` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/SweetPea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/firebase/
--rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.957672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 15:20:13.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:13.961672 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 15:20:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/test_experimentation_manager_firebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.148324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-10 17:17:39.148324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/docs/SweetPea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:17:39.148324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora/experiment_runner/experimentation_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.144324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora/experiment_runner/experimentation_manager/firebase/
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.148324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-10 17:17:39.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-10 17:17:39.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:17:39.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-10 17:17:39.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 17:17:39.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:39.148324 autora-experiment-runner-experimentation-manager-firebase-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-10 17:17:21.000000 autora-experiment-runner-experimentation-manager-firebase-1.1.0/tests/test_experimentation_manager_firebase.py
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/.github/workflows/python-publish.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/.gitignore` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/.pre-commit-config.yaml` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.2
+Version: 1.1.0
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observations between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/docs/SweetPea.ipynb` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/docs/SweetPea.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/mkdocs/base.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/pyproject.toml` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import warnings
 
 import firebase_admin
 from firebase_admin import credentials, firestore
 import json
 
+
 def _sequence_to_db_object(iterable, save=False):
     """
     Helper function to convert an array into a dictionary for a database
     Args:
         iterable: an iterable
 
     Returns:
@@ -36,15 +37,17 @@
     for t in iterable:
         is_int64 = is_int64 or isinstance(t, np.int64)
         is_float64 = is_float64 or isinstance(t, np.float64)
     if is_int64:
         warnings.warn('Converting np.int64 to int to store in Firestore, may loose precision')
     if is_float64:
         warnings.warn('Converting np.float64 to float to store in Firestore, may loose precision')
-    return {i: int(t) if isinstance(t, np.integer) else float(t) if isinstance(t, np.floating) else t if isinstance(t, dict) else json.dumps(t) for i, t in enumerate(iterable)}
+    return {i: int(t) if isinstance(t, np.integer) else float(t) if isinstance(t, np.floating) else t if isinstance(t,
+                                                                                                                    dict) else json.dumps(
+        t) for i, t in enumerate(iterable)}
 
 
 def _get_collection(
         collection_name: str,
         firebase_credentials: dict
 ):
     """
@@ -310,24 +313,25 @@
     for doc in docs:
         observations.update(doc.reference.get().to_dict())
     firebase_admin.delete_app(app)
     return observations
 
 
 def check_firebase_status(
-        collection_name: str, firebase_credentials: dict, time_out: int
+        collection_name: str, firebase_credentials: dict, time_out: int, pids_aborted: list = []
 ) -> str:
     """
     check the status of the condition
 
     Args:
         collection_name: name of the collection as given in firebase
         firebase_credentials: credentials for firebase
         time_out: time out for participants that started the condition
             but didn't finish (after this time spots are freed)
+        pids_aborted: a list of personal ids that aborted the experiment (free the places)
 
     Returns:
         Can have three different outcomes:
             (1) available -> no action needed, recruitment should be started (if paused)
             (2) finished -> collection of observations is finished
             (3) unavailable -> all conditions are running, recruitment should be paused
     """
@@ -349,18 +353,21 @@
         # return available if there are conditions that haven't been started
         if value["start_time"] is None:
             available = True
         else:
             if not value["finished"]:
                 unix_time_seconds = int(time.time())
                 time_from_started = unix_time_seconds - value["start_time"]
+                is_aborted = False
+                if "pId" in value:
+                    is_aborted = value['pId'] in pids_aborted
                 # check weather the started condition has timed out, if so, reset start_time and
                 # set available True
-                if time_from_started > time_out:
-                    doc_ref_meta.update({key: {"start_time": None, "finished": False}})
+                if time_from_started > time_out or is_aborted:
+                    doc_ref_meta.update({key: {"start_time": None, "finished": False, "pId": None}})
                     available = True
                 else:
                     finished = False
     firebase_admin.delete_app(app)
     if available:
         return 'available'
     if finished:
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.2
+Version: 1.1.0
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observations between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.2/tests/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.1.0/tests/README.md`

 * *Files identical despite different names*


# Comparing `tmp/pylovens-0.1.0.tar.gz` & `tmp/pylovens-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylovens-0.1.0.tar", last modified: Fri Jun  2 12:00:08 2023, max compression
+gzip compressed data, was "pylovens-0.2.0.tar", last modified: Sat Jun 10 07:32:07 2023, max compression
```

## Comparing `pylovens-0.1.0.tar` & `pylovens-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:00:08.627731 pylovens-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:00:08.627731 pylovens-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:00:08.627731 pylovens-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 11:59:59.000000 pylovens-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-02 11:59:59.000000 pylovens-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-02 11:59:59.000000 pylovens-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 11:59:59.000000 pylovens-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-02 12:00:08.627731 pylovens-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-02 11:59:59.000000 pylovens-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-02 11:59:59.000000 pylovens-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 12:00:08.627731 pylovens-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:00:08.627731 pylovens-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:00:08.627731 pylovens-0.1.0/src/pylovens/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 11:59:59.000000 pylovens-0.1.0/src/pylovens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 12:00:08.000000 pylovens-0.1.0/src/pylovens/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-06-02 11:59:59.000000 pylovens-0.1.0/src/pylovens/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 11:59:59.000000 pylovens-0.1.0/src/pylovens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:00:08.627731 pylovens-0.1.0/src/pylovens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-02 12:00:08.000000 pylovens-0.1.0/src/pylovens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-02 12:00:08.000000 pylovens-0.1.0/src/pylovens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:00:08.000000 pylovens-0.1.0/src/pylovens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 12:00:08.000000 pylovens-0.1.0/src/pylovens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 12:00:08.000000 pylovens-0.1.0/src/pylovens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:00:08.627731 pylovens-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-02 11:59:59.000000 pylovens-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-02 11:59:59.000000 pylovens-0.1.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-10 07:31:58.000000 pylovens-0.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-10 07:31:58.000000 pylovens-0.2.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-10 07:31:58.000000 pylovens-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-10 07:31:58.000000 pylovens-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-10 07:32:07.899435 pylovens-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-10 07:31:58.000000 pylovens-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-10 07:31:58.000000 pylovens-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 07:32:07.903435 pylovens-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/src/pylovens/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-10 07:31:58.000000 pylovens-0.2.0/src/pylovens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26398 2023-06-10 07:31:58.000000 pylovens-0.2.0/src/pylovens/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/src/pylovens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 07:31:58.000000 pylovens-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12094 2023-06-10 07:31:58.000000 pylovens-0.2.0/tests/test_client.py
```

### Comparing `pylovens-0.1.0/.github/workflows/publish.yaml` & `pylovens-0.2.0/.github/workflows/publish.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     timeout-minutes: 10
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.x"
 
       - name: Build
```

### Comparing `pylovens-0.1.0/.gitignore` & `pylovens-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pylovens-0.1.0/LICENSE` & `pylovens-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylovens-0.1.0/pyproject.toml` & `pylovens-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylovens-0.1.0/tests/conftest.py` & `pylovens-0.2.0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from os import environ
 
 from pytest import fixture, mark
 
 from pylovens import LovensClient
 
 
@@ -17,7 +18,13 @@
     return client
 
 
 @fixture(scope="session")
 def bike_id(authenticated_client: LovensClient) -> int:
     bikes = authenticated_client.get_bikes()
     return bikes[0]["id"]
+
+
+@fixture(scope="session")
+def ride(authenticated_client: LovensClient, bike_id: int) -> dict:
+    for ride in authenticated_client.iterate_rides(bike_id):
+        return ride
```


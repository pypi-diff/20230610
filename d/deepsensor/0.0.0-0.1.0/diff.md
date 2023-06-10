# Comparing `tmp/deepsensor-0.0.0.tar.gz` & `tmp/deepsensor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsensor-0.0.0.tar", last modified: Sat Jun 10 14:43:15 2023, max compression
+gzip compressed data, was "deepsensor-0.1.0.tar", last modified: Sat Jun 10 14:43:15 2023, max compression
```

## Comparing `deepsensor-0.0.0.tar` & `deepsensor-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.467128 deepsensor-0.0.0/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     1076 2023-05-16 13:27:41.000000 deepsensor-0.0.0/LICENSE
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4960 2023-06-10 14:43:15.467128 deepsensor-0.0.0/PKG-INFO
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4563 2023-06-10 14:36:02.000000 deepsensor-0.0.0/README.md
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      329 2023-05-24 13:52:11.000000 deepsensor-0.0.0/deepsensor/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/active_learning/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-19 14:49:00.000000 deepsensor-0.0.0/deepsensor/active_learning/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8772 2023-05-22 14:39:54.000000 deepsensor-0.0.0/deepsensor/active_learning/acquisition_fns.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      170 2023-06-09 15:07:15.000000 deepsensor-0.0.0/deepsensor/config.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/data/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.0.0/deepsensor/data/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    22102 2023-06-07 17:20:41.000000 deepsensor-0.0.0/deepsensor/data/loader.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    14246 2023-06-09 15:07:15.000000 deepsensor-0.0.0/deepsensor/data/processor.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3509 2023-05-31 22:34:31.000000 deepsensor-0.0.0/deepsensor/data/task.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3717 2023-06-07 17:20:41.000000 deepsensor-0.0.0/deepsensor/data/utils.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/model/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.0.0/deepsensor/model/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     2704 2023-06-07 17:20:41.000000 deepsensor-0.0.0/deepsensor/model/defaults.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    28006 2023-06-10 13:53:55.000000 deepsensor-0.0.0/deepsensor/model/models.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8046 2023-06-10 13:48:53.000000 deepsensor-0.0.0/deepsensor/model/nps.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/plot/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.0.0/deepsensor/plot/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     6091 2023-05-31 22:34:31.000000 deepsensor-0.0.0/deepsensor/plot/utils.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 14:47:21.000000 deepsensor-0.0.0/deepsensor/py.typed
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/tensorflow/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      826 2023-06-09 15:07:15.000000 deepsensor-0.0.0/deepsensor/tensorflow/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/torch/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      788 2023-06-09 15:03:43.000000 deepsensor-0.0.0/deepsensor/torch/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor/train/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-06 13:04:03.000000 deepsensor-0.0.0/deepsensor/train/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3770 2023-06-09 17:05:13.000000 deepsensor-0.0.0/deepsensor/train/train.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-17 10:49:11.000000 deepsensor-0.0.0/deepsensor/utils.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.463128 deepsensor-0.0.0/deepsensor.egg-info/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4960 2023-06-10 14:43:15.000000 deepsensor-0.0.0/deepsensor.egg-info/PKG-INFO
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      942 2023-06-10 14:43:15.000000 deepsensor-0.0.0/deepsensor.egg-info/SOURCES.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 14:43:15.000000 deepsensor-0.0.0/deepsensor.egg-info/dependency_links.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 14:42:57.000000 deepsensor-0.0.0/deepsensor.egg-info/not-zip-safe
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      127 2023-06-10 14:43:15.000000 deepsensor-0.0.0/deepsensor.egg-info/requires.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)       17 2023-06-10 14:43:15.000000 deepsensor-0.0.0/deepsensor.egg-info/top_level.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      411 2023-06-05 14:42:05.000000 deepsensor-0.0.0/pyproject.toml
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      866 2023-06-10 14:43:15.467128 deepsensor-0.0.0/setup.cfg
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      446 2023-06-10 13:08:32.000000 deepsensor-0.0.0/setup.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.467128 deepsensor-0.0.0/tests/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 15:06:33.000000 deepsensor-0.0.0/tests/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     7896 2023-06-09 15:07:18.000000 deepsensor-0.0.0/tests/test_data_processor.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8740 2023-06-07 17:20:41.000000 deepsensor-0.0.0/tests/test_model.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     5845 2023-06-07 17:20:41.000000 deepsensor-0.0.0/tests/test_task_loader.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     2028 2023-06-08 17:10:45.000000 deepsensor-0.0.0/tests/utils.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.375126 deepsensor-0.1.0/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     1076 2023-05-16 13:27:41.000000 deepsensor-0.1.0/LICENSE
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     4960 2023-06-10 14:43:15.375126 deepsensor-0.1.0/PKG-INFO
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     4563 2023-06-10 14:36:02.000000 deepsensor-0.1.0/README.md
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.371126 deepsensor-0.1.0/deepsensor/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      329 2023-05-24 13:52:11.000000 deepsensor-0.1.0/deepsensor/__init__.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.371126 deepsensor-0.1.0/deepsensor/active_learning/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-19 14:49:00.000000 deepsensor-0.1.0/deepsensor/active_learning/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     8772 2023-05-22 14:39:54.000000 deepsensor-0.1.0/deepsensor/active_learning/acquisition_fns.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      170 2023-06-09 15:07:15.000000 deepsensor-0.1.0/deepsensor/config.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.371126 deepsensor-0.1.0/deepsensor/data/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.0/deepsensor/data/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)    22102 2023-06-07 17:20:41.000000 deepsensor-0.1.0/deepsensor/data/loader.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)    14246 2023-06-09 15:07:15.000000 deepsensor-0.1.0/deepsensor/data/processor.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     3509 2023-05-31 22:34:31.000000 deepsensor-0.1.0/deepsensor/data/task.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     3717 2023-06-07 17:20:41.000000 deepsensor-0.1.0/deepsensor/data/utils.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.375126 deepsensor-0.1.0/deepsensor/model/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.0/deepsensor/model/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     2704 2023-06-07 17:20:41.000000 deepsensor-0.1.0/deepsensor/model/defaults.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)    28006 2023-06-10 13:53:55.000000 deepsensor-0.1.0/deepsensor/model/models.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     8046 2023-06-10 13:48:53.000000 deepsensor-0.1.0/deepsensor/model/nps.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.375126 deepsensor-0.1.0/deepsensor/plot/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.0/deepsensor/plot/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     6091 2023-05-31 22:34:31.000000 deepsensor-0.1.0/deepsensor/plot/utils.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 14:47:21.000000 deepsensor-0.1.0/deepsensor/py.typed
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.375126 deepsensor-0.1.0/deepsensor/tensorflow/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      826 2023-06-09 15:07:15.000000 deepsensor-0.1.0/deepsensor/tensorflow/__init__.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.375126 deepsensor-0.1.0/deepsensor/torch/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      788 2023-06-09 15:03:43.000000 deepsensor-0.1.0/deepsensor/torch/__init__.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.375126 deepsensor-0.1.0/deepsensor/train/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-06 13:04:03.000000 deepsensor-0.1.0/deepsensor/train/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     3770 2023-06-09 17:05:13.000000 deepsensor-0.1.0/deepsensor/train/train.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-17 10:49:11.000000 deepsensor-0.1.0/deepsensor/utils.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.371126 deepsensor-0.1.0/deepsensor.egg-info/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     4960 2023-06-10 14:43:15.000000 deepsensor-0.1.0/deepsensor.egg-info/PKG-INFO
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      942 2023-06-10 14:43:15.000000 deepsensor-0.1.0/deepsensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 14:43:15.000000 deepsensor-0.1.0/deepsensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 14:42:57.000000 deepsensor-0.1.0/deepsensor.egg-info/not-zip-safe
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      121 2023-06-10 14:43:15.000000 deepsensor-0.1.0/deepsensor.egg-info/requires.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)       17 2023-06-10 14:43:15.000000 deepsensor-0.1.0/deepsensor.egg-info/top_level.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      411 2023-06-05 14:42:05.000000 deepsensor-0.1.0/pyproject.toml
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      866 2023-06-10 14:43:15.375126 deepsensor-0.1.0/setup.cfg
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      446 2023-06-10 13:08:32.000000 deepsensor-0.1.0/setup.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 14:43:15.375126 deepsensor-0.1.0/tests/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 15:06:33.000000 deepsensor-0.1.0/tests/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     7896 2023-06-09 15:07:18.000000 deepsensor-0.1.0/tests/test_data_processor.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     8740 2023-06-07 17:20:41.000000 deepsensor-0.1.0/tests/test_model.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     5845 2023-06-07 17:20:41.000000 deepsensor-0.1.0/tests/test_task_loader.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     2028 2023-06-08 17:10:45.000000 deepsensor-0.1.0/tests/utils.py
```

### Comparing `deepsensor-0.0.0/LICENSE` & `deepsensor-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/PKG-INFO` & `deepsensor-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.0.0
+Version: 0.1.0
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.0.0/README.md` & `deepsensor-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/active_learning/acquisition_fns.py` & `deepsensor-0.1.0/deepsensor/active_learning/acquisition_fns.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/data/loader.py` & `deepsensor-0.1.0/deepsensor/data/loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/data/processor.py` & `deepsensor-0.1.0/deepsensor/data/processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/data/task.py` & `deepsensor-0.1.0/deepsensor/data/task.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/data/utils.py` & `deepsensor-0.1.0/deepsensor/data/utils.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/model/defaults.py` & `deepsensor-0.1.0/deepsensor/model/defaults.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/model/models.py` & `deepsensor-0.1.0/deepsensor/model/models.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/model/nps.py` & `deepsensor-0.1.0/deepsensor/model/nps.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/plot/utils.py` & `deepsensor-0.1.0/deepsensor/plot/utils.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/tensorflow/__init__.py` & `deepsensor-0.1.0/deepsensor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/torch/__init__.py` & `deepsensor-0.1.0/deepsensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor/train/train.py` & `deepsensor-0.1.0/deepsensor/train/train.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/deepsensor.egg-info/PKG-INFO` & `deepsensor-0.1.0/deepsensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.0.0
+Version: 0.1.0
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.0.0/deepsensor.egg-info/SOURCES.txt` & `deepsensor-0.1.0/deepsensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/setup.cfg` & `deepsensor-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/tests/test_data_processor.py` & `deepsensor-0.1.0/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/tests/test_model.py` & `deepsensor-0.1.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/tests/test_task_loader.py` & `deepsensor-0.1.0/tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.0.0/tests/utils.py` & `deepsensor-0.1.0/tests/utils.py`

 * *Files identical despite different names*


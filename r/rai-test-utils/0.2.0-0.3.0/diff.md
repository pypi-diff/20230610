# Comparing `tmp/rai_test_utils-0.2.0.tar.gz` & `tmp/rai_test_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rai_test_utils-0.2.0.tar", last modified: Wed May 17 22:20:03 2023, max compression
+gzip compressed data, was "dist/rai_test_utils-0.3.0.tar", last modified: Sat Jun 10 05:19:13 2023, max compression
```

## Comparing `rai_test_utils-0.2.0.tar` & `rai_test_utils-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/tabular/tabular_data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/lightgbm/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/lightgbm/lightgbm_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/sklearn/sklearn_model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/xgboost/xgboost_model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/tests/test_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/datasets/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/datasets/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/datasets/tabular/classification_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/datasets/tabular/regression_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/datasets/tabular/timeseries_data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/models/lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/lightgbm/lightgbm_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/models/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/sklearn/sklearn_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/models/xgboost/xgboost_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/rai_test_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/rai_test_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 05:19:13.000000 rai_test_utils-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/tests/test_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-10 05:18:16.000000 rai_test_utils-0.3.0/tests/test_utils.py
```

### Comparing `rai_test_utils-0.2.0/LICENSE` & `rai_test_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/PKG-INFO` & `rai_test_utils-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai_test_utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Common basic test utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Gaurav Gupta
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `rai_test_utils-0.2.0/README.md` & `rai_test_utils-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/rai_test_utils/models/lightgbm/lightgbm_model_utils.py` & `rai_test_utils-0.3.0/rai_test_utils/models/lightgbm/lightgbm_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/rai_test_utils/models/model_utils.py` & `rai_test_utils-0.3.0/rai_test_utils/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/rai_test_utils/models/sklearn/__init__.py` & `rai_test_utils-0.3.0/rai_test_utils/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/rai_test_utils/models/sklearn/sklearn_model_utils.py` & `rai_test_utils-0.3.0/rai_test_utils/models/sklearn/sklearn_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/rai_test_utils/models/xgboost/xgboost_model_utils.py` & `rai_test_utils-0.3.0/rai_test_utils/models/xgboost/xgboost_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/rai_test_utils.egg-info/PKG-INFO` & `rai_test_utils-0.3.0/rai_test_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-test-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Common basic test utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Gaurav Gupta
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `rai_test_utils-0.2.0/rai_test_utils.egg-info/SOURCES.txt` & `rai_test_utils-0.3.0/rai_test_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 rai_test_utils.egg-info/PKG-INFO
 rai_test_utils.egg-info/SOURCES.txt
 rai_test_utils.egg-info/dependency_links.txt
 rai_test_utils.egg-info/requires.txt
 rai_test_utils.egg-info/top_level.txt
 rai_test_utils/datasets/__init__.py
 rai_test_utils/datasets/tabular/__init__.py
-rai_test_utils/datasets/tabular/tabular_data_utils.py
+rai_test_utils/datasets/tabular/classification_data_utils.py
+rai_test_utils/datasets/tabular/regression_data_utils.py
+rai_test_utils/datasets/tabular/timeseries_data_utils.py
 rai_test_utils/models/__init__.py
 rai_test_utils/models/model_utils.py
 rai_test_utils/models/lightgbm/__init__.py
 rai_test_utils/models/lightgbm/lightgbm_model_utils.py
 rai_test_utils/models/sklearn/__init__.py
 rai_test_utils/models/sklearn/sklearn_model_utils.py
 rai_test_utils/models/xgboost/__init__.py
```

### Comparing `rai_test_utils-0.2.0/setup.py` & `rai_test_utils-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/tests/test_data_utils.py` & `rai_test_utils-0.3.0/tests/test_data_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 import pytest
 
 from rai_test_utils.datasets.tabular import (
     create_adult_census_data, create_binary_classification_dataset,
-    create_cancer_data, create_diabetes_data, create_housing_data,
-    create_iris_data, create_simple_titanic_data, create_wine_data)
+    create_cancer_data, create_complex_titanic_data, create_diabetes_data,
+    create_energy_data, create_housing_data, create_iris_data, create_msx_data,
+    create_multiclass_classification_dataset, create_reviews_data,
+    create_simple_titanic_data, create_timeseries_data, create_wine_data)
 
 
 class TestDataUtils:
     @pytest.mark.parametrize('if_small_data', [True, False])
     def test_create_housing_data(self, if_small_data):
         X_train, X_test, y_train, y_test, feature_names = \
             create_housing_data(if_small_data)
@@ -85,7 +87,57 @@
         X_train, X_test, y_train, y_test, feature_names = \
             create_adult_census_data(string_labels)
         assert X_train is not None
         assert X_test is not None
         assert y_train is not None
         assert y_test is not None
         assert feature_names is not None
+
+    def test_create_timeseries_data(self):
+        X_train, y_train = create_timeseries_data(
+            sample_cnt_per_grain=10,
+            time_column_name='time',
+            target_column_name='target',
+        )
+        assert X_train is not None
+        assert y_train is not None
+
+    def test_create_msx_data(self):
+        X_train, X_test, y_train, y_test = \
+            create_msx_data(test_size=0.2)
+        assert X_train is not None
+        assert X_test is not None
+        assert y_train is not None
+        assert y_test is not None
+
+    def test_create_energy_data(self):
+        X_train, X_test, y_train, y_test, feature_names = \
+            create_energy_data()
+        assert X_train is not None
+        assert X_test is not None
+        assert y_train is not None
+        assert y_test is not None
+        assert feature_names is not None
+
+    def test_create_complex_titanic_data(self):
+        X_train, X_test, y_train, y_test = create_complex_titanic_data()
+        assert X_train is not None
+        assert X_test is not None
+        assert y_train is not None
+        assert y_test is not None
+
+    def test_create_multiclass_classification_dataset(self):
+        X_train, X_test, y_train, y_test, classes = \
+            create_multiclass_classification_dataset()
+        assert X_train is not None
+        assert X_test is not None
+        assert y_train is not None
+        assert y_test is not None
+        assert classes is not None
+
+    def test_create_reviews_data(self):
+        X_train, X_test, y_train, y_test = \
+            create_reviews_data(test_size=0.2)
+        assert X_train is not None
+        assert X_test is not None
+        assert y_train is not None
+        assert y_test is not None
```

### Comparing `rai_test_utils-0.2.0/tests/test_model_utils.py` & `rai_test_utils-0.3.0/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.2.0/tests/test_utils.py` & `rai_test_utils-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*


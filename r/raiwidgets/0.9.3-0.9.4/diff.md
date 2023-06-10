# Comparing `tmp/raiwidgets-0.9.3.tar.gz` & `tmp/raiwidgets-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/raiwidgets-0.9.3.tar", last modified: Tue Aug 17 20:08:15 2021, max compression
+gzip compressed data, was "dist/raiwidgets-0.9.4.tar", last modified: Wed Aug 18 22:18:07 2021, max compression
```

## Comparing `raiwidgets-0.9.3.tar` & `raiwidgets-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:15.000000 raiwidgets-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    22123 2021-08-17 20:08:15.000000 raiwidgets-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21414 2021-08-17 20:08:14.000000 raiwidgets-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:15.000000 raiwidgets-0.9.3/raiwidgets/
--rw-r--r--   0 runner    (1001) docker     (121)      658 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-17 20:02:44.000000 raiwidgets-0.9.3/raiwidgets/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8272 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4231 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/error_analysis_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6904 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/error_analysis_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    24400 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/error_analysis_dashboard_input.py
--rw-r--r--   0 runner    (1001) docker     (121)      239 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/explanation_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/explanation_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    13701 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/explanation_dashboard_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     5027 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/fairness_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     5880 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/fairness_metric_calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/model_analysis_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     5319 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/model_analysis_dashboard_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/raiwidgets/model_performance_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:15.000000 raiwidgets-0.9.3/raiwidgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22123 2021-08-17 20:08:14.000000 raiwidgets-0.9.3/raiwidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      809 2021-08-17 20:08:14.000000 raiwidgets-0.9.3/raiwidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-17 20:08:14.000000 raiwidgets-0.9.3/raiwidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-17 20:08:14.000000 raiwidgets-0.9.3/raiwidgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-08-17 20:08:14.000000 raiwidgets-0.9.3/raiwidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-17 20:08:14.000000 raiwidgets-0.9.3/raiwidgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-17 20:08:15.000000 raiwidgets-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-08-17 20:00:58.000000 raiwidgets-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    22123 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    21414 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets/
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-18 22:11:39.000000 raiwidgets-0.9.4/raiwidgets/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8272 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4231 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/error_analysis_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6904 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/error_analysis_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24400 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/error_analysis_dashboard_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/explanation_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/explanation_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13701 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/explanation_dashboard_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5027 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/fairness_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5880 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/fairness_metric_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2104 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/model_analysis_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5319 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/model_analysis_dashboard_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2336 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/raiwidgets/model_performance_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    22123 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/raiwidgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-18 22:18:07.000000 raiwidgets-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-08-18 22:09:44.000000 raiwidgets-0.9.4/setup.py
```

### Comparing `raiwidgets-0.9.3/PKG-INFO` & `raiwidgets-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raiwidgets
-Version: 0.9.3
+Version: 0.9.4
 Summary: Interactive visualizations to assess fairness, explain models, and analyze errors in Machine Learning
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `raiwidgets-0.9.3/README.md` & `raiwidgets-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/__init__.py` & `raiwidgets-0.9.4/raiwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/constants.py` & `raiwidgets-0.9.4/raiwidgets/constants.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/dashboard.py` & `raiwidgets-0.9.4/raiwidgets/dashboard.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/error_analysis_dashboard.py` & `raiwidgets-0.9.4/raiwidgets/error_analysis_dashboard.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/error_analysis_dashboard_input.py` & `raiwidgets-0.9.4/raiwidgets/error_analysis_dashboard_input.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/explanation_constants.py` & `raiwidgets-0.9.4/raiwidgets/explanation_constants.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/explanation_dashboard.py` & `raiwidgets-0.9.4/raiwidgets/explanation_dashboard.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/explanation_dashboard_input.py` & `raiwidgets-0.9.4/raiwidgets/explanation_dashboard_input.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/fairness_dashboard.py` & `raiwidgets-0.9.4/raiwidgets/fairness_dashboard.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/fairness_metric_calculation.py` & `raiwidgets-0.9.4/raiwidgets/fairness_metric_calculation.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/model_analysis_dashboard.py` & `raiwidgets-0.9.4/raiwidgets/model_analysis_dashboard.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/model_analysis_dashboard_input.py` & `raiwidgets-0.9.4/raiwidgets/model_analysis_dashboard_input.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets/model_performance_dashboard.py` & `raiwidgets-0.9.4/raiwidgets/model_performance_dashboard.py`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/raiwidgets.egg-info/PKG-INFO` & `raiwidgets-0.9.4/raiwidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raiwidgets
-Version: 0.9.3
+Version: 0.9.4
 Summary: Interactive visualizations to assess fairness, explain models, and analyze errors in Machine Learning
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `raiwidgets-0.9.3/raiwidgets.egg-info/SOURCES.txt` & `raiwidgets-0.9.4/raiwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raiwidgets-0.9.3/setup.py` & `raiwidgets-0.9.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/psense_common-0.4.8.tar.gz` & `tmp/psense_common-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psense_common-0.4.8.tar", last modified: Wed Jan 18 01:34:35 2023, max compression
+gzip compressed data, was "psense_common-0.4.9.tar", last modified: Fri Jan 20 18:05:27 2023, max compression
```

## Comparing `psense_common-0.4.8.tar` & `psense_common-0.4.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-18 01:34:35.523580 psense_common-0.4.8/
--rw-rw-rw-   0 root         (0) root         (0)     6973 2023-01-18 01:34:35.523580 psense_common-0.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6552 2023-01-18 01:34:26.000000 psense_common-0.4.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-18 01:34:35.519580 psense_common-0.4.8/psense_common/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-18 01:34:35.519580 psense_common-0.4.8/psense_common/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4099 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/analysis/calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     6894 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/analysis/excelwriter.py
--rw-rw-rw-   0 root         (0) root         (0)     9455 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/analysis/response.py
--rw-rw-rw-   0 root         (0) root         (0)     9696 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/kfilter.py
--rw-rw-rw-   0 root         (0) root         (0)    28456 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/psense_aws_itfc.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/psense_format.py
--rw-rw-rw-   0 root         (0) root         (0)    35257 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/psense_parser.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-18 01:34:26.000000 psense_common-0.4.8/psense_common/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-18 01:34:35.519580 psense_common-0.4.8/psense_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6973 2023-01-18 01:34:35.000000 psense_common-0.4.8/psense_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      728 2023-01-18 01:34:35.000000 psense_common-0.4.8/psense_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-18 01:34:35.000000 psense_common-0.4.8/psense_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-01-18 01:34:35.000000 psense_common-0.4.8/psense_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-01-18 01:34:35.000000 psense_common-0.4.8/psense_common.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-18 01:34:35.523580 psense_common-0.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-01-18 01:34:26.000000 psense_common-0.4.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-18 01:34:35.523580 psense_common-0.4.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6429 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/test_analysis_calibration.py
--rw-rw-rw-   0 root         (0) root         (0)    11748 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/test_analysis_excelwriter.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/test_analysis_response.py
--rw-rw-rw-   0 root         (0) root         (0)    25242 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/test_aws_itfc.py
--rw-rw-rw-   0 root         (0) root         (0)    14943 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/test_kfilter.py
--rw-rw-rw-   0 root         (0) root         (0)    10502 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/test_pformat.py
--rw-rw-rw-   0 root         (0) root         (0)    41964 2023-01-18 01:34:26.000000 psense_common-0.4.8/tests/test_pparser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-20 18:05:27.604455 psense_common-0.4.9/
+-rw-rw-rw-   0 root         (0) root         (0)     6973 2023-01-20 18:05:27.604455 psense_common-0.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6552 2023-01-20 18:05:17.000000 psense_common-0.4.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-20 18:05:27.604455 psense_common-0.4.9/psense_common/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-20 18:05:27.604455 psense_common-0.4.9/psense_common/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4099 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/analysis/calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6894 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/analysis/excelwriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9455 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/analysis/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     9696 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/kfilter.py
+-rw-rw-rw-   0 root         (0) root         (0)    28574 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/psense_aws_itfc.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/psense_format.py
+-rw-rw-rw-   0 root         (0) root         (0)    35257 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/psense_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-20 18:05:17.000000 psense_common-0.4.9/psense_common/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-20 18:05:27.604455 psense_common-0.4.9/psense_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6973 2023-01-20 18:05:27.000000 psense_common-0.4.9/psense_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      728 2023-01-20 18:05:27.000000 psense_common-0.4.9/psense_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-20 18:05:27.000000 psense_common-0.4.9/psense_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-01-20 18:05:27.000000 psense_common-0.4.9/psense_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-01-20 18:05:27.000000 psense_common-0.4.9/psense_common.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-20 18:05:27.604455 psense_common-0.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-01-20 18:05:17.000000 psense_common-0.4.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-20 18:05:27.604455 psense_common-0.4.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6429 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/test_analysis_calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)    11748 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/test_analysis_excelwriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/test_analysis_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    25242 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/test_aws_itfc.py
+-rw-rw-rw-   0 root         (0) root         (0)    14943 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/test_kfilter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10502 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/test_pformat.py
+-rw-rw-rw-   0 root         (0) root         (0)    41964 2023-01-20 18:05:17.000000 psense_common-0.4.9/tests/test_pparser.py
```

### Comparing `psense_common-0.4.8/PKG-INFO` & `psense_common-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psense_common
-Version: 0.4.8
+Version: 0.4.9
 Summary: PercuSense Common Modules
 Home-page: https://bitbucket.org/psense/psense-common
 Author: Brad Liang
 Author-email: brad.liang@percusense.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `psense_common-0.4.8/README.md` & `psense_common-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/psense_common/analysis/calibration.py` & `psense_common-0.4.9/psense_common/analysis/calibration.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/psense_common/analysis/excelwriter.py` & `psense_common-0.4.9/psense_common/analysis/excelwriter.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/psense_common/analysis/response.py` & `psense_common-0.4.9/psense_common/analysis/response.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/psense_common/kfilter.py` & `psense_common-0.4.9/psense_common/kfilter.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/psense_common/psense_aws_itfc.py` & `psense_common-0.4.9/psense_common/psense_aws_itfc.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,17 +714,20 @@
                 return None
 
         data = res
         records = data["Items"]
         count = data["Count"]
 
         res = pd.json_normalize(records)
-        res["set"] = res["timestamp"].map(lambda a: a.split("|")[0])
-        res["timestamp"] = res["timestamp"].map(lambda a: a.split("|")[1])
-        log.debug(f"{LOG_PREFIX}.get_event_data: found {count} items")
+        if count > 0:
+            res["set"] = res["timestamp"].map(lambda a: a.split("|")[0])
+            res["timestamp"] = res["timestamp"].map(lambda a: a.split("|")[1])
+            log.debug(f"{LOG_PREFIX}.get_event_data: found {count} items")
+        else:
+            log.debug(f"{LOG_PREFIX}.get_event_data: found no items")
 
         return res
 
     def add_event(self, set: int, timestamp: str, type: str, reference: float):
         expid = self.get_experiment()
         assert self.exp_is_valid, f"Experiment [{expid}] has not been validated"
         assert type in valid_types, f"Type [{type}] is not valid"
```

### Comparing `psense_common-0.4.8/psense_common/psense_format.py` & `psense_common-0.4.9/psense_common/psense_format.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/psense_common/psense_parser.py` & `psense_common-0.4.9/psense_common/psense_parser.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/psense_common.egg-info/PKG-INFO` & `psense_common-0.4.9/psense_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psense-common
-Version: 0.4.8
+Version: 0.4.9
 Summary: PercuSense Common Modules
 Home-page: https://bitbucket.org/psense/psense-common
 Author: Brad Liang
 Author-email: brad.liang@percusense.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `psense_common-0.4.8/psense_common.egg-info/SOURCES.txt` & `psense_common-0.4.9/psense_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/setup.py` & `psense_common-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/tests/test_analysis_calibration.py` & `psense_common-0.4.9/tests/test_analysis_calibration.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/tests/test_analysis_excelwriter.py` & `psense_common-0.4.9/tests/test_analysis_excelwriter.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/tests/test_analysis_response.py` & `psense_common-0.4.9/tests/test_analysis_response.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/tests/test_aws_itfc.py` & `psense_common-0.4.9/tests/test_aws_itfc.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/tests/test_kfilter.py` & `psense_common-0.4.9/tests/test_kfilter.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/tests/test_pformat.py` & `psense_common-0.4.9/tests/test_pformat.py`

 * *Files identical despite different names*

### Comparing `psense_common-0.4.8/tests/test_pparser.py` & `psense_common-0.4.9/tests/test_pparser.py`

 * *Files identical despite different names*


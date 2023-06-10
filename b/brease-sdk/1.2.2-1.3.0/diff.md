# Comparing `tmp/brease-sdk-1.2.2.tar.gz` & `tmp/brease-sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brease-sdk-1.2.2.tar", last modified: Sat Jun 10 00:46:28 2023, max compression
+gzip compressed data, was "brease-sdk-1.3.0.tar", last modified: Thu Jun  1 00:59:37 2023, max compression
```

## Comparing `brease-sdk-1.2.2.tar` & `brease-sdk-1.3.0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.273272 brease-sdk-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-10 00:46:28.273272 brease-sdk-1.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2638 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 00:46:28.273272 brease-sdk-1.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.265272 brease-sdk-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.269272 brease-sdk-1.2.2/src/brease_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-10 00:46:28.000000 brease-sdk-1.2.2/src/brease_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-10 00:46:28.000000 brease-sdk-1.2.2/src/brease_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 00:46:28.000000 brease-sdk-1.2.2/src/brease_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-10 00:46:28.000000 brease-sdk-1.2.2/src/brease_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-10 00:46:28.000000 brease-sdk-1.2.2/src/brease_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.269272 brease-sdk-1.2.2/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7573 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/contextid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.269272 brease-sdk-1.2.2/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.269272 brease-sdk-1.2.2/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/operations/addrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1308 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/operations/evaluaterules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/operations/getallrules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/operations/removerule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/operations/replacerule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.269272 brease-sdk-1.2.2/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/addruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/apiaddruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/apiallrulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/apievaluaterulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/apireplaceruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1317 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/condition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/conditionbasekey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/conditionbaseref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/conditiontype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/evaluaterulesinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/expressionarray.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/modelsevaluationresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2126 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/modelsrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/modelstarget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/models/shared/replaceruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1685 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 00:46:28.269272 brease-sdk-1.2.2/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-10 00:46:18.000000 brease-sdk-1.2.2/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.613705 brease-sdk-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-01 00:59:37.613705 brease-sdk-1.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2660 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 00:59:37.613705 brease-sdk-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.609705 brease-sdk-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.609705 brease-sdk-1.3.0/src/brease_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-01 00:59:37.000000 brease-sdk-1.3.0/src/brease_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-01 00:59:37.000000 brease-sdk-1.3.0/src/brease_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 00:59:37.000000 brease-sdk-1.3.0/src/brease_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-01 00:59:37.000000 brease-sdk-1.3.0/src/brease_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 00:59:37.000000 brease-sdk-1.3.0/src/brease_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.609705 brease-sdk-1.3.0/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7170 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/contextid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.609705 brease-sdk-1.3.0/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.609705 brease-sdk-1.3.0/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/operations/addrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1308 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/operations/evaluaterules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/operations/getallrules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/operations/removerule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/operations/replacerule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.613705 brease-sdk-1.3.0/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/addruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/apiaddruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/apiallrulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/apievaluaterulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/apireplaceruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1317 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/condition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/conditionbasekey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/conditionbaseref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/conditiontype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/evaluaterulesinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/expressionarray.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/modelsevaluationresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2126 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/modelsrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/modelstarget.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/models/shared/replaceruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:59:37.613705 brease-sdk-1.3.0/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-01 00:59:27.000000 brease-sdk-1.3.0/src/sdk/utils/utils.py
```

### Comparing `brease-sdk-1.2.2/LICENSE.md` & `brease-sdk-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/PKG-INFO` & `brease-sdk-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: brease-sdk
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: dotindustries
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.md
 
 # brease-sdk
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
@@ -54,15 +53,15 @@
             ),
         ),
     ),
     context_id='quod',
 )
 
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
-    api_token="",
+    api_token="YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
```

### Comparing `brease-sdk-1.2.2/README.md` & `brease-sdk-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             ),
         ),
     ),
     context_id='quod',
 )
 
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
-    api_token="",
+    api_token="YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
```

### Comparing `brease-sdk-1.2.2/setup.py` & `brease-sdk-1.3.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,37 +6,34 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="brease-sdk",
-    version="1.2.2",
+    version="1.3.0",
     author="dotindustries",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
-        "certifi>=2022.12.7",
-        "charset-normalizer>=2.1.1",
-        "dataclasses-json-speakeasy>=0.5.8",
-        "idna>=3.3",
-        "jsonpath-python>=1.0.6 ",
-        "marshmallow>=3.17.1",
-        "marshmallow-enum>=1.5.1",
-        "mypy-extensions>=0.4.3",
-        "packaging>=21.3",
-        "pyparsing>=3.0.9",
-        "python-dateutil>=2.8.2",
-        "requests>=2.28.1",
-        "six>=1.16.0",
-        "typing-inspect>=0.8.0",
-        "typing_extensions>=4.3.0",
-        "urllib3>=1.26.12",
+        "certifi==2022.12.7",
+        "charset-normalizer==2.1.1",
+        "dataclasses-json-speakeasy==0.5.8",
+        "idna==3.3",
+        "marshmallow==3.17.1",
+        "marshmallow-enum==1.5.1",
+        "mypy-extensions==0.4.3",
+        "packaging==21.3",
+        "pyparsing==3.0.9",
+        "python-dateutil==2.8.2",
+        "requests==2.28.1",
+        "six==1.16.0",
+        "typing-inspect==0.8.0",
+        "typing_extensions==4.3.0",
+        "urllib3==1.26.12",
+        "pylint==2.16.2",
     ],
-    extras_require={
-        "dev":["pylint==2.16.2"]
-    },
     package_dir={'': 'src'},
     python_requires='>=3.9'
 )
```

### Comparing `brease-sdk-1.2.2/src/brease_sdk.egg-info/PKG-INFO` & `brease-sdk-1.3.0/src/brease_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: brease-sdk
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: dotindustries
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.md
 
 # brease-sdk
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
@@ -54,15 +53,15 @@
             ),
         ),
     ),
     context_id='quod',
 )
 
 res = s.context_id.add_rule(req, operations.AddRuleSecurity(
-    api_token="",
+    api_token="YOUR_BEARER_TOKEN_HERE",
 ))
 
 if res.api_add_rule_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
```

### Comparing `brease-sdk-1.2.2/src/brease_sdk.egg-info/SOURCES.txt` & `brease-sdk-1.3.0/src/brease_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 src/brease_sdk.egg-info/SOURCES.txt
 src/brease_sdk.egg-info/dependency_links.txt
 src/brease_sdk.egg-info/requires.txt
 src/brease_sdk.egg-info/top_level.txt
 src/sdk/__init__.py
 src/sdk/contextid.py
 src/sdk/sdk.py
-src/sdk/sdkconfiguration.py
 src/sdk/models/__init__.py
 src/sdk/models/operations/__init__.py
 src/sdk/models/operations/addrule.py
 src/sdk/models/operations/evaluaterules.py
 src/sdk/models/operations/getallrules.py
 src/sdk/models/operations/removerule.py
 src/sdk/models/operations/replacerule.py
```

### Comparing `brease-sdk-1.2.2/src/sdk/contextid.py` & `brease-sdk-1.3.0/src/sdk/contextid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
 from typing import Optional
 
 class ContextID:
     r"""Rule domain context"""
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def add_rule(self, request: operations.AddRuleRequest, security: operations.AddRuleSecurity) -> operations.AddRuleResponse:
         r"""Adds a new rule to the context"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.AddRuleRequest, base_url, '/{contextID}/rules/add', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "add_rule_input", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self.sdk_configuration.client, security)
+        client = utils.configure_security_client(self._client, security)
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.AddRuleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -38,25 +48,25 @@
                 res.api_add_rule_response = out
 
         return res
 
     
     def evaluate_rules(self, request: operations.EvaluateRulesRequest, security: operations.EvaluateRulesSecurity) -> operations.EvaluateRulesResponse:
         r"""Evaluate rules within a context on the provided object"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.EvaluateRulesRequest, base_url, '/{contextID}/evaluate', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "evaluate_rules_input", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self.sdk_configuration.client, security)
+        client = utils.configure_security_client(self._client, security)
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.EvaluateRulesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -65,22 +75,22 @@
                 res.api_evaluate_rules_response = out
 
         return res
 
     
     def get_all_rules(self, request: operations.GetAllRulesRequest, security: operations.GetAllRulesSecurity) -> operations.GetAllRulesResponse:
         r"""Returns all rules with the context"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetAllRulesRequest, base_url, '/{contextID}/rules', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self.sdk_configuration.client, security)
+        client = utils.configure_security_client(self._client, security)
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllRulesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -89,45 +99,45 @@
                 res.api_all_rules_response = out
 
         return res
 
     
     def remove_rule(self, request: operations.RemoveRuleRequest, security: operations.RemoveRuleSecurity) -> operations.RemoveRuleResponse:
         r"""Removes a rule from the context"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.RemoveRuleRequest, base_url, '/{contextID}/rules/{id}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self.sdk_configuration.client, security)
+        client = utils.configure_security_client(self._client, security)
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.RemoveRuleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def replace_rule(self, request: operations.ReplaceRuleRequest, security: operations.ReplaceRuleSecurity) -> operations.ReplaceRuleResponse:
         r"""Replaces an existing rule within the context"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ReplaceRuleRequest, base_url, '/{contextID}/rules/{id}', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "replace_rule_input", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self.sdk_configuration.client, security)
+        client = utils.configure_security_client(self._client, security)
         
         http_res = client.request('PUT', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ReplaceRuleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `brease-sdk-1.2.2/src/sdk/models/operations/__init__.py` & `brease-sdk-1.3.0/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/operations/addrule.py` & `brease-sdk-1.3.0/src/sdk/models/operations/addrule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/operations/evaluaterules.py` & `brease-sdk-1.3.0/src/sdk/models/operations/evaluaterules.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/operations/getallrules.py` & `brease-sdk-1.3.0/src/sdk/models/operations/getallrules.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/operations/removerule.py` & `brease-sdk-1.3.0/src/sdk/models/operations/removerule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/operations/replacerule.py` & `brease-sdk-1.3.0/src/sdk/models/operations/replacerule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/__init__.py` & `brease-sdk-1.3.0/src/sdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/addruleinput.py` & `brease-sdk-1.3.0/src/sdk/models/shared/addruleinput.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/apiaddruleresponse.py` & `brease-sdk-1.3.0/src/sdk/models/shared/apiaddruleresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/apiallrulesresponse.py` & `brease-sdk-1.3.0/src/sdk/models/shared/apiallrulesresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/apievaluaterulesresponse.py` & `brease-sdk-1.3.0/src/sdk/models/shared/apievaluaterulesresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/apireplaceruleresponse.py` & `brease-sdk-1.3.0/src/sdk/models/shared/apireplaceruleresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/condition.py` & `brease-sdk-1.3.0/src/sdk/models/shared/condition.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/conditionbaseref.py` & `brease-sdk-1.3.0/src/sdk/models/shared/conditionbaseref.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/evaluaterulesinput.py` & `brease-sdk-1.3.0/src/sdk/models/shared/evaluaterulesinput.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/expressionarray.py` & `brease-sdk-1.3.0/src/sdk/models/shared/expressionarray.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/modelsevaluationresult.py` & `brease-sdk-1.3.0/src/sdk/models/shared/modelsevaluationresult.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/modelsrule.py` & `brease-sdk-1.3.0/src/sdk/models/shared/modelsrule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/models/shared/modelstarget.py` & `brease-sdk-1.3.0/src/sdk/models/shared/modelstarget.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/sdk.py` & `brease-sdk-1.3.0/src/sdk/sdk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,68 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
+from . import utils
 from .contextid import ContextID
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+
+SERVERS = [
+    "http://localhost:4400",
+    r"""Development server"""
+    "https://api.brease.run",
+    r"""Cloud hosted production server"""
+]
+"""Contains the list of servers available to the SDK"""
 
 class SDK:
-    r"""brease API: Business rule engine as a service API spec."""
+    r"""Business rule engine as a service API spec."""
     context_id: ContextID
     r"""Rule domain context"""
 
-    sdk_configuration: SDKConfiguration
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str = SERVERS[0]
+    _language: str = "python"
+    _sdk_version: str = "1.3.0"
+    _gen_version: str = "2.32.7"
 
     def __init__(self,
-                 server_idx: int = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
         
-        :param server_idx: The index of the server to use for all operations
-        :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session        
         """
-        if client is None:
-            client = requests_http.Session()
+        self._client = requests_http.Session()
         
-        security_client = client
         
         if server_url is not None:
             if url_params is not None:
-                server_url = utils.template_url(server_url, url_params)
+                self._server_url = utils.template_url(server_url, url_params)
+            else:
+                self._server_url = server_url
+
+        if client is not None:
+            self._client = client
+        
+        self._security_client = self._client
+        
 
-        self.sdk_configuration = SDKConfiguration(client, security_client, server_url, server_idx)
-       
         self._init_sdks()
     
     def _init_sdks(self):
-        self.context_id = ContextID(self.sdk_configuration)
+        self.context_id = ContextID(
+            self._client,
+            self._security_client,
+            self._server_url,
+            self._language,
+            self._sdk_version,
+            self._gen_version
+        )
+
```

### Comparing `brease-sdk-1.2.2/src/sdk/utils/retries.py` & `brease-sdk-1.3.0/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.2.2/src/sdk/utils/utils.py` & `brease-sdk-1.3.0/src/sdk/utils/utils.py`

 * *Files identical despite different names*


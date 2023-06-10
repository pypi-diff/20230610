# Comparing `tmp/python-alipay-sdk-3.2.0.tar.gz` & `tmp/python-alipay-sdk-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-alipay-sdk-3.2.0.tar", last modified: Tue Feb 28 03:51:29 2023, max compression
+gzip compressed data, was "python-alipay-sdk-3.3.0.tar", last modified: Sat Jun 10 06:12:47 2023, max compression
```

## Comparing `python-alipay-sdk-3.2.0.tar` & `python-alipay-sdk-3.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 03:51:29.810102 python-alipay-sdk-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-02-28 03:51:29.810102 python-alipay-sdk-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 03:51:29.806102 python-alipay-sdk-3.2.0/alipay/
--rw-r--r--   0 runner    (1001) docker     (122)    30758 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/alipay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/alipay/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/alipay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/alipay/loggers.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/alipay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 03:51:29.810102 python-alipay-sdk-3.2.0/python_alipay_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-02-28 03:51:29.000000 python-alipay-sdk-3.2.0/python_alipay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-02-28 03:51:29.000000 python-alipay-sdk-3.2.0/python_alipay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 03:51:29.000000 python-alipay-sdk-3.2.0/python_alipay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-02-28 03:51:29.000000 python-alipay-sdk-3.2.0/python_alipay_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-28 03:51:29.000000 python-alipay-sdk-3.2.0/python_alipay_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-28 03:51:29.810102 python-alipay-sdk-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-02-28 03:51:19.000000 python-alipay-sdk-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 06:12:47.669755 python-alipay-sdk-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-10 06:12:47.669755 python-alipay-sdk-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 06:12:47.669755 python-alipay-sdk-3.3.0/alipay/
+-rw-r--r--   0 runner    (1001) docker     (122)    30842 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/alipay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/alipay/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/alipay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/alipay/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/alipay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 06:12:47.669755 python-alipay-sdk-3.3.0/python_alipay_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-10 06:12:47.000000 python-alipay-sdk-3.3.0/python_alipay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-06-10 06:12:47.000000 python-alipay-sdk-3.3.0/python_alipay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-10 06:12:47.000000 python-alipay-sdk-3.3.0/python_alipay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-10 06:12:47.000000 python-alipay-sdk-3.3.0/python_alipay_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-10 06:12:47.000000 python-alipay-sdk-3.3.0/python_alipay_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-10 06:12:47.669755 python-alipay-sdk-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-06-10 06:12:38.000000 python-alipay-sdk-3.3.0/setup.py
```

### Comparing `python-alipay-sdk-3.2.0/LICENSE.txt` & `python-alipay-sdk-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-alipay-sdk-3.2.0/PKG-INFO` & `python-alipay-sdk-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alipay-sdk
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python SDK for AliPay, RSA is the only sign method we support
 Home-page: https://github.com/fzlee/alipay
 Author: fzlee
 Author-email: hi@ifconfiger.com
 License: BSD
 Keywords: python sdk alipay
 Platform: UNKNOWN
```

### Comparing `python-alipay-sdk-3.2.0/README.md` & `python-alipay-sdk-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-alipay-sdk-3.2.0/alipay/__init__.py` & `python-alipay-sdk-3.3.0/alipay/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,16 @@
         self._alipay_public_key = None
         if sign_type not in ("RSA", "RSA2"):
             message = "Unsupported sign type {}".format(sign_type)
             raise AliPayException(None, message)
         self._sign_type = sign_type
 
         if debug:
-            self._gateway = "https://openapi.alipaydev.com/gateway.do"
+            # self._gateway = "https://openapi.alipaydev.com/gateway.do"
+            self._gateway = "https://openapi-sandbox.dl.alipaydev.com/gateway.do"
         else:
             self._gateway = "https://openapi.alipay.com/gateway.do"
 
         # load key file immediately
         self._load_key()
 
     def _load_key(self):
```

### Comparing `python-alipay-sdk-3.2.0/alipay/loggers.py` & `python-alipay-sdk-3.3.0/alipay/loggers.py`

 * *Files identical despite different names*

### Comparing `python-alipay-sdk-3.2.0/python_alipay_sdk.egg-info/PKG-INFO` & `python-alipay-sdk-3.3.0/python_alipay_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alipay-sdk
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python SDK for AliPay, RSA is the only sign method we support
 Home-page: https://github.com/fzlee/alipay
 Author: fzlee
 Author-email: hi@ifconfiger.com
 License: BSD
 Keywords: python sdk alipay
 Platform: UNKNOWN
```

### Comparing `python-alipay-sdk-3.2.0/setup.py` & `python-alipay-sdk-3.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover('tests')
     return test_suite
 
 
 setup(
     name="python-alipay-sdk",
-    version="3.2.0",
+    version="3.3.0",
     author="fzlee",
     author_email="hi@ifconfiger.com",
     description="Python SDK for AliPay, RSA is the only sign method we support",
     license="BSD",
     keywords="python sdk alipay",
     url="https://github.com/fzlee/alipay",
     packages=['alipay'],
```


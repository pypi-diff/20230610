# Comparing `tmp/solax-0.3.1.tar.gz` & `tmp/solax-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solax-0.3.1.tar", last modified: Sat May 27 23:24:10 2023, max compression
+gzip compressed data, was "solax-0.3.2.tar", last modified: Sat Jun 10 09:45:47 2023, max compression
```

## Comparing `solax-0.3.1.tar` & `solax-0.3.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.519456 solax-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.507456 solax-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.511457 solax-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-27 23:23:57.000000 solax-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-27 23:23:57.000000 solax-0.3.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 23:23:57.000000 solax-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-27 23:23:57.000000 solax-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-27 23:24:10.519456 solax-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-27 23:23:57.000000 solax-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-27 23:23:57.000000 solax-0.3.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 23:24:10.519456 solax-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-27 23:23:57.000000 solax-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/solax/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-27 23:23:57.000000 solax-0.3.1/solax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-27 23:23:57.000000 solax-0.3.1/solax/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverter_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/solax/inverters/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/qvolt_hyb_g3_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_boost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_hybrid_gen4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_mini.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_mini_v34.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x1_smart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x3_hybrid_g4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x3_v34.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-27 23:23:57.000000 solax-0.3.1/solax/inverters/x_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-27 23:23:57.000000 solax-0.3.1/solax/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-27 23:23:57.000000 solax-0.3.1/solax/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-27 23:23:57.000000 solax-0.3.1/solax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/solax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 23:24:10.000000 solax-0.3.1/solax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 23:23:57.000000 solax-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-27 23:23:57.000000 solax-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-27 23:23:57.000000 solax-0.3.1/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/tests/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 23:24:10.515457 solax-0.3.1/tests/samples/api/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-27 23:23:57.000000 solax-0.3.1/tests/samples/api/realTimeData.htm
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-05-27 23:23:57.000000 solax-0.3.1/tests/samples/expected_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    35171 2023-05-27 23:23:57.000000 solax-0.3.1/tests/samples/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_base_inverter.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_solax.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 23:23:57.000000 solax-0.3.1/tests/test_vol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-27 23:23:57.000000 solax-0.3.1/verify.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.264831 solax-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.260831 solax-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.260831 solax-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-10 09:45:36.000000 solax-0.3.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-10 09:45:36.000000 solax-0.3.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-10 09:45:36.000000 solax-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-10 09:45:36.000000 solax-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-10 09:45:47.264831 solax-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-10 09:45:36.000000 solax-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-10 09:45:36.000000 solax-0.3.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:45:47.264831 solax-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-10 09:45:36.000000 solax-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.260831 solax-0.3.2/solax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-10 09:45:36.000000 solax-0.3.2/solax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-10 09:45:36.000000 solax-0.3.2/solax/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverter_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.264831 solax-0.3.2/solax/inverters/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/qvolt_hyb_g3_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x1_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x1_hybrid_gen4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x1_mini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x1_mini_v34.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x1_smart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x3_hybrid_g4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x3_mic_pro_g2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x3_v34.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-10 09:45:36.000000 solax-0.3.2/solax/inverters/x_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-10 09:45:36.000000 solax-0.3.2/solax/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-10 09:45:36.000000 solax-0.3.2/solax/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-10 09:45:36.000000 solax-0.3.2/solax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.260831 solax-0.3.2/solax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-10 09:45:47.000000 solax-0.3.2/solax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-10 09:45:47.000000 solax-0.3.2/solax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:45:47.000000 solax-0.3.2/solax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-10 09:45:47.000000 solax-0.3.2/solax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 09:45:47.000000 solax-0.3.2/solax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.264831 solax-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:36.000000 solax-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-10 09:45:36.000000 solax-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-10 09:45:36.000000 solax-0.3.2/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.264831 solax-0.3.2/tests/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:45:47.264831 solax-0.3.2/tests/samples/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-10 09:45:36.000000 solax-0.3.2/tests/samples/api/realTimeData.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-10 09:45:36.000000 solax-0.3.2/tests/samples/expected_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36536 2023-06-10 09:45:36.000000 solax-0.3.2/tests/samples/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-10 09:45:36.000000 solax-0.3.2/tests/test_base_inverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-10 09:45:36.000000 solax-0.3.2/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-10 09:45:36.000000 solax-0.3.2/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-10 09:45:36.000000 solax-0.3.2/tests/test_solax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-10 09:45:36.000000 solax-0.3.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-10 09:45:36.000000 solax-0.3.2/tests/test_vol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-06-10 09:45:36.000000 solax-0.3.2/verify.sh
```

### Comparing `solax-0.3.1/.github/workflows/publish.yml` & `solax-0.3.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/.github/workflows/tests.yaml` & `solax-0.3.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/LICENSE` & `solax-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/PKG-INFO` & `solax-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solax
-Version: 0.3.1
+Version: 0.3.2
 Summary: Solax inverter API client
 Home-page: https://github.com/squishykid/solax
 Author: Robin Wohlers-Reichel
 Author-email: me@robinwr.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `solax-0.3.1/README.md` & `solax-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/setup.py` & `solax-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/__init__.py` & `solax-0.3.2/solax/__init__.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/discovery.py` & `solax-0.3.2/solax/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     X3V34,
     X1Boost,
     X1HybridGen4,
     X1Mini,
     X1MiniV34,
     X1Smart,
     X3HybridG4,
+    X3MicProG2,
     XHybrid,
 )
 
 # registry of inverters
 REGISTRY = [
     XHybrid,
     X3,
@@ -26,14 +27,15 @@
     X1,
     X1Mini,
     X1MiniV34,
     X1Smart,
     QVOLTHYBG33P,
     X1Boost,
     X1HybridGen4,
+    X3MicProG2,
 ]
 
 
 logging.basicConfig(level=logging.INFO)
 
 
 class DiscoveryState:
```

### Comparing `solax-0.3.1/solax/inverter.py` & `solax-0.3.2/solax/inverter.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverter_http_client.py` & `solax-0.3.2/solax/inverter_http_client.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/__init__.py` & `solax-0.3.2/solax/inverters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .x1_boost import X1Boost
 from .x1_hybrid_gen4 import X1HybridGen4
 from .x1_mini import X1Mini
 from .x1_mini_v34 import X1MiniV34
 from .x1_smart import X1Smart
 from .x3 import X3
 from .x3_hybrid_g4 import X3HybridG4
+from .x3_mic_pro_g2 import X3MicProG2
 from .x3_v34 import X3V34
 from .x_hybrid import XHybrid
 
 __all__ = [
     "QVOLTHYBG33P",
     "XHybrid",
     "X1",
@@ -18,8 +19,9 @@
     "X1MiniV34",
     "X1Smart",
     "X3V34",
     "X3HybridG4",
     "X3",
     "X1Boost",
     "X1HybridGen4",
+    "X3MicProG2",
 ]
```

### Comparing `solax-0.3.1/solax/inverters/qvolt_hyb_g3_3p.py` & `solax-0.3.2/solax/inverters/qvolt_hyb_g3_3p.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x1.py` & `solax-0.3.2/solax/inverters/x1.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x1_boost.py` & `solax-0.3.2/solax/inverters/x1_boost.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x1_hybrid_gen4.py` & `solax-0.3.2/solax/inverters/x1_hybrid_gen4.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x1_mini.py` & `solax-0.3.2/solax/inverters/x1_mini.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x1_mini_v34.py` & `solax-0.3.2/solax/inverters/x1_mini_v34.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x1_smart.py` & `solax-0.3.2/solax/inverters/x1_smart.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x3.py` & `solax-0.3.2/solax/inverters/x3.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x3_hybrid_g4.py` & `solax-0.3.2/solax/inverters/x3_hybrid_g4.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x3_v34.py` & `solax-0.3.2/solax/inverters/x3_v34.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/inverters/x_hybrid.py` & `solax-0.3.2/solax/inverters/x_hybrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,13 +62,15 @@
             "PV2 Power": (12, Units.W),
             "Battery Voltage": (13, Units.V),
             "Battery Current": (14, Units.A),
             "Battery Power": (15, Units.W),
             "Battery Temperature": (16, Units.C),
             "Battery Remaining Capacity": (17, Units.PERCENT),
             "Month's Energy": (19, Units.KWH),
+            "Grid Exported Energy": (41, Units.KWH),
+            "Grid Imported Energy": (42, Units.KWH),
             "Grid Frequency": (50, Units.HZ),
             "EPS Voltage": (53, Units.V),
             "EPS Current": (54, Units.A),
             "EPS Power": (55, Units.W),
             "EPS Frequency": (56, Units.HZ),
         }
```

### Comparing `solax-0.3.1/solax/response_parser.py` & `solax-0.3.2/solax/response_parser.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/units.py` & `solax-0.3.2/solax/units.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax/utils.py` & `solax-0.3.2/solax/utils.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/solax.egg-info/PKG-INFO` & `solax-0.3.2/solax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solax
-Version: 0.3.1
+Version: 0.3.2
 Summary: Solax inverter API client
 Home-page: https://github.com/squishykid/solax
 Author: Robin Wohlers-Reichel
 Author-email: me@robinwr.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `solax-0.3.1/solax.egg-info/SOURCES.txt` & `solax-0.3.2/solax.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 solax/inverters/x1_boost.py
 solax/inverters/x1_hybrid_gen4.py
 solax/inverters/x1_mini.py
 solax/inverters/x1_mini_v34.py
 solax/inverters/x1_smart.py
 solax/inverters/x3.py
 solax/inverters/x3_hybrid_g4.py
+solax/inverters/x3_mic_pro_g2.py
 solax/inverters/x3_v34.py
 solax/inverters/x_hybrid.py
 tests/__init__.py
 tests/conftest.py
 tests/fixtures.py
 tests/test_base_inverter.py
 tests/test_discovery.py
```

### Comparing `solax-0.3.1/tests/fixtures.py` & `solax-0.3.2/tests/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     X1_HYBRID_G4_VALUES,
     X1_MINI_VALUES,
     X1_MINI_VALUES_V34,
     X1_SMART_VALUES,
     X1_VALUES,
     X3_HYBRID_G4_VALUES,
     X3_HYBRID_VALUES,
+    X3_MICPRO_G2_VALUES,
     X3_VALUES,
     X3V34_HYBRID_VALUES,
     X3V34_HYBRID_VALUES_EPS_MODE,
     X3V34_HYBRID_VALUES_NEGATIVE_POWER,
     XHYBRID_VALUES,
 )
 from tests.samples.responses import (
@@ -31,14 +32,15 @@
     X3_HYBRID_G3_2X_MPPT_RESPONSE,
     X3_HYBRID_G3_2X_MPPT_RESPONSE_V34,
     X3_HYBRID_G3_2X_MPPT_RESPONSE_V34_EPS_MODE,
     X3_HYBRID_G3_2X_MPPT_RESPONSE_V34_NEGATIVE_POWER,
     X3_HYBRID_G3_RESPONSE,
     X3_HYBRID_G4_RESPONSE,
     X3_MIC_RESPONSE,
+    X3_MICPRO_G2_RESPONSE,
     XHYBRID_DE01_RESPONSE,
     XHYBRID_DE02_RESPONSE,
 )
 
 X_FORWARDED_HEADER = {"X-Forwarded-For": "5.8.8.8"}
 
 
@@ -215,14 +217,24 @@
         values=X3_HYBRID_G4_VALUES,
         headers=None,
         data="optType=ReadRealTimeData",
     ),
     InverterUnderTest(
         uri="/",
         method="POST",
+        query_string=None,
+        response=X3_MICPRO_G2_RESPONSE,
+        inverter=inverter.X3MicProG2,
+        values=X3_MICPRO_G2_VALUES,
+        headers=None,
+        data="optType=ReadRealTimeData",
+    ),
+    InverterUnderTest(
+        uri="/",
+        method="POST",
         query_string="",
         response=QVOLTHYBG33P_RESPONSE_V34,
         inverter=inverter.QVOLTHYBG33P,
         values=QVOLTHYBG33P_VALUES,
         headers=None,
         data=None,
     ),
```

### Comparing `solax-0.3.1/tests/samples/expected_values.py` & `solax-0.3.2/tests/samples/expected_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     "PV1 Power": 11,
     "PV1 Voltage": 2,
     "PV2 Current": 1,
     "PV2 Power": 12,
     "PV2 Voltage": 3,
     "Power Now": 6,
     "Total Energy": 9,
+    "Grid Exported Energy": 41,
+    "Grid Imported Energy": 42,
 }
 
 
 X3_VALUES = {
     "PV1 Current": 0,
     "PV2 Current": 1,
     "PV1 Voltage": 2,
@@ -260,14 +262,44 @@
     "Feed-in Energy": 0.0,
     "Consumed Energy": 20.09,
     "Battery Remaining Capacity": 30.0,
     "Battery Temperature": 22.0,
     "Battery Voltage": 234.6,
 }
 
+X3_MICPRO_G2_VALUES = {
+    "Grid 1 Voltage": 237.1,
+    "Grid 2 Voltage": 234.5,
+    "Grid 3 Voltage": 237.8,
+    "Grid 1 Current": 4.1,
+    "Grid 2 Current": 4.1,
+    "Grid 3 Current": 4.1,
+    "Grid 1 Power": 1018.0,
+    "Grid 2 Power": 992.0,
+    "Grid 3 Power": 970.0,
+    "PV1 Voltage": 174.1,
+    "PV2 Voltage": 174.5,
+    "PV3 Voltage": 0.0,
+    "PV1 Current": 8.8,
+    "PV2 Current": 8.7,
+    "PV3 Current": 0.0,
+    "PV1 Power": 1544.0,
+    "PV2 Power": 1531.0,
+    "PV3 Power": 0.0,
+    "Grid 1 Frequency": 49.98,
+    "Grid 2 Frequency": 49.99,
+    "Grid 3 Frequency": 49.94,
+    "Run Mode": "Normal",
+    "Total Yield": 795.7,
+    "Daily Yield": 20.0,
+    "Feed-in Power ": 2707.0,
+    "Total Feed-in Energy": 657.24,
+    "Total Consumption": 307.33,
+}
+
 X1_VALUES = {
     "PV1 Current": 0,
     "PV2 Current": 1,
     "PV1 Voltage": 2,
     "PV2 Voltage": 3,
     "Output Current": 4,
     "Network Voltage": 5,
```

### Comparing `solax-0.3.1/tests/samples/responses.py` & `solax-0.3.2/tests/samples/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1211,15 +1211,14 @@
         "masterVer": "0.00",
         "slaveNum": "0",
         "slaveVer": [0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00],
         "slaveType": [0, 0, 0, 0, 0, 0, 0, 0],
     },
 }
 
-
 X1_HYBRID_G4_RESPONSE = {
     "type": 15,
     "sn": "SXxxxxxxxx",
     "ver": "3.003.02",
     "Data": [
         2470,
         11,
@@ -1543,15 +1542,14 @@
         99,
         100,
         101,
     ],
     "Information": [0.000, 5, "X3-Hybiyd-G3", "XXXXXXX", 1, 3.00, 0.00, 3.17, 1.01],
 }
 
-
 X3_HYBRID_G3_2X_MPPT_RESPONSE = {
     "type": "X3-Hybiyd-G3",
     "SN": "XXXXXXXXXX",
     "ver": "2.033.20",
     "Data": [
         0.0,
         0.0,
@@ -2602,14 +2600,123 @@
         0,
         0,
         0,
     ],
     "Information": [10.000, 14, "H34A**********", 8, 1.23, 0.00, 1.24, 1.09, 0.00, 1],
 }
 
+X3_MICPRO_G2_RESPONSE = {
+    "sn": "SRE*******",
+    "ver": "3.008.10",
+    "type": 16,
+    "Data": [
+        2371,
+        2345,
+        2378,
+        41,
+        41,
+        41,
+        1018,
+        992,
+        970,
+        1741,
+        1745,
+        0,
+        88,
+        87,
+        0,
+        1544,
+        1531,
+        0,
+        4998,
+        4999,
+        4994,
+        2,
+        7957,
+        0,
+        200,
+        4000,
+        57,
+        43,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        2707,
+        0,
+        188,
+        1,
+        30733,
+        0,
+        2982,
+        0,
+        1,
+        4,
+        1,
+        0,
+        13468,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+        0,
+    ],
+    "Information": [4.000, 16, "MC20**********", 8, 1.20, 0.00, 1.18, 1.00, 0.00, 1],
+}
+
 QVOLTHYBG33P_RESPONSE_V34 = {
     "sn": "SWX***",
     "ver": "2.034.06",
     "type": 14,
     "Data": [
         2214,
         2238,
```

### Comparing `solax-0.3.1/tests/test_discovery.py` & `solax-0.3.2/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/tests/test_smoke.py` & `solax-0.3.2/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/tests/test_solax.py` & `solax-0.3.2/tests/test_solax.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/tests/test_utils.py` & `solax-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `solax-0.3.1/verify.sh` & `solax-0.3.2/verify.sh`

 * *Files identical despite different names*


# Comparing `tmp/computing-toolbox-0.4.1.tar.gz` & `tmp/computing-toolbox-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.4.1.tar", last modified: Wed Jun  7 18:59:30 2023, max compression
+gzip compressed data, was "computing-toolbox-0.5.0.tar", last modified: Sat Jun 10 07:31:01 2023, max compression
```

## Comparing `computing-toolbox-0.4.1.tar` & `computing-toolbox-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.971042 computing-toolbox-0.4.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.971042 computing-toolbox-0.4.1/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 18:59:20.000000 computing-toolbox-0.4.1/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:59:30.975043 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 18:59:30.000000 computing-toolbox-0.4.1/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/gcp/gs_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-10 07:30:50.000000 computing-toolbox-0.5.0/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:31:01.127738 computing-toolbox-0.5.0/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-10 07:31:01.000000 computing-toolbox-0.5.0/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-10 07:31:01.000000 computing-toolbox-0.5.0/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 07:31:01.000000 computing-toolbox-0.5.0/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-10 07:31:01.000000 computing-toolbox-0.5.0/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 07:31:01.000000 computing-toolbox-0.5.0/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.4.1/LICENSE` & `computing-toolbox-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/PKG-INFO` & `computing-toolbox-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.4.1
+Version: 0.5.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.4.1/README.md` & `computing-toolbox-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.5.0/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.5.0/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.5.0/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.5.0/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.5.0/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/utils/http_async_request.py` & `computing-toolbox-0.5.0/src/computing_toolbox/utils/http_async_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.5.0/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.5.0/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.5.0/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.5.0/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.5.0/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.4.1
+Version: 0.5.0
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.4.1/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.5.0/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/computing_toolbox.egg-info/dependency_links.txt
 src/computing_toolbox.egg-info/requires.txt
 src/computing_toolbox.egg-info/top_level.txt
 src/computing_toolbox/algorithms/__init__.py
 src/computing_toolbox/algorithms/split_range.py
 src/computing_toolbox/gcp/__init__.py
 src/computing_toolbox/gcp/gs.py
+src/computing_toolbox/gcp/gs_async.py
 src/computing_toolbox/gcp/secret_manager.py
 src/computing_toolbox/utils/__init__.py
 src/computing_toolbox/utils/deep_get.py
 src/computing_toolbox/utils/es_long_search.py
 src/computing_toolbox/utils/http_async_request.py
 src/computing_toolbox/utils/http_fake_headers.py
 src/computing_toolbox/utils/http_request.py
```


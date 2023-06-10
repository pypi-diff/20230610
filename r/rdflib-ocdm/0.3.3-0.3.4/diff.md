# Comparing `tmp/rdflib_ocdm-0.3.3.tar.gz` & `tmp/rdflib_ocdm-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdflib_ocdm-0.3.3.tar", max compression
+gzip compressed data, was "rdflib_ocdm-0.3.4.tar", max compression
```

## Comparing `rdflib_ocdm-0.3.3.tar` & `rdflib_ocdm-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      515 2023-06-10 14:54:25.924675 rdflib_ocdm-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      840 2023-06-10 14:49:29.039605 rdflib_ocdm-0.3.3/rdflib_ocdm/__init__.py
--rw-r--r--   0        0        0     6176 2023-06-10 14:49:29.040616 rdflib_ocdm-0.3.3/rdflib_ocdm/abstract_entity.py
--rw-r--r--   0        0        0      839 2023-06-10 14:49:29.042607 rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     2444 2023-06-10 14:49:29.043617 rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0     5348 2023-06-10 14:49:29.044751 rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0     3119 2023-06-10 14:49:29.045767 rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     2081 2023-06-10 14:53:45.715249 rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/redis_counter_handler.py
--rw-r--r--   0        0        0     3529 2023-06-10 14:49:29.048401 rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     4612 2023-06-10 14:49:29.049425 rdflib_ocdm-0.3.3/rdflib_ocdm/ocdm_graph.py
--rw-r--r--   0        0        0      839 2023-06-10 14:49:29.050418 rdflib_ocdm-0.3.3/rdflib_ocdm/prov/__init__.py
--rw-r--r--   0        0        0     2906 2023-06-10 14:49:29.051418 rdflib_ocdm-0.3.3/rdflib_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0     7604 2023-06-10 14:49:29.052467 rdflib_ocdm-0.3.3/rdflib_ocdm/prov/provenance.py
--rw-r--r--   0        0        0    13514 2023-06-10 14:49:29.053989 rdflib_ocdm-0.3.3/rdflib_ocdm/prov/snapshot_entity.py
--rw-r--r--   0        0        0     4447 2023-06-10 14:49:29.055024 rdflib_ocdm-0.3.3/rdflib_ocdm/query_utils.py
--rw-r--r--   0        0        0     2259 2023-06-10 14:49:29.055534 rdflib_ocdm-0.3.3/rdflib_ocdm/reader.py
--rw-r--r--   0        0        0     9000 2023-06-10 14:49:29.057559 rdflib_ocdm-0.3.3/rdflib_ocdm/storer.py
--rw-r--r--   0        0        0     2570 2023-06-10 14:49:29.057559 rdflib_ocdm-0.3.3/rdflib_ocdm/support.py
--rw-r--r--   0        0        0      600 2023-06-10 14:49:29.035949 rdflib_ocdm-0.3.3/README.md
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.3/setup.py
--rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-06-10 14:58:14.054313 rdflib_ocdm-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      840 2023-06-10 14:49:29.039605 rdflib_ocdm-0.3.4/rdflib_ocdm/__init__.py
+-rw-r--r--   0        0        0     6176 2023-06-10 14:49:29.040616 rdflib_ocdm-0.3.4/rdflib_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0      839 2023-06-10 14:49:29.042607 rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     2444 2023-06-10 14:49:29.043617 rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0     5348 2023-06-10 14:49:29.044751 rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0     3119 2023-06-10 14:49:29.045767 rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     2144 2023-06-10 14:58:08.663200 rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/redis_counter_handler.py
+-rw-r--r--   0        0        0     3529 2023-06-10 14:49:29.048401 rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     4612 2023-06-10 14:49:29.049425 rdflib_ocdm-0.3.4/rdflib_ocdm/ocdm_graph.py
+-rw-r--r--   0        0        0      839 2023-06-10 14:49:29.050418 rdflib_ocdm-0.3.4/rdflib_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0     2906 2023-06-10 14:49:29.051418 rdflib_ocdm-0.3.4/rdflib_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0     7604 2023-06-10 14:49:29.052467 rdflib_ocdm-0.3.4/rdflib_ocdm/prov/provenance.py
+-rw-r--r--   0        0        0    13514 2023-06-10 14:49:29.053989 rdflib_ocdm-0.3.4/rdflib_ocdm/prov/snapshot_entity.py
+-rw-r--r--   0        0        0     4447 2023-06-10 14:49:29.055024 rdflib_ocdm-0.3.4/rdflib_ocdm/query_utils.py
+-rw-r--r--   0        0        0     2259 2023-06-10 14:49:29.055534 rdflib_ocdm-0.3.4/rdflib_ocdm/reader.py
+-rw-r--r--   0        0        0     9000 2023-06-10 14:49:29.057559 rdflib_ocdm-0.3.4/rdflib_ocdm/storer.py
+-rw-r--r--   0        0        0     2570 2023-06-10 14:49:29.057559 rdflib_ocdm-0.3.4/rdflib_ocdm/support.py
+-rw-r--r--   0        0        0      600 2023-06-10 14:49:29.035949 rdflib_ocdm-0.3.4/README.md
+-rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.4/setup.py
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.4/PKG-INFO
```

### Comparing `rdflib_ocdm-0.3.3/pyproject.toml` & `rdflib_ocdm-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rdflib-ocdm"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = ["arcangelo7 <arcangelomas@gmail.com>"]
 license = "ISC"
 readme = "README.md"
 packages = [{include = "rdflib_ocdm"}]
 
 [tool.poetry.dependencies]
```

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/__init__.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/abstract_entity.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/__init__.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/counter_handler.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/filesystem_counter_handler.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/in_memory_counter_handler.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/redis_counter_handler.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/redis_counter_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,7 +48,10 @@
         
     def increment_counter(self, entity_name: str) -> int:
         entity_name = str(entity_name)
         cur_count = self.read_counter(entity_name)
         count = cur_count + 1
         self.set_counter(count, entity_name)
         return count
+    
+    def flush(self):
+        self.connection.flushdb()
```

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/counter_handler/sqlite_counter_handler.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/ocdm_graph.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/ocdm_graph.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/prov/__init__.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/prov/prov_entity.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/prov/provenance.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/prov/provenance.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/prov/snapshot_entity.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/prov/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/query_utils.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/query_utils.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/reader.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/reader.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/storer.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/storer.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/rdflib_ocdm/support.py` & `rdflib_ocdm-0.3.4/rdflib_ocdm/support.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/README.md` & `rdflib_ocdm-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.3/setup.py` & `rdflib_ocdm-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['oc-ocdm>=7.1.7,<8.0.0',
  'rdflib>=6.2.0,<7.0.0',
  'redis>=4.5.5,<5.0.0',
  'sparqlwrapper>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'rdflib-ocdm',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': '',
     'long_description': '[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/rdflib-ocdm/main/test/coverage/coverage.svg)\n![PyPI](https://img.shields.io/pypi/pyversions/rdflib-ocdm)\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/rdflib-ocdm)\n\n# rdflib-ocdm\n',
     'author': 'arcangelo7',
     'author_email': 'arcangelomas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rdflib_ocdm-0.3.3/PKG-INFO` & `rdflib_ocdm-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdflib-ocdm
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```


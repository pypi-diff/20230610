# Comparing `tmp/grapdb-0.8.tar.gz` & `tmp/grapdb-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grapdb-0.8.tar", last modified: Mon Oct  4 23:29:56 2021, max compression
+gzip compressed data, was "grapdb-0.9.tar", last modified: Wed Oct  6 01:22:15 2021, max compression
```

## Comparing `grapdb-0.8.tar` & `grapdb-0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2019-06-13 19:55:11.051133 grapdb-0.8/grapdb/__init__.py
--rw-r--r--   0        0        0     2116 2021-02-13 09:01:17.637872 grapdb-0.8/grapdb/cli.py
--rw-r--r--   0        0        0    21975 2021-10-04 23:29:46.558102 grapdb-0.8/grapdb/graph.py
--rw-r--r--   0        0        0    15654 2021-10-04 23:29:46.558102 grapdb-0.8/grapdb/parser.py
--rw-r--r--   0        0        0     1548 2021-08-20 08:34:52.437061 grapdb-0.8/grapdb/planner.py
--rw-r--r--   0        0        0        0 2019-06-13 19:55:11.051133 grapdb-0.8/grapdb/py.typed
--rw-r--r--   0        0        0        0 2019-06-13 19:55:11.051133 grapdb-0.8/grapdb/target/__init__.py
--rw-r--r--   0        0        0    19125 2021-10-04 23:29:46.558102 grapdb-0.8/grapdb/target/rsrc/graph_orm_base.py
--rw-r--r--   0        0        0    12006 2021-08-25 20:18:03.905512 grapdb-0.8/grapdb/target/sa_orm.py
--rw-r--r--   0        0        0      505 2021-10-04 23:29:46.558102 grapdb-0.8/pyproject.toml
--rw-r--r--   0        0        0      798 2021-10-04 23:29:56.311520 grapdb-0.8/setup.py
--rw-r--r--   0        0        0      471 2021-10-04 23:29:56.311846 grapdb-0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2019-06-13 19:55:11.051133 grapdb-0.9/grapdb/__init__.py
+-rw-r--r--   0        0        0     2116 2021-02-13 09:01:17.637872 grapdb-0.9/grapdb/cli.py
+-rw-r--r--   0        0        0    21975 2021-10-04 23:29:46.558102 grapdb-0.9/grapdb/graph.py
+-rw-r--r--   0        0        0    15653 2021-10-06 01:21:25.837528 grapdb-0.9/grapdb/parser.py
+-rw-r--r--   0        0        0     1548 2021-08-20 08:34:52.437061 grapdb-0.9/grapdb/planner.py
+-rw-r--r--   0        0        0        0 2019-06-13 19:55:11.051133 grapdb-0.9/grapdb/py.typed
+-rw-r--r--   0        0        0        0 2019-06-13 19:55:11.051133 grapdb-0.9/grapdb/target/__init__.py
+-rw-r--r--   0        0        0    19125 2021-10-04 23:29:46.558102 grapdb-0.9/grapdb/target/rsrc/graph_orm_base.py
+-rw-r--r--   0        0        0    12006 2021-08-25 20:18:03.905512 grapdb-0.9/grapdb/target/sa_orm.py
+-rw-r--r--   0        0        0      505 2021-10-06 01:21:44.337231 grapdb-0.9/pyproject.toml
+-rw-r--r--   0        0        0      798 2021-10-06 01:22:15.872913 grapdb-0.9/setup.py
+-rw-r--r--   0        0        0      471 2021-10-06 01:22:15.873151 grapdb-0.9/PKG-INFO
```

### Comparing `grapdb-0.8/grapdb/cli.py` & `grapdb-0.9/grapdb/cli.py`

 * *Files identical despite different names*

### Comparing `grapdb-0.8/grapdb/graph.py` & `grapdb-0.9/grapdb/graph.py`

 * *Files identical despite different names*

### Comparing `grapdb-0.8/grapdb/parser.py` & `grapdb-0.9/grapdb/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
     elif data_type_raw.startswith("-)"):
         ref_name = data_type_raw[len("-)") :]
         raise InvalidSpec(f"Unsupported reference to colo-ed vertex '{ref_name}'.")
     elif data_type_raw.startswith("enum:"):
         ref_name = data_type_raw[len("enum:") :]
         if ref_name not in enums:
             raise InvalidSpec("Undefined enum: %r" % ref_name)
-        data_type = ctypes[ref_name]
+        data_type = enums[ref_name]
     elif data_type_raw.startswith("ctype:"):
         ref_name = data_type_raw[len("ctype:") :]
         if ref_name not in ctypes:
             raise InvalidSpec("Undefined composite type: %r" % ref_name)
         data_type = ctypes[ref_name]
     else:
         data_type: DataType = data_type_raw
```

### Comparing `grapdb-0.8/grapdb/planner.py` & `grapdb-0.9/grapdb/planner.py`

 * *Files identical despite different names*

### Comparing `grapdb-0.8/grapdb/target/rsrc/graph_orm_base.py` & `grapdb-0.9/grapdb/target/rsrc/graph_orm_base.py`

 * *Files identical despite different names*

### Comparing `grapdb-0.8/grapdb/target/sa_orm.py` & `grapdb-0.9/grapdb/target/sa_orm.py`

 * *Files identical despite different names*

### Comparing `grapdb-0.8/setup.py` & `grapdb-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['code-writer>=1.1.1,<2.0.0', 'toml>=0.10.0,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['grapdb = grapdb.cli:main']}
 
 setup_kwargs = {
     'name': 'grapdb',
-    'version': '0.8',
+    'version': '0.9',
     'description': 'Graph data modeling and code generator for Postgres.',
     'long_description': None,
     'author': 'Ken Elkabany',
     'author_email': 'ken@elkabany.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```


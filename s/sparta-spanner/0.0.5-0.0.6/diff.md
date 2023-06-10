# Comparing `tmp/sparta-spanner-0.0.5.tar.gz` & `tmp/sparta-spanner-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparta-spanner-0.0.5.tar", last modified: Sat Apr  1 13:51:40 2023, max compression
+gzip compressed data, was "sparta-spanner-0.0.6.tar", last modified: Sat Jun 10 10:23:31 2023, max compression
```

## Comparing `sparta-spanner-0.0.5.tar` & `sparta-spanner-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 13:51:40.448780 sparta-spanner-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1619 2023-04-01 13:51:40.448780 sparta-spanner-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1202 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 13:51:40.448780 sparta-spanner-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1648 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 13:51:40.440779 sparta-spanner-0.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 13:51:40.444780 sparta-spanner-0.0.5/src/sparta/
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/src/sparta/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 13:51:40.444780 sparta-spanner-0.0.5/src/sparta/spanner/
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/src/sparta/spanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/src/sparta/spanner/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/src/sparta/spanner/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/src/sparta/spanner/service.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/src/sparta/spanner/utils.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-04-01 13:50:42.000000 sparta-spanner-0.0.5/src/sparta/spanner/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 13:51:40.448780 sparta-spanner-0.0.5/src/sparta_spanner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1619 2023-04-01 13:51:40.000000 sparta-spanner-0.0.5/src/sparta_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-01 13:51:40.000000 sparta-spanner-0.0.5/src/sparta_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 13:51:40.000000 sparta-spanner-0.0.5/src/sparta_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-01 13:51:40.000000 sparta-spanner-0.0.5/src/sparta_spanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-01 13:51:40.000000 sparta-spanner-0.0.5/src/sparta_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-01 13:51:40.000000 sparta-spanner-0.0.5/src/sparta_spanner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.892651 sparta-spanner-0.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.892651 sparta-spanner-0.0.6/src/sparta/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.892651 sparta-spanner-0.0.6/src/sparta/spanner/
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/service.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/top_level.txt
```

### Comparing `sparta-spanner-0.0.5/LICENSE` & `sparta-spanner-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.5/PKG-INFO` & `sparta-spanner-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-spanner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sparta spanner library
 Home-page: https://github.com/Spartan-Approach/sparta-spanner
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sparta-spanner-0.0.5/README.md` & `sparta-spanner-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.5/setup.py` & `sparta-spanner-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.5/src/sparta/spanner/concurrency.py` & `sparta-spanner-0.0.6/src/sparta/spanner/concurrency.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.5/src/sparta/spanner/metadata.py` & `sparta-spanner-0.0.6/src/sparta/spanner/metadata.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.5/src/sparta/spanner/service.py` & `sparta-spanner-0.0.6/src/sparta/spanner/service.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.5/src/sparta/spanner/utils.py` & `sparta-spanner-0.0.6/src/sparta/spanner/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,39 @@
     for row in result_set:
         if field_names is None:
             field_names = [field.name for field in result_set.fields]
         _results.append(dict(zip(field_names, row)))
     return _results
 
 
+def zip_first_result(
+    result_set: StreamedResultSet, field_names: typing.List[str] = None
+) -> typing.Optional[dict]:
+    """
+    :param result_set: the results
+    :param field_names: list of field names. If none is provided, then we use the column names.
+    :return: a single dict zipped with {field_name/column_name: column_value} or None
+    """
+    for row in result_set:
+        if field_names is None:
+            field_names = [field.name for field in result_set.fields]
+        return dict(zip(field_names, row))
+    return None
+
+
+def single_result(result_set: StreamedResultSet) -> typing.Optional[typing.Any]:
+    """
+    :param result_set: the results
+    :return: the first column value of the first row or None
+    """
+    for row in result_set:
+        return row[0]
+    return None
+
+
 def _sanitize_value(v: typing.Any):
     if isinstance(v, dict):
         return JsonObject(v)
     return v
 
 
 def _resolve_type(v: typing.Any) -> Type:
@@ -37,17 +62,17 @@
         return param_types.STRING
     if isinstance(v, (datetime.datetime, DatetimeWithNanoseconds)):
         return param_types.TIMESTAMP
     if isinstance(v, datetime.date):
         return param_types.DATE
     if isinstance(v, dict):
         return param_types.JSON
-    if isinstance(v, list):
+    if isinstance(v, (list, set, tuple)):
         if not len(v):
-            raise ValueError(f"Cannot resolve type of empty list")
+            raise ValueError(f"Cannot resolve type of empty list/set/tuple")
         item_type = _resolve_type(v[0])
         return param_types.Array(item_type)
     raise ValueError(f"Unsupported type {type(v)}")
 
 
 def build_params_ptypes(
     values: dict,
```

### Comparing `sparta-spanner-0.0.5/src/sparta/spanner/wrapper.py` & `sparta-spanner-0.0.6/src/sparta/spanner/wrapper.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.5/src/sparta_spanner.egg-info/PKG-INFO` & `sparta-spanner-0.0.6/src/sparta_spanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-spanner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sparta spanner library
 Home-page: https://github.com/Spartan-Approach/sparta-spanner
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```


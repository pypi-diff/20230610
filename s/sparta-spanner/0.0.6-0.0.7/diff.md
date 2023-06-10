# Comparing `tmp/sparta-spanner-0.0.6.tar.gz` & `tmp/sparta-spanner-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparta-spanner-0.0.6.tar", last modified: Sat Jun 10 10:23:31 2023, max compression
+gzip compressed data, was "sparta-spanner-0.0.7.tar", last modified: Sat Jun 10 11:58:22 2023, max compression
```

## Comparing `sparta-spanner-0.0.6.tar` & `sparta-spanner-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1619 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1202 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1648 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.892651 sparta-spanner-0.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.892651 sparta-spanner-0.0.6/src/sparta/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.892651 sparta-spanner-0.0.6/src/sparta/spanner/
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/service.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/utils.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-06-10 10:23:03.000000 sparta-spanner-0.0.6/src/sparta/spanner/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 10:23:31.896652 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1619 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 10:23:31.000000 sparta-spanner-0.0.6/src/sparta_spanner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:58:22.674958 sparta-spanner-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-06-10 11:58:22.674958 sparta-spanner-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 11:58:22.674958 sparta-spanner-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:58:22.670958 sparta-spanner-0.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:58:22.670958 sparta-spanner-0.0.7/src/sparta/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/src/sparta/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:58:22.674958 sparta-spanner-0.0.7/src/sparta/spanner/
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/src/sparta/spanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/src/sparta/spanner/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/src/sparta/spanner/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/src/sparta/spanner/service.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/src/sparta/spanner/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-06-10 11:57:54.000000 sparta-spanner-0.0.7/src/sparta/spanner/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 11:58:22.674958 sparta-spanner-0.0.7/src/sparta_spanner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-06-10 11:58:22.000000 sparta-spanner-0.0.7/src/sparta_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-10 11:58:22.000000 sparta-spanner-0.0.7/src/sparta_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 11:58:22.000000 sparta-spanner-0.0.7/src/sparta_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 11:58:22.000000 sparta-spanner-0.0.7/src/sparta_spanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-10 11:58:22.000000 sparta-spanner-0.0.7/src/sparta_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 11:58:22.000000 sparta-spanner-0.0.7/src/sparta_spanner.egg-info/top_level.txt
```

### Comparing `sparta-spanner-0.0.6/LICENSE` & `sparta-spanner-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.6/PKG-INFO` & `sparta-spanner-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-spanner
-Version: 0.0.6
+Version: 0.0.7
 Summary: Sparta spanner library
 Home-page: https://github.com/Spartan-Approach/sparta-spanner
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sparta-spanner-0.0.6/README.md` & `sparta-spanner-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.6/setup.py` & `sparta-spanner-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.6/src/sparta/spanner/concurrency.py` & `sparta-spanner-0.0.7/src/sparta/spanner/concurrency.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.6/src/sparta/spanner/metadata.py` & `sparta-spanner-0.0.7/src/sparta/spanner/metadata.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.6/src/sparta/spanner/service.py` & `sparta-spanner-0.0.7/src/sparta/spanner/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             )
 
         # Create client
         self.spanner_client = spanner.Client()
         self.instance = self.spanner_client.instance(instance_id)
         self.database = self.instance.database(database_id, pool=_pool)
 
-        self.logger.info(
+        self.logger.debug(
             f"Created {type(self).__name__} for {project_id}/{instance_id}/{database_id}"
         )
 
     def ping(self):
         self.execute_sql("SELECT 1")
 
     def execute_sql(self, *arg, **kwarg):
```

### Comparing `sparta-spanner-0.0.6/src/sparta/spanner/utils.py` & `sparta-spanner-0.0.7/src/sparta/spanner/utils.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.6/src/sparta/spanner/wrapper.py` & `sparta-spanner-0.0.7/src/sparta/spanner/wrapper.py`

 * *Files identical despite different names*

### Comparing `sparta-spanner-0.0.6/src/sparta_spanner.egg-info/PKG-INFO` & `sparta-spanner-0.0.7/src/sparta_spanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-spanner
-Version: 0.0.6
+Version: 0.0.7
 Summary: Sparta spanner library
 Home-page: https://github.com/Spartan-Approach/sparta-spanner
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```


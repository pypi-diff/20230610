# Comparing `tmp/pyfiredb-0.0.1.tar.gz` & `tmp/pyfiredb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfiredb-0.0.1.tar", last modified: Fri Jun  9 02:20:40 2023, max compression
+gzip compressed data, was "pyfiredb-0.0.2.tar", last modified: Sat Jun 10 21:40:37 2023, max compression
```

## Comparing `pyfiredb-0.0.1.tar` & `pyfiredb-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-09 02:20:40.555122 pyfiredb-0.0.1/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 pyfiredb-0.0.1/LICENSE.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-09 02:20:40.555122 pyfiredb-0.0.1/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)     1295 2023-06-09 02:20:03.000000 pyfiredb-0.0.1/README.md
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-09 02:20:40.555122 pyfiredb-0.0.1/pyfiredb/
--rw-rw-r--   0 andres    (1000) andres    (1000)      128 2023-06-09 02:15:32.000000 pyfiredb-0.0.1/pyfiredb/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1536 2023-06-09 01:08:29.000000 pyfiredb-0.0.1/pyfiredb/database.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      666 2023-06-09 00:39:10.000000 pyfiredb-0.0.1/pyfiredb/session.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      257 2023-06-09 02:15:35.000000 pyfiredb-0.0.1/pyfiredb/settings.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-09 02:20:40.555122 pyfiredb-0.0.1/pyfiredb.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-09 02:20:40.000000 pyfiredb-0.0.1/pyfiredb.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      272 2023-06-09 02:20:40.000000 pyfiredb-0.0.1/pyfiredb.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-09 02:20:40.000000 pyfiredb-0.0.1/pyfiredb.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-09 02:20:40.000000 pyfiredb-0.0.1/pyfiredb.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-09 02:20:40.000000 pyfiredb-0.0.1/pyfiredb.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-09 02:20:40.555122 pyfiredb-0.0.1/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)     1089 2023-06-09 02:20:22.000000 pyfiredb-0.0.1/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-10 21:40:37.672865 pyfiredb-0.0.2/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 pyfiredb-0.0.2/LICENSE.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-10 21:40:37.672865 pyfiredb-0.0.2/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1295 2023-06-09 02:20:03.000000 pyfiredb-0.0.2/README.md
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-10 21:40:37.672865 pyfiredb-0.0.2/pyfiredb/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      128 2023-06-09 02:15:32.000000 pyfiredb-0.0.2/pyfiredb/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1837 2023-06-09 22:37:43.000000 pyfiredb-0.0.2/pyfiredb/database.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      666 2023-06-09 00:39:10.000000 pyfiredb-0.0.2/pyfiredb/session.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      299 2023-06-09 21:36:30.000000 pyfiredb-0.0.2/pyfiredb/settings.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-10 21:40:37.672865 pyfiredb-0.0.2/pyfiredb.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-10 21:40:37.000000 pyfiredb-0.0.2/pyfiredb.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      272 2023-06-10 21:40:37.000000 pyfiredb-0.0.2/pyfiredb.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-10 21:40:37.000000 pyfiredb-0.0.2/pyfiredb.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-10 21:40:37.000000 pyfiredb-0.0.2/pyfiredb.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-10 21:40:37.000000 pyfiredb-0.0.2/pyfiredb.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-10 21:40:37.672865 pyfiredb-0.0.2/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1089 2023-06-10 21:39:26.000000 pyfiredb-0.0.2/setup.py
```

### Comparing `pyfiredb-0.0.1/LICENSE.txt` & `pyfiredb-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.1/PKG-INFO` & `pyfiredb-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfiredb
-Version: 0.0.1
+Version: 0.0.2
 Summary: pyfire is a package that simplifies querying with Pyrebase,    making interactions with Firebase databases effortless.
 Home-page: https://github.com/andresroh/pyfire
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
```

### Comparing `pyfiredb-0.0.1/README.md` & `pyfiredb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.1/pyfiredb/database.py` & `pyfiredb-0.0.2/pyfiredb/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,30 +23,38 @@
         session.db.update(data)
 
     def get(self, path) -> tuple:
         session = self.session
         result = session.db.child(path).get(session.login['idToken']).val()
         return tuple(dict(result).values())
 
-    def equal(self, path, param, equal_to) -> tuple:
+    def equal(self, path, param, equal_to) -> dict:
 
         session = self.session
         result = session.db.child(path).order_by_child(param).equal_to(
             equal_to).get(session.login['idToken']).val()
-
-        return tuple(dict(result).values())
+        if result:
+            return list(dict(result).values())[0]
+        return {}
 
     def between(self, path, param, start, end) -> tuple:
 
         session = self.session
         result = session.db.child(path).order_by_child(param).start_at(
             start).end_at(end).get(session.login['idToken']).val()
 
         return tuple(dict(result).values())
 
-    def max(self, path, param) -> tuple:
+    def max(self, path, param, equal_to=False) -> dict:
 
         session = self.session
-        result = session.db.child(path).order_by_child(param).limit_to_last(
-            1).get(self.login['idToken']).val()
 
-        return tuple(dict(result).values())
+        if equal_to:
+            result = session.db.child(path).order_by_child(param).equal_to(
+                equal_to).limit_to_last(1).get(session.login['idToken']).val()
+        else:
+            result = session.db.child(path).order_by_child(
+                param).limit_to_last(1).get(session.login['idToken']).val()
+
+        if result:
+            return list(dict(result).values())[0]
+        return {}
```

### Comparing `pyfiredb-0.0.1/pyfiredb/session.py` & `pyfiredb-0.0.2/pyfiredb/session.py`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.1/pyfiredb.egg-info/PKG-INFO` & `pyfiredb-0.0.2/pyfiredb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfiredb
-Version: 0.0.1
+Version: 0.0.2
 Summary: pyfire is a package that simplifies querying with Pyrebase,    making interactions with Firebase databases effortless.
 Home-page: https://github.com/andresroh/pyfire
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
```

### Comparing `pyfiredb-0.0.1/setup.py` & `pyfiredb-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'pyfire is a package that simplifies querying with Pyrebase,\
     making interactions with Firebase databases effortless.'
 PACKAGE_NAME = 'pyfiredb'
 AUTHOR = 'Camilo Andrés Rodríguez'
 EMAIL = 'andres.roh@gmail.com'
 GITHUB_URL = 'https://github.com/andresroh/pyfire'
```


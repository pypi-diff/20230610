# Comparing `tmp/pystorz-0.3.3.tar.gz` & `tmp/pystorz-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorz-0.3.3.tar", last modified: Fri Jun  9 19:50:16 2023, max compression
+gzip compressed data, was "pystorz-0.3.4.tar", last modified: Sat Jun 10 16:54:26 2023, max compression
```

## Comparing `pystorz-0.3.3.tar` & `pystorz-0.3.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.908916 pystorz-0.3.3/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.3/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-09 19:50:16.908727 pystorz-0.3.3/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.3/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.899392 pystorz-0.3.3/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.3/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.900287 pystorz-0.3.3/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.3/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.900806 pystorz-0.3.3/pystorz/meta/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:40.000000 pystorz-0.3.3/pystorz/meta/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.3.3/pystorz/meta/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.902210 pystorz-0.3.3/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.3/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4164 2023-06-05 18:53:35.000000 pystorz-0.3.3/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.3/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.904196 pystorz-0.3.3/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.3/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.3/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.3/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.3/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.3/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.3/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.906020 pystorz-0.3.3/pystorz/rest/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:44.000000 pystorz-0.3.3/pystorz/rest/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/rest/client.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.3/pystorz/rest/headers.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/rest/internals.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.3/pystorz/rest/server.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.906432 pystorz-0.3.3/pystorz/router/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:42.000000 pystorz-0.3.3/pystorz/router/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2344 2023-06-06 17:21:47.000000 pystorz-0.3.3/pystorz/router/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.907350 pystorz-0.3.3/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.3/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2617 2023-06-09 19:48:52.000000 pystorz-0.3.3/pystorz/sql/mysql.py
--rw-r--r--   0 wazofski   (501) staff       (20)      192 2023-06-04 16:07:46.000000 pystorz-0.3.3/pystorz/sql/sqlite.py
--rw-r--r--   0 wazofski   (501) staff       (20)    15493 2023-06-09 19:44:00.000000 pystorz-0.3.3/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.908463 pystorz-0.3.3/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.3/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.3/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.3/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.3/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-09 19:50:16.900058 pystorz-0.3.3/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1081 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)      128 2023-06-09 19:50:16.000000 pystorz-0.3.3/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-09 19:50:16.908959 pystorz-0.3.3/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)     1316 2023-06-09 19:48:07.000000 pystorz-0.3.3/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.490068 pystorz-0.3.4/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.4/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-10 16:54:26.489895 pystorz-0.3.4/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.4/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.481989 pystorz-0.3.4/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.4/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.482869 pystorz-0.3.4/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.4/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.483231 pystorz-0.3.4/pystorz/meta/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:40.000000 pystorz-0.3.4/pystorz/meta/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.3.4/pystorz/meta/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.484578 pystorz-0.3.4/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.4/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4164 2023-06-05 18:53:35.000000 pystorz-0.3.4/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.4/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.486153 pystorz-0.3.4/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.4/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.4/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.4/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.4/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.4/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.487190 pystorz-0.3.4/pystorz/rest/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:44.000000 pystorz-0.3.4/pystorz/rest/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/rest/client.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.4/pystorz/rest/headers.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/rest/internals.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.4/pystorz/rest/server.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.487536 pystorz-0.3.4/pystorz/router/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:42.000000 pystorz-0.3.4/pystorz/router/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2344 2023-06-06 17:21:47.000000 pystorz-0.3.4/pystorz/router/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.488422 pystorz-0.3.4/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.4/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2734 2023-06-10 16:53:04.000000 pystorz-0.3.4/pystorz/sql/mysql.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      192 2023-06-04 16:07:46.000000 pystorz-0.3.4/pystorz/sql/sqlite.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    15493 2023-06-09 19:44:00.000000 pystorz-0.3.4/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.489631 pystorz-0.3.4/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.4/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.4/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.4/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.482648 pystorz-0.3.4/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1081 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)      128 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-10 16:54:26.490149 pystorz-0.3.4/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)     1316 2023-06-10 16:53:46.000000 pystorz-0.3.4/setup.py
```

### Comparing `pystorz-0.3.3/LICENSE` & `pystorz-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/PKG-INFO` & `pystorz-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.3.3/README.md` & `pystorz-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/meta/store.py` & `pystorz-0.3.4/pystorz/meta/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/mgen/builder.py` & `pystorz-0.3.4/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/mgen/loader.py` & `pystorz-0.3.4/pystorz/mgen/loader.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/mgen/templates/structure.py` & `pystorz-0.3.4/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.3.4/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/mgen/test.py` & `pystorz-0.3.4/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/mgen/utils.py` & `pystorz-0.3.4/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/rest/client.py` & `pystorz-0.3.4/pystorz/rest/client.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/rest/headers.py` & `pystorz-0.3.4/pystorz/rest/headers.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/rest/internals.py` & `pystorz-0.3.4/pystorz/rest/internals.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/rest/server.py` & `pystorz-0.3.4/pystorz/rest/server.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/router/store.py` & `pystorz-0.3.4/pystorz/router/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/sql/mysql.py` & `pystorz-0.3.4/pystorz/sql/mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,19 @@
             
             if self._cursor is None:
                 self._cursor = self.connection.cursor()
 
             return self._cursor
         except Exception as err:
             log.error("cursor", err)
-            raise err
+            if self.connection is None:
+                raise err
+            self.connection = None
+        
+        return self.cursor()
 
     def close(self):
         try:
             if self._cursor:
                 self._cursor.close()
             if self.connection:
                 self.connection.close()
```

### Comparing `pystorz-0.3.3/pystorz/sql/store.py` & `pystorz-0.3.4/pystorz/sql/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/store/meta.py` & `pystorz-0.3.4/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/store/options.py` & `pystorz-0.3.4/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/store/store.py` & `pystorz-0.3.4/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz/store/utils.py` & `pystorz-0.3.4/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/pystorz.egg-info/PKG-INFO` & `pystorz-0.3.4/pystorz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.3.3/pystorz.egg-info/SOURCES.txt` & `pystorz-0.3.4/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.3/setup.py` & `pystorz-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.3.3',
+    version='0.3.4',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```


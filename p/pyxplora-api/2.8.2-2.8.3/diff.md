# Comparing `tmp/pyxplora_api-2.8.2.tar.gz` & `tmp/pyxplora_api-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxplora_api-2.8.2.tar", last modified: Thu Jun  8 02:40:44 2023, max compression
+gzip compressed data, was "pyxplora_api-2.8.3.tar", last modified: Sat Jun 10 09:35:41 2023, max compression
```

## Comparing `pyxplora_api-2.8.2.tar` & `pyxplora_api-2.8.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.771526 pyxplora_api-2.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-08 02:40:44.771526 pyxplora_api-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 02:40:44.771526 pyxplora_api-2.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.767526 pyxplora_api-2.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.767526 pyxplora_api-2.8.2/src/pyxplora_api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/const_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    44320 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_handler_async.py
--rw-r--r--   0 runner    (1001) docker     (123)   118669 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)    64798 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/graphql_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/handler_gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/pyxplora.py
--rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30154 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.767526 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.424478 pyxplora_api-2.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/src/pyxplora_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/const_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44320 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_handler_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118669 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64798 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/graphql_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/handler_gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/pyxplora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30909 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/top_level.txt
```

### Comparing `pyxplora_api-2.8.2/LICENSE` & `pyxplora_api-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/PKG-INFO` & `pyxplora_api-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxplora_api
-Version: 2.8.2
+Version: 2.8.3
 Summary: Python Xplora® Api
 Home-page: https://github.com/Ludy87/pyxplora_api
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyxplora_api/issues
 Keywords: api xplora watch
```

### Comparing `pyxplora_api-2.8.2/README.md` & `pyxplora_api-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/setup.py` & `pyxplora_api-2.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/exception_classes.py` & `pyxplora_api-2.8.3/src/pyxplora_api/exception_classes.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/gql_handler.py` & `pyxplora_api-2.8.3/src/pyxplora_api/gql_handler.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/gql_handler_async.py` & `pyxplora_api-2.8.3/src/pyxplora_api/gql_handler_async.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/gql_mutations.py` & `pyxplora_api-2.8.3/src/pyxplora_api/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/gql_queries.py` & `pyxplora_api-2.8.3/src/pyxplora_api/gql_queries.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/graphql_client.py` & `pyxplora_api-2.8.3/src/pyxplora_api/graphql_client.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/handler_gql.py` & `pyxplora_api-2.8.3/src/pyxplora_api/handler_gql.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/model.py` & `pyxplora_api-2.8.3/src/pyxplora_api/model.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/pyxplora.py` & `pyxplora_api-2.8.3/src/pyxplora_api/pyxplora.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api.py` & `pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api_async.py` & `pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,14 +713,32 @@
 
     async def get_chat_voice(self, wuid: str, msgId: str):
         data = await self._gql_handler.fetchChatVoice_a(wuid, msgId)
         if data.get("fetchChatVoice"):
             return data.get("fetchChatVoice")
         return None
 
+    async def get_chat_image(self, wuid: str, msgId: str):
+        data = await self._gql_handler.fetchChatImage_a(wuid, msgId)
+        if data.get("fetchChatImage"):
+            return data.get("fetchChatImage")
+        return None
+
+    async def get_short_video(self, wuid: str, msgId: str):
+        data = await self._gql_handler.fetchChatShortVideo_a(wuid, msgId)
+        if data.get("fetchChatShortVideo"):
+            return data.get("fetchChatShortVideo")
+        return None
+
+    async def get_short_video_cover(self, wuid: str, msgId: str):
+        data = await self._gql_handler.fetchChatShortVideoCover_a(wuid, msgId)
+        if data.get("fetchChatShortVideoCover"):
+            return data.get("fetchChatShortVideoCover")
+        return None
+
     async def set_read_chat_msg(self, wuid: str, msgId: str = "", id: str = ""):
         data = await self._gql_handler.setReadChatMsg_a(wuid, msgId, id)
         return data
 
     async def refresh_token(self, wuid: str, refresh_token: str = ""):
         data = await self._gql_handler.refresh_token_a(wuid, self._refresh_token)
         return data.get("refreshToken", None)
```

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api/status.py` & `pyxplora_api-2.8.3/src/pyxplora_api/status.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api.egg-info/PKG-INFO` & `pyxplora_api-2.8.3/src/pyxplora_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxplora-api
-Version: 2.8.2
+Version: 2.8.3
 Summary: Python Xplora® Api
 Home-page: https://github.com/Ludy87/pyxplora_api
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyxplora_api/issues
 Keywords: api xplora watch
```

### Comparing `pyxplora_api-2.8.2/src/pyxplora_api.egg-info/SOURCES.txt` & `pyxplora_api-2.8.3/src/pyxplora_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*


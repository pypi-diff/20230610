# Comparing `tmp/heaven-0.0.2.tar.gz` & `tmp/heaven-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.2.tar", max compression
+gzip compressed data, was "heaven-0.0.3.tar", max compression
```

## Comparing `heaven-0.0.2.tar` & `heaven-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.2/LICENSE
--rw-r--r--   0        0        0     1312 2023-05-03 15:13:50.357871 heaven-0.0.2/README.md
--rw-r--r--   0        0        0      216 2023-06-01 15:02:47.533018 heaven-0.0.2/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-04-04 16:11:34.731647 heaven-0.0.2/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-04-04 16:11:34.731908 heaven-0.0.2/heaven/context.py
--rw-r--r--   0        0        0      141 2023-04-04 16:11:34.732086 heaven-0.0.2/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-05-03 15:18:16.753088 heaven-0.0.2/heaven/form.py
--rw-r--r--   0        0        0     2920 2023-05-03 15:18:08.445234 heaven-0.0.2/heaven/mocks.py
--rw-r--r--   0        0        0     3188 2023-05-04 09:15:57.271144 heaven-0.0.2/heaven/request.py
--rw-r--r--   0        0        0     2830 2023-05-03 15:15:09.488292 heaven-0.0.2/heaven/response.py
--rw-r--r--   0        0        0    19425 2023-06-01 15:02:38.459653 heaven-0.0.2/heaven/router.py
--rw-r--r--   0        0        0        0 2023-04-04 16:11:34.733604 heaven-0.0.2/heaven/server.py
--rw-r--r--   0        0        0      926 2023-04-04 16:11:34.734047 heaven-0.0.2/heaven/utils.py
--rw-r--r--   0        0        0      467 2023-06-01 15:03:12.819675 heaven-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 heaven-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1312 2023-06-10 13:10:30.152074 heaven-0.0.3/README.md
+-rw-r--r--   0        0        0      216 2023-06-10 13:11:18.625084 heaven-0.0.3/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.3/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.3/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.3/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.3/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.3/heaven/mocks.py
+-rw-r--r--   0        0        0     3188 2023-06-10 13:10:30.157851 heaven-0.0.3/heaven/request.py
+-rw-r--r--   0        0        0     3999 2023-06-10 13:10:30.158043 heaven-0.0.3/heaven/response.py
+-rw-r--r--   0        0        0    20838 2023-06-10 13:10:30.158327 heaven-0.0.3/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.3/heaven/server.py
+-rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.3/heaven/tutorials.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.3/heaven/utils.py
+-rw-r--r--   0        0        0      485 2023-06-10 13:12:13.066504 heaven-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 heaven-0.0.3/PKG-INFO
```

### Comparing `heaven-0.0.2/LICENSE` & `heaven-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.2/README.md` & `heaven-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.0.2/heaven/constants.py` & `heaven-0.0.3/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.2/heaven/form.py` & `heaven-0.0.3/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.2/heaven/mocks.py` & `heaven-0.0.3/heaven/mocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,9 +90,9 @@
         scope['headers'] = _listify_headers(headers)
         scope['query_string'] = query_string
         metadata = subdomain, headers or {}
         super().__init__(scope, body, receive, metadata=metadata)
 
 
 class MockResponse(Response):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, app, context):
+        super().__init__(app, context)
```

### Comparing `heaven-0.0.2/heaven/request.py` & `heaven-0.0.3/heaven/request.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.2/heaven/router.py` & `heaven-0.0.3/heaven/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from asyncio import gather
 from collections import deque
 from functools import wraps
+from http import HTTPStatus
 from inspect import iscoroutinefunction
+from os import path, getcwd
+
+from aiofiles import open as async_open_file
+from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 from typing import Callable
 
 from .constants import (
     CONNECT,
     DEFAULT,
     DELETE,
@@ -214,16 +219,16 @@
         more = True
         while more:
             msg = await receive()
             body += msg.get('body', b'')
             more = msg.get('more_body', False)
 
         r = Request(scope, body, receive, metadata, application)
-        w = Response()
         c = Context(application)
+        w = Response(context=c, app=application)
 
         method = scope.get('method')
         matched = None
         handler = None
 
         # if the cache has nothing under its GET, POST etc it means nothing's been registered and we can leave early
         roots = self.cache.get(method, {})
@@ -319,14 +324,15 @@
         self.finalized = False
         self.initializers = deque()
         self.deinitializers = deque()
         self.subdomains = {}
         self.subdomains[DEFAULT] = Routes()
         self._buckets = {}
         self._configuration = _get_configuration(configurator)
+        self._templater = None
 
     async def __call__(self, scope, receive, send):
         if scope['type'] == 'lifespan':
             while True:
                 message = await receive()
                 if message['type'] == 'lifespan.startup':
                     try: await self._register()
@@ -434,14 +440,35 @@
 
             try: assert isinstance(second, Callable)
             except AssertionError: raise TypeError(error_message)
 
             if first.lower() == STARTUP: self.initializers.append(closure(second))
             else: self.deinitializers.append(closure(second))
 
+    def TEMPLATES(self, folder: str, escape=None, asynchronous=True):
+        files_to_escape = escape or ['htm', 'html']
+        file_system_loader = FileSystemLoader(path.join(getcwd(), folder))
+        environment = Environment(loader=file_system_loader, autoescape=select_autoescape(files_to_escape))
+        environment.is_async = asynchronous
+        self._templater = environment
+
+    def ASSETS(self, folder: str, route='/public/*', subdomain=DEFAULT):
+        async def serve_assets(req: Request, res: Response, ctx: Context):
+            static_asset = f"{req.params.get('*', '')}"
+            remove_symlinks_if_present = path.realpath(getcwd())
+            location = path.join(remove_symlinks_if_present, f'{folder}')
+            target_resource_path = path.join(location, static_asset)
+            try:
+                async with async_open_file(target_resource_path, 'rb') as opened_asset_file:
+                    res.body = b''.join(await opened_asset_file.readlines())
+            except Exception as exc:
+                print(exc)
+                res.status = HTTPStatus.INTERNAL_SERVER_ERROR
+        self.GET(route, serve_assets, subdomain)
+
     async def _register(self):
         i = len(self.initializers)
         while self.initializers:
             initializer, c = self.initializers.popleft(), len(self.initializers)
             index = i - c
             print(f'({index}): ', initializer.__name__, '\n')
             if iscoroutinefunction(initializer): await initializer(self)
@@ -451,15 +478,15 @@
         i = len(self.deinitializers)
         while self.deinitializers:
             deinitializer, c = self.deinitializers.popleft(), len(self.deinitializers)
             index = i - c
             print(f'({index}): ', deinitializer.__name__, '\n')
             if iscoroutinefunction(deinitializer): await deinitializer(self)
             else: deinitializer(self)
-    
+
     def keep(self, key, value):
         self._buckets[key] = value
 
     def unkeep(self, key):
         value = self._buckets[key]
         del self._buckets[key]
         return value
```

### Comparing `heaven-0.0.2/heaven/utils.py` & `heaven-0.0.3/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.2/PKG-INFO` & `heaven-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jinja2 (>=3.1.0,<4.0.0)
 Requires-Dist: uvicorn (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # Routerling : <img src="https://img.shields.io/badge/coverage-95%25-green" />
 
 Routerling is a very very small, extremely tiny, and insanely fast [ASGI](https://asgi.readthedocs.io) web application framework. It was designed to facilitate productivity by allowing for complete mastery in 7 minutes or less.
```


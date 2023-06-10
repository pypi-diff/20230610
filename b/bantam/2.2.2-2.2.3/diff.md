# Comparing `tmp/bantam-2.2.2.tar.gz` & `tmp/bantam-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.2.2.tar", last modified: Mon Jun  5 00:33:32 2023, max compression
+gzip compressed data, was "bantam-2.2.3.tar", last modified: Sat Jun 10 17:04:08 2023, max compression
```

## Comparing `bantam-2.2.2.tar` & `bantam-2.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-05 00:33:32.454154 bantam-2.2.2/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.2/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.2/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-05 00:33:32.454154 bantam-2.2.2/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-05 00:23:53.000000 bantam-2.2.2/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.450154 bantam-2.2.2/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.450154 bantam-2.2.2/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.2/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    10547 2023-06-04 23:41:07.000000 bantam-2.2.2/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.2/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.2/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    19764 2023-06-04 23:29:54.000000 bantam-2.2.2/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.2/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.2.2/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    45348 2023-06-05 00:08:58.000000 bantam-2.2.2/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.2/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.2/src/bantam/js_async.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.2/src/bantam/pythonclient.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-05 00:33:32.000000 bantam-2.2.2/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 00:33:32.454154 bantam-2.2.2/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4472 2023-06-04 02:18:21.000000 bantam-2.2.2/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4636 2023-06-05 00:12:39.000000 bantam-2.2.2/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4573 2023-06-04 14:26:39.000000 bantam-2.2.2/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.2/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.2/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.2/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     7531 2023-06-03 15:33:20.000000 bantam-2.2.2/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2845 2023-06-04 03:14:39.000000 bantam-2.2.2/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 17:04:08.646937 bantam-2.2.3/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.2.3/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-03 15:15:17.000000 bantam-2.2.3/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-10 17:04:08.646937 bantam-2.2.3/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-10 17:03:19.000000 bantam-2.2.3/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4011 2023-06-04 04:49:42.000000 bantam-2.2.3/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    10547 2023-06-04 23:41:07.000000 bantam-2.2.3/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.2.3/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.2.3/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20981 2023-06-10 16:40:12.000000 bantam-2.2.3/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5520 2023-06-04 02:57:43.000000 bantam-2.2.3/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.2.3/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    45360 2023-06-10 16:04:45.000000 bantam-2.2.3/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22133 2023-06-04 14:44:14.000000 bantam-2.2.3/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.2.3/src/bantam/js_async.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    13103 2023-06-03 15:15:17.000000 bantam-2.2.3/src/bantam/pythonclient.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      699 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       28 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-10 17:04:08.000000 bantam-2.2.3/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 17:04:08.646937 bantam-2.2.3/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4785 2023-06-10 04:24:24.000000 bantam-2.2.3/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4634 2023-06-10 04:24:36.000000 bantam-2.2.3/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4942 2023-06-10 04:23:32.000000 bantam-2.2.3/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.2.3/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.2.3/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.2.3/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3254 2023-06-10 16:56:43.000000 bantam-2.2.3/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.2.3/test/test_js_async.py
```

### Comparing `bantam-2.2.2/PKG-INFO` & `bantam-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.2
+Version: 2.2.3
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.2
+Download-URL: https://github.com/bantam/dist/2.2.3
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.2/setup.py` & `bantam-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.2.2"
+VERSION = "2.2.3"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.2.2/src/bantam/__init__.py` & `bantam-2.2.3/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam/api.py` & `bantam-2.2.3/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam/autogen/main.py` & `bantam-2.2.3/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam/client.py` & `bantam-2.2.3/src/bantam/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,30 +80,31 @@
 ...              yield text
 ...
 
 One can then declare a Client that acts as a proxy to make calls to the server, thereby keeping the
 http protocol details hidden (abstracted away frm the user):
 
 >>>  def async_call():
-...      client = MyServerApiInterface.Client(end_point='https://blahblahblah')
-...      instance = await client.constructor()
+...      client_end_point_mapping = MyServerApiInterface.ClientEndpointMapping()
+...      client = await client_end_point_mapping['https://blahblahblah']
+...      instance = client.constructor()
 ...      async for text in instance.instance_method_api():
 ...          print(text)
 ...
 
 If you do not fallow the recommended practice of the interface have the same name as the concreate class, only with
 an "Interface" suffix, you will have to specify *impl_name=<name-of-concrete-class>* as a parameter to Client class
 method above.  The *end_point* parameter specifies the base url to the server that serves up MyServceApi class.
 
 """
 import inspect
 import json
 from abc import ABC
 from functools import wraps
-from typing import Any, Dict, TypeVar, Optional, Type, AsyncIterator, Generic
+from typing import Any, Dict, TypeVar, Optional, Type, AsyncIterator, Generic, Mapping, Iterator
 
 import aiohttp
 
 from bantam import conversions
 from bantam.api import API, RestMethod
 
 __all__ = ["WebInterface"]
@@ -210,15 +211,15 @@
                 url = f"{base_url}{url_args}"
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.get(url) as resp:
                         resp.raise_for_status()
                         buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             if data:
-                                if api.return_type == str:
+                                if api.return_type != bytes:
                                     buffer += data.decode('utf-8')
                                     *data_items, buffer = buffer.split('\0')
                                     for datum in data_items:
                                         yield conversions.from_str(datum, api.return_type)
                                 else:
                                     data = data.decode('utf-8')
                                     yield conversions.from_str(data, api.return_type)
@@ -227,15 +228,15 @@
                                       for k, v in kwargs.items()})
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.post(base_url, data=payload) as resp:
                         buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             resp.raise_for_status()
                             if data:
-                                if api.return_type == str:
+                                if api.return_type != bytes:
                                     buffer += data.decode('utf-8')
                                     *data_items, buffer = buffer.split('\0')
                                     for datum in data_items:
                                         yield conversions.from_str(datum, api.return_type)
                                 else:
                                     data = data.decode('utf-8')
                                     yield conversions.from_str(data, api.return_type)
@@ -311,15 +312,15 @@
                 url = f"{base_url}{url_args}"
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.get(url) as resp:
                         resp.raise_for_status()
                         buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             if data:
-                                if api.return_type == str:
+                                if api.return_type != bytes:
                                     buffer += data.decode('utf-8')
                                     *data_items, buffer = buffer.split('\0')
                                     for datum in data_items:
                                         yield conversions.from_str(datum, api.return_type)
                                 else:
                                     data = data.decode('utf-8')
                                     yield conversions.from_str(data, api.return_type)
@@ -329,83 +330,102 @@
                 payload = json.dumps({k: conversions.to_str(v) for k, v in kwargs_.items()})
                 async with aiohttp.ClientSession(timeout=api.timeout, headers=common_headers) as session:
                     async with session.post(url, data=payload) as resp:
                         resp.raise_for_status()
                         buffer = ""
                         async for data, _ in resp.content.iter_chunks():
                             if data:
-                                if api.return_type == str:
+                                if api.return_type != bytes:
                                     buffer += data.decode('utf-8')
                                     *data_items, buffer = buffer.split('\0')
                                     for datum in data_items:
                                         yield conversions.from_str(datum, api.return_type)
                                 else:
                                     data = data.decode('utf-8')
                                     yield conversions.from_str(data, api.return_type)
         setattr(clazz, name, instance_method_streamed)
 
     # noinspection PyPep8Naming
     @classmethod
-    def Client(cls: C, end_point: str, impl_name: Optional[str] = None,
-               common_headers: Optional[dict] = None) -> C:
+    def ClientEndpointMapping(cls: C, impl_name: Optional[str] = None,
+                              common_headers: Optional[dict] = None) -> Mapping[str, C]:
         if cls == WebInterface:
             raise Exception("Must call Client with concrete class of WebInterface, not WebInterface itself")
         if impl_name is None:
             if not cls.__name__.endswith('Interface'):
                 raise Exception("Call to Client must specify impl_name explicitly since class name does not end in "
                                 "'Interface'")
             impl_name = cls.__name__[:-len('Interface')]
-        while end_point.endswith('/'):
-            end_point = end_point[:-1]
-        key = f"{cls.__name__}.{end_point}"
-        if key in WebInterface._clients:
-            return WebInterface._clients[key]
-
-        class Impl:
-
-            def __init__(self, self_id: str):
-                super().__init__()
-                self._id = self_id
-
-            @property
-            def self_id(self):
-                return self._id
-
-        non_class_methods = inspect.getmembers(cls, predicate=inspect.isfunction)
-        for name, method in non_class_methods:
-            if isinstance(inspect.getattr_static(cls, name), staticmethod):
-                if hasattr(method, '_bantam_web_api'):
-                    raise Exception(f"Static method {name} of {cls.__name__} cannot have @web_api decorator. "
-                                    "WebInterface's can only have instance and class methods that are @web_api's")
-                continue
-            if not inspect.iscoroutinefunction(method) and not inspect.isasyncgenfunction(method):
-                raise Exception(f"Function {name} of {cls.__name__} is not async as expected.")
-            if isinstance(inspect.getattr_static(cls, name), staticmethod):
-                raise Exception(f"Method {name} of {cls.__name__}")
-            else:
-                if inspect.isasyncgenfunction(method):
-                    cls._add_instance_method_streamed(Impl, impl_name, end_point, method, common_headers)
-                else:
-                    cls._add_instance_method(Impl, impl_name, end_point, method, common_headers)
-
-        class_methods = inspect.getmembers(cls, predicate=inspect.ismethod)
-        for name, method in class_methods:
-            if name == 'Client' or name.startswith('_'):
-                continue
-            if not inspect.iscoroutinefunction(method) and not inspect.isasyncgenfunction(method):
-                raise Exception(f"Function {name} of {cls.__name__} is not async as expected.")
-            if inspect.isasyncgenfunction(method):
-                cls._add_class_method_streamed(Impl, impl_name, end_point, method, common_headers)
-            else:
-                cls._add_class_method(Impl, impl_name, end_point, method, common_headers)
 
-        class ImplProper(Impl, Generic[C]):
-            """
-            provides proper typing on return value, without conflicting with Python's abstract class rules
-            which ignore dynamically added methods as above for the concrete implementations
-            """
+        class ClientFactory(Mapping[str, C]):
 
-            def __init__(self, *args, **kwargs):
-                Impl.__init__(self, *args, **kwargs)
+            def __iter__(self) -> Iterator[str]:
+                for key in [k for k in WebInterface._clients if k.startswith(cls.__name__)]:
+                    yield key
+
+            def __len__(self) -> int:
+                return len([k for k in WebInterface._clients if k.startswith(cls.__name__)])
+
+            @staticmethod
+            def add_dynamic_methods(clazz: Type, end_point: str):
+
+                non_class_methods = inspect.getmembers(cls, predicate=inspect.isfunction)
+                for name, method in non_class_methods:
+                    if isinstance(inspect.getattr_static(cls, name), staticmethod):
+                        if hasattr(method, '_bantam_web_api'):
+                            raise Exception(
+                                f"Static method {name} of {cls.__name__} cannot have @web_api decorator. "
+                                "WebInterface's can only have instance and class methods that are @web_api's")
+                        continue
+                    if not inspect.iscoroutinefunction(method) and not inspect.isasyncgenfunction(method):
+                        raise Exception(f"Function {name} of {cls.__name__} is not async as expected.")
+                    if isinstance(inspect.getattr_static(cls, name), staticmethod):
+                        raise Exception(f"Method {name} of {cls.__name__}")
+                    else:
+                        if inspect.isasyncgenfunction(method):
+                            cls._add_instance_method_streamed(clazz, impl_name, end_point, method, common_headers)
+                        else:
+                            cls._add_instance_method(clazz, impl_name, end_point, method, common_headers)
+
+                class_methods = inspect.getmembers(cls, predicate=inspect.ismethod)
+                for name, method in class_methods:
+                    if name == cls.ClientEndpointMapping.__name__ or name.startswith('_'):
+                        continue
+                    if not inspect.iscoroutinefunction(method) and not inspect.isasyncgenfunction(method):
+                        raise Exception(f"Function {name} of {cls.__name__} is not async as expected.")
+                    if inspect.isasyncgenfunction(method):
+                        cls._add_class_method_streamed(clazz, impl_name, end_point, method, common_headers)
+                    else:
+                        cls._add_class_method(clazz, impl_name, end_point, method, common_headers)
+
+            def __getitem__(self, end_point: str):
+                class Impl:
+
+                    def __init__(self, self_id: str):
+                        super().__init__()
+                        self._id = self_id
+
+                    @property
+                    def self_id(self):
+                        return self._id
+
+                class ImplProper(Impl, Generic[C]):
+                    """
+                    provides proper typing on return value, without conflicting with Python's abstract class rules
+                    which ignore dynamically added methods as above for the concrete implementations
+                    """
+
+                    def __init__(self, *args, **kwargs):
+                        Impl.__init__(self, *args, **kwargs)
+
+                while end_point.endswith('/'):
+                    end_point = end_point[:-1]
+                key = f"{cls.__name__}@{end_point}"
+                if key in WebInterface._clients:
+                    return WebInterface._clients[key]
+
+                if key not in WebInterface._clients:
+                    ClientFactory.add_dynamic_methods(Impl, end_point)
+                    WebInterface._clients[key] = ImplProper
+                return WebInterface._clients[key]
 
-        WebInterface._clients[key] = ImplProper[C]
-        return ImplProper[C]
+        return ClientFactory()
```

### Comparing `bantam-2.2.2/src/bantam/conversions.py` & `bantam-2.2.3/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam/decorators.py` & `bantam-2.2.3/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam/http.py` & `bantam-2.2.3/src/bantam/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,15 +692,15 @@
                 response = StreamResponse(status=200, reason='OK', headers={'Content-Type': content_type})
                 await response.prepare(request)
                 try:
                     # iterate to get the one (and hopefully only) yielded element:
                     # noinspection PyTypeChecker
                     async for res in result:
                         serialized = _serialize_return_value(res, encoding)
-                        if isinstance(res, str):
+                        if not isinstance(res, bytes):
                             serialized += b'\0'
                         await response.write(serialized)
                 except Exception as e:
                     print(str(e))
                     raise asyncio.CancelledError(f"Error in server-side logic: {e}") from e
                 await response.write_eof()
                 return response
@@ -853,15 +853,15 @@
                 await response.prepare(request)
                 try:
                     # iterate to get the one (and hopefully only) yielded element:
                     # noinspection PyTypeChecker
                     count = 0
                     async for res in awaitable:
                         serialized = _serialize_return_value(res, encoding)
-                        if isinstance(res, str):
+                        if not isinstance(res, bytes):
                             serialized += b'\0'
                         await response.write(serialized)
                         count += 1
                 except (CancelledError, ConnectionResetError, ClientConnectionError):
                     raise
                 except Exception as e:
                     print(str(e))
```

### Comparing `bantam-2.2.2/src/bantam/js.py` & `bantam-2.2.3/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam/js_async.py` & `bantam-2.2.3/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam/pythonclient.py` & `bantam-2.2.3/src/bantam/pythonclient.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/src/bantam.egg-info/PKG-INFO` & `bantam-2.2.3/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.2.2
+Version: 2.2.3
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.2.2
+Download-URL: https://github.com/bantam/dist/2.2.3
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.2.2/src/bantam.egg-info/SOURCES.txt` & `bantam-2.2.3/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/test/test_client_get.py` & `bantam-2.2.3/test/test_client_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,112 +5,116 @@
 import sys
 if True:
     sys.path.insert(0, str(Path(__file__).parent / 'example'))
 from pathlib import Path
 
 import pytest
 from bantam.http import WebApplication
-from class_rest_get import RestAPIExampleAsyncInterface
+
+PORT = 8239
 
 
 @pytest.mark.asyncio
 async def test_client_class_method(tmpdir):
-    PORT = 8237
+    from class_rest_get import RestAPIExampleAsyncInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
-        client: RestAPIExampleAsyncInterface = RestAPIExampleAsyncInterface.Client(end_point=f'http://localhost:{PORT}/')
-        response = await client.api_get_basic(42, True, 992.123)
+        end_point = f'http://localhost:{PORT}/'
+        client_mapping = RestAPIExampleAsyncInterface.ClientEndpointMapping()
+        Client = client_mapping[end_point]
+        response = await Client.api_get_basic(42, True, 992.123)
         assert response == f"Response to test_api_basic 1.0 2"
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_constructor(tmpdir):
-    PORT = 8237
+    from class_rest_get import RestAPIExampleAsyncInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
-        client: RestAPIExampleAsyncInterface = RestAPIExampleAsyncInterface.Client(end_point=f'http://localhost:{PORT}/')
-        response = await client.explicit_constructor(42)
-        assert response.self_id is not None
+        client_mapping = RestAPIExampleAsyncInterface.ClientEndpointMapping()
+        Client = client_mapping[f'http://localhost:{PORT}/']
+        instance = await Client.explicit_constructor(42)
+        assert instance.self_id is not None
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_instance_method(tmpdir):
-    PORT = 8237
+    from class_rest_get import RestAPIExampleAsyncInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(4242)
         response = await instance.my_value()
         assert response == 4242
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_class_method_streamed(tmpdir):
-    PORT = 8237
+    from class_rest_get import RestAPIExampleAsyncInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
-        client = RestAPIExampleAsyncInterface.Client(end_point=f'http://localhost:{PORT}/')
+        client = RestAPIExampleAsyncInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         count = 0
         async for item in client.api_get_stream(42, True, 992.123, "They're here..."):
             assert item == count
             count += 1
         assert count == 10
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed(tmpdir):
-    PORT = 8237
+    from class_rest_get import RestAPIExampleAsyncInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(29)
         count = 0
         async for item in instance.my_value_repeated(200):
             assert item == 29
             count += 1
         assert count == 200
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed_str(tmpdir):
-    PORT = 8237
+    from class_rest_get import RestAPIExampleAsyncInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_get']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(29)
         count = 0
         async for item in instance.my_value_repeated_string(200):
             assert item == str(29)
             count += 1
         assert count == 200
     finally:
```

### Comparing `bantam-2.2.2/test/test_client_post.py` & `bantam-2.2.3/test/test_client_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,54 +7,55 @@
     sys.path.insert(0, str(Path(__file__).parent / 'example'))
 from pathlib import Path
 
 import pytest
 from bantam.http import WebApplication
 from class_rest_post import RestAPIExampleAsyncPostInterface, RestAPIExampleAsyncPost
 
-PORT = 8237
+PORT = 8240
 
 
 @pytest.mark.asyncio
 async def test_client_class_method(tmpdir):
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
-        client: RestAPIExampleAsyncPostInterface = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        client = RestAPIExampleAsyncPostInterface.ClientEndpointMapping()
+        client = client[f'http://localhost:{PORT}/']
         response = await client.api_post_basic(42, True, 992.123)
         assert response == f"Response to test_api_basic 1.0 2"
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_constructor(tmpdir):
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
-        client: RestAPIExampleAsyncPostInterface = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        client = RestAPIExampleAsyncPostInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         response = await client.explicit_constructor(42)
         assert response.self_id is not None
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_instance_method(tmpdir):
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncPostInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(4242)
         response = await instance.my_value()
         assert response == 4242
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
@@ -62,15 +63,15 @@
 
 @pytest.mark.asyncio
 async def test_client_class_method_streamed(tmpdir):
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
-        client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        client = RestAPIExampleAsyncPostInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         count = 0
         async for item in client.api_post_stream(42, True, 992.123, "They're here..."):
             assert item == count
             count += 1
         assert count == 10
     finally:
         task.cancel()
@@ -80,15 +81,15 @@
 
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed(tmpdir):
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncPostInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(29)
         count = 0
         async for item in instance.my_value_repeated(200):
             assert item == 29
             count += 1
         assert count == 200
     finally:
@@ -99,15 +100,15 @@
 
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed_str(tmpdir):
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_post']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncPostInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(29)
         count = 0
         async for item in instance.my_value_repeated_string(200):
             assert item == str(29)*65537
             count += 1
             if count == 121:
                 break  # disconnects client
```

### Comparing `bantam-2.2.2/test/test_client_post_inherited_apis.py` & `bantam-2.2.3/test/test_client_post_inherited_apis.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,112 +5,114 @@
 import sys
 if True:
     sys.path.insert(0, str(Path(__file__).parent / 'example'))
 from pathlib import Path
 
 import pytest
 from bantam.http import WebApplication
-from class_rest_inherit_apis import RestAPIExampleAsyncPostInterface
+
+PORT = 8238
 
 
 @pytest.mark.asyncio
 async def test_client_class_method(tmpdir):
-    PORT = 8237
+    from class_rest_inherit_apis import RestAPIExampleAsyncPostInheritedInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_inherit_apis']))
     try:
         await asyncio.sleep(1)
-        client: RestAPIExampleAsyncPostInterface = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        client = RestAPIExampleAsyncPostInheritedInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         response = await client.api_post_basic(42, True, 992.123)
         assert response == f"Response to test_api_basic 1.0 2"
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_constructor(tmpdir):
-    PORT = 8237
+    from class_rest_inherit_apis import RestAPIExampleAsyncPostInheritedInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_inherit_apis']))
     try:
         await asyncio.sleep(1)
-        client: RestAPIExampleAsyncPostInterface = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        client = RestAPIExampleAsyncPostInheritedInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         response = await client.explicit_constructor(42)
         assert response.self_id is not None
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_instance_method(tmpdir):
-    PORT = 8237
+    from class_rest_inherit_apis import RestAPIExampleAsyncPostInheritedInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_inherit_apis']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncPostInheritedInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(4242)
         response = await instance.my_value()
         assert response == 4242
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_class_method_streamed(tmpdir):
-    PORT = 8237
+    from class_rest_inherit_apis import RestAPIExampleAsyncPostInheritedInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_inherit_apis']))
     try:
         await asyncio.sleep(1)
-        client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        client = RestAPIExampleAsyncPostInheritedInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         count = 0
         async for item in client.api_post_stream(42, True, 992.123, "They're here..."):
             assert item == count
             count += 1
         assert count == 10
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
 
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed(tmpdir):
-    PORT = 8237
+    from class_rest_inherit_apis import RestAPIExampleAsyncPostInheritedInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_inherit_apis']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncPostInheritedInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(29)
         count = 0
         async for item in instance.my_value_repeated(200):
             assert item == 29
             count += 1
         assert count == 200
     finally:
         task.cancel()
         with suppress(CancelledError):
             await task
 
+
 @pytest.mark.asyncio
 async def test_client_instance_method_streamed_str(tmpdir):
-    PORT = 8237
+    from class_rest_inherit_apis import RestAPIExampleAsyncPostInheritedInterface
     app = WebApplication(static_path=Path(tmpdir), js_bundle_name='generated', using_async=False)
     task = asyncio.create_task(app.start(host='localhost', port=PORT, modules=['class_rest_inherit_apis']))
     try:
         await asyncio.sleep(1)
-        Client = RestAPIExampleAsyncPostInterface.Client(end_point=f'http://localhost:{PORT}/')
+        Client = RestAPIExampleAsyncPostInheritedInterface.ClientEndpointMapping()[f'http://localhost:{PORT}/']
         instance = await Client.explicit_constructor(29)
         count = 0
         async for item in instance.my_value_repeated_string(200):
             assert item == str(29)
             count += 1
         assert count == 200
     finally:
```

### Comparing `bantam-2.2.2/test/test_conversions.py` & `bantam-2.2.3/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/test/test_decorators.py` & `bantam-2.2.3/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.2.2/test/test_js_async.py` & `bantam-2.2.3/test/test_js_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,24 +45,24 @@
             except Exception:
                 with suppress(Exception):
                     browser = webbrowser.get("google-chrome")
                 if not browser:
                     browser = webbrowser.get()
             if not browser:
                 os.write(sys.stderr.fileno(),
-                         b"UNABLE TO GET BROWSER SUPPORINT HEADLESS CONFIGURATION. DEFAULTING TO NON_HEADLESSS")
+                         b"UNABLE TO GET BROWSER SUPPORT IN HEADLESS CONFIGURATION. DEFAULTING TO NON_HEADLESS")
                 browser = webbrowser.get()
-            browser.open("http://localhost:8080/static/index_async.html")
+            browser.open("http://localhost:8081/static/index_async.html")
             result = await RestAPIExampleAsync.result_queue.get()
             await asyncio.sleep(2.0)
             await app.shutdown()
             return result
 
         try:
-            completed, _ = await asyncio.wait([app.start(modules=['class_rest_get']),
+            completed, _ = await asyncio.wait([app.start(modules=['class_rest_get'], port=8081),
                                                launch_browser()], timeout=100000, return_when=asyncio.FIRST_COMPLETED)
             results = [c.result() for c in completed if c is not None]
         except Exception as e:
             assert False, f"Exception processing javascript results: {traceback.format_exc()}"
         if any([isinstance(r, Exception) for r in results]):
             assert False, "At least one javascript test failed. See browser window for details"
         assert results[0] == "PASSED", \
```


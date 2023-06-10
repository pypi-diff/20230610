# Comparing `tmp/flask-fullstack-0.4.8.tar.gz` & `tmp/flask-fullstack-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-fullstack-0.4.8.tar", last modified: Sun Oct  9 21:52:40 2022, max compression
+gzip compressed data, was "flask-fullstack-0.4.9.tar", last modified: Sun Nov 13 22:59:29 2022, max compression
```

## Comparing `flask-fullstack-0.4.8.tar` & `flask-fullstack-0.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-10-09 21:52:40.183399 flask-fullstack-0.4.8/
--rw-rw-rw-   0        0        0     3104 2022-10-09 21:52:40.182429 flask-fullstack-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2022-10-09 20:23:56.000000 flask-fullstack-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-09 21:52:40.141787 flask-fullstack-0.4.8/flask_fullstack/
--rw-rw-rw-   0        0        0      744 2022-10-09 19:49:37.000000 flask-fullstack-0.4.8/flask_fullstack/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-09 21:52:40.155718 flask-fullstack-0.4.8/flask_fullstack/base/
--rw-rw-rw-   0        0        0      131 2022-09-05 19:01:58.000000 flask-fullstack-0.4.8/flask_fullstack/base/__init__.py
--rw-rw-rw-   0        0        0     1029 2022-10-09 20:23:56.000000 flask-fullstack-0.4.8/flask_fullstack/base/interfaces.py
--rw-rw-rw-   0        0        0     5788 2022-10-09 21:44:41.000000 flask-fullstack-0.4.8/flask_fullstack/base/mixins.py
--rw-rw-rw-   0        0        0     6412 2022-10-09 19:49:37.000000 flask-fullstack-0.4.8/flask_fullstack/core.py
-drwxrwxrwx   0        0        0        0 2022-10-09 21:52:40.159491 flask-fullstack-0.4.8/flask_fullstack/restx/
--rw-rw-rw-   0        0        0      282 2022-09-05 22:36:49.000000 flask-fullstack-0.4.8/flask_fullstack/restx/__init__.py
--rw-rw-rw-   0        0        0    12634 2022-10-09 21:44:41.000000 flask-fullstack-0.4.8/flask_fullstack/restx/controller.py
--rw-rw-rw-   0        0        0    25169 2022-09-06 15:05:48.000000 flask-fullstack-0.4.8/flask_fullstack/restx/marshals.py
--rw-rw-rw-   0        0        0      474 2022-09-05 23:20:01.000000 flask-fullstack-0.4.8/flask_fullstack/restx/parsers.py
-drwxrwxrwx   0        0        0        0 2022-10-09 21:52:40.167919 flask-fullstack-0.4.8/flask_fullstack/siox/
--rw-rw-rw-   0        0        0      302 2022-09-05 23:02:48.000000 flask-fullstack-0.4.8/flask_fullstack/siox/__init__.py
--rw-rw-rw-   0        0        0     6968 2022-09-06 14:21:57.000000 flask-fullstack-0.4.8/flask_fullstack/siox/controller.py
--rw-rw-rw-   0        0        0     8603 2022-10-09 20:23:56.000000 flask-fullstack-0.4.8/flask_fullstack/siox/eventor.py
--rw-rw-rw-   0        0        0    11754 2022-09-06 14:27:29.000000 flask-fullstack-0.4.8/flask_fullstack/siox/events.py
--rw-rw-rw-   0        0        0     4252 2022-09-06 13:51:45.000000 flask-fullstack-0.4.8/flask_fullstack/siox/groups.py
--rw-rw-rw-   0        0        0     2347 2022-09-06 13:51:10.000000 flask-fullstack-0.4.8/flask_fullstack/siox/interfaces.py
--rw-rw-rw-   0        0        0     4658 2022-09-06 14:27:13.000000 flask-fullstack-0.4.8/flask_fullstack/siox/structures.py
-drwxrwxrwx   0        0        0        0 2022-10-09 21:52:40.180386 flask-fullstack-0.4.8/flask_fullstack/utils/
--rw-rw-rw-   0        0        0      484 2022-09-05 23:04:58.000000 flask-fullstack-0.4.8/flask_fullstack/utils/__init__.py
--rw-rw-rw-   0        0        0      869 2022-09-06 13:47:45.000000 flask-fullstack-0.4.8/flask_fullstack/utils/columns.py
--rw-rw-rw-   0        0        0      535 2022-09-06 13:48:27.000000 flask-fullstack-0.4.8/flask_fullstack/utils/dicts.py
--rw-rw-rw-   0        0        0      603 2022-09-05 23:21:45.000000 flask-fullstack-0.4.8/flask_fullstack/utils/flask.py
--rw-rw-rw-   0        0        0      546 2022-09-06 13:47:45.000000 flask-fullstack-0.4.8/flask_fullstack/utils/named.py
--rw-rw-rw-   0        0        0     1000 2022-09-06 13:47:45.000000 flask-fullstack-0.4.8/flask_fullstack/utils/other.py
--rw-rw-rw-   0        0        0      440 2022-09-05 23:14:15.000000 flask-fullstack-0.4.8/flask_fullstack/utils/pydantic.py
--rw-rw-rw-   0        0        0      378 2022-09-06 13:48:36.000000 flask-fullstack-0.4.8/flask_fullstack/utils/pytest.py
--rw-rw-rw-   0        0        0     4301 2022-09-06 14:14:39.000000 flask-fullstack-0.4.8/flask_fullstack/utils/sqlalchemy.py
--rw-rw-rw-   0        0        0     1831 2022-09-06 14:14:32.000000 flask-fullstack-0.4.8/flask_fullstack/utils/whoosh.py
-drwxrwxrwx   0        0        0        0 2022-10-09 21:52:40.152714 flask-fullstack-0.4.8/flask_fullstack.egg-info/
--rw-rw-rw-   0        0        0     3104 2022-10-09 21:52:40.000000 flask-fullstack-0.4.8/flask_fullstack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2022-10-09 21:52:40.000000 flask-fullstack-0.4.8/flask_fullstack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-09 21:52:40.000000 flask-fullstack-0.4.8/flask_fullstack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2022-10-09 21:52:40.000000 flask-fullstack-0.4.8/flask_fullstack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-10-09 21:52:40.000000 flask-fullstack-0.4.8/flask_fullstack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2022-10-09 20:23:56.000000 flask-fullstack-0.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-09 21:52:40.183399 flask-fullstack-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1030 2022-10-09 21:51:41.000000 flask-fullstack-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-13 22:59:29.319935 flask-fullstack-0.4.9/
+-rw-rw-rw-   0        0        0     3104 2022-11-13 22:59:29.318936 flask-fullstack-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2022-11-13 17:10:56.000000 flask-fullstack-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-13 22:59:29.207255 flask-fullstack-0.4.9/flask_fullstack/
+-rw-rw-rw-   0        0        0      744 2022-10-09 19:49:37.000000 flask-fullstack-0.4.9/flask_fullstack/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-13 22:59:29.232813 flask-fullstack-0.4.9/flask_fullstack/base/
+-rw-rw-rw-   0        0        0      131 2022-09-05 19:01:58.000000 flask-fullstack-0.4.9/flask_fullstack/base/__init__.py
+-rw-rw-rw-   0        0        0     1029 2022-11-13 16:59:59.000000 flask-fullstack-0.4.9/flask_fullstack/base/interfaces.py
+-rw-rw-rw-   0        0        0     5788 2022-11-13 16:59:59.000000 flask-fullstack-0.4.9/flask_fullstack/base/mixins.py
+-rw-rw-rw-   0        0        0     6412 2022-10-09 19:49:37.000000 flask-fullstack-0.4.9/flask_fullstack/core.py
+drwxrwxrwx   0        0        0        0 2022-11-13 22:59:29.253023 flask-fullstack-0.4.9/flask_fullstack/restx/
+-rw-rw-rw-   0        0        0      282 2022-09-05 22:36:49.000000 flask-fullstack-0.4.9/flask_fullstack/restx/__init__.py
+-rw-rw-rw-   0        0        0    12634 2022-11-13 16:59:59.000000 flask-fullstack-0.4.9/flask_fullstack/restx/controller.py
+-rw-rw-rw-   0        0        0    25169 2022-11-13 16:04:38.000000 flask-fullstack-0.4.9/flask_fullstack/restx/marshals.py
+-rw-rw-rw-   0        0        0      474 2022-09-05 23:20:01.000000 flask-fullstack-0.4.9/flask_fullstack/restx/parsers.py
+drwxrwxrwx   0        0        0        0 2022-11-13 22:59:29.265357 flask-fullstack-0.4.9/flask_fullstack/siox/
+-rw-rw-rw-   0        0        0      216 2022-11-13 18:07:26.000000 flask-fullstack-0.4.9/flask_fullstack/siox/__init__.py
+-rw-rw-rw-   0        0        0     6123 2022-11-13 22:21:49.000000 flask-fullstack-0.4.9/flask_fullstack/siox/controller.py
+-rw-rw-rw-   0        0        0     9195 2022-11-13 22:13:31.000000 flask-fullstack-0.4.9/flask_fullstack/siox/eventor.py
+-rw-rw-rw-   0        0        0    11539 2022-11-13 21:59:16.000000 flask-fullstack-0.4.9/flask_fullstack/siox/events.py
+-rw-rw-rw-   0        0        0     2347 2022-09-06 13:51:10.000000 flask-fullstack-0.4.9/flask_fullstack/siox/interfaces.py
+-rw-rw-rw-   0        0        0     4974 2022-11-13 17:11:00.000000 flask-fullstack-0.4.9/flask_fullstack/siox/structures.py
+drwxrwxrwx   0        0        0        0 2022-11-13 22:59:29.317934 flask-fullstack-0.4.9/flask_fullstack/utils/
+-rw-rw-rw-   0        0        0      551 2022-11-13 17:11:00.000000 flask-fullstack-0.4.9/flask_fullstack/utils/__init__.py
+-rw-rw-rw-   0        0        0      869 2022-09-06 13:47:45.000000 flask-fullstack-0.4.9/flask_fullstack/utils/columns.py
+-rw-rw-rw-   0        0        0      535 2022-09-06 13:48:27.000000 flask-fullstack-0.4.9/flask_fullstack/utils/dicts.py
+-rw-rw-rw-   0        0        0      603 2022-09-05 23:21:45.000000 flask-fullstack-0.4.9/flask_fullstack/utils/flask.py
+-rw-rw-rw-   0        0        0      776 2022-11-13 17:22:53.000000 flask-fullstack-0.4.9/flask_fullstack/utils/models.py
+-rw-rw-rw-   0        0        0      546 2022-09-06 13:47:45.000000 flask-fullstack-0.4.9/flask_fullstack/utils/named.py
+-rw-rw-rw-   0        0        0     1000 2022-09-06 13:47:45.000000 flask-fullstack-0.4.9/flask_fullstack/utils/other.py
+-rw-rw-rw-   0        0        0      440 2022-09-05 23:14:15.000000 flask-fullstack-0.4.9/flask_fullstack/utils/pydantic.py
+-rw-rw-rw-   0        0        0      378 2022-09-06 13:48:36.000000 flask-fullstack-0.4.9/flask_fullstack/utils/pytest.py
+-rw-rw-rw-   0        0        0     4301 2022-09-06 14:14:39.000000 flask-fullstack-0.4.9/flask_fullstack/utils/sqlalchemy.py
+-rw-rw-rw-   0        0        0     1831 2022-09-06 14:14:32.000000 flask-fullstack-0.4.9/flask_fullstack/utils/whoosh.py
+drwxrwxrwx   0        0        0        0 2022-11-13 22:59:29.225697 flask-fullstack-0.4.9/flask_fullstack.egg-info/
+-rw-rw-rw-   0        0        0     3104 2022-11-13 22:59:29.000000 flask-fullstack-0.4.9/flask_fullstack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1073 2022-11-13 22:59:29.000000 flask-fullstack-0.4.9/flask_fullstack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-13 22:59:29.000000 flask-fullstack-0.4.9/flask_fullstack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2022-11-13 22:59:29.000000 flask-fullstack-0.4.9/flask_fullstack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-11-13 22:59:29.000000 flask-fullstack-0.4.9/flask_fullstack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2022-10-09 20:23:56.000000 flask-fullstack-0.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-11-13 22:59:29.319935 flask-fullstack-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2022-11-13 17:11:00.000000 flask-fullstack-0.4.9/setup.py
```

### Comparing `flask-fullstack-0.4.8/PKG-INFO` & `flask-fullstack-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fullstack
-Version: 0.4.8
+Version: 0.4.9
 Summary: A utility package for projects using flask, sqlalchemy, socketio and pytest
 Home-page: https://github.com/niqzart/flask-fullstack
 Author: niqzart
 Author-email: qwert45hi@yandex.ru
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `flask-fullstack-0.4.8/README.md` & `flask-fullstack-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/__init__.py` & `flask-fullstack-0.4.9/flask_fullstack/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/base/interfaces.py` & `flask-fullstack-0.4.9/flask_fullstack/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/base/mixins.py` & `flask-fullstack-0.4.9/flask_fullstack/base/mixins.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/core.py` & `flask-fullstack-0.4.9/flask_fullstack/core.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/restx/controller.py` & `flask-fullstack-0.4.9/flask_fullstack/restx/controller.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/restx/marshals.py` & `flask-fullstack-0.4.9/flask_fullstack/restx/marshals.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/siox/controller.py` & `flask-fullstack-0.4.9/flask_fullstack/siox/controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 from .events import ClientEvent, DuplexEvent, BaseEvent
 from .interfaces import EventGroupBase
 from ..utils import kebabify_model
 
 
 class EventController(EventGroupBase):
-    model_kwarg_names = ("include", "exclude", "exclude_none")
-    ack_kwarg_names = {n: "ack_" + n for n in model_kwarg_names + ("force_wrap",)}
-    ack_kwarg_names["force_ack"] = "force_ack"
+    server_kwarg_names = ("include", "exclude", "exclude_none")
+    client_kwarg_names = {n: "ack_" + n for n in server_kwarg_names + ("force_wrap",)}
+    client_kwarg_names["force_ack"] = "force_ack"
+    client_kwarg_names["additional_models"] = "additional_models"
 
     @staticmethod
     def _update_event_data(function: Callable, data: dict) -> Callable:
         if hasattr(function, "__event_data__"):
             function.__event_data__.update(data)
         else:
             function.__event_data__ = data
@@ -26,68 +27,48 @@
     def _maybe_bind_model(self, model: type[BaseModel] | None = None) -> None:
         if model is None:
             return
         if self.use_kebab_case:
             kebabify_model(model)
         self._bind_model(model)
 
-    def add_docs(self, additional_docs: dict):
-        # TODO clearly label: Callable -> Callable & ClientEvent -> ClientEvent & DuplexEvent -> DuplexEvent
-        def add_docs_wrapper(
-            function: Callable | ClientEvent | DuplexEvent,
-        ) -> Callable | ClientEvent | DuplexEvent:
-            if isinstance(function, BaseEvent):
-                if function.additional_docs is None:
-                    function.additional_docs = additional_docs
-                else:
-                    function.additional_docs.update(additional_docs)
-            else:
-                self._update_event_data(function, {"additional_docs": additional_docs})
-
-            return function
-
-        return add_docs_wrapper
-
     def argument_parser(self, client_model: type[BaseModel] = BaseModel):
         self._maybe_bind_model(client_model)
 
         def argument_parser_wrapper(function: Callable) -> ClientEvent | DuplexEvent:
             event_data: dict = getattr(function, "__event_data__", {})
-            additional_docs: dict = getattr(function, "additional_docs", {})
 
-            ack_kwargs = {
+            client_kwargs = {
                 n: event_data.get(v, None)
-                for n, v in self.ack_kwarg_names.items()
+                for n, v in self.client_kwarg_names.items()
             }
             client_event = self.ClientEvent(
                 client_model,
                 event_data.get("ack_model", None),
-                **ack_kwargs,
+                **client_kwargs,
             )
 
             if event_data.get("duplex", False):
                 server_kwargs = {
                     n: event_data.get(n, None)
-                    for n in self.model_kwarg_names
+                    for n in self.server_kwarg_names
                 }
                 server_event = self.ServerEvent(
                     event_data.get("server_model", None) or client_model,
                     **server_kwargs,
                 )
                 duplex_event = self.DuplexEvent(
                     client_event,
                     server_event,
                     event_data.get("use_event", None),
-                    additional_docs=additional_docs,
                 )
                 duplex_event.bind(function)
                 return duplex_event
 
             client_event.bind(function)
-            client_event.additional_docs = additional_docs
             return client_event
 
         return argument_parser_wrapper
 
     def mark_duplex(
         self,
         server_model: type[BaseModel] = None,
```

### Comparing `flask-fullstack-0.4.8/flask_fullstack/siox/eventor.py` & `flask-fullstack-0.4.9/flask_fullstack/siox/eventor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,30 @@
 from __future__ import annotations
 
-from abc import ABCMeta
 from collections.abc import Callable
 from datetime import datetime
 from functools import wraps
 from json import dumps, loads
 
 from flask_jwt_extended import jwt_required, get_jwt_identity
-from flask_restx import Model
 from flask_socketio import join_room
 from pydantic import BaseModel
 from socketio.exceptions import ConnectionRefusedError
 
 from .controller import EventController as _EventController
 from .events import (
     ClientEvent as _ClientEvent,
     ServerEvent as _ServerEvent,
     DuplexEvent as _DuplexEvent,
 )
-from .groups import EventGroup as _EventGroup
 from .structures import EventException
-from .structures import (
-    EventGroupBase as _EventGroupBase,
-    Namespace as _Namespace,
-    SocketIO as _SocketIO,
-)
+from .structures import Namespace as _Namespace, SocketIO as _SocketIO
 from ..base import DatabaseSearcherMixin, JWTAuthorizerMixin
 from ..restx import PydanticModel
-from ..utils import Nameable, TypeEnum
-
-
-class EventGroupBaseMixedIn(
-    _EventGroupBase,
-    DatabaseSearcherMixin,
-    JWTAuthorizerMixin,
-    metaclass=ABCMeta,
-):
-    pass
+from ..utils import Nameable, TypeEnum, restx_model_to_message
 
 
 class ClientEvent(_ClientEvent):
     def __init__(
         self,
         model: type[BaseModel],
         ack_model: type[BaseModel] = None,
@@ -49,29 +33,29 @@
         description: str = None,
         handler: Callable = None,
         include: set[str] = None,
         exclude: set[str] = None,
         exclude_none: bool = None,
         force_wrap: bool = None,
         force_ack: bool = None,
-        additional_docs: dict = None,
+        additional_models: list[dict] = None,
     ):
         super().__init__(
             model,
             ack_model,
             namespace,
             name,
             description,
             handler,
             include,
             exclude,
             exclude_none,
             force_wrap is not False,
             force_ack is not False,
-            additional_docs,
+            additional_models,
         )
 
     def _force_wrap(self, data) -> dict:
         result = {"code": 200, "message": "Success"}
         if isinstance(data, str):
             result["message"] = data
         elif data is not None:
@@ -157,15 +141,15 @@
             user_id,
             namespace,
             broadcast,
             **kwargs,
         )
 
 
-class EventGroupBase(EventGroupBaseMixedIn):
+class EventController(_EventController, DatabaseSearcherMixin, JWTAuthorizerMixin):
     ClientEvent = ClientEvent
     ServerEvent = ServerEvent
     DuplexEvent = DuplexEvent
 
     def _bind_model(self, bound_model: type[BaseModel]):
         if isinstance(bound_model, type) and issubclass(bound_model, PydanticModel):
             bound_model.Config.title = bound_model.name
@@ -174,36 +158,47 @@
     def _get_model_name(self, bound_model: type[BaseModel]):
         if isinstance(bound_model, type) and issubclass(bound_model, Nameable):
             return bound_model.name or bound_model.__name__
         return super()._get_model_name(bound_model)
 
     def _get_model_schema(self, bound_model: type[BaseModel]):
         if isinstance(bound_model, type) and issubclass(bound_model, PydanticModel):
-            return {
-                "payload": Model(
-                    self._get_model_name(bound_model), bound_model.model()
-                ).__schema__
-            }
+            return restx_model_to_message(
+                self._get_model_name(bound_model), bound_model.model()
+            )
         return super()._get_model_schema(bound_model)
 
     def doc_abort(self, error_code: int | str, description: str):
-        def doc_abort_wrapper(function):
+        def doc_abort_wrapper(function: _ClientEvent | _DuplexEvent | Callable):
+            payload = {
+                "type": "object",
+                "required": ["code", "message"],
+                "properties": {
+                    "code": {"const": int(error_code)},
+                    "message": {"const": description},
+                },
+            }
+
+            if isinstance(function, _ClientEvent):
+                function.additional_models.append(payload)
+            elif isinstance(function, _DuplexEvent):
+                function.client_event.additional_models.append(payload)
+            elif not hasattr(function, "__event_data__"):
+                function.__event_data__ = {"additional_models": [payload]}
+            elif "additional_models" in function.__event_data__:
+                function.__event_data__["additional_models"].append(payload)
+            else:
+                function.__event_data__["additional_models"] = [payload]
             return function
 
         return doc_abort_wrapper
 
     def abort(self, error_code: int | str, description: str):
         raise EventException(error_code, description, False)
 
-
-class EventGroup(_EventGroup, EventGroupBase):  # DEPRECATED
-    pass
-
-
-class EventController(_EventController, EventGroupBase):
     def _marshal_ack_wrapper(
         self,
         ack_model: type[BaseModel],
         ack_kwargs: dict,
         function: Callable,
     ) -> Callable:
         if isinstance(ack_model, type) and issubclass(ack_model, PydanticModel):
@@ -237,15 +232,18 @@
             if protected is True:
                 protected = ""
 
             @self.on_connect()
             @jwt_required(optional=True)
             def user_connect(*_):
                 identity = get_jwt_identity()
-                if identity is None or (user_id := identity.get(protected, None)) is None:
+                if (
+                    identity is None
+                    or (user_id := identity.get(protected, None)) is None
+                ):
                     raise ConnectionRefusedError("unauthorized!")
                 join_room(f"user-{user_id}")
 
 
 class CustomJSON:
     @staticmethod
     def default(value: ...) -> ...:
@@ -271,15 +269,15 @@
         if "json" not in kwargs:
             kwargs["json"] = CustomJSON()
         super().__init__(*args, **kwargs)
 
     def add_namespace(
         self,
         name: str = None,
-        *event_groups: EventGroupBase,
+        *event_groups: EventController,
         protected: str | bool = False,
     ):
         namespace = self.namespace_class(name, self.use_kebab_case)
         if isinstance(namespace, Namespace):
             namespace.mark_protected(protected)
         self._add_namespace(namespace, *event_groups)
```

### Comparing `flask-fullstack-0.4.8/flask_fullstack/siox/events.py` & `flask-fullstack-0.4.9/flask_fullstack/siox/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,65 +11,60 @@
 
 
 class BaseEvent:  # do not instantiate!
     def __init__(
         self,
         name: str = None,
         namespace: str = None,
-        additional_docs: dict = None,
     ):
         self.name = None
         self.namespace = namespace
-        self.additional_docs: dict | None = additional_docs
         if name is not None:
             self.attach_name(name)
 
     def attach_name(self, name: str):
         raise NotImplementedError
 
     def attach_namespace(self, namespace: str):
         raise NotImplementedError
 
-    def create_doc(self, namespace: str, additional_docs: dict = None):
+    def create_doc(self, namespace: str):
         raise NotImplementedError
 
 
 class Event(BaseEvent):  # do not instantiate!
     def __init__(
         self,
         model: type[BaseModel],
         namespace: str = None,
         name: str = None,
         description: str = None,
-        additional_docs: dict = None,
     ):
-        super().__init__(name, namespace, additional_docs)
+        super().__init__(name, namespace)
         self.model: type[BaseModel] = model
         self.description: str = description
 
     def attach_name(self, name: str):
         self.name = name
 
     def attach_namespace(self, namespace: str):
         self.namespace = namespace
 
-    def create_doc(self, namespace: str = None, additional_docs: dict = None):
+    def create_doc(self, namespace: str = None):
         model_name: str = getattr(self.model, "name", None) or self.model.__name__
         if namespace is None:
             namespace = self.namespace
         return remove_none(
             {
                 "description": self.description,
                 "tags": [{"name": f"namespace-{namespace}"}]
                 if namespace is not None
                 else None,
                 "message": {"$ref": f"#/components/messages/{model_name}"},
-            },
-            **(self.additional_docs or {}),
-            **(additional_docs or {}),
+            }
         )
 
 
 @dataclass()
 class ClientEvent(Event):
     def __init__(
         self,
@@ -80,27 +75,28 @@
         description: str = None,
         handler: Callable = None,
         include: set[str] = None,
         exclude: set[str] = None,
         exclude_none: bool = None,
         force_wrap: bool = None,
         force_ack: bool = None,
-        additional_docs: dict = None,
+        additional_models: list[dict] = None,
     ):
-        super().__init__(model, namespace, name, description, additional_docs)
+        super().__init__(model, namespace, name, description)
         self._ack_kwargs = {
             "exclude_none": exclude_none is not False,
             "include": include,
             "exclude": exclude,
             "by_alias": True,
         }
         self.handler: Callable[[dict | None], dict] = handler
         self.ack_model: type[BaseModel] = ack_model
         self.force_wrap: bool = force_wrap is True
         self.forced_ack: bool = force_ack is True and ack_model is None
+        self.additional_models: list[dict] = additional_models or []
 
     def parse(self, data: dict):
         return self.model.parse_obj(data).dict()
 
     def _force_wrap(self, result) -> dict:
         return {"data": result}
 
@@ -176,37 +172,41 @@
                     "code": {"type": "integer"},
                     "message": {"type": "string"},
                     "data": data,
                 },
             },
         }
 
-    def create_doc(self, namespace: str = None, additional_docs: dict = None):
-        result = super().create_doc(namespace, additional_docs)
+    def create_doc(self, namespace: str = None):
+        result = super().create_doc(namespace)
+        models = [result["message"]] + [
+            {"name": f"{self.name}-error-{i}", "payload": model}
+            for i, model in enumerate(self.additional_models)
+        ]
 
         if self.ack_model or self.forced_ack:
-            result["message"] = {"oneOf": [result["message"], self.ack_model_doc()]}
+            models.insert(1, self.ack_model_doc())
 
+        result["message"] = {"oneOf": models}
         return {"publish": result}
 
 
 @dataclass()
 class ServerEvent(Event):
     def __init__(
         self,
         model: type[BaseModel],
         namespace: str = None,
         name: str = None,
         description: str = None,
         include: set[str] = None,
         exclude: set[str] = None,
         exclude_none: bool = None,
-        additional_docs: dict = None,
     ):
-        super().__init__(model, namespace, name, description, additional_docs)
+        super().__init__(model, namespace, name, description)
         self._emit_kwargs = {
             "exclude_none": exclude_none is not False,
             "include": include,
             "exclude": exclude,
             "by_alias": True,
         }
         self.model.Config.allow_population_by_field_name = True
@@ -243,31 +243,30 @@
             render_model(self.model, _data, **self._emit_kwargs),
             _namespace,
             _room,
             _include_self,
             _broadcast,
         )
 
-    def create_doc(self, namespace: str = None, additional_docs: dict = None):
-        return {"subscribe": super().create_doc(namespace, additional_docs)}
+    def create_doc(self, namespace: str = None):
+        return {"subscribe": super().create_doc(namespace)}
 
 
 @dataclass()
 class DuplexEvent(BaseEvent):
     def __init__(
         self,
         client_event: ClientEvent = None,
         server_event: ServerEvent = None,
         use_event: bool = None,
         namespace: str = None,
         name: str = None,
         description: str = None,
-        additional_docs: dict = None,
     ):
-        super().__init__(name, namespace, additional_docs)
+        super().__init__(name, namespace)
         self.client_event: ClientEvent = client_event
         self.server_event: ServerEvent = server_event
         self.description: str = description
         self.use_event: bool = bool(use_event)
 
     @classmethod
     def similar(
@@ -283,44 +282,44 @@
         exclude: set[str] = None,
         exclude_none: bool = True,
         ack_include: set[str] = None,
         ack_exclude: set[str] = None,
         ack_exclude_none: bool = True,
         ack_force_wrap: bool = None,
         ack_force: bool = None,
-        additional_docs: dict = None,
+        additional_models: list[dict] = None,
     ):
         return cls(
             ClientEvent(
-                model,
-                ack_model,
-                namespace,
-                name,
-                description,
-                handler,
-                ack_include,
-                ack_exclude,
-                ack_exclude_none,
-                ack_force_wrap,
-                ack_force,
+                model=model,
+                ack_model=ack_model,
+                namespace=namespace,
+                name=name,
+                description=description,
+                handler=handler,
+                include=ack_include,
+                exclude=ack_exclude,
+                exclude_none=ack_exclude_none,
+                force_wrap=ack_force_wrap,
+                force_ack=ack_force,
+                additional_models=additional_models,
             ),
             ServerEvent(
-                model,
-                name,
-                namespace,
-                description,
-                include,
-                exclude,
-                exclude_none,
+                model=model,
+                name=name,
+                namespace=namespace,
+                description=description,
+                include=include,
+                exclude=exclude,
+                exclude_none=exclude_none,
             ),
-            use_event,
-            namespace,
-            name,
-            description,
-            additional_docs,
+            use_event=use_event,
+            namespace=namespace,
+            name=name,
+            description=description,
         )
 
     def attach_name(self, name: str):
         self.name = name
         self.client_event.name = name
         self.server_event.name = name
 
@@ -355,16 +354,13 @@
 
             return self.client_event.bind(duplex_handler)
         return self.client_event.bind(function)
 
     def __call__(self, data=None):
         return self.client_event(data)
 
-    def create_doc(self, namespace: str = None, additional_docs: dict = None):
-        if additional_docs is None:
-            additional_docs = {}
-        additional_docs.update(self.additional_docs or {})
-        result: dict = self.client_event.create_doc(namespace, additional_docs)
-        result.update(self.server_event.create_doc(namespace, additional_docs))
+    def create_doc(self, namespace: str = None):
+        result: dict = self.client_event.create_doc(namespace)
+        result.update(self.server_event.create_doc(namespace))
         if self.description is not None:
             result["description"] = self.description
         return result
```

### Comparing `flask-fullstack-0.4.8/flask_fullstack/siox/interfaces.py` & `flask-fullstack-0.4.9/flask_fullstack/siox/interfaces.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/siox/structures.py` & `flask-fullstack-0.4.9/flask_fullstack/siox/structures.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 from collections import OrderedDict
 from collections.abc import Callable
 from dataclasses import dataclass
 from logging import Filter, getLogger
 
+from flask_restx import Model
 from flask_socketio import Namespace as _Namespace, SocketIO as _SocketIO, disconnect
 
 from .interfaces import EventGroupBase
-from ..utils import render_packed
+from ..utils import render_packed, restx_model_to_message
 
 
 @dataclass
 class EventException(Exception):
     code: int
     message: str
     critical: bool = False
@@ -82,30 +83,38 @@
         app=None,
         title: str = "SIO",
         version: str = "1.0.0",
         doc_path: str = "/sio-doc/",
         remove_ping_pong_logs: bool = False,
         use_kebab_case: bool = False,
         namespace_class: type[Namespace] = None,
+        restx_models: dict[str, Model] = None,  # TODO get rid of restx
         **kwargs,
     ):
+        self.doc_path = doc_path
         self.use_kebab_case = use_kebab_case
         self.namespace_class = (
             self.default_namespace_class if namespace_class is None else namespace_class
         )
 
         self.async_api = {
             "asyncapi": "2.2.0",
             "info": {"title": title, "version": version},
             "channels": OrderedDict(),
-            "components": {"messages": OrderedDict()},
+            "components": {
+                "messages": OrderedDict(
+                    (name, restx_model_to_message(name, model))
+                    for name, model in (restx_models or {}).items()
+                )
+            },
         }
-        self.doc_path = doc_path
+
         if remove_ping_pong_logs:
             getLogger("engineio.server").addFilter(NoPingPongFilter())
+
         super().__init__(app, **kwargs)
 
     def docs(self):
         return self.async_api
 
     def init_app(self, app, **kwargs):
         app.config["JSON_SORT_KEYS"] = False  # TODO kinda bad for a library
```

### Comparing `flask-fullstack-0.4.8/flask_fullstack/utils/columns.py` & `flask-fullstack-0.4.9/flask_fullstack/utils/columns.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/utils/dicts.py` & `flask-fullstack-0.4.9/flask_fullstack/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/utils/flask.py` & `flask-fullstack-0.4.9/flask_fullstack/utils/flask.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/utils/named.py` & `flask-fullstack-0.4.9/flask_fullstack/utils/named.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/utils/other.py` & `flask-fullstack-0.4.9/flask_fullstack/utils/other.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/utils/sqlalchemy.py` & `flask-fullstack-0.4.9/flask_fullstack/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack/utils/whoosh.py` & `flask-fullstack-0.4.9/flask_fullstack/utils/whoosh.py`

 * *Files identical despite different names*

### Comparing `flask-fullstack-0.4.8/flask_fullstack.egg-info/PKG-INFO` & `flask-fullstack-0.4.9/flask_fullstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fullstack
-Version: 0.4.8
+Version: 0.4.9
 Summary: A utility package for projects using flask, sqlalchemy, socketio and pytest
 Home-page: https://github.com/niqzart/flask-fullstack
 Author: niqzart
 Author-email: qwert45hi@yandex.ru
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `flask-fullstack-0.4.8/flask_fullstack.egg-info/SOURCES.txt` & `flask-fullstack-0.4.9/flask_fullstack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 flask_fullstack/restx/controller.py
 flask_fullstack/restx/marshals.py
 flask_fullstack/restx/parsers.py
 flask_fullstack/siox/__init__.py
 flask_fullstack/siox/controller.py
 flask_fullstack/siox/eventor.py
 flask_fullstack/siox/events.py
-flask_fullstack/siox/groups.py
 flask_fullstack/siox/interfaces.py
 flask_fullstack/siox/structures.py
 flask_fullstack/utils/__init__.py
 flask_fullstack/utils/columns.py
 flask_fullstack/utils/dicts.py
 flask_fullstack/utils/flask.py
+flask_fullstack/utils/models.py
 flask_fullstack/utils/named.py
 flask_fullstack/utils/other.py
 flask_fullstack/utils/pydantic.py
 flask_fullstack/utils/pytest.py
 flask_fullstack/utils/sqlalchemy.py
 flask_fullstack/utils/whoosh.py
```

### Comparing `flask-fullstack-0.4.8/setup.py` & `flask-fullstack-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 )
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="flask-fullstack",
     py_modules=["flask_fullstack"],
-    version="0.4.8",
+    version="0.4.9",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="niqzart",
     author_email="qwert45hi@yandex.ru",
     url="https://github.com/niqzart/flask-fullstack",
     packages=find_packages(),
```


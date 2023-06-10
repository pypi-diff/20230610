# Comparing `tmp/django_nats_client-0.3.5.tar.gz` & `tmp/django_nats_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nats_client-0.3.5.tar", max compression
+gzip compressed data, was "django_nats_client-0.4.0.tar", max compression
```

## Comparing `django_nats_client-0.3.5.tar` & `django_nats_client-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/LICENSE
--rw-r--r--   0        0        0     3886 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/README.md
--rw-r--r--   0        0        0      125 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/nats_client/__init__.py
--rw-r--r--   0        0        0       96 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/nats_client/apps.py
--rw-r--r--   0        0        0     1198 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/nats_client/clients.py
--rw-r--r--   0        0        0     3470 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/nats_client/management/commands/nats_listener.py
--rw-r--r--   0        0        0     1021 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/nats_client/registry.py
--rw-r--r--   0        0        0       84 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/nats_client/types.py
--rw-r--r--   0        0        0      896 2023-03-10 17:04:54.803822 django_nats_client-0.3.5/nats_client/utils.py
--rw-r--r--   0        0        0      881 2023-03-10 17:05:12.772703 django_nats_client-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 django_nats_client-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5566 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/README.md
+-rw-r--r--   0        0        0       79 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/apps.py
+-rw-r--r--   0        0        0     1980 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/clients.py
+-rw-r--r--   0        0        0      114 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/exceptions.py
+-rw-r--r--   0        0        0      473 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/handlers.py
+-rw-r--r--   0        0        0     5557 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/management/commands/nats_listener.py
+-rw-r--r--   0        0        0     1336 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/registry.py
+-rw-r--r--   0        0        0       84 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/types.py
+-rw-r--r--   0        0        0      849 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/utils.py
+-rw-r--r--   0        0        0      901 2023-06-10 18:55:43.474210 django_nats_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6334 1970-01-01 00:00:00.000000 django_nats_client-0.4.0/PKG-INFO
```

### Comparing `django_nats_client-0.3.5/LICENSE` & `django_nats_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.3.5/README.md` & `django_nats_client-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-nats-client)](https://github.com/C0D1UM/django-nats-client)
 
 ## Features
 
 - Wrapper of NATS's [nats-py](https://github.com/nats-io/nats.py)
 - Django management command to listen for incoming NATS messages
 - Automatically serialize/deserialize message from/to JSON format
-- Easy-to-call method for sending NATS messages
+- Easy-to-call method for publishing NATS messages
+- Support NATS JetStream pull subscription
 
 ## Installation
 
 ```bash
 pip install django-nats-client
 ```
 
@@ -33,47 +34,56 @@
    ```
 
 1. Put NATS connection configuration in settings
 
    ```python
    # settings.py
 
-   NATS_OPTIONS = {
-       'servers': ['nats://localhost:4222'],
-       'max_reconnect_attempts': 2,
-       'connect_timeout': 1,
-       ...
-   }
-   NATS_LISTENING_SUBJECT = 'default'
+   NATS_SERVERS = 'nats://localhost:4222'
+   NATS_NAMESPACE = 'foo'
    ```
 
 ## Usage
 
 ### Listen for messages
 
 1. Create a new callback method and register
 
    ```python
    # common/nats.py
 
    import nats_client
+   
+   @nats_client.register
+   def new_message(message: str):
+       print(message)
 
    @nats_client.register
    def get_year_from_date(date: str):
        return date.year
 
    # custom name
    @nats_client.register('get_current_time')
    def current_time():
        return datetime.datetime.now().strftime('%H:%M')
 
    # without decorator
    def current_time():
        return datetime.datetime.now().strftime('%H:%M')
    nats_client.register('get_current_time', current_time)
+   
+   # JetStream
+   @nats_client.register(js=True)
+   def new_message(message: str):
+       print(message)
+   
+   # JetStream from other namespace
+   @nats_client.register(namespace='bar', js=True)
+   def new_message_from_bar(message: str):
+       print(message)
    ```
 
 1. Import previously file in `ready` method of your `apps.py`
 
    ```python
    # common/apps.py
 
@@ -89,69 +99,78 @@
    ```bash
    python manage.py nats_listener
 
    # or with autoreload enabled (suite for development)
    python manage.py nats_listener --reload
    ```
 
-### Sending message
+### Publishing message
 
 ```python
 import nats_client
 
 arg = 'some arg'
-nats_client.send(
-   'subject_name',
-   'method_name',
-   arg,
-   keyword_arg=1,
-   another_keyword_arg=2,
+await nats_client.publish(
+    'subject_name',
+    'method_name',
+    arg,
+    keyword_arg=1,
+    another_keyword_arg=2,
 )
 ```
 
 Examples
 
 ```python
 import nats_client
 
-nats_client.send('default', 'new_message', 'Hello, world!')
-nats_client.send('default', 'project_created', 1, name='ACME')
+await nats_client.publish('default', 'new_message', 'Hello, world!')
+await nats_client.publish('default', 'project_created', 1, name='ACME')
+
+# JetStream
+await nats_client.publish('default', 'new_message', 'Hello, world!', _js=True)
+await nats_client.js_publish('default', 'new_message', 'Hello, world!')
 ```
 
 ### Request-Reply
 
 ```python
 import nats_client
 
 arg = 'some arg'
-nats_client.request(
-   'subject_name',
-   'method_name',
-   arg,
-   keyword_arg=1,
-   another_keyword_arg=2,
+await nats_client.request(
+    'subject_name',
+    'method_name',
+    arg,
+    keyword_arg=1,
+    another_keyword_arg=2,
 )
 ```
 
 Examples
 
 ```python
 import nats_client
 
-year = nats_client.request('default', 'get_year_from_date', datetime.date(2022, 1, 1))  # 2022
-current_time = nats_client.request('default', 'get_current_time')  # 12:11
+year = await nats_client.request('default', 'get_year_from_date', datetime.date(2022, 1, 1))  # 2022
+current_time = await nats_client.request('default', 'get_current_time')  # 12:11
 ```
 
 ## Settings
 
-| Key                      | Required | Default   | Description                                       |
-|--------------------------|----------|-----------|---------------------------------------------------|
-| `NATS_OPTIONS`           | Yes      |           | Configuration to be passed in `nats.connect()`    |
-| `NATS_LISTENING_SUBJECT` | No       | 'default' | Subject for registering callback function         |
-| `NATS_REQUEST_TIMEOUT`   | No       | 1         | Timeout when using `request()` (in seconds)       |
+| Key                            | Type               | Required | Default                   | Description                                                       |
+|--------------------------------|--------------------|----------|---------------------------|-------------------------------------------------------------------|
+| `NATS_SERVERS`                 | `str \| list[str]` | Yes      |                           | NATS server's host(s)                                             |                                                                   |
+| `NATS_NAMESPACE`               | `str`              | No       | `'default'`               | Main namespace using for prefixing subject, stream name, and etc. |
+| `NATS_REQUEST_TIMEOUT`         | `int`              | No       | `1`                       | Timeout when using `request()` (in seconds)                       |
+| `NATS_OPTIONS`                 | `dict`             | No       | `{}`                      | Other configuration to be passed in `nats.connect()`              |
+| `NATS_JETSTREAM_ENABLED`       | `bool`             | No       | `True`                    | Enable JetStream                                                  |
+| `NATS_JETSTREAM_DURABLE_NAME`  | `str`              | No       | `settings.NATS_NAMESPACE` | Durable name which is unique across all subscriptions             |
+| `NATS_JETSTREAM_CREATE_STREAM` | `bool`             | No       | `True`                    | Automatically create stream named in `NATS_NAMESPACE`             |
+| `NATS_JETSTREAM_CONFIG`        | `dict`             | No       | `{}`                      | Extra configuration for JetStream streams                         |
 
 ## Development
 
 ### Requirements
 
 - Docker
 - Python
```

### Comparing `django_nats_client-0.3.5/nats_client/clients.py` & `django_nats_client-0.4.0/nats_client/clients.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,75 @@
+__all__ = ['request', 'request_sync', 'publish', 'publish_sync', 'js_publish', 'js_publish_sync']
+
 import asyncio
+import functools
 import json
 
+import jsonpickle
 from django.conf import settings
 from nats.aio.client import Client
 
+from .exceptions import NatsClientException
 from .types import ResponseType
 from .utils import parse_arguments
 
 DEFAULT_REQUEST_TIMEOUT = 1
 
 
-async def request_async(subject_name: str, method_name: str, *args, _timeout: float = None, **kwargs) -> ResponseType:
-    payload = parse_arguments(method_name, args, kwargs)
+async def request(
+        namespace: str, method_name: str, *args, _timeout: float = None, _raw=False, **kwargs
+) -> ResponseType:
+    payload = parse_arguments(args, kwargs)
 
     nc = Client()
     await nc.connect(**settings.NATS_OPTIONS)
 
     timeout = _timeout or getattr(settings, 'NATS_REQUEST_TIMEOUT', DEFAULT_REQUEST_TIMEOUT)
     try:
-        response = await nc.request(subject_name, payload, timeout=timeout)
+        response = await nc.request(f'{namespace}.{method_name}', payload, timeout=timeout)
     finally:
         await nc.close()
 
     data = response.data.decode()
-    return json.loads(data)['result']
+    parsed = json.loads(data)
+
+    if _raw:
+        parsed.pop('pickled_exc', None)
+        return parsed
+
+    if not parsed['success']:
+        try:
+            exc = jsonpickle.decode(parsed['pickled_exc'])
+        except TypeError:
+            exc = NatsClientException(parsed['error'] + ': ' + parsed['message'])
+
+        raise exc
+
+    return parsed['result']
+
+
+def request_sync(*args, **kwargs):
+    return asyncio.run(request(*args, **kwargs))
 
 
-async def send_async(subject_name: str, method_name: str, *args, **kwargs) -> None:
-    payload = parse_arguments(method_name, args, kwargs)
+async def publish(namespace: str, method_name: str, *args, _js=False, **kwargs) -> None:
+    payload = parse_arguments(args, kwargs)
 
     nc = Client()
     await nc.connect(**settings.NATS_OPTIONS)
 
     try:
-        await nc.publish(subject_name, payload)
+        if _js:
+            js = nc.jetstream()
+            await js.publish(f'{namespace}.js.{method_name}', payload)
+        else:
+            await nc.publish(f'{namespace}.{method_name}', payload)
     finally:
         await nc.close()
 
 
-def request(*args, **kwargs):
-    return asyncio.run(request_async(*args, **kwargs))
+def publish_sync(*args, **kwargs):
+    return asyncio.run(publish(*args, **kwargs))
 
 
-def send(*args, **kwargs):
-    return asyncio.run(send_async(*args, **kwargs))
+js_publish = functools.partial(publish, _js=True)
+js_publish_sync = functools.partial(publish_sync, _js=True)
```

### Comparing `django_nats_client-0.3.5/nats_client/utils.py` & `django_nats_client-0.4.0/nats_client/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 
 from asgiref.sync import SyncToAsync
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import close_old_connections
 
 
-def parse_arguments(method_name: str, args: tuple, kwargs: dict) -> bytes:
+def parse_arguments(args: tuple, kwargs: dict) -> bytes:
     msg = {
-        'name': method_name,
         'args': args,
         'kwargs': kwargs,
     }
     return json.dumps(msg, cls=DjangoJSONEncoder).encode()
 
 
 # pylint: disable=invalid-name
```

### Comparing `django_nats_client-0.3.5/pyproject.toml` & `django_nats_client-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "django-nats-client"
-version = "0.3.5"
+version = "0.4.0"
 description = ""
 authors = ["CODIUM <support@codium.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/C0D1UM/django-nats-client"
 keywords = ["django", "nats", "listener", "python"]
 packages = [
     { include = "nats_client" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = ">=3.1"
 nats-py = "^2"
+jsonpickle = "^3.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2"
 yapf = "^0"
 toml = "^0"
 ipdb = "^0"
 django-environ = "^0.9"
```

### Comparing `django_nats_client-0.3.5/PKG-INFO` & `django_nats_client-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-nats-client
-Version: 0.3.5
+Version: 0.4.0
 Summary: 
 Home-page: https://github.com/C0D1UM/django-nats-client
 License: MIT
 Keywords: django,nats,listener,python
 Author: CODIUM
 Author-email: support@codium.co
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=3.1)
+Requires-Dist: jsonpickle (>=3.0,<4.0)
 Requires-Dist: nats-py (>=2,<3)
 Project-URL: Repository, https://github.com/C0D1UM/django-nats-client
 Description-Content-Type: text/markdown
 
 # Django NATS
 
 [![GitHub](https://img.shields.io/github/license/C0D1UM/django-nats-client)](https://github.com/C0D1UM/django-nats-client/blob/main/LICENSE)
@@ -28,15 +29,16 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-nats-client)](https://github.com/C0D1UM/django-nats-client)
 
 ## Features
 
 - Wrapper of NATS's [nats-py](https://github.com/nats-io/nats.py)
 - Django management command to listen for incoming NATS messages
 - Automatically serialize/deserialize message from/to JSON format
-- Easy-to-call method for sending NATS messages
+- Easy-to-call method for publishing NATS messages
+- Support NATS JetStream pull subscription
 
 ## Installation
 
 ```bash
 pip install django-nats-client
 ```
 
@@ -54,47 +56,56 @@
    ```
 
 1. Put NATS connection configuration in settings
 
    ```python
    # settings.py
 
-   NATS_OPTIONS = {
-       'servers': ['nats://localhost:4222'],
-       'max_reconnect_attempts': 2,
-       'connect_timeout': 1,
-       ...
-   }
-   NATS_LISTENING_SUBJECT = 'default'
+   NATS_SERVERS = 'nats://localhost:4222'
+   NATS_NAMESPACE = 'foo'
    ```
 
 ## Usage
 
 ### Listen for messages
 
 1. Create a new callback method and register
 
    ```python
    # common/nats.py
 
    import nats_client
+   
+   @nats_client.register
+   def new_message(message: str):
+       print(message)
 
    @nats_client.register
    def get_year_from_date(date: str):
        return date.year
 
    # custom name
    @nats_client.register('get_current_time')
    def current_time():
        return datetime.datetime.now().strftime('%H:%M')
 
    # without decorator
    def current_time():
        return datetime.datetime.now().strftime('%H:%M')
    nats_client.register('get_current_time', current_time)
+   
+   # JetStream
+   @nats_client.register(js=True)
+   def new_message(message: str):
+       print(message)
+   
+   # JetStream from other namespace
+   @nats_client.register(namespace='bar', js=True)
+   def new_message_from_bar(message: str):
+       print(message)
    ```
 
 1. Import previously file in `ready` method of your `apps.py`
 
    ```python
    # common/apps.py
 
@@ -110,69 +121,78 @@
    ```bash
    python manage.py nats_listener
 
    # or with autoreload enabled (suite for development)
    python manage.py nats_listener --reload
    ```
 
-### Sending message
+### Publishing message
 
 ```python
 import nats_client
 
 arg = 'some arg'
-nats_client.send(
-   'subject_name',
-   'method_name',
-   arg,
-   keyword_arg=1,
-   another_keyword_arg=2,
+await nats_client.publish(
+    'subject_name',
+    'method_name',
+    arg,
+    keyword_arg=1,
+    another_keyword_arg=2,
 )
 ```
 
 Examples
 
 ```python
 import nats_client
 
-nats_client.send('default', 'new_message', 'Hello, world!')
-nats_client.send('default', 'project_created', 1, name='ACME')
+await nats_client.publish('default', 'new_message', 'Hello, world!')
+await nats_client.publish('default', 'project_created', 1, name='ACME')
+
+# JetStream
+await nats_client.publish('default', 'new_message', 'Hello, world!', _js=True)
+await nats_client.js_publish('default', 'new_message', 'Hello, world!')
 ```
 
 ### Request-Reply
 
 ```python
 import nats_client
 
 arg = 'some arg'
-nats_client.request(
-   'subject_name',
-   'method_name',
-   arg,
-   keyword_arg=1,
-   another_keyword_arg=2,
+await nats_client.request(
+    'subject_name',
+    'method_name',
+    arg,
+    keyword_arg=1,
+    another_keyword_arg=2,
 )
 ```
 
 Examples
 
 ```python
 import nats_client
 
-year = nats_client.request('default', 'get_year_from_date', datetime.date(2022, 1, 1))  # 2022
-current_time = nats_client.request('default', 'get_current_time')  # 12:11
+year = await nats_client.request('default', 'get_year_from_date', datetime.date(2022, 1, 1))  # 2022
+current_time = await nats_client.request('default', 'get_current_time')  # 12:11
 ```
 
 ## Settings
 
-| Key                      | Required | Default   | Description                                       |
-|--------------------------|----------|-----------|---------------------------------------------------|
-| `NATS_OPTIONS`           | Yes      |           | Configuration to be passed in `nats.connect()`    |
-| `NATS_LISTENING_SUBJECT` | No       | 'default' | Subject for registering callback function         |
-| `NATS_REQUEST_TIMEOUT`   | No       | 1         | Timeout when using `request()` (in seconds)       |
+| Key                            | Type               | Required | Default                   | Description                                                       |
+|--------------------------------|--------------------|----------|---------------------------|-------------------------------------------------------------------|
+| `NATS_SERVERS`                 | `str \| list[str]` | Yes      |                           | NATS server's host(s)                                             |                                                                   |
+| `NATS_NAMESPACE`               | `str`              | No       | `'default'`               | Main namespace using for prefixing subject, stream name, and etc. |
+| `NATS_REQUEST_TIMEOUT`         | `int`              | No       | `1`                       | Timeout when using `request()` (in seconds)                       |
+| `NATS_OPTIONS`                 | `dict`             | No       | `{}`                      | Other configuration to be passed in `nats.connect()`              |
+| `NATS_JETSTREAM_ENABLED`       | `bool`             | No       | `True`                    | Enable JetStream                                                  |
+| `NATS_JETSTREAM_DURABLE_NAME`  | `str`              | No       | `settings.NATS_NAMESPACE` | Durable name which is unique across all subscriptions             |
+| `NATS_JETSTREAM_CREATE_STREAM` | `bool`             | No       | `True`                    | Automatically create stream named in `NATS_NAMESPACE`             |
+| `NATS_JETSTREAM_CONFIG`        | `dict`             | No       | `{}`                      | Extra configuration for JetStream streams                         |
 
 ## Development
 
 ### Requirements
 
 - Docker
 - Python
```


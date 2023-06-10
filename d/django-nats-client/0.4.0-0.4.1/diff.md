# Comparing `tmp/django_nats_client-0.4.0.tar.gz` & `tmp/django_nats_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nats_client-0.4.0.tar", max compression
+gzip compressed data, was "django_nats_client-0.4.1.tar", max compression
```

## Comparing `django_nats_client-0.4.0.tar` & `django_nats_client-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/LICENSE
--rw-r--r--   0        0        0     5566 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/README.md
--rw-r--r--   0        0        0       79 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/__init__.py
--rw-r--r--   0        0        0       96 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/apps.py
--rw-r--r--   0        0        0     1980 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/clients.py
--rw-r--r--   0        0        0      114 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/exceptions.py
--rw-r--r--   0        0        0      473 2023-06-10 18:55:29.402135 django_nats_client-0.4.0/nats_client/handlers.py
--rw-r--r--   0        0        0     5557 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/management/commands/nats_listener.py
--rw-r--r--   0        0        0     1336 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/registry.py
--rw-r--r--   0        0        0       84 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/types.py
--rw-r--r--   0        0        0      849 2023-06-10 18:55:29.406135 django_nats_client-0.4.0/nats_client/utils.py
--rw-r--r--   0        0        0      901 2023-06-10 18:55:43.474210 django_nats_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6334 1970-01-01 00:00:00.000000 django_nats_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6037 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/README.md
+-rw-r--r--   0        0        0       79 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/apps.py
+-rw-r--r--   0        0        0     2246 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/clients.py
+-rw-r--r--   0        0        0      114 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/exceptions.py
+-rw-r--r--   0        0        0      473 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/handlers.py
+-rw-r--r--   0        0        0     5545 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/management/commands/nats_listener.py
+-rw-r--r--   0        0        0     1336 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/registry.py
+-rw-r--r--   0        0        0       84 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/types.py
+-rw-r--r--   0        0        0      849 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/utils.py
+-rw-r--r--   0        0        0      901 2023-06-10 19:36:07.825202 django_nats_client-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6805 1970-01-01 00:00:00.000000 django_nats_client-0.4.1/PKG-INFO
```

### Comparing `django_nats_client-0.4.0/LICENSE` & `django_nats_client-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.0/README.md` & `django_nats_client-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-# Django NATS
+# Django NATS Client
 
 [![GitHub](https://img.shields.io/github/license/C0D1UM/django-nats-client)](https://github.com/C0D1UM/django-nats-client/blob/main/LICENSE)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/C0D1UM/django-nats-client/ci.yml?branch=main)](https://github.com/C0D1UM/django-nats-client/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/C0D1UM/django-nats-client/branch/main/graph/badge.svg?token=PN19DJ3SDF)](https://codecov.io/gh/C0D1UM/django-nats-client)
 [![PyPI](https://img.shields.io/pypi/v/django-nats-client)](https://pypi.org/project/django-nats-client/)  
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-nats-client)](https://github.com/C0D1UM/django-nats-client)
 
+## Important Notes
+
+> 🚨 The latest major version of this package, `v0.4.0`, has a numerous breaking changes.
+> Please review its [release note](https://github.com/C0D1UM/django-nats-client/releases/tag/v0.4.0).
+
 ## Features
 
 - Wrapper of NATS's [nats-py](https://github.com/nats-io/nats.py)
 - Django management command to listen for incoming NATS messages
 - Automatically serialize/deserialize message from/to JSON format
 - Easy-to-call method for publishing NATS messages
 - Support NATS JetStream pull subscription
@@ -153,24 +158,25 @@
 
 year = await nats_client.request('default', 'get_year_from_date', datetime.date(2022, 1, 1))  # 2022
 current_time = await nats_client.request('default', 'get_current_time')  # 12:11
 ```
 
 ## Settings
 
-| Key                            | Type               | Required | Default                   | Description                                                       |
-|--------------------------------|--------------------|----------|---------------------------|-------------------------------------------------------------------|
-| `NATS_SERVERS`                 | `str \| list[str]` | Yes      |                           | NATS server's host(s)                                             |                                                                   |
-| `NATS_NAMESPACE`               | `str`              | No       | `'default'`               | Main namespace using for prefixing subject, stream name, and etc. |
-| `NATS_REQUEST_TIMEOUT`         | `int`              | No       | `1`                       | Timeout when using `request()` (in seconds)                       |
-| `NATS_OPTIONS`                 | `dict`             | No       | `{}`                      | Other configuration to be passed in `nats.connect()`              |
-| `NATS_JETSTREAM_ENABLED`       | `bool`             | No       | `True`                    | Enable JetStream                                                  |
-| `NATS_JETSTREAM_DURABLE_NAME`  | `str`              | No       | `settings.NATS_NAMESPACE` | Durable name which is unique across all subscriptions             |
-| `NATS_JETSTREAM_CREATE_STREAM` | `bool`             | No       | `True`                    | Automatically create stream named in `NATS_NAMESPACE`             |
-| `NATS_JETSTREAM_CONFIG`        | `dict`             | No       | `{}`                      | Extra configuration for JetStream streams                         |
+| Key                            | Type        | Required                      | Default                   | Description                                                       |
+|--------------------------------|-------------|-------------------------------|---------------------------|-------------------------------------------------------------------|
+| `NATS_SERVER`                  | `str`       | Required if no `NATS_SERVERS` |                           | NATS server's host                                                |
+| `NATS_SERVERS`                 | `list[str]` | Required if no `NATS_SERVER`  |                           | NATS server's hosts (for NATS cluster)                            |
+| `NATS_NAMESPACE`               | `str`       | No                            | `'default'`               | Main namespace using for prefixing subject, stream name, and etc. |
+| `NATS_REQUEST_TIMEOUT`         | `int`       | No                            | `1`                       | Timeout when using `request()` (in seconds)                       |
+| `NATS_OPTIONS`                 | `dict`      | No                            | `{}`                      | Other configuration to be passed in `nats.connect()`              |
+| `NATS_JETSTREAM_ENABLED`       | `bool`      | No                            | `True`                    | Enable JetStream                                                  |
+| `NATS_JETSTREAM_DURABLE_NAME`  | `str`       | No                            | `settings.NATS_NAMESPACE` | Durable name which is unique across all subscriptions             |
+| `NATS_JETSTREAM_CREATE_STREAM` | `bool`      | No                            | `True`                    | Automatically create stream named in `NATS_NAMESPACE`             |
+| `NATS_JETSTREAM_CONFIG`        | `dict`      | No                            | `{}`                      | Extra configuration for JetStream streams                         |
 
 ## Development
 
 ### Requirements
 
 - Docker
 - Python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_nats_client-0.4.0/nats_client/clients.py` & `django_nats_client-0.4.1/nats_client/clients.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,21 +11,32 @@
 from .exceptions import NatsClientException
 from .types import ResponseType
 from .utils import parse_arguments
 
 DEFAULT_REQUEST_TIMEOUT = 1
 
 
+async def get_nc_client(nc: Client = None):
+    if nc is None:
+        nc = Client()
+
+    server = getattr(settings, 'NATS_SERVER', None)
+    servers = [server] if server else getattr(settings, 'NATS_SERVERS', [])
+    options = getattr(settings, 'NATS_OPTIONS', {})
+
+    await nc.connect(servers=servers, **options)
+    return nc
+
+
 async def request(
         namespace: str, method_name: str, *args, _timeout: float = None, _raw=False, **kwargs
 ) -> ResponseType:
     payload = parse_arguments(args, kwargs)
 
-    nc = Client()
-    await nc.connect(**settings.NATS_OPTIONS)
+    nc = await get_nc_client()
 
     timeout = _timeout or getattr(settings, 'NATS_REQUEST_TIMEOUT', DEFAULT_REQUEST_TIMEOUT)
     try:
         response = await nc.request(f'{namespace}.{method_name}', payload, timeout=timeout)
     finally:
         await nc.close()
 
@@ -50,16 +61,15 @@
 def request_sync(*args, **kwargs):
     return asyncio.run(request(*args, **kwargs))
 
 
 async def publish(namespace: str, method_name: str, *args, _js=False, **kwargs) -> None:
     payload = parse_arguments(args, kwargs)
 
-    nc = Client()
-    await nc.connect(**settings.NATS_OPTIONS)
+    nc = await get_nc_client()
 
     try:
         if _js:
             js = nc.jetstream()
             await js.publish(f'{namespace}.js.{method_name}', payload)
         else:
             await nc.publish(f'{namespace}.{method_name}', payload)
```

### Comparing `django_nats_client-0.4.0/nats_client/management/commands/nats_listener.py` & `django_nats_client-0.4.1/nats_client/management/commands/nats_listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from django.core.serializers.json import DjangoJSONEncoder
 from django.utils import autoreload
 from nats.aio.client import Client
 from nats.aio.errors import ErrNoServers
 from nats.aio.errors import ErrTimeout
 from nats.aio.msg import Msg
 
+from ...clients import get_nc_client
 from ...handlers import nats_handler
 from ...registry import default_registry
 
 
 class Command(BaseCommand):
     help = "Starts a NATS listener."
 
@@ -59,18 +60,18 @@
     async def nats_coroutine(self):
         namespace = getattr(settings, 'NATS_NAMESPACE', 'default')
         durable_name = getattr(settings, 'NATS_JETSTREAM_DURABLE_NAME', namespace)
         create_stream = getattr(settings, 'NATS_JETSTREAM_CRATE_STREAM', True)
         stream_config = getattr(settings, 'NATS_JETSTREAM_CONFIG', {})
 
         try:
-            await self.nats.connect(**settings.NATS_OPTIONS)
+            await get_nc_client(self.nats)
             print('** Connected to NATS server')
 
-            if getattr(settings, 'NATS_JETSTREAM_ENABLED', False):
+            if getattr(settings, 'NATS_JETSTREAM_ENABLED', True):
                 self.js = self.nats.jetstream()
                 print('** Initialized JetStream')
         except (ErrNoServers, ErrTimeout) as e:
             raise e
 
         if not default_registry.registry:
             print('** No function found!')
@@ -90,15 +91,14 @@
             data = msg.data.decode()
             reply = msg.reply
             func_name = msg.subject
             print(f'Received a message on function `{func_name}`: {data}')
             asyncio.ensure_future(self.handler(func_name, data, reply=reply))
 
         async def fetch(psub):
-            print('fetching')
             try:
                 msgs = await psub.fetch(timeout=1)
                 for msg in msgs:
                     data = msg.data.decode()
                     func_name = msg.subject
                     print(f'Received a message on JetStream function `{func_name}`: {data}')
                     asyncio.ensure_future(self.handler(func_name, data))
```

### Comparing `django_nats_client-0.4.0/nats_client/registry.py` & `django_nats_client-0.4.1/nats_client/registry.py`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.0/nats_client/utils.py` & `django_nats_client-0.4.1/nats_client/utils.py`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.0/pyproject.toml` & `django_nats_client-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-nats-client"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["CODIUM <support@codium.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/C0D1UM/django-nats-client"
 keywords = ["django", "nats", "listener", "python"]
 packages = [
```

### Comparing `django_nats_client-0.4.0/PKG-INFO` & `django_nats_client-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nats-client
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Home-page: https://github.com/C0D1UM/django-nats-client
 License: MIT
 Keywords: django,nats,listener,python
 Author: CODIUM
 Author-email: support@codium.co
 Requires-Python: >=3.8,<4.0
@@ -16,22 +16,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=3.1)
 Requires-Dist: jsonpickle (>=3.0,<4.0)
 Requires-Dist: nats-py (>=2,<3)
 Project-URL: Repository, https://github.com/C0D1UM/django-nats-client
 Description-Content-Type: text/markdown
 
-# Django NATS
+# Django NATS Client
 
 [![GitHub](https://img.shields.io/github/license/C0D1UM/django-nats-client)](https://github.com/C0D1UM/django-nats-client/blob/main/LICENSE)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/C0D1UM/django-nats-client/ci.yml?branch=main)](https://github.com/C0D1UM/django-nats-client/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/C0D1UM/django-nats-client/branch/main/graph/badge.svg?token=PN19DJ3SDF)](https://codecov.io/gh/C0D1UM/django-nats-client)
 [![PyPI](https://img.shields.io/pypi/v/django-nats-client)](https://pypi.org/project/django-nats-client/)  
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-nats-client)](https://github.com/C0D1UM/django-nats-client)
 
+## Important Notes
+
+> 🚨 The latest major version of this package, `v0.4.0`, has a numerous breaking changes.
+> Please review its [release note](https://github.com/C0D1UM/django-nats-client/releases/tag/v0.4.0).
+
 ## Features
 
 - Wrapper of NATS's [nats-py](https://github.com/nats-io/nats.py)
 - Django management command to listen for incoming NATS messages
 - Automatically serialize/deserialize message from/to JSON format
 - Easy-to-call method for publishing NATS messages
 - Support NATS JetStream pull subscription
@@ -175,24 +180,25 @@
 
 year = await nats_client.request('default', 'get_year_from_date', datetime.date(2022, 1, 1))  # 2022
 current_time = await nats_client.request('default', 'get_current_time')  # 12:11
 ```
 
 ## Settings
 
-| Key                            | Type               | Required | Default                   | Description                                                       |
-|--------------------------------|--------------------|----------|---------------------------|-------------------------------------------------------------------|
-| `NATS_SERVERS`                 | `str \| list[str]` | Yes      |                           | NATS server's host(s)                                             |                                                                   |
-| `NATS_NAMESPACE`               | `str`              | No       | `'default'`               | Main namespace using for prefixing subject, stream name, and etc. |
-| `NATS_REQUEST_TIMEOUT`         | `int`              | No       | `1`                       | Timeout when using `request()` (in seconds)                       |
-| `NATS_OPTIONS`                 | `dict`             | No       | `{}`                      | Other configuration to be passed in `nats.connect()`              |
-| `NATS_JETSTREAM_ENABLED`       | `bool`             | No       | `True`                    | Enable JetStream                                                  |
-| `NATS_JETSTREAM_DURABLE_NAME`  | `str`              | No       | `settings.NATS_NAMESPACE` | Durable name which is unique across all subscriptions             |
-| `NATS_JETSTREAM_CREATE_STREAM` | `bool`             | No       | `True`                    | Automatically create stream named in `NATS_NAMESPACE`             |
-| `NATS_JETSTREAM_CONFIG`        | `dict`             | No       | `{}`                      | Extra configuration for JetStream streams                         |
+| Key                            | Type        | Required                      | Default                   | Description                                                       |
+|--------------------------------|-------------|-------------------------------|---------------------------|-------------------------------------------------------------------|
+| `NATS_SERVER`                  | `str`       | Required if no `NATS_SERVERS` |                           | NATS server's host                                                |
+| `NATS_SERVERS`                 | `list[str]` | Required if no `NATS_SERVER`  |                           | NATS server's hosts (for NATS cluster)                            |
+| `NATS_NAMESPACE`               | `str`       | No                            | `'default'`               | Main namespace using for prefixing subject, stream name, and etc. |
+| `NATS_REQUEST_TIMEOUT`         | `int`       | No                            | `1`                       | Timeout when using `request()` (in seconds)                       |
+| `NATS_OPTIONS`                 | `dict`      | No                            | `{}`                      | Other configuration to be passed in `nats.connect()`              |
+| `NATS_JETSTREAM_ENABLED`       | `bool`      | No                            | `True`                    | Enable JetStream                                                  |
+| `NATS_JETSTREAM_DURABLE_NAME`  | `str`       | No                            | `settings.NATS_NAMESPACE` | Durable name which is unique across all subscriptions             |
+| `NATS_JETSTREAM_CREATE_STREAM` | `bool`      | No                            | `True`                    | Automatically create stream named in `NATS_NAMESPACE`             |
+| `NATS_JETSTREAM_CONFIG`        | `dict`      | No                            | `{}`                      | Extra configuration for JetStream streams                         |
 
 ## Development
 
 ### Requirements
 
 - Docker
 - Python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


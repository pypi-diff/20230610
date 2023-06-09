# Comparing `tmp/yatracker_linker-0.3.6.tar.gz` & `tmp/yatracker_linker-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatracker_linker-0.3.6.tar", max compression
+gzip compressed data, was "yatracker_linker-0.3.7.tar", max compression
```

## Comparing `yatracker_linker-0.3.6.tar` & `yatracker_linker-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1072 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/LICENSE
--rw-r--r--   0        0        0      111 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/README.rst
--rw-r--r--   0        0        0     1051 2023-04-30 08:45:43.050813 yatracker_linker-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/__init__.py
--rw-r--r--   0        0        0     1236 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/__main__.py
--rw-r--r--   0        0        0      825 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/args.py
--rw-r--r--   0        0        0      621 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/deps.py
--rw-r--r--   0        0        0      621 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/service.py
--rw-r--r--   0        0        0      865 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/tracker_client.py
--rw-r--r--   0        0        0        0 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/utils.py
--rw-r--r--   0        0        0        0 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/views/__init__.py
--rw-r--r--   0        0        0      444 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/views/base.py
--rw-r--r--   0        0        0     4775 2023-04-30 08:45:19.626605 yatracker_linker-0.3.6/yatracker_linker/views/events.py
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-09 22:28:06.063791 yatracker_linker-0.3.7/LICENSE
+-rw-r--r--   0        0        0      111 2023-06-09 22:28:06.063791 yatracker_linker-0.3.7/README.rst
+-rw-r--r--   0        0        0     1051 2023-06-09 22:28:34.705704 yatracker_linker-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/__init__.py
+-rw-r--r--   0        0        0     1245 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/__main__.py
+-rw-r--r--   0        0        0     1142 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/args.py
+-rw-r--r--   0        0        0      963 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/deps.py
+-rw-r--r--   0        0        0      808 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/gitlab_client.py
+-rw-r--r--   0        0        0      916 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/service.py
+-rw-r--r--   0        0        0      865 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/tracker_client.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/__init__.py
+-rw-r--r--   0        0        0      609 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/base.py
+-rw-r--r--   0        0        0     4775 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/events.py
+-rw-r--r--   0        0        0     1829 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/proxy.py
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.7/PKG-INFO
```

### Comparing `yatracker_linker-0.3.6/LICENSE` & `yatracker_linker-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.6/pyproject.toml` & `yatracker_linker-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yatracker-linker"
-version = "0.3.6"
+version = "0.3.7"
 description = "Yandex Tracker issues integration"
 license = "MIT"
 authors = ["Alexander Vasin <hi@alvass.in>"]
 readme = "README.rst"
 packages = [{include = "yatracker_linker"}]
 
 [tool.poetry.scripts]
```

### Comparing `yatracker_linker-0.3.6/yatracker_linker/__main__.py` & `yatracker_linker-0.3.7/yatracker_linker/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     config_deps(parser)
 
     services: List[Service] = [
         HttpService(
             address=parser.address,
             port=parser.port,
-            gitlab_tokens=parser.gitlab_token
+            gitlab_tokens=parser.gitlab.incoming_token
         )
     ]
 
     if parser.sentry.dsn:
         services.append(
             RavenSender(
                 sentry_dsn=parser.sentry.dsn,
```

### Comparing `yatracker_linker-0.3.6/yatracker_linker/args.py` & `yatracker_linker-0.3.7/yatracker_linker/args.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,23 +12,33 @@
 
 class TrackerGroup(argclass.Group):
     url: URL
     token: str
     link_origin: str
 
 
+class GitlabGroup(argclass.Group):
+    url: URL
+    incoming_token: frozenset[str] = argclass.Argument(
+        type=str, nargs='*', converter=frozenset, help=(
+            'Tokens used by gitlab to authenticate at linker using '
+            'X-Gitlab-Token header'
+        )
+    )
+    outgoing_token: str = argclass.Argument(type=str, help=(
+        'Token used by linker to authenticate at gitlab to retrieve merge '
+        'requests information'
+    ))
+
+
 class Parser(argclass.Parser):
     log_level: int = argclass.LogLevel
     log_format: str = argclass.Argument(
         choices=LogFormat.choices(),
         default=LogFormat.default()
     )
     address: str = argclass.Argument(default='0.0.0.0')
     port: int
 
-    gitlab_token: frozenset[str] = argclass.Argument(
-        type=str, nargs='*', converter=frozenset,
-        help='Tokens used by gitlab to authenticate with X-Gitlab-Token header'
-    )
-
+    gitlab = GitlabGroup(title='Gitlab options')
     sentry = SentryGroup(title='Sentry options')
     tracker = TrackerGroup(title='Tracker options')
```

### Comparing `yatracker_linker-0.3.6/yatracker_linker/service.py` & `yatracker_linker-0.3.7/yatracker_linker/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from aiohttp import web
 from aiomisc.service.aiohttp import AIOHTTPService
 
+from yatracker_linker.gitlab_client import GitlabClient
 from yatracker_linker.tracker_client import TrackerClient
 from yatracker_linker.views.events import GitlabView
+from yatracker_linker.views.proxy import ProxyView
 
 
 class HttpService(AIOHTTPService):
-    __dependencies__ = ('st_client',)
+    __dependencies__ = (
+        'st_client',
+        'gitlab_client',
+    )
     __required__ = ('gitlab_tokens', )
 
     gitlab_tokens: frozenset[str]
     st_client: TrackerClient
+    gitlab_client: GitlabClient
 
     async def create_application(self):
         app = web.Application()
         app.router.add_route('POST', GitlabView.URL_PATH, GitlabView)
+        app.router.add_route('GET', ProxyView.URL_PATH, ProxyView)
 
         app['gitlab_tokens'] = self.gitlab_tokens
         app['st_client'] = self.st_client
+        app['gitlab_client'] = self.gitlab_client
 
         return app
```

### Comparing `yatracker_linker-0.3.6/yatracker_linker/tracker_client.py` & `yatracker_linker-0.3.7/yatracker_linker/tracker_client.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.6/yatracker_linker/views/events.py` & `yatracker_linker-0.3.7/yatracker_linker/views/events.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.6/PKG-INFO` & `yatracker_linker-0.3.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatracker-linker
-Version: 0.3.6
+Version: 0.3.7
 Summary: Yandex Tracker issues integration
 License: MIT
 Author: Alexander Vasin
 Author-email: hi@alvass.in
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/yatracker_linker-0.3.7.tar.gz` & `tmp/yatracker_linker-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatracker_linker-0.3.7.tar", max compression
+gzip compressed data, was "yatracker_linker-0.3.8.tar", max compression
```

## Comparing `yatracker_linker-0.3.7.tar` & `yatracker_linker-0.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1072 2023-06-09 22:28:06.063791 yatracker_linker-0.3.7/LICENSE
--rw-r--r--   0        0        0      111 2023-06-09 22:28:06.063791 yatracker_linker-0.3.7/README.rst
--rw-r--r--   0        0        0     1051 2023-06-09 22:28:34.705704 yatracker_linker-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/__init__.py
--rw-r--r--   0        0        0     1245 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/__main__.py
--rw-r--r--   0        0        0     1142 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/args.py
--rw-r--r--   0        0        0      963 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/deps.py
--rw-r--r--   0        0        0      808 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/gitlab_client.py
--rw-r--r--   0        0        0      916 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/service.py
--rw-r--r--   0        0        0      865 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/tracker_client.py
--rw-r--r--   0        0        0        0 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/utils.py
--rw-r--r--   0        0        0        0 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/__init__.py
--rw-r--r--   0        0        0      609 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/base.py
--rw-r--r--   0        0        0     4775 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/events.py
--rw-r--r--   0        0        0     1829 2023-06-09 22:28:06.067791 yatracker_linker-0.3.7/yatracker_linker/views/proxy.py
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/LICENSE
+-rw-r--r--   0        0        0      111 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/README.rst
+-rw-r--r--   0        0        0     1051 2023-06-09 22:50:04.490176 yatracker_linker-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/__init__.py
+-rw-r--r--   0        0        0     1245 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/__main__.py
+-rw-r--r--   0        0        0     1142 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/args.py
+-rw-r--r--   0        0        0     1213 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/deps.py
+-rw-r--r--   0        0        0      973 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/gitlab_client.py
+-rw-r--r--   0        0        0     1018 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/service.py
+-rw-r--r--   0        0        0      865 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/tracker_client.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/views/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/views/base.py
+-rw-r--r--   0        0        0     4775 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/views/events.py
+-rw-r--r--   0        0        0     1787 2023-06-09 22:49:38.477478 yatracker_linker-0.3.8/yatracker_linker/views/proxy.py
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 yatracker_linker-0.3.8/PKG-INFO
```

### Comparing `yatracker_linker-0.3.7/LICENSE` & `yatracker_linker-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.7/pyproject.toml` & `yatracker_linker-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yatracker-linker"
-version = "0.3.7"
+version = "0.3.8"
 description = "Yandex Tracker issues integration"
 license = "MIT"
 authors = ["Alexander Vasin <hi@alvass.in>"]
 readme = "README.rst"
 packages = [{include = "yatracker_linker"}]
 
 [tool.poetry.scripts]
```

### Comparing `yatracker_linker-0.3.7/yatracker_linker/__main__.py` & `yatracker_linker-0.3.8/yatracker_linker/__main__.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.7/yatracker_linker/args.py` & `yatracker_linker-0.3.8/yatracker_linker/args.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.7/yatracker_linker/deps.py` & `yatracker_linker-0.3.8/yatracker_linker/deps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+import logging
+
 from aiohttp import ClientSession
 from aiomisc_dependency import dependency, reset_store
 
 from yatracker_linker.args import Parser
 from yatracker_linker.gitlab_client import GitlabClient
 from yatracker_linker.tracker_client import TrackerClient
 
 
+log = logging.getLogger(__name__)
+
+
 async def st_client(parser: Parser):
     async with ClientSession() as session:
         yield TrackerClient(
             session=session,
             url=parser.tracker.url,
             token=parser.tracker.token,
             link_origin=parser.tracker.link_origin
@@ -21,19 +26,26 @@
         yield GitlabClient(
             session=session,
             url=parser.gitlab.url,
             token=parser.gitlab.outgoing_token
         )
 
 
+async def gitlab_favicon(gitlab_client: GitlabClient):
+    icon = await gitlab_client.get_favicon()
+    log.info('Got favicon for gitlab: %r', icon)
+    return icon
+
+
 def config_deps(args):
 
     @dependency
     def parser() -> Parser:
         return args
 
     dependency(st_client)
     dependency(gitlab_client)
+    dependency(gitlab_favicon)
 
 
 def reset_deps():
     reset_store()
```

### Comparing `yatracker_linker-0.3.7/yatracker_linker/service.py` & `yatracker_linker-0.3.8/yatracker_linker/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 from yatracker_linker.views.proxy import ProxyView
 
 
 class HttpService(AIOHTTPService):
     __dependencies__ = (
         'st_client',
         'gitlab_client',
+        'gitlab_favicon',
     )
     __required__ = ('gitlab_tokens', )
 
     gitlab_tokens: frozenset[str]
     st_client: TrackerClient
     gitlab_client: GitlabClient
+    gitlab_favicon: str
 
     async def create_application(self):
         app = web.Application()
         app.router.add_route('POST', GitlabView.URL_PATH, GitlabView)
         app.router.add_route('GET', ProxyView.URL_PATH, ProxyView)
 
         app['gitlab_tokens'] = self.gitlab_tokens
         app['st_client'] = self.st_client
         app['gitlab_client'] = self.gitlab_client
+        app['gitlab_favicon'] = self.gitlab_favicon
 
         return app
```

### Comparing `yatracker_linker-0.3.7/yatracker_linker/tracker_client.py` & `yatracker_linker-0.3.8/yatracker_linker/tracker_client.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.7/yatracker_linker/views/base.py` & `yatracker_linker-0.3.8/yatracker_linker/views/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,7 +18,11 @@
     @property
     def st_client(self) -> TrackerClient:
         return self.request.app['st_client']
 
     @property
     def gitlab_client(self) -> GitlabClient:
         return self.request.app['gitlab_client']
+
+    @property
+    def gitlab_favicon(self) -> str:
+        return self.request.app['gitlab_favicon']
```

### Comparing `yatracker_linker-0.3.7/yatracker_linker/views/events.py` & `yatracker_linker-0.3.8/yatracker_linker/views/events.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.3.7/yatracker_linker/views/proxy.py` & `yatracker_linker-0.3.8/yatracker_linker/views/proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,18 +29,15 @@
 
             log.exception(
                 'Unable to get merge request %r in project_id %r',
                 project_id, merge_request_id
             )
             raise
 
-        # self.request.url.path
-        # self.gitlab_client.get_merge_request()
-        # GET /projects/:id/merge_requests/:merge_request_iid
-        return json_response({
+        data = {
             'key': self.request.url.path,
             'summary': merge_request['title'],
             'assignee': {
                 'login': merge_request['author']['username']
             },
             'updated': merge_request['updated_at'],
             'resolution': {
@@ -50,8 +47,13 @@
                     else 'resolved'
                 ),
             },
             # opened, closed, merged or locked
             'status': {
                 'name': merge_request['state']
             }
-        })
+        }
+
+        if self.gitlab_favicon:
+            data['icon'] = self.gitlab_favicon
+
+        return json_response(data)
```

### Comparing `yatracker_linker-0.3.7/PKG-INFO` & `yatracker_linker-0.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatracker-linker
-Version: 0.3.7
+Version: 0.3.8
 Summary: Yandex Tracker issues integration
 License: MIT
 Author: Alexander Vasin
 Author-email: hi@alvass.in
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


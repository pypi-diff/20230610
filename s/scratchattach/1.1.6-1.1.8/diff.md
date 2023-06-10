# Comparing `tmp/scratchattach-1.1.6.tar.gz` & `tmp/scratchattach-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.1.6.tar", last modified: Sat May 20 15:27:15 2023, max compression
+gzip compressed data, was "scratchattach-1.1.8.tar", last modified: Sat Jun 10 15:52:15 2023, max compression
```

## Comparing `scratchattach-1.1.6.tar` & `scratchattach-1.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 15:27:15.134757 scratchattach-1.1.6/
--rw-rw-rw-   0        0        0    22055 2023-05-20 15:27:15.132676 scratchattach-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    20740 2023-05-07 17:32:19.000000 scratchattach-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 15:27:15.064044 scratchattach-1.1.6/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    12776 2023-05-20 15:26:23.000000 scratchattach-1.1.6/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    15496 2023-05-04 17:24:58.000000 scratchattach-1.1.6/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-05-07 17:01:33.000000 scratchattach-1.1.6/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6542 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18157 2023-05-07 17:16:17.000000 scratchattach-1.1.6/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17923 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9646 2023-05-07 17:16:12.000000 scratchattach-1.1.6/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-05-07 17:30:43.000000 scratchattach-1.1.6/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:27:15.128687 scratchattach-1.1.6/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22055 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 15:27:15.135875 scratchattach-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-05-20 15:26:45.000000 scratchattach-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:52:15.230413 scratchattach-1.1.8/
+-rw-rw-rw-   0        0        0    22096 2023-06-10 15:52:15.230413 scratchattach-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    20740 2023-05-07 17:32:19.000000 scratchattach-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 15:52:15.216995 scratchattach-1.1.8/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.1.8/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    13089 2023-06-10 15:19:07.000000 scratchattach-1.1.8/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    15620 2023-06-10 15:18:42.000000 scratchattach-1.1.8/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.1.8/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.1.8/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.1.8/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.1.8/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17923 2023-06-10 15:03:02.000000 scratchattach-1.1.8/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.1.8/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.1.8/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:52:15.229414 scratchattach-1.1.8/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22096 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 15:52:15.230413 scratchattach-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-06-10 15:19:12.000000 scratchattach-1.1.8/setup.py
```

### Comparing `scratchattach-1.1.6/PKG-INFO` & `scratchattach-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.6
+Version: 1.1.8
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
+License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -611,7 +613,9 @@
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
 
 If you need help with your code, leave a comment on TimMcCool's Scratch
 profile: https://scratch.mit.edu/users/TimMcCool/
+
+
```

### Comparing `scratchattach-1.1.6/README.md` & `scratchattach-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.6/scratchattach/_cloud.py` & `scratchattach-1.1.8/scratchattach/_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import websocket
 import json
 import requests
 from threading import Thread
 import time
 from . import _exceptions
 import traceback
+import warnings
 
 class _CloudMixin:
 
     def __init__(self, *, project_id, username="python", session_id=None, cloud_host=None, _allow_non_numeric=False, _no_reconnect=False):
         self._session_id = session_id
         self._username = username
         try:
@@ -75,23 +76,24 @@
                 enable_multithread=True,
             )
         except Exception:
             raise(_exceptions.ConnectionError)
 
     def set_var(self, variable, value):
         variable = variable.replace("☁ ", "")
-        value = str(value)
-        if len(value) > 256:
-            print("invalid cloud var (too long):", value)
-            raise(_exceptions.InvalidCloudValue)
-        x = value.replace(".", "")
-        x = x.replace("-", "")
-        if not x.isnumeric():
-            print("invalid cloud var (not numeric):", value)
-            raise(_exceptions.InvalidCloudValue)
+        if not (value is True or value is False or value in [float('inf'), -float('inf')]):
+            value = str(value)
+            if len(value) > 256:
+                warnings.warn("invalid cloud var (too long): "+str(value), Warning)
+                raise(_exceptions.InvalidCloudValue)
+            x = value.replace(".", "")
+            x = x.replace("-", "")
+            if not x.isnumeric():
+                warnings.warn("invalid cloud var (not numeric): "+str(value), Warning)
+                raise(_exceptions.InvalidCloudValue)
         while self._ratelimited_until + 0.1 >= time.time():
             pass
         try:
             self._send_packet(
                 {
                     "method": "set",
                     "name": "☁ " + variable,
@@ -151,20 +153,21 @@
                 return data
         except Exception as e:
             raise _exceptions.FetchError
 
 
     def set_var(self, variable, value):
         variable = variable.replace("☁ ", "")
-        value = str(value)
-        x = value.replace(".", "")
-        x = x.replace("-", "")
-        if not x.isnumeric():
-            if self.allow_non_numeric is False:
-                raise(_exceptions.InvalidCloudValue)
+        if not (value is True or value is False or value in [float('inf'), -float('inf')]):
+            value = str(value)
+            x = value.replace(".", "")
+            x = x.replace("-", "")
+            if not x.isnumeric():
+                if self.allow_non_numeric is False:
+                    raise(_exceptions.InvalidCloudValue)
 
         while self._ratelimited_until + 0.1 > time.time():
             pass
         try:
             self._send_packet(
                 {
                     "method": "set",
@@ -228,15 +231,15 @@
                     for activity in data:
                         if activity in self.data:
                             break
                         if "on_"+activity["verb"][:-4] in self._events:
                             try:
                                 self._events["on_"+activity["verb"][:-4]](self.Event(user=activity["user"], var=activity["name"][2:], name=activity["name"][2:], value=activity["value"], timestamp=activity["timestamp"]))
                             except Exception as e:
-                                print("Caught error in cloud event - Full error below")
+                                print("Warning: Caught error in cloud event - Full error below")
                                 try:
                                     traceback.print_exc()
                                 except Exception:
                                     print(e)
                 self.data = data
             else:
                 return
```

### Comparing `scratchattach-1.1.6/scratchattach/_cloud_requests.py` & `scratchattach-1.1.8/scratchattach/_cloud_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from . import _cloud
 import time
 from ._encoder import *
 import math
 from threading import Thread
 import json
 import traceback
+import warnings
 
 class CloudRequests:
 
     class Request:
         def __init__(self, **entries):
             self.__dict__.update(entries)
             self.id = self.request_id
@@ -27,17 +28,17 @@
         self.respond_in_thread= False
         self.current_var = 0
         self.idle_since = 0
 
     def __init__(self, cloud_connection : _cloud.CloudConnection, *, used_cloud_vars = ["1","2","3","4","5","6","7","8","9"], ignore_exceptions=True, force_reconnect=True, _log_url="https://clouddata.scratch.mit.edu/logs", _packet_length=245):
         print("\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m")
         if _log_url != "https://clouddata.scratch.mit.edu/logs":
-            print("Warning: Log URL isn't the URL of Scratch's clouddata logs. Don't use the _log_url parameter unless you know what you are doing.")
+            warnings.warn("Log URL isn't the URL of Scratch's clouddata logs. Don't use the _log_url parameter unless you know what you are doing", RuntimeWarning)
         if _packet_length > 245:
-            print("Warning: The packet length was set to a value higher than default (245). Your project most likely won't work on Scratch.")
+            warnings.warn("The packet length was set to a value higher than default (245). Your project most likely won't work on Scratch.", RuntimeWarning)
 
         self.used_cloud_vars = used_cloud_vars
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.log_url = _log_url
@@ -45,15 +46,15 @@
 
         self.init_attributes()
 
     def request(self, function=None, *, enabled=True, name=None, thread=False):
         def inner(function):
             if thread:
                 self.respond_in_thread = True
-                print("Warning: Running individual requests in threads increases CPU usage")
+                warnings.warn("Running individual requests in threads increases CPU usage", RuntimeWarning)
             self.requests[function.__name__ if name is None else name] = {"name":function.__name__ if name is None else name,"enabled":enabled,"on_call":function,"thread":thread}
         if function is None:
             return inner
         else:
             self.requests[function.__name__] = {"name":function.__name__,"enabled":True,"on_call":function,"thread":False}
 
     def call_request(self, request_id, req_obj, arguments):
@@ -67,21 +68,21 @@
             if req_obj["thread"]:
                 self.outputs[request_id] = {"output":output, "request":req_obj}
             else:
                 self._parse_output(output, request, req_obj, request_id)
         except Exception as e:
             self.call_event("on_error", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id), e])
             if self.ignore_exceptions:
-                print(f"Caught error in request '{request}' - Full error below")
+                print(f"Warning: Caught error in request '{request}' - Full error below")
                 try:
                     traceback.print_exc()
                 except Exception:
                     print(e)
             else:
-                print(f"Exception in request '{request}':")
+                print(f"Warning: Exception in request '{request}':")
                 raise(e)
             if req_obj["thread"]:
                 self.outputs[request_id] = {"output":f"Error: Check the Python console", "request":req_obj}
             else:
                 self._parse_output("Error: Check the Python console", request, req_obj, request_id)
 
     def add_request(self, function, *, enabled=True, name=None):
@@ -260,26 +261,26 @@
                 pass
             else:
                 self.last_timestamp = data[0]["timestamp"]
 
         self.call_event("on_ready")
 
         if self.requests == []:
-            print("Warning: You haven't added any requests!")
+            warnings.warn("You haven't added any requests!", RuntimeWarning)
 
         while True:
 
             if data_from_websocket or self.respond_in_thread:
                 data = self.ws_data
             else:
                 data = _cloud.get_cloud_logs(self.project_id, limit=100, log_url=self.log_url, filter_by_var_named="TO_HOST")
                 self.ws_data = data
             if self.ws_data == []:
                 continue
-            data.reverse()
+            data = reversed(data)
             if self.last_data == data:
                 pass
             else:
                 for activity in data:
                     if activity['timestamp'] > self.last_timestamp:
                         self.last_requester = activity["user"]
                         self.last_timestamp = activity['timestamp']
@@ -308,15 +309,15 @@
                         request = Encoding.decode(raw_request)
                         arguments = request.split("&")
                         request = arguments.pop(0)
                         self.call_event("on_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id,id=request_id)])
                         output = ""
 
                         if request not in self.requests:
-                            print(f"Warning: Client received an unknown request called '{request}'")
+                            warnings.warn(f"Warning: Client received an unknown request called '{request}'")
                             self.call_event("on_unknown_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id)])
                             continue
                         else:
                             req_obj = self.requests[request]
                             self.last_request_id = request_id
                             if req_obj["thread"]:
                                 Thread(target=self.call_request, args=(request_id, req_obj, arguments)).start()
@@ -333,15 +334,15 @@
                     self._parse_output(output, request, req_obj, request_id)
 
 class TwCloudRequests(CloudRequests):
 
     def __init__(self, cloud_connection, *, used_cloud_vars = ["1","2","3","4","5","6","7","8","9"], ignore_exceptions=True, force_reconnect=True, _packet_length=98800):
         print("\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m")
         if _packet_length > 98800:
-            print("Warning: The packet length was set to a value higher than TurboWarp's default (98800).")
+            warnings.warn("The packet length was set to a value higher than TurboWarp's default (98800).", RuntimeWarning)
         self.used_cloud_vars = used_cloud_vars
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.packet_length = _packet_length
```

### Comparing `scratchattach-1.1.6/scratchattach/_encoder.py` & `scratchattach-1.1.8/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.6/scratchattach/_exceptions.py` & `scratchattach-1.1.8/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.6/scratchattach/_forum.py` & `scratchattach-1.1.8/scratchattach/_forum.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         topic = ForumTopic(id=int(topic_id))
         topic.update()
         return topic
     except KeyError:
         return None
 
 def get_topic_list(category_name, *, page=0, include_deleted=False):
-    category_name.replace(" ", "%20")
+    category_name = category_name.replace(" ", "%20")
     if include_deleted:
         filter = 0
     else:
         filter = 1
     try:
         data = requests.get(f"https://scratchdb.lefty.one/v3/forum/category/topics/{category_name}/{page}?detail=1&filter={filter}").json()
         return_data = []
```

### Comparing `scratchattach-1.1.6/scratchattach/_project.py` & `scratchattach-1.1.8/scratchattach/_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,26 +190,28 @@
     def comments(self, *, limit=40, offset=0):#
         comments = []
         while len(comments) < limit:
             r = requests.get(
                 f"https://api.scratch.mit.edu/users/{self.author}/projects/{self.id}/comments/?limit={min(40, limit-len(comments))}&offset={offset}"
             ).json()
             if len(r) != 40:
+                comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
 
     def get_comment_replies(self, *, comment_id, limit=40, offset=0):
         comments = []
         while len(comments) < limit:
             r = requests.get(
                 f"https://api.scratch.mit.edu/users/{self.author}/projects/{self.id}/comments/{comment_id}/replies?limit={min(40, limit-len(comments))}&offset={offset}"
             ).json()
             if len(r) != 40:
+                comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
 
     def love(self):
         if self._headers is None:
```

### Comparing `scratchattach-1.1.6/scratchattach/_session.py` & `scratchattach-1.1.8/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.6/scratchattach/_studio.py` & `scratchattach-1.1.8/scratchattach/_studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,26 +74,28 @@
     def comments(self, *, limit=40, offset=0):
         comments = []
         while len(comments) < limit:
             r = requests.get(
                 f"https://api.scratch.mit.edu/studios/{self.id}/comments/?limit={min(40, limit-len(comments))}&offset={offset}"
             ).json()
             if len(r) != 40:
+                comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
 
     def get_comment_replies(self, *, comment_id, limit=40, offset=0):
         comments = []
         while len(comments) < limit:
             r = requests.get(
                 f"https://api.scratch.mit.edu/studios/{self.id}/comments/{comment_id}/replies?limit={min(40, limit-len(comments))}&offset={offset}"
             ).json()
             if len(r) != 40:
+                comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
 
 
     def post_comment(self, content, *, parent_id="", commentee_id=""):
```

### Comparing `scratchattach-1.1.6/scratchattach/_user.py` & `scratchattach-1.1.8/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.6/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.1.8/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.6
+Version: 1.1.8
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
+License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -611,7 +613,9 @@
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
 
 If you need help with your code, leave a comment on TimMcCool's Scratch
 profile: https://scratch.mit.edu/users/TimMcCool/
+
+
```

### Comparing `scratchattach-1.1.6/setup.py` & `scratchattach-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.6'
+VERSION = '1.1.8'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```


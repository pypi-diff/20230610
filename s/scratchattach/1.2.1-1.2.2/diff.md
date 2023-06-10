# Comparing `tmp/scratchattach-1.2.1.tar.gz` & `tmp/scratchattach-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.2.1.tar", last modified: Sat Jun 10 18:51:14 2023, max compression
+gzip compressed data, was "scratchattach-1.2.2.tar", last modified: Sat Jun 10 20:00:58 2023, max compression
```

## Comparing `scratchattach-1.2.1.tar` & `scratchattach-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 18:51:14.475710 scratchattach-1.2.1/
--rw-rw-rw-   0        0        0    22094 2023-06-10 18:51:14.474710 scratchattach-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 18:51:14.462707 scratchattach-1.2.1/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.1/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    13288 2023-06-10 17:51:03.000000 scratchattach-1.2.1/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    14671 2023-06-10 18:47:39.000000 scratchattach-1.2.1/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.1/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.1/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.1/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.1/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.1/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.1/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.1/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-06-10 18:51:14.474710 scratchattach-1.2.1/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22094 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 18:51:14.475710 scratchattach-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-06-10 18:51:05.000000 scratchattach-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:00:58.637782 scratchattach-1.2.2/
+-rw-rw-rw-   0        0        0    22094 2023-06-10 20:00:58.636781 scratchattach-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 20:00:58.614599 scratchattach-1.2.2/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.2/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-06-10 19:50:37.000000 scratchattach-1.2.2/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18193 2023-06-10 20:00:46.000000 scratchattach-1.2.2/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.2/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.2/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.2/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.2/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.2/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.2/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.2/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-06-10 20:00:58.635781 scratchattach-1.2.2/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22094 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 20:00:58.000000 scratchattach-1.2.2/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 20:00:58.637782 scratchattach-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-06-10 19:51:52.000000 scratchattach-1.2.2/setup.py
```

### Comparing `scratchattach-1.2.1/PKG-INFO` & `scratchattach-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.1
+Version: 1.2.2
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Platform: UNKNOWN
```

### Comparing `scratchattach-1.2.1/README.md` & `scratchattach-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach/_cloud.py` & `scratchattach-1.2.2/scratchattach/_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,24 @@
             self.websocket.connect(
                 "wss://clouddata.scratch.mit.edu",
                 cookie="scratchsessionsid=" + self._session_id + ";",
                 origin="https://scratch.mit.edu",
                 enable_multithread=True,
             )
         except Exception:
-            raise(_exceptions.ConnectionError)
+            try:
+                self.websocket = websocket.WebSocket()
+                self.websocket.connect(
+                    "wss://clouddata.scratch.mit.edu",
+                    cookie="scratchsessionsid=" + self._session_id + ";",
+                    origin="https://scratch.mit.edu",
+                    enable_multithread=True,
+                )
+            except Exception:
+                raise(_exceptions.ConnectionError)
 
     def set_var(self, variable, value):
         variable = variable.replace("☁ ", "")
         if not (value is True or value is False or value in [float('inf'), -float('inf')]):
             value = str(value)
             if len(value) > 256:
                 warnings.warn("invalid cloud var (too long): "+str(value), Warning)
```

### Comparing `scratchattach-1.2.1/scratchattach/_cloud_requests.py` & `scratchattach-1.2.2/scratchattach/_cloud_requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from ._encoder import *
 import math
 from threading import Thread
 import json
 import traceback
 import warnings
 
-class CloudRequests:
 
+class CloudRequests:
     class Request:
         def __init__(self, **entries):
             self.__dict__.update(entries)
             self.id = self.request_id
 
     def init_attributes(self):
         self.last_requester = None
@@ -21,25 +21,38 @@
         self.last_request_id = None
 
         self.requests = {}
         self.events = []
 
         self.request_parts = {}
         self.outputs = {}
-        self.respond_in_thread= False
+        self.respond_in_thread = False
         self.current_var = 0
         self.idle_since = 0
         self.force_reconnect = False
 
-    def __init__(self, cloud_connection : _cloud.CloudConnection, *, used_cloud_vars = ["1","2","3","4","5","6","7","8","9"], ignore_exceptions=True, force_reconnect=True, _log_url="https://clouddata.scratch.mit.edu/logs", _packet_length=245):
-        print("\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m")
+    def __init__(self,
+                 cloud_connection: _cloud.CloudConnection,
+                 *,
+                 used_cloud_vars=["1", "2", "3", "4", "5", "6", "7", "8", "9"],
+                 ignore_exceptions=True,
+                 force_reconnect=True,
+                 _log_url="https://clouddata.scratch.mit.edu/logs",
+                 _packet_length=245):
+        print(
+            "\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m"
+        )
         if _log_url != "https://clouddata.scratch.mit.edu/logs":
-            warnings.warn("Log URL isn't the URL of Scratch's clouddata logs. Don't use the _log_url parameter unless you know what you are doing", RuntimeWarning)
+            warnings.warn(
+                "Log URL isn't the URL of Scratch's clouddata logs. Don't use the _log_url parameter unless you know what you are doing",
+                RuntimeWarning)
         if _packet_length > 245:
-            warnings.warn("The packet length was set to a value higher than default (245). Your project most likely won't work on Scratch.", RuntimeWarning)
+            warnings.warn(
+                "The packet length was set to a value higher than default (245). Your project most likely won't work on Scratch.",
+                RuntimeWarning)
 
         self.used_cloud_vars = used_cloud_vars
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.log_url = _log_url
@@ -47,58 +60,102 @@
 
         self.init_attributes()
 
     def request(self, function=None, *, enabled=True, name=None, thread=False):
         def inner(function):
             if thread:
                 self.respond_in_thread = True
-                warnings.warn("Running individual requests in threads increases CPU usage", RuntimeWarning)
-            self.requests[function.__name__ if name is None else name] = {"name":function.__name__ if name is None else name,"enabled":enabled,"on_call":function,"thread":thread}
+                warnings.warn(
+                    "Running individual requests in threads increases CPU usage",
+                    RuntimeWarning)
+            self.requests[function.__name__ if name is None else name] = {
+                "name": function.__name__ if name is None else name,
+                "enabled": enabled,
+                "on_call": function,
+                "thread": thread
+            }
+
         if function is None:
             return inner
         else:
-            self.requests[function.__name__] = {"name":function.__name__,"enabled":True,"on_call":function,"thread":False}
+            self.requests[function.__name__] = {
+                "name": function.__name__,
+                "enabled": True,
+                "on_call": function,
+                "thread": False
+            }
 
     def call_request(self, request_id, req_obj, arguments):
         request = req_obj["name"]
         try:
             if not req_obj["enabled"]:
-                print(f"Warning: Client received the disabled request '{request}'")
-                self.call_event("on_disabled_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id)])
+                print(
+                    f"Warning: Client received the disabled request '{request}'"
+                )
+                self.call_event("on_disabled_request", [
+                    self.Request(name=request,
+                                 request=request,
+                                 requester=self.last_requester,
+                                 timestamp=self.last_timestamp,
+                                 arguments=arguments,
+                                 request_id=request_id)
+                ])
                 return None
             output = req_obj["on_call"](*arguments)
             if req_obj["thread"]:
-                self.outputs[request_id] = {"output":output, "request":req_obj}
+                self.outputs[request_id] = {
+                    "output": output,
+                    "request": req_obj
+                }
             else:
                 self._parse_output(output, request, req_obj, request_id)
         except Exception as e:
-            self.call_event("on_error", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id), e])
+            self.call_event("on_error", [
+                self.Request(name=request,
+                             request=request,
+                             requester=self.last_requester,
+                             timestamp=self.last_timestamp,
+                             arguments=arguments,
+                             request_id=request_id), e
+            ])
             if self.ignore_exceptions:
-                print(f"Warning: Caught error in request '{request}' - Full error below")
+                print(
+                    f"Warning: Caught error in request '{request}' - Full error below"
+                )
                 try:
                     traceback.print_exc()
                 except Exception:
                     print(e)
             else:
                 print(f"Warning: Exception in request '{request}':")
-                raise(e)
+                raise (e)
             if req_obj["thread"]:
-                self.outputs[request_id] = {"output":f"Error: Check the Python console", "request":req_obj}
+                self.outputs[request_id] = {
+                    "output": f"Error: Check the Python console",
+                    "request": req_obj
+                }
             else:
-                self._parse_output("Error: Check the Python console", request, req_obj, request_id)
+                self._parse_output("Error: Check the Python console", request,
+                                   req_obj, request_id)
 
     def add_request(self, function, *, enabled=True, name=None):
         self.request(enabled=enabled, name=name)(function)
 
     def remove_request(self, name):
         self.requests.pop(name)
 
-    def edit_request(self, name, *, enabled=None, new_name=None, new_function=None, thread=None):
+    def edit_request(self,
+                     name,
+                     *,
+                     enabled=None,
+                     new_name=None,
+                     new_function=None,
+                     thread=None):
         if name not in self.requests:
-            raise(_exceptions.RequestNotFound(name))
+            raise (_exceptions.RequestNotFound(name))
         if enabled is not None:
             self.requests[name]["enabled"] = enabled
         if new_name is not None:
             self.requests[name]["name"] = new_name
         if new_function is not None:
             self.requests[name]["on_call"] = new_function
         if thread is not None:
@@ -107,16 +164,19 @@
     def event(self, function):
 
         self.events.append(function)
 
     def get_requester(self):
 
         if self.last_requester is None:
-            logs = _cloud.get_cloud_logs(self.project_id, filter_by_var_named="TO_HOST")
-            activity = list(filter(lambda x : "."+self.last_request_id in x["value"], logs))
+            logs = _cloud.get_cloud_logs(self.project_id,
+                                         filter_by_var_named="TO_HOST")
+            activity = list(
+                filter(lambda x: "." + self.last_request_id in x["value"],
+                       logs))
             if len(activity) > 0:
                 self.last_requester = activity[0]["user"]
 
         return self.last_requester
 
     def get_timestamp(self):
 
@@ -126,91 +186,107 @@
 
         if self.idle_since + 8 < time.time() or self.force_reconnect:
             self.connection._connect(cloud_host=self.connection.cloud_host)
             self.connection._handshake()
 
         remaining_response = str(response)
 
-
         i = 0
         while not remaining_response == "":
             if len(remaining_response) > limit:
                 response_part = remaining_response[:limit]
                 remaining_response = remaining_response[limit:]
 
-                i+=1
+                i += 1
                 if i > 99:
                     iteration_string = str(i)
                 elif i > 9:
-                    iteration_string = "0"+str(i)
+                    iteration_string = "0" + str(i)
                 else:
-                    iteration_string = "00"+str(i)
+                    iteration_string = "00" + str(i)
 
                 try:
-                    self.connection.set_var(f"FROM_HOST_{self.used_cloud_vars[self.current_var]}", f"{response_part}.{request_id}{iteration_string}1")
+                    self.connection.set_var(
+                        f"FROM_HOST_{self.used_cloud_vars[self.current_var]}",
+                        f"{response_part}.{request_id}{iteration_string}1")
                 except Exception:
                     self.call_event("on_disconnect")
                 self.current_var += 1
                 if self.current_var == len(self.used_cloud_vars):
                     self.current_var = 0
                 time.sleep(0.1)
             else:
                 try:
-                    self.connection.set_var(f"FROM_HOST_{self.used_cloud_vars[self.current_var]}", f"{remaining_response}.{request_id}{validation}")
+                    self.connection.set_var(
+                        f"FROM_HOST_{self.used_cloud_vars[self.current_var]}",
+                        f"{remaining_response}.{request_id}{validation}")
                 except Exception:
                     self.call_event("on_disconnect")
                 self.current_var += 1
                 if self.current_var == len(self.used_cloud_vars):
                     self.current_var = 0
 
                 remaining_response = ""
                 time.sleep(0.1)
 
         self.idle_since = time.time()
 
-    def run(self, thread=False, data_from_websocket=True, no_packet_loss=False):
+    def run(self,
+            thread=False,
+            data_from_websocket=True,
+            no_packet_loss=False):
         self.force_reconnect = no_packet_loss
         if data_from_websocket is True:
             events = [
-                _cloud.WsCloudEvents(self.project_id, _cloud.CloudConnection(project_id = self.project_id, username = self.connection._username, session_id=self.connection._session_id), update_interval=0),
-                _cloud.CloudEvents(self.project_id, update_interval=4.5, cloud_log_limit=25)
+                _cloud.WsCloudEvents(
+                    self.project_id,
+                    _cloud.CloudConnection(
+                        project_id=self.project_id,
+                        username=self.connection._username,
+                        session_id=self.connection._session_id),
+                    update_interval=0),
+                _cloud.CloudEvents(self.project_id,
+                                   update_interval=4.5,
+                                   cloud_log_limit=25)
             ]
         else:
-            events = [
-                _cloud.CloudEvents(self.project_id, update_interval=0, cloud_log_limit=100)
-            ]
+            events = []
         if thread:
-            thread = Thread(target=self._run, args=[events])
+            thread = Thread(
+                target=self._run,
+                args=[events],
+                kwargs={"data_from_websocket": data_from_websocket})
             thread.start()
         else:
-            self._run(events)
+            self._run(events, data_from_websocket=data_from_websocket)
 
     def call_event(self, event, args=[]):
         events = list(filter(lambda k: k.__name__ == event, self.events))
         if events == []:
             return False
         else:
             events[0](*args)
             return True
 
     def _parse_output(self, output, request, req_obj, request_id):
         if len(str(output)) > 3000:
-            print(f"Warning: Output of request '{request}' is longer than 3000 characters (length: {len(str(output))} characters). Responding the request will take >4 seconds.")
+            print(
+                f"Warning: Output of request '{request}' is longer than 3000 characters (length: {len(str(output))} characters). Responding the request will take >4 seconds."
+            )
 
         if str(request_id).endswith("0"):
             try:
                 int(output) == output
             except Exception:
                 send_as_integer = False
             else:
                 send_as_integer = not "-" in str(output)
         else:
             send_as_integer = False
 
-
         if output is None:
             print(f"Warning: Request '{request}' didn't return anything.")
             return
         elif send_as_integer:
             output = str(output)
         elif not isinstance(output, list):
             if output == "":
@@ -219,28 +295,29 @@
         else:
             input = output
             output = ""
             for i in input:
                 output += Encoding.encode(i)
                 output += "89"
         if send_as_integer:
-            self._respond(request_id, output, self.packet_length, validation=3222)
+            self._respond(request_id,
+                          output,
+                          self.packet_length,
+                          validation=3222)
         else:
             self._respond(request_id, output, self.packet_length)
 
-
-    def _run(self, events):
+    def _run(self, events, data_from_websocket=True):
         self.ws_data = []
 
         def on_set(event):
             if event.name == "TO_HOST":
-                self.ws_data.insert(0,event)
+                self.ws_data.insert(0, event)
                 self.ws_data = self.ws_data[:50]
 
-
         try:
             self.connection._connect(cloud_host=self.connection.cloud_host)
             self.connection._handshake()
         except Exception:
             self.call_event("on_disconnect")
 
         self.idle_since = time.time()
@@ -248,41 +325,56 @@
 
         if self.requests == []:
             warnings.warn("You haven't added any requests!", RuntimeWarning)
 
         while events != []:
             event_handler = events.pop()
             event_handler.event(on_set)
-            event_handler.start(
-                update_interval=event_handler.update_interval,
-                thread=True
-            )
+            event_handler.start(update_interval=event_handler.update_interval,
+                                thread=True)
 
-        self.call_event("on_ready") #Calls the on_ready event
+        old_clouddata = []
+        self.call_event("on_ready")  #Calls the on_ready event
 
         while True:
 
+            if data_from_websocket is False:
+                clouddata = _cloud.get_cloud_logs(
+                    self.project_id, filter_by_var_named="TO_HOST", limit=100)[::-1]
+                if clouddata == old_clouddata:
+                    continue
+                else:
+                    old_clouddata = list(clouddata)
+                self.ws_data = [
+                    _cloud.CloudEvents.Event(user=activity["user"],
+                                             var=activity["name"][2:],
+                                             name=activity["name"][2:],
+                                             value=activity["value"],
+                                             timestamp=activity["timestamp"])
+                    for activity in clouddata
+                ]
+
             if self.ws_data != []:
                 event = self.ws_data.pop()
 
                 try:
                     raw_request, request_id = event.value.split(".")
                     if request_id in self.responded_request_ids:
                         continue
                     else:
                         self.responded_request_ids.insert(0, request_id)
-                        self.responded_request_ids = self.responded_request_ids[:15]
+                        self.responded_request_ids = self.responded_request_ids[:
+                                                                                15]
                 except Exception:
                     self.last_timestamp = event.timestamp
                     continue
 
                 self.last_requester = event.user
                 self.last_timestamp = event.timestamp
 
-
                 if event.value[0] == "-":
                     if not request_id in self.request_parts:
                         self.request_parts[request_id] = []
                     self.request_parts[request_id].append(raw_request[1:])
                     continue
 
                 _raw_request = ""
@@ -292,58 +384,89 @@
                         _raw_request += i
                     self.request_parts.pop(request_id)
                 raw_request = _raw_request + raw_request
 
                 request = Encoding.decode(raw_request)
                 arguments = request.split("&")
                 request = arguments.pop(0)
-                self.call_event("on_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id,id=request_id)])
+                self.call_event("on_request", [
+                    self.Request(name=request,
+                                 request=request,
+                                 requester=self.last_requester,
+                                 timestamp=self.last_timestamp,
+                                 arguments=arguments,
+                                 request_id=request_id,
+                                 id=request_id)
+                ])
                 output = ""
 
                 if request not in self.requests:
-                    print(f"Warning: Client received an unknown request called '{request}'")
-                    self.call_event("on_unknown_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id)])
+                    print(
+                        f"Warning: Client received an unknown request called '{request}'"
+                    )
+                    self.call_event("on_unknown_request", [
+                        self.Request(name=request,
+                                     request=request,
+                                     requester=self.last_requester,
+                                     timestamp=self.last_timestamp,
+                                     arguments=arguments,
+                                     request_id=request_id)
+                    ])
                     continue
                 else:
                     req_obj = self.requests[request]
                     self.last_request_id = request_id
                     if req_obj["thread"]:
-                        Thread(target=self.call_request, args=(request_id, req_obj, arguments)).start()
+                        Thread(target=self.call_request,
+                               args=(request_id, req_obj, arguments)).start()
                     else:
                         self.call_request(request_id, req_obj, arguments)
 
             #Send outputs
             output_ids = list(self.outputs.keys())
             while len(output_ids) > 0:
                 for request_id in output_ids:
                     output = self.outputs[request_id]["output"]
                     request = self.outputs[request_id]["request"]["name"]
                     req_obj = self.outputs[request_id]["request"]
                     self._parse_output(output, request, req_obj, request_id)
                     self.outputs.pop(request_id)
 
-class TwCloudRequests(CloudRequests):
 
-    def __init__(self, cloud_connection, *, used_cloud_vars = ["1","2","3","4","5","6","7","8","9"], ignore_exceptions=True, force_reconnect=True, _packet_length=98800):
-        print("\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m")
+class TwCloudRequests(CloudRequests):
+    def __init__(self,
+                 cloud_connection,
+                 *,
+                 used_cloud_vars=["1", "2", "3", "4", "5", "6", "7", "8", "9"],
+                 ignore_exceptions=True,
+                 force_reconnect=True,
+                 _packet_length=98800):
+        print(
+            "\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m"
+        )
         if _packet_length > 98800:
-            warnings.warn("The packet length was set to a value higher than TurboWarp's default (98800).", RuntimeWarning)
+            warnings.warn(
+                "The packet length was set to a value higher than TurboWarp's default (98800).",
+                RuntimeWarning)
         self.used_cloud_vars = used_cloud_vars
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.packet_length = _packet_length
 
         self.init_attributes()
 
     def get_requester(self):
         return None
 
-    def run(self, thread=False, data_from_websocket=True, no_packet_loss=False):
+    def run(self,
+            thread=False,
+            data_from_websocket=True,
+            no_packet_loss=False):
         self.force_reconnect = no_packet_loss
         events = [_cloud.TwCloudEvents(self.project_id, update_interval=0)]
         if thread:
             thread = Thread(target=self._run, args=[events])
             thread.start()
         else:
             self._run(events)
```

### Comparing `scratchattach-1.2.1/scratchattach/_encoder.py` & `scratchattach-1.2.2/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach/_exceptions.py` & `scratchattach-1.2.2/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach/_forum.py` & `scratchattach-1.2.2/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach/_project.py` & `scratchattach-1.2.2/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach/_session.py` & `scratchattach-1.2.2/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach/_studio.py` & `scratchattach-1.2.2/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach/_user.py` & `scratchattach-1.2.2/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.1/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.2.2/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.1
+Version: 1.2.2
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Platform: UNKNOWN
```

### Comparing `scratchattach-1.2.1/setup.py` & `scratchattach-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```


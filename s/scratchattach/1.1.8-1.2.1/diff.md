# Comparing `tmp/scratchattach-1.1.8.tar.gz` & `tmp/scratchattach-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.1.8.tar", last modified: Sat Jun 10 15:52:15 2023, max compression
+gzip compressed data, was "scratchattach-1.2.1.tar", last modified: Sat Jun 10 18:51:14 2023, max compression
```

## Comparing `scratchattach-1.1.8.tar` & `scratchattach-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 15:52:15.230413 scratchattach-1.1.8/
--rw-rw-rw-   0        0        0    22096 2023-06-10 15:52:15.230413 scratchattach-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    20740 2023-05-07 17:32:19.000000 scratchattach-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 15:52:15.216995 scratchattach-1.1.8/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.1.8/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    13089 2023-06-10 15:19:07.000000 scratchattach-1.1.8/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    15620 2023-06-10 15:18:42.000000 scratchattach-1.1.8/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.1.8/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.1.8/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.1.8/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.1.8/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17923 2023-06-10 15:03:02.000000 scratchattach-1.1.8/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.1.8/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.1.8/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:52:15.229414 scratchattach-1.1.8/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22096 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-10 15:52:15.000000 scratchattach-1.1.8/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 15:52:15.230413 scratchattach-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-06-10 15:19:12.000000 scratchattach-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:51:14.475710 scratchattach-1.2.1/
+-rw-rw-rw-   0        0        0    22094 2023-06-10 18:51:14.474710 scratchattach-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20730 2023-06-10 15:56:43.000000 scratchattach-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 18:51:14.462707 scratchattach-1.2.1/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.1/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    13288 2023-06-10 17:51:03.000000 scratchattach-1.2.1/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    14671 2023-06-10 18:47:39.000000 scratchattach-1.2.1/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.1/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.1/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.1/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.1/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.1/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.1/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.1/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:51:14.474710 scratchattach-1.2.1/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22094 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 18:51:14.000000 scratchattach-1.2.1/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 18:51:14.475710 scratchattach-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-06-10 18:51:05.000000 scratchattach-1.2.1/setup.py
```

### Comparing `scratchattach-1.1.8/PKG-INFO` & `scratchattach-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.8
+Version: 1.2.1
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Platform: UNKNOWN
@@ -44,15 +44,15 @@
 Add this to your Python code:
 ```python
 import os
 
 os.system("pip install -U scratchattach")
 ```
 
-# Logging in  `scratch3.Session`
+# Logging in
 
 **Logging in with username / password:**
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.login("username", "password")
@@ -75,16 +75,15 @@
 session.xtoken
 session.email #Returns the email address associated with the account
 session.new_scratcher #Returns True if the associated account is a New Scratcher
 session.mute_status
 session.banned #Returns True if the associated account is banned
 ```
 
-# Cloud variables  `scratch3.CloudConnection`
-*Make sure you're using the latest scratchattach version. Update scratchattach with `pip install scratchattach --upgrade`*
+# Cloud variables
 
 **Connect to the Scratch cloud:**
 
 With a `Session` object:
 
 ```python
 conn = session.connect_cloud("project_id")
@@ -134,32 +133,32 @@
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
 
-# Encoding / Decoding  `scratch3.Encoding`
+# Encoding / Decoding
 
 Scratchattach has a built in encoder. Scratch sprite to decode texts encoded with scratchattach: https://scratch3-assets.1tim.repl.co/Encoder.sprite3
 
 ```python
 from scratchattach import Encoding
 
 Encoding.encode("input") #will return the encoded text
 Encoding.decode("encoded") #will decode an encoded text
 ```
 
-# Cloud events  `scratch3.CloudEvents`
+# Cloud events
 
 *Cloud events allow reacting to cloud events in real time. If a Scratcher
 sets / creates / deletes a cloud var on the given project, an
 event will be called.*
 
-They do not require a session.
+They do not require a session because they use the clouddata logs to receive cloud updates.
 
 **How to use with Scratch:**
 
 ```python
 import scratchattach as scratch3
 
 events = scratch3.CloudEvents("project_id")
@@ -179,48 +178,60 @@
 @events.event #Called when the event listener is ready
 def on_ready():
    print("Event listener ready!")
 
 events.start()
 ```
 
-**How to use with TurboWarp:** (new in v0.4.7)
+**How to use with TurboWarp:**
 
 ```python
 import scratchattach as scratch3
 
 events = scratch3.TwCloudEvents("project_id")
 
 ...
 ```
 
+**Cloud events that use a `scratch3.CloudConnection` object to receive cloud updates:**
+
+```python
+import scratchattach as scratch3
+
+session = scratch3.Session("session_id", username="username") #Replace with your data
+conn = session.connect_cloud("project_id")
+events = scratch3.WsCloudEvents("project_id", conn)
+
+...
+```
+
 **Functions:**
 ```py
 events.start(thread=True)
 events.pause()
 events.resume()
 events.stop()
 ```
 
-# Cloud Requests  `scratch3.CloudRequests`
+# Cloud Requests
 
 Cloud Requests Framework (inspired by discord.py) that allows Scratch projects and Python to interact
 
 *This makes it possible to access data like message counts, user stats and more from Scratch projects! Uses cloud variables to transmit data.*
 
 **[Cloud Requests are documented on this page:](https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests)**
 
 [https://github.com/TimMcCool/scratchattach/blob/main/CLOUD_REQUESTS.md](https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests)
 
 If you want to access external information in Scratch projects or store data on an external database, scratchattach's Cloud Requests are ideal for your project:
 - Similar to cloud events, but send back data to the project
 - Automatically encode / decode sent data
 - Tons of extra features
 
-# Users  `scratch3.User`
+# Users
 
 **Get a user:**
 ```python
 user = session.connect_user("username")
 ```
 
 Get the user that you are logged in with:
@@ -295,15 +306,15 @@
 user.forum_counts_over_time() #Fetched from ScratchDB
 user.forum_signature() #Fetched from ScratchDB
 user.forum_signature_history() #A change log for the user's forum history. Fetched from ScratchDB
 
 user.ocular_status() #Returns information about the user's ocular status, like the status text, the color, and the time of the last update.
 ```
 
-# Projects  `scratch3.Project`
+# Projects
 
 **Get a project:**
 ```python
 project = session.connect_project("project_id")
 ```
 
 You can also get projects without logging in: (but then you can't use any functions that require a login, and you can't get your unshared projects)
@@ -369,25 +380,24 @@
 project.studios(limit=None, offset=0) #Returns the studios the project is in as list of dicts
 
 project.download(filename="project_name.sb3", dir="") #Downloads the project to your computer. The downloaded file will only work in the online editor
 project.get_raw_json() #Returns the json of the project content as dict
 project.get_creator_agent() #Returns the user-agent of the user who created the project (with information about their browser and OS)
 ```
 
-# Unshared projects  `scratch3.PartialProject`
+# Unshared projects
 
 When connecting / getting a project that you can't access, a `PartialProject` object is returned instead.
 
 **Most attributes and most functions don't work for such projects. However, these still work:**
 ```python
 project.remixes(limit=None, offset=0)
 ```
 
-# Studios  `scratch3.Studio`
-(New in v0.5.0)
+# Studios
 
 **Get a studio:**
 ```python
 studio = session.connect_studio("studio_id")
 ```
 You can also get studios without logging in: (But then you can't use any functions that require a login, like studio.follow(), studio.add_project(), ...)
 ```python
@@ -490,16 +500,15 @@
 scratch3.newest_projects() #Returns a list with the newest Scratch projects. This list is not present on the Scratch home page, but the API still provides it.
 scratch3.design_studio_projects()
 
 session.get_feed(limit=20, offset=0) #Returns your "What's happening" section from the Scratch front page as list
 session.loved_by_followed_users(limit=40, offset=0) #Returns the projects loved by users you are following as list
 ```
 
-# Forum topics `scratch3.ForumTopic`
-(New in v0.5.5)
+# Forum topics
 All of this data is fetched from ScratchDB v3, therefore it may be slighty off.
 
 **Get a forum topic:**
 ```python
 topic = session.connect_topic("topic_id")
 ```
 You can also get topics without logging in:
@@ -536,16 +545,15 @@
 
 topic.post_count_by_user("username")
 topic.activity() #Returns an activity / change log for the topic
 ```
 
 To prevent spam, adding posts to topics is not a scratchattach feature and never will be.
 
-# Forum posts `scratch3.ForumPost`
-(New in v0.5.5)
+# Forum posts
 All of this data is fetched from ScratchDB v3, therefore it may be slighty off.
 
 **Get a forum post:**
 ```python
 post = session.connect_post("post_id")
 ```
 You can also get posts without logging in:
@@ -612,10 +620,10 @@
 - Allmost all code by TimMcCool.
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
 
 If you need help with your code, leave a comment on TimMcCool's Scratch
-profile: https://scratch.mit.edu/users/TimMcCool/
+profile (https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
```

### Comparing `scratchattach-1.1.8/README.md` & `scratchattach-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Add this to your Python code:
 ```python
 import os
 
 os.system("pip install -U scratchattach")
 ```
 
-# Logging in  `scratch3.Session`
+# Logging in
 
 **Logging in with username / password:**
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.login("username", "password")
@@ -57,16 +57,15 @@
 session.xtoken
 session.email #Returns the email address associated with the account
 session.new_scratcher #Returns True if the associated account is a New Scratcher
 session.mute_status
 session.banned #Returns True if the associated account is banned
 ```
 
-# Cloud variables  `scratch3.CloudConnection`
-*Make sure you're using the latest scratchattach version. Update scratchattach with `pip install scratchattach --upgrade`*
+# Cloud variables
 
 **Connect to the Scratch cloud:**
 
 With a `Session` object:
 
 ```python
 conn = session.connect_cloud("project_id")
@@ -116,32 +115,32 @@
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
 
-# Encoding / Decoding  `scratch3.Encoding`
+# Encoding / Decoding
 
 Scratchattach has a built in encoder. Scratch sprite to decode texts encoded with scratchattach: https://scratch3-assets.1tim.repl.co/Encoder.sprite3
 
 ```python
 from scratchattach import Encoding
 
 Encoding.encode("input") #will return the encoded text
 Encoding.decode("encoded") #will decode an encoded text
 ```
 
-# Cloud events  `scratch3.CloudEvents`
+# Cloud events
 
 *Cloud events allow reacting to cloud events in real time. If a Scratcher
 sets / creates / deletes a cloud var on the given project, an
 event will be called.*
 
-They do not require a session.
+They do not require a session because they use the clouddata logs to receive cloud updates.
 
 **How to use with Scratch:**
 
 ```python
 import scratchattach as scratch3
 
 events = scratch3.CloudEvents("project_id")
@@ -161,48 +160,60 @@
 @events.event #Called when the event listener is ready
 def on_ready():
    print("Event listener ready!")
 
 events.start()
 ```
 
-**How to use with TurboWarp:** (new in v0.4.7)
+**How to use with TurboWarp:**
 
 ```python
 import scratchattach as scratch3
 
 events = scratch3.TwCloudEvents("project_id")
 
 ...
 ```
 
+**Cloud events that use a `scratch3.CloudConnection` object to receive cloud updates:**
+
+```python
+import scratchattach as scratch3
+
+session = scratch3.Session("session_id", username="username") #Replace with your data
+conn = session.connect_cloud("project_id")
+events = scratch3.WsCloudEvents("project_id", conn)
+
+...
+```
+
 **Functions:**
 ```py
 events.start(thread=True)
 events.pause()
 events.resume()
 events.stop()
 ```
 
-# Cloud Requests  `scratch3.CloudRequests`
+# Cloud Requests
 
 Cloud Requests Framework (inspired by discord.py) that allows Scratch projects and Python to interact
 
 *This makes it possible to access data like message counts, user stats and more from Scratch projects! Uses cloud variables to transmit data.*
 
 **[Cloud Requests are documented on this page:](https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests)**
 
 [https://github.com/TimMcCool/scratchattach/blob/main/CLOUD_REQUESTS.md](https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests)
 
 If you want to access external information in Scratch projects or store data on an external database, scratchattach's Cloud Requests are ideal for your project:
 - Similar to cloud events, but send back data to the project
 - Automatically encode / decode sent data
 - Tons of extra features
 
-# Users  `scratch3.User`
+# Users
 
 **Get a user:**
 ```python
 user = session.connect_user("username")
 ```
 
 Get the user that you are logged in with:
@@ -277,15 +288,15 @@
 user.forum_counts_over_time() #Fetched from ScratchDB
 user.forum_signature() #Fetched from ScratchDB
 user.forum_signature_history() #A change log for the user's forum history. Fetched from ScratchDB
 
 user.ocular_status() #Returns information about the user's ocular status, like the status text, the color, and the time of the last update.
 ```
 
-# Projects  `scratch3.Project`
+# Projects
 
 **Get a project:**
 ```python
 project = session.connect_project("project_id")
 ```
 
 You can also get projects without logging in: (but then you can't use any functions that require a login, and you can't get your unshared projects)
@@ -351,25 +362,24 @@
 project.studios(limit=None, offset=0) #Returns the studios the project is in as list of dicts
 
 project.download(filename="project_name.sb3", dir="") #Downloads the project to your computer. The downloaded file will only work in the online editor
 project.get_raw_json() #Returns the json of the project content as dict
 project.get_creator_agent() #Returns the user-agent of the user who created the project (with information about their browser and OS)
 ```
 
-# Unshared projects  `scratch3.PartialProject`
+# Unshared projects
 
 When connecting / getting a project that you can't access, a `PartialProject` object is returned instead.
 
 **Most attributes and most functions don't work for such projects. However, these still work:**
 ```python
 project.remixes(limit=None, offset=0)
 ```
 
-# Studios  `scratch3.Studio`
-(New in v0.5.0)
+# Studios
 
 **Get a studio:**
 ```python
 studio = session.connect_studio("studio_id")
 ```
 You can also get studios without logging in: (But then you can't use any functions that require a login, like studio.follow(), studio.add_project(), ...)
 ```python
@@ -472,16 +482,15 @@
 scratch3.newest_projects() #Returns a list with the newest Scratch projects. This list is not present on the Scratch home page, but the API still provides it.
 scratch3.design_studio_projects()
 
 session.get_feed(limit=20, offset=0) #Returns your "What's happening" section from the Scratch front page as list
 session.loved_by_followed_users(limit=40, offset=0) #Returns the projects loved by users you are following as list
 ```
 
-# Forum topics `scratch3.ForumTopic`
-(New in v0.5.5)
+# Forum topics
 All of this data is fetched from ScratchDB v3, therefore it may be slighty off.
 
 **Get a forum topic:**
 ```python
 topic = session.connect_topic("topic_id")
 ```
 You can also get topics without logging in:
@@ -518,16 +527,15 @@
 
 topic.post_count_by_user("username")
 topic.activity() #Returns an activity / change log for the topic
 ```
 
 To prevent spam, adding posts to topics is not a scratchattach feature and never will be.
 
-# Forum posts `scratch3.ForumPost`
-(New in v0.5.5)
+# Forum posts
 All of this data is fetched from ScratchDB v3, therefore it may be slighty off.
 
 **Get a forum post:**
 ```python
 post = session.connect_post("post_id")
 ```
 You can also get posts without logging in:
@@ -594,8 +602,8 @@
 - Allmost all code by TimMcCool.
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
 
 If you need help with your code, leave a comment on TimMcCool's Scratch
-profile: https://scratch.mit.edu/users/TimMcCool/
+profile (https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
```

### Comparing `scratchattach-1.1.8/scratchattach/_cloud.py` & `scratchattach-1.2.1/scratchattach/_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,20 +198,22 @@
 
 class CloudEvents:
 
     class Event:
         def __init__(self, **entries):
             self.__dict__.update(entries)
 
-    def __init__(self, project_id):
+    def __init__(self, project_id, **entries):
         self.project_id = int(project_id)
         self.data = get_cloud_logs(project_id=self.project_id, limit = 15)
         self._thread = None
         self.running = False
         self._events = {}
+        self.cloud_log_limit = 15
+        self.__dict__.update(entries)
 
     def start(self, *, update_interval = 0.1, thread=True, daemon=False):
         if self.running is False:
             self.update_interval = update_interval
             self.running = True
             if "on_ready" in self._events:
                 self._events["on_ready"]()
@@ -222,15 +224,15 @@
             else:
                 self._thread = None
                 self._update()
 
     def _update(self):
         while True:
             if self.running:
-                data = get_cloud_logs(project_id = self.project_id, limit = 15)
+                data = get_cloud_logs(project_id = self.project_id, limit = self.cloud_log_limit)
                 if data != self.data:
                     for activity in data:
                         if activity in self.data:
                             break
                         if "on_"+activity["verb"][:-4] in self._events:
                             try:
                                 self._events["on_"+activity["verb"][:-4]](self.Event(user=activity["user"], var=activity["name"][2:], name=activity["name"][2:], value=activity["value"], timestamp=activity["timestamp"]))
@@ -260,21 +262,22 @@
             self.start(update_interval=self.update_interval, thread=True)
 
     def event(self, function):
         self._events[function.__name__] = function
 
 class TwCloudEvents(CloudEvents):
 
-    def __init__(self, project_id):
+    def __init__(self, project_id, **entries):
         cloud_connection = TwCloudConnection(project_id=project_id)
         self.data = []
         self._thread = None
         self.running = False
         self._events = {}
         self.connection = cloud_connection
+        self.__dict__.update(entries)
 
     def _update(self):
         while True:
             try:
                 data = self.connection.websocket.recv().split('\n')
                 result = []
                 for i in data:
@@ -290,20 +293,21 @@
                     self.connection._handshake()
                 except Exception:
                     if "on_disconnect" in self._events:
                         self._events["on_disconnect"]()
 
 class WsCloudEvents(CloudEvents):
 
-    def __init__(self, project_id, connection):
+    def __init__(self, project_id, connection, **entries):
         self.data = []
         self._thread = None
         self.running = False
         self._events = {}
         self.connection = connection
+        self.__dict__.update(entries)
 
     def _update(self):
         while True:
             try:
                 data = self.connection.websocket.recv().split('\n')
                 result = []
                 for i in data:
```

### Comparing `scratchattach-1.1.8/scratchattach/_cloud_requests.py` & `scratchattach-1.2.1/scratchattach/_cloud_requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self.events = []
 
         self.request_parts = {}
         self.outputs = {}
         self.respond_in_thread= False
         self.current_var = 0
         self.idle_since = 0
+        self.force_reconnect = False
 
     def __init__(self, cloud_connection : _cloud.CloudConnection, *, used_cloud_vars = ["1","2","3","4","5","6","7","8","9"], ignore_exceptions=True, force_reconnect=True, _log_url="https://clouddata.scratch.mit.edu/logs", _packet_length=245):
         print("\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m")
         if _log_url != "https://clouddata.scratch.mit.edu/logs":
             warnings.warn("Log URL isn't the URL of Scratch's clouddata logs. Don't use the _log_url parameter unless you know what you are doing", RuntimeWarning)
         if _packet_length > 245:
             warnings.warn("The packet length was set to a value higher than default (245). Your project most likely won't work on Scratch.", RuntimeWarning)
@@ -117,17 +118,17 @@
 
         return self.last_requester
 
     def get_timestamp(self):
 
         return self.last_timestamp
 
-    def _respond(self, request_id, response, limit, *, force_reconnect=False, validation=2222):
+    def _respond(self, request_id, response, limit, *, validation=2222):
 
-        if self.idle_since + 8 < time.time() or force_reconnect:
+        if self.idle_since + 8 < time.time() or self.force_reconnect:
             self.connection._connect(cloud_host=self.connection.cloud_host)
             self.connection._handshake()
 
         remaining_response = str(response)
 
 
         i = 0
@@ -162,35 +163,41 @@
                     self.current_var = 0
 
                 remaining_response = ""
                 time.sleep(0.1)
 
         self.idle_since = time.time()
 
-    def run(self, thread=False, data_from_websocket=True):
+    def run(self, thread=False, data_from_websocket=True, no_packet_loss=False):
+        self.force_reconnect = no_packet_loss
         if data_from_websocket is True:
-            events = _cloud.WsCloudEvents(self.project_id, _cloud.CloudConnection(project_id = self.project_id, username = self.connection._username, session_id=self.connection._session_id))
+            events = [
+                _cloud.WsCloudEvents(self.project_id, _cloud.CloudConnection(project_id = self.project_id, username = self.connection._username, session_id=self.connection._session_id), update_interval=0),
+                _cloud.CloudEvents(self.project_id, update_interval=4.5, cloud_log_limit=25)
+            ]
         else:
-            events = _cloud.CloudEvents(self.project_id)
+            events = [
+                _cloud.CloudEvents(self.project_id, update_interval=0, cloud_log_limit=100)
+            ]
         if thread:
-            thread = Thread(target=self._run, args=[events], kwargs={"data_from_websocket":data_from_websocket})
+            thread = Thread(target=self._run, args=[events])
             thread.start()
         else:
-            self._run(events, data_from_websocket=data_from_websocket)
+            self._run(events)
 
     def call_event(self, event, args=[]):
         events = list(filter(lambda k: k.__name__ == event, self.events))
         if events == []:
             return False
         else:
             events[0](*args)
             return True
 
     def _parse_output(self, output, request, req_obj, request_id):
-        if len(str(output)) > 3000 and not self.data_from_websocket:
+        if len(str(output)) > 3000:
             print(f"Warning: Output of request '{request}' is longer than 3000 characters (length: {len(str(output))} characters). Responding the request will take >4 seconds.")
 
         if str(request_id).endswith("0"):
             try:
                 int(output) == output
             except Exception:
                 send_as_integer = False
@@ -217,125 +224,106 @@
                 output += "89"
         if send_as_integer:
             self._respond(request_id, output, self.packet_length, validation=3222)
         else:
             self._respond(request_id, output, self.packet_length)
 
 
-    def _run(self, events, data_from_websocket=False):
+    def _run(self, events):
         self.ws_data = []
-        self.data_from_websocket = data_from_websocket
 
-        if data_from_websocket or self.respond_in_thread:
-            self.cloud_events = events
-
-            @self.cloud_events.event
-            def on_set(event):
-                if event.name == "TO_HOST":
-                    self.ws_data.insert(0, {"user":event.user,"value":event.value,"timestamp":event.timestamp})
-                self.ws_data = self.ws_data[:100]
-
-            @self.cloud_events.event
-            def on_disconnect():
-                self.call_event("on_disconnect")
-
-            self.cloud_events.start(update_interval=0)
-        else:
-            self.cloud_events = None
+        def on_set(event):
+            if event.name == "TO_HOST":
+                self.ws_data.insert(0,event)
+                self.ws_data = self.ws_data[:50]
 
 
         try:
             self.connection._connect(cloud_host=self.connection.cloud_host)
             self.connection._handshake()
         except Exception:
             self.call_event("on_disconnect")
-        self.idle_since = time.time()
-        if data_from_websocket:
-            self.last_data = []
-        else:
-            self.last_data = _cloud.get_cloud_logs(self.project_id, limit=100, log_url=self.log_url)
-        self.last_timestamp = 0
 
-        if not data_from_websocket:
-            data = _cloud.get_cloud_logs(self.project_id, limit=100, log_url=self.log_url)
-            if data == []:
-                pass
-            else:
-                self.last_timestamp = data[0]["timestamp"]
-
-        self.call_event("on_ready")
+        self.idle_since = time.time()
+        self.responded_request_ids = []
 
         if self.requests == []:
             warnings.warn("You haven't added any requests!", RuntimeWarning)
 
+        while events != []:
+            event_handler = events.pop()
+            event_handler.event(on_set)
+            event_handler.start(
+                update_interval=event_handler.update_interval,
+                thread=True
+            )
+
+        self.call_event("on_ready") #Calls the on_ready event
+
         while True:
 
-            if data_from_websocket or self.respond_in_thread:
-                data = self.ws_data
-            else:
-                data = _cloud.get_cloud_logs(self.project_id, limit=100, log_url=self.log_url, filter_by_var_named="TO_HOST")
-                self.ws_data = data
-            if self.ws_data == []:
-                continue
-            data = reversed(data)
-            if self.last_data == data:
-                pass
-            else:
-                for activity in data:
-                    if activity['timestamp'] > self.last_timestamp:
-                        self.last_requester = activity["user"]
-                        self.last_timestamp = activity['timestamp']
-
-                        try:
-                            raw_request, request_id = activity["value"].split(".")
-                        except Exception:
-                            self.last_timestamp = activity['timestamp']
-                            continue
-
-
-                        if activity["value"][0] == "-":
-                            if not request_id in self.request_parts:
-                                self.request_parts[request_id] = []
-                            self.request_parts[request_id].append(raw_request[1:])
-                            continue
-
-                        _raw_request = ""
-                        if request_id in self.request_parts:
-                            data = self.request_parts[request_id]
-                            for i in data:
-                                _raw_request += i
-                            self.request_parts.pop(request_id)
-                        raw_request = _raw_request + raw_request
-
-                        request = Encoding.decode(raw_request)
-                        arguments = request.split("&")
-                        request = arguments.pop(0)
-                        self.call_event("on_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id,id=request_id)])
-                        output = ""
-
-                        if request not in self.requests:
-                            warnings.warn(f"Warning: Client received an unknown request called '{request}'")
-                            self.call_event("on_unknown_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id)])
-                            continue
-                        else:
-                            req_obj = self.requests[request]
-                            self.last_request_id = request_id
-                            if req_obj["thread"]:
-                                Thread(target=self.call_request, args=(request_id, req_obj, arguments)).start()
-                            else:
-                                self.call_request(request_id, req_obj, arguments)
-                self.last_data = data
+            if self.ws_data != []:
+                event = self.ws_data.pop()
+
+                try:
+                    raw_request, request_id = event.value.split(".")
+                    if request_id in self.responded_request_ids:
+                        continue
+                    else:
+                        self.responded_request_ids.insert(0, request_id)
+                        self.responded_request_ids = self.responded_request_ids[:15]
+                except Exception:
+                    self.last_timestamp = event.timestamp
+                    continue
+
+                self.last_requester = event.user
+                self.last_timestamp = event.timestamp
+
+
+                if event.value[0] == "-":
+                    if not request_id in self.request_parts:
+                        self.request_parts[request_id] = []
+                    self.request_parts[request_id].append(raw_request[1:])
+                    continue
+
+                _raw_request = ""
+                if request_id in self.request_parts:
+                    data = self.request_parts[request_id]
+                    for i in data:
+                        _raw_request += i
+                    self.request_parts.pop(request_id)
+                raw_request = _raw_request + raw_request
+
+                request = Encoding.decode(raw_request)
+                arguments = request.split("&")
+                request = arguments.pop(0)
+                self.call_event("on_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id,id=request_id)])
+                output = ""
+
+                if request not in self.requests:
+                    print(f"Warning: Client received an unknown request called '{request}'")
+                    self.call_event("on_unknown_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id)])
+                    continue
+                else:
+                    req_obj = self.requests[request]
+                    self.last_request_id = request_id
+                    if req_obj["thread"]:
+                        Thread(target=self.call_request, args=(request_id, req_obj, arguments)).start()
+                    else:
+                        self.call_request(request_id, req_obj, arguments)
 
+            #Send outputs
             output_ids = list(self.outputs.keys())
-            if len(output_ids) > 0:
+            while len(output_ids) > 0:
                 for request_id in output_ids:
                     output = self.outputs[request_id]["output"]
                     request = self.outputs[request_id]["request"]["name"]
                     req_obj = self.outputs[request_id]["request"]
                     self._parse_output(output, request, req_obj, request_id)
+                    self.outputs.pop(request_id)
 
 class TwCloudRequests(CloudRequests):
 
     def __init__(self, cloud_connection, *, used_cloud_vars = ["1","2","3","4","5","6","7","8","9"], ignore_exceptions=True, force_reconnect=True, _packet_length=98800):
         print("\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m")
         if _packet_length > 98800:
             warnings.warn("The packet length was set to a value higher than TurboWarp's default (98800).", RuntimeWarning)
@@ -347,14 +335,15 @@
         self.packet_length = _packet_length
 
         self.init_attributes()
 
     def get_requester(self):
         return None
 
-    def run(self, thread=False, data_from_websocket=True):
-        events = _cloud.TwCloudEvents(self.project_id)
+    def run(self, thread=False, data_from_websocket=True, no_packet_loss=False):
+        self.force_reconnect = no_packet_loss
+        events = [_cloud.TwCloudEvents(self.project_id, update_interval=0)]
         if thread:
-            thread = Thread(target=self._run, args=[events], kwargs={"data_from_websocket":True})
+            thread = Thread(target=self._run, args=[events])
             thread.start()
         else:
-            self._run(events, data_from_websocket=True)
+            self._run(events)
```

### Comparing `scratchattach-1.1.8/scratchattach/_encoder.py` & `scratchattach-1.2.1/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.8/scratchattach/_exceptions.py` & `scratchattach-1.2.1/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.8/scratchattach/_forum.py` & `scratchattach-1.2.1/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.8/scratchattach/_project.py` & `scratchattach-1.2.1/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.8/scratchattach/_session.py` & `scratchattach-1.2.1/scratchattach/_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #----- Connecting to a Scratch account
 
 import json
 import re
 import requests
+import warnings
 
 from . import _user
 from . import _cloud
 from . import _project
 from . import _exceptions
 from . import _studio
 from . import _forum
@@ -67,21 +68,21 @@
             self._headers["X-Token"] = self.xtoken
             self.email = response["user"]["email"]
             self.new_scratcher = response["permissions"]["new_scratcher"]
             self.mute_status = response["permissions"]["mute_status"]
             self._username = response["user"]["username"]
             self.banned = response["user"]["banned"]
             if self.banned:
-                print("Warning: The account you logged in to is BANNED. Some features may not work properly.")
+                warnings.warn(f"Warning: The account {self._username} you logged in to is BANNED. Some features may not work properly.")
 
         except Exception:
             if self._username is None:
                 print("Warning: Logged in, but couldn't fetch XToken.\nSome features (including cloud variables) will not work properly. To get cloud variables to work, provide a username argument: Session('session_id', username='username')\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
             else:
-                print("Warning: Logged in, but couldn't fetch XToken. Cloud variables will still work, but other features may not work properly.\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
+                print(f"Warning: Logged in as {self._username}, but couldn't fetch XToken. Cloud variables will still work, but other features may not work properly.\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
             self.xtoken = ""
 
     def get_linked_user(self):
 
         #this will fetch the user who is associated to the session
         if not "_user" in self.__dict__:
             self._user = self.connect_user(self._username)
```

### Comparing `scratchattach-1.1.8/scratchattach/_studio.py` & `scratchattach-1.2.1/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.8/scratchattach/_user.py` & `scratchattach-1.2.1/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.8/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.2.1/scratchattach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.8
+Version: 1.2.1
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 License: UNKNOWN
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Platform: UNKNOWN
@@ -44,15 +44,15 @@
 Add this to your Python code:
 ```python
 import os
 
 os.system("pip install -U scratchattach")
 ```
 
-# Logging in  `scratch3.Session`
+# Logging in
 
 **Logging in with username / password:**
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.login("username", "password")
@@ -75,16 +75,15 @@
 session.xtoken
 session.email #Returns the email address associated with the account
 session.new_scratcher #Returns True if the associated account is a New Scratcher
 session.mute_status
 session.banned #Returns True if the associated account is banned
 ```
 
-# Cloud variables  `scratch3.CloudConnection`
-*Make sure you're using the latest scratchattach version. Update scratchattach with `pip install scratchattach --upgrade`*
+# Cloud variables
 
 **Connect to the Scratch cloud:**
 
 With a `Session` object:
 
 ```python
 conn = session.connect_cloud("project_id")
@@ -134,32 +133,32 @@
 
 **Close the cloud connection:**
 
 ```python
 conn.disconnect()
 ```
 
-# Encoding / Decoding  `scratch3.Encoding`
+# Encoding / Decoding
 
 Scratchattach has a built in encoder. Scratch sprite to decode texts encoded with scratchattach: https://scratch3-assets.1tim.repl.co/Encoder.sprite3
 
 ```python
 from scratchattach import Encoding
 
 Encoding.encode("input") #will return the encoded text
 Encoding.decode("encoded") #will decode an encoded text
 ```
 
-# Cloud events  `scratch3.CloudEvents`
+# Cloud events
 
 *Cloud events allow reacting to cloud events in real time. If a Scratcher
 sets / creates / deletes a cloud var on the given project, an
 event will be called.*
 
-They do not require a session.
+They do not require a session because they use the clouddata logs to receive cloud updates.
 
 **How to use with Scratch:**
 
 ```python
 import scratchattach as scratch3
 
 events = scratch3.CloudEvents("project_id")
@@ -179,48 +178,60 @@
 @events.event #Called when the event listener is ready
 def on_ready():
    print("Event listener ready!")
 
 events.start()
 ```
 
-**How to use with TurboWarp:** (new in v0.4.7)
+**How to use with TurboWarp:**
 
 ```python
 import scratchattach as scratch3
 
 events = scratch3.TwCloudEvents("project_id")
 
 ...
 ```
 
+**Cloud events that use a `scratch3.CloudConnection` object to receive cloud updates:**
+
+```python
+import scratchattach as scratch3
+
+session = scratch3.Session("session_id", username="username") #Replace with your data
+conn = session.connect_cloud("project_id")
+events = scratch3.WsCloudEvents("project_id", conn)
+
+...
+```
+
 **Functions:**
 ```py
 events.start(thread=True)
 events.pause()
 events.resume()
 events.stop()
 ```
 
-# Cloud Requests  `scratch3.CloudRequests`
+# Cloud Requests
 
 Cloud Requests Framework (inspired by discord.py) that allows Scratch projects and Python to interact
 
 *This makes it possible to access data like message counts, user stats and more from Scratch projects! Uses cloud variables to transmit data.*
 
 **[Cloud Requests are documented on this page:](https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests)**
 
 [https://github.com/TimMcCool/scratchattach/blob/main/CLOUD_REQUESTS.md](https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests)
 
 If you want to access external information in Scratch projects or store data on an external database, scratchattach's Cloud Requests are ideal for your project:
 - Similar to cloud events, but send back data to the project
 - Automatically encode / decode sent data
 - Tons of extra features
 
-# Users  `scratch3.User`
+# Users
 
 **Get a user:**
 ```python
 user = session.connect_user("username")
 ```
 
 Get the user that you are logged in with:
@@ -295,15 +306,15 @@
 user.forum_counts_over_time() #Fetched from ScratchDB
 user.forum_signature() #Fetched from ScratchDB
 user.forum_signature_history() #A change log for the user's forum history. Fetched from ScratchDB
 
 user.ocular_status() #Returns information about the user's ocular status, like the status text, the color, and the time of the last update.
 ```
 
-# Projects  `scratch3.Project`
+# Projects
 
 **Get a project:**
 ```python
 project = session.connect_project("project_id")
 ```
 
 You can also get projects without logging in: (but then you can't use any functions that require a login, and you can't get your unshared projects)
@@ -369,25 +380,24 @@
 project.studios(limit=None, offset=0) #Returns the studios the project is in as list of dicts
 
 project.download(filename="project_name.sb3", dir="") #Downloads the project to your computer. The downloaded file will only work in the online editor
 project.get_raw_json() #Returns the json of the project content as dict
 project.get_creator_agent() #Returns the user-agent of the user who created the project (with information about their browser and OS)
 ```
 
-# Unshared projects  `scratch3.PartialProject`
+# Unshared projects
 
 When connecting / getting a project that you can't access, a `PartialProject` object is returned instead.
 
 **Most attributes and most functions don't work for such projects. However, these still work:**
 ```python
 project.remixes(limit=None, offset=0)
 ```
 
-# Studios  `scratch3.Studio`
-(New in v0.5.0)
+# Studios
 
 **Get a studio:**
 ```python
 studio = session.connect_studio("studio_id")
 ```
 You can also get studios without logging in: (But then you can't use any functions that require a login, like studio.follow(), studio.add_project(), ...)
 ```python
@@ -490,16 +500,15 @@
 scratch3.newest_projects() #Returns a list with the newest Scratch projects. This list is not present on the Scratch home page, but the API still provides it.
 scratch3.design_studio_projects()
 
 session.get_feed(limit=20, offset=0) #Returns your "What's happening" section from the Scratch front page as list
 session.loved_by_followed_users(limit=40, offset=0) #Returns the projects loved by users you are following as list
 ```
 
-# Forum topics `scratch3.ForumTopic`
-(New in v0.5.5)
+# Forum topics
 All of this data is fetched from ScratchDB v3, therefore it may be slighty off.
 
 **Get a forum topic:**
 ```python
 topic = session.connect_topic("topic_id")
 ```
 You can also get topics without logging in:
@@ -536,16 +545,15 @@
 
 topic.post_count_by_user("username")
 topic.activity() #Returns an activity / change log for the topic
 ```
 
 To prevent spam, adding posts to topics is not a scratchattach feature and never will be.
 
-# Forum posts `scratch3.ForumPost`
-(New in v0.5.5)
+# Forum posts
 All of this data is fetched from ScratchDB v3, therefore it may be slighty off.
 
 **Get a forum post:**
 ```python
 post = session.connect_post("post_id")
 ```
 You can also get posts without logging in:
@@ -612,10 +620,10 @@
 - Allmost all code by TimMcCool.
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
 
 If you need help with your code, leave a comment on TimMcCool's Scratch
-profile: https://scratch.mit.edu/users/TimMcCool/
+profile (https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
```

### Comparing `scratchattach-1.1.8/setup.py` & `scratchattach-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.8'
+VERSION = '1.2.1'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```


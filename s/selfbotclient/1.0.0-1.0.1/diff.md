# Comparing `tmp/selfbotclient-1.0.0.tar.gz` & `tmp/selfbotclient-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfbotclient-1.0.0.tar", last modified: Fri Jun  9 22:49:30 2023, max compression
+gzip compressed data, was "selfbotclient-1.0.1.tar", last modified: Fri Jun  9 22:56:53 2023, max compression
```

## Comparing `selfbotclient-1.0.0.tar` & `selfbotclient-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 22:49:30.490368 selfbotclient-1.0.0/
--rw-rw-rw-   0        0        0      913 2023-06-09 22:49:30.489368 selfbotclient-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-06-07 14:22:37.000000 selfbotclient-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 22:49:30.471368 selfbotclient-1.0.0/SelfBotClient/
--rw-rw-rw-   0        0        0      376 2023-06-09 22:25:15.000000 selfbotclient-1.0.0/SelfBotClient/__init__.py
--rw-rw-rw-   0        0        0      472 2023-06-09 21:55:30.000000 selfbotclient-1.0.0/SelfBotClient/__main__.py
--rw-rw-rw-   0        0        0    16893 2023-06-09 21:57:25.000000 selfbotclient-1.0.0/SelfBotClient/client.py
--rw-rw-rw-   0        0        0     1399 2023-06-07 23:57:30.000000 selfbotclient-1.0.0/SelfBotClient/enums.py
--rw-rw-rw-   0        0        0      826 2023-06-06 22:37:48.000000 selfbotclient-1.0.0/SelfBotClient/errors.py
--rw-rw-rw-   0        0        0    11955 2023-06-09 21:57:25.000000 selfbotclient-1.0.0/SelfBotClient/http.py
--rw-rw-rw-   0        0        0     1046 2023-06-08 23:49:03.000000 selfbotclient-1.0.0/SelfBotClient/logger.py
--rw-rw-rw-   0        0        0      807 2023-06-09 13:27:08.000000 selfbotclient-1.0.0/SelfBotClient/permissionbuilder.py
--rw-rw-rw-   0        0        0      313 2023-06-07 23:24:53.000000 selfbotclient-1.0.0/SelfBotClient/typings.py
--rw-rw-rw-   0        0        0    17057 2023-06-09 21:55:30.000000 selfbotclient-1.0.0/SelfBotClient/user.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:49:30.489368 selfbotclient-1.0.0/selfbotclient.egg-info/
--rw-rw-rw-   0        0        0      913 2023-06-09 22:49:30.000000 selfbotclient-1.0.0/selfbotclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-06-09 22:49:30.000000 selfbotclient-1.0.0/selfbotclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 22:49:30.000000 selfbotclient-1.0.0/selfbotclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 22:49:30.000000 selfbotclient-1.0.0/selfbotclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 22:49:30.000000 selfbotclient-1.0.0/selfbotclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 22:49:30.490368 selfbotclient-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-06-09 22:48:32.000000 selfbotclient-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:56:53.656158 selfbotclient-1.0.1/
+-rw-rw-rw-   0        0        0     1161 2023-06-09 22:56:53.655158 selfbotclient-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-06-09 22:56:48.000000 selfbotclient-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 22:56:53.647157 selfbotclient-1.0.1/SelfBotClient/
+-rw-rw-rw-   0        0        0      376 2023-06-09 22:25:15.000000 selfbotclient-1.0.1/SelfBotClient/__init__.py
+-rw-rw-rw-   0        0        0      472 2023-06-09 21:55:30.000000 selfbotclient-1.0.1/SelfBotClient/__main__.py
+-rw-rw-rw-   0        0        0    16893 2023-06-09 22:56:48.000000 selfbotclient-1.0.1/SelfBotClient/client.py
+-rw-rw-rw-   0        0        0     1399 2023-06-07 23:57:30.000000 selfbotclient-1.0.1/SelfBotClient/enums.py
+-rw-rw-rw-   0        0        0      826 2023-06-06 22:37:48.000000 selfbotclient-1.0.1/SelfBotClient/errors.py
+-rw-rw-rw-   0        0        0    11955 2023-06-09 21:57:25.000000 selfbotclient-1.0.1/SelfBotClient/http.py
+-rw-rw-rw-   0        0        0     1046 2023-06-08 23:49:03.000000 selfbotclient-1.0.1/SelfBotClient/logger.py
+-rw-rw-rw-   0        0        0      807 2023-06-09 13:27:08.000000 selfbotclient-1.0.1/SelfBotClient/permissionbuilder.py
+-rw-rw-rw-   0        0        0      313 2023-06-07 23:24:53.000000 selfbotclient-1.0.1/SelfBotClient/typings.py
+-rw-rw-rw-   0        0        0    17057 2023-06-09 21:55:30.000000 selfbotclient-1.0.1/SelfBotClient/user.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:56:53.655158 selfbotclient-1.0.1/selfbotclient.egg-info/
+-rw-rw-rw-   0        0        0     1161 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 22:56:53.656158 selfbotclient-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-09 22:56:48.000000 selfbotclient-1.0.1/setup.py
```

### Comparing `selfbotclient-1.0.0/PKG-INFO` & `selfbotclient-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfbotclient
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library that will allow you to manage selfbots
 Home-page: UNKNOWN
 Author: xXenvy
 Author-email: <xpimepk01@gmail.com>
 License: UNKNOWN
 Keywords: python,requests,discord selfbot,selfbot,discord.py,aiohttp
 Platform: UNKNOWN
@@ -14,15 +14,23 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Self Bot Client
-## ⚡ Fastest selfbotting client
+## ⚡ Fast SelfBotClient
 - Token Checker | `1` token / `140`ms
-- Delay between command and execution - `16ms`
+- 3 requests / 1s `(in feature 10 requests / 1s using threads)`
+
 ## 🔧 Full control
-- A separate method for making your own commands
-- Ability to perform a specific action only on selected users
+- A separate method to send your own requests
+- Ability to manage individual selfbots
+
+## 📌 Ratelimit handler
+
+- The library itself detects whether you have reached the ratelimit of the discord and, if so, forces you to wait a certain time.
+
+## 💫 Examples
+**See examples on github:** https://github.com/xXenvy?tab=repositories
```

### Comparing `selfbotclient-1.0.0/SelfBotClient/client.py` & `selfbotclient-1.0.1/SelfBotClient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from collections.abc import AsyncIterable
 
 from typing import Union
 from asyncio import AbstractEventLoop
 
 
 class Client(HTTPClient):
-    __version__: str = "1.0.0"
+    __version__: str = "1.0.1"
 
     def __init__(
             self,
             api_version: API_VERSION,
             loop: AbstractEventLoop = None,
             logger: bool = True,
             request_latency: float = 0.1,
```

### Comparing `selfbotclient-1.0.0/SelfBotClient/enums.py` & `selfbotclient-1.0.1/SelfBotClient/enums.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.0/SelfBotClient/errors.py` & `selfbotclient-1.0.1/SelfBotClient/errors.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.0/SelfBotClient/http.py` & `selfbotclient-1.0.1/SelfBotClient/http.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.0/SelfBotClient/logger.py` & `selfbotclient-1.0.1/SelfBotClient/logger.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.0/SelfBotClient/permissionbuilder.py` & `selfbotclient-1.0.1/SelfBotClient/permissionbuilder.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.0/SelfBotClient/user.py` & `selfbotclient-1.0.1/SelfBotClient/user.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.0/selfbotclient.egg-info/PKG-INFO` & `selfbotclient-1.0.1/selfbotclient.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfbotclient
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library that will allow you to manage selfbots
 Home-page: UNKNOWN
 Author: xXenvy
 Author-email: <xpimepk01@gmail.com>
 License: UNKNOWN
 Keywords: python,requests,discord selfbot,selfbot,discord.py,aiohttp
 Platform: UNKNOWN
@@ -14,15 +14,23 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Self Bot Client
-## ⚡ Fastest selfbotting client
+## ⚡ Fast SelfBotClient
 - Token Checker | `1` token / `140`ms
-- Delay between command and execution - `16ms`
+- 3 requests / 1s `(in feature 10 requests / 1s using threads)`
+
 ## 🔧 Full control
-- A separate method for making your own commands
-- Ability to perform a specific action only on selected users
+- A separate method to send your own requests
+- Ability to manage individual selfbots
+
+## 📌 Ratelimit handler
+
+- The library itself detects whether you have reached the ratelimit of the discord and, if so, forces you to wait a certain time.
+
+## 💫 Examples
+**See examples on github:** https://github.com/xXenvy?tab=repositories
```

### Comparing `selfbotclient-1.0.0/setup.py` & `selfbotclient-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Library that will allow you to manage selfbots'
 LONG_DESCRIPTION = 'The library logs into your account thanks to the entered tokens and can manage them. ' \
                    'such as sending messages, deleting roles, etc.'
 
 # Setting up
 setup(
     name="selfbotclient",
```


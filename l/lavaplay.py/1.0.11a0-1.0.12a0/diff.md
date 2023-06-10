# Comparing `tmp/lavaplay.py-1.0.11a0.tar.gz` & `tmp/lavaplay.py-1.0.12a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavaplay.py-1.0.11a0.tar", last modified: Tue May 30 09:37:46 2023, max compression
+gzip compressed data, was "lavaplay.py-1.0.12a0.tar", last modified: Sat Jun 10 07:11:43 2023, max compression
```

## Comparing `lavaplay.py-1.0.11a0.tar` & `lavaplay.py-1.0.12a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:37:46.320205 lavaplay.py-1.0.11a0/
--rw-rw-rw-   0        0        0     1068 2021-12-23 20:00:48.000000 lavaplay.py-1.0.11a0/LICENSE
--rw-rw-rw-   0        0        0     2939 2023-05-30 09:37:46.318203 lavaplay.py-1.0.11a0/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-05-30 09:23:53.000000 lavaplay.py-1.0.11a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 09:37:46.272202 lavaplay.py-1.0.11a0/lavaplay/
--rw-rw-rw-   0        0        0      476 2023-05-30 08:18:24.000000 lavaplay.py-1.0.11a0/lavaplay/__init__.py
--rw-rw-rw-   0        0        0     2196 2023-05-30 08:45:21.000000 lavaplay.py-1.0.11a0/lavaplay/client.py
--rw-rw-rw-   0        0        0     2329 2023-05-30 08:40:08.000000 lavaplay.py-1.0.11a0/lavaplay/emitter.py
--rw-rw-rw-   0        0        0     1675 2023-05-29 06:25:13.000000 lavaplay.py-1.0.11a0/lavaplay/events.py
--rw-rw-rw-   0        0        0     2849 2023-05-30 06:39:36.000000 lavaplay.py-1.0.11a0/lavaplay/exceptions.py
--rw-rw-rw-   0        0        0     8907 2023-05-30 09:24:12.000000 lavaplay.py-1.0.11a0/lavaplay/node_manager.py
--rw-rw-rw-   0        0        0     7354 2023-05-30 08:38:17.000000 lavaplay.py-1.0.11a0/lavaplay/objects.py
--rw-rw-rw-   0        0        0    10155 2023-05-30 08:44:10.000000 lavaplay.py-1.0.11a0/lavaplay/player.py
--rw-rw-rw-   0        0        0     7833 2023-05-30 08:45:48.000000 lavaplay.py-1.0.11a0/lavaplay/rest.py
--rw-rw-rw-   0        0        0      844 2023-05-30 08:45:58.000000 lavaplay.py-1.0.11a0/lavaplay/routes.py
--rw-rw-rw-   0        0        0     1263 2023-01-25 04:56:45.000000 lavaplay.py-1.0.11a0/lavaplay/utlits.py
--rw-rw-rw-   0        0        0     8697 2023-05-30 08:42:11.000000 lavaplay.py-1.0.11a0/lavaplay/ws.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:37:46.316202 lavaplay.py-1.0.11a0/lavaplay.py.egg-info/
--rw-rw-rw-   0        0        0     2939 2023-05-30 09:37:45.000000 lavaplay.py-1.0.11a0/lavaplay.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-05-30 09:37:46.000000 lavaplay.py-1.0.11a0/lavaplay.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:37:45.000000 lavaplay.py-1.0.11a0/lavaplay.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 09:37:46.000000 lavaplay.py-1.0.11a0/lavaplay.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 09:37:46.000000 lavaplay.py-1.0.11a0/lavaplay.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 09:37:46.320205 lavaplay.py-1.0.11a0/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-05-30 08:26:32.000000 lavaplay.py-1.0.11a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:11:43.815950 lavaplay.py-1.0.12a0/
+-rw-rw-rw-   0        0        0     1089 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-06-10 07:11:43.813950 lavaplay.py-1.0.12a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1863 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 07:11:43.778950 lavaplay.py-1.0.12a0/lavaplay/
+-rw-rw-rw-   0        0        0      497 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/client.py
+-rw-rw-rw-   0        0        0     2377 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/emitter.py
+-rw-rw-rw-   0        0        0     1675 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/events.py
+-rw-rw-rw-   0        0        0     2994 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/exceptions.py
+-rw-rw-rw-   0        0        0     8966 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/node_manager.py
+-rw-rw-rw-   0        0        0     7272 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/objects.py
+-rw-rw-rw-   0        0        0    10567 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/player.py
+-rw-rw-rw-   0        0        0     7938 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/rest.py
+-rw-rw-rw-   0        0        0      866 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/routes.py
+-rw-rw-rw-   0        0        0     1259 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/utlits.py
+-rw-rw-rw-   0        0        0     8887 2023-06-10 07:05:17.000000 lavaplay.py-1.0.12a0/lavaplay/ws.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:11:43.809949 lavaplay.py-1.0.12a0/lavaplay.py.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-06-10 07:11:43.000000 lavaplay.py-1.0.12a0/lavaplay.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-06-10 07:11:43.000000 lavaplay.py-1.0.12a0/lavaplay.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 07:11:43.000000 lavaplay.py-1.0.12a0/lavaplay.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 07:11:43.000000 lavaplay.py-1.0.12a0/lavaplay.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 07:11:43.000000 lavaplay.py-1.0.12a0/lavaplay.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 07:11:43.815950 lavaplay.py-1.0.12a0/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-06-10 07:11:03.000000 lavaplay.py-1.0.12a0/setup.py
```

### Comparing `lavaplay.py-1.0.11a0/LICENSE` & `lavaplay.py-1.0.12a0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 HazemMeqdad
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 HazemMeqdad
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `lavaplay.py-1.0.11a0/PKG-INFO` & `lavaplay.py-1.0.12a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavaplay.py
-Version: 1.0.11a0
+Version: 1.0.12a0
 Summary: Its a lavalink nodes manger to make a music bots for discord with python.
 Home-page: https://github.com/HazemMeqdad/lavaplay.py
 Author: HazemMeqdad
 Author-email: hazemmeqdad@outlook.com
 Project-URL: Bug Reports, https://github.com/HazemMeqdad/lavaplay.py/issues
 Project-URL: Source, https://github.com/HazemMeqdad/lavaplay.py/
 Project-URL: Documentation, https://lavaplay.readthedocs.io/en/latest
@@ -63,40 +63,44 @@
     port=2333,
     password="youshallnotpass",
     user_id=123
 )
 
 @bot.listen()
 async def on_ready(event: hikari.ShardReadyEvent) -> None:
-    await node.connect()
+    node.connect()
 
 bot.run()
 ```
 
 examples for some methods.
 ```python
+# Player object
+player = node.get_player(guild_id)
+
 # Auto search mix with track or query
-await lavalink.auto_search_tracks("Rick Astley")
+await player.auto_search_tracks("Rick Astley")
 
 # Play track
-await lavalink.play(guild_id, track)
+await player.play(track)
 
 # Skip
-await lavalink.skip(guild_id)
+await player.skip()
 
 # Pause
-await lavalink.pause(guild_id, stats)
+await player.pause(stats)
 
 # Volume
-await lavalink.volume(guild_id, volume)
+await player.volume(volume)
 ```
 
 # Features
 
 - [ ] Spotify support
+- [x] new Rest api for lavalink support
 - [x] connection handler
 - [x] Support youtube playlist
 - [x] Add example for other discord wrapper library
 
 # Installation
 
 ```shell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lavaplay.py Version: 1.0.11a0 Summary: Its a
+Metadata-Version: 2.1 Name: lavaplay.py Version: 1.0.12a0 Summary: Its a
 lavalink nodes manger to make a music bots for discord with python. Home-page:
 https://github.com/HazemMeqdad/lavaplay.py Author: HazemMeqdad Author-email:
 hazemmeqdad@outlook.com Project-URL: Bug Reports, https://github.com/
 HazemMeqdad/lavaplay.py/issues Project-URL: Source, https://github.com/
 HazemMeqdad/lavaplay.py/ Project-URL: Documentation, https://
 lavaplay.readthedocs.io/en/latest Keywords: lavalink,discord,discord-
 lavalink,lavaplay,lavaplay.py Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,16 @@
 About lavaplay.py is a nodes manager to connection with discord voice gateway,
 easy to create a music bot, you can use to anything async discord wrapper
 library # Usage example for create connecting with lavalink server using
 [hikari](https://github.com/hikari-py/hikari). ```python import hikari import
 lavaplay bot = hikari.GatewayBot("token") lavalink = lavaplay.Lavalink() node =
 lavalink.create_node( host="localhost", port=2333, password="youshallnotpass",
 user_id=123 ) @bot.listen() async def on_ready(event: hikari.ShardReadyEvent) -
-> None: await node.connect() bot.run() ``` examples for some methods. ```python
-# Auto search mix with track or query await lavalink.auto_search_tracks("Rick
-Astley") # Play track await lavalink.play(guild_id, track) # Skip await
-lavalink.skip(guild_id) # Pause await lavalink.pause(guild_id, stats) # Volume
-await lavalink.volume(guild_id, volume) ``` # Features - [ ] Spotify support -
-[x] connection handler - [x] Support youtube playlist - [x] Add example for
-other discord wrapper library # Installation ```shell # Linux/OS X $ pip3
-install -U lavaplay.py # Windows $ pip install -U lavaplay.py ```
+> None: node.connect() bot.run() ``` examples for some methods. ```python #
+Player object player = node.get_player(guild_id) # Auto search mix with track
+or query await player.auto_search_tracks("Rick Astley") # Play track await
+player.play(track) # Skip await player.skip() # Pause await player.pause(stats)
+# Volume await player.volume(volume) ``` # Features - [ ] Spotify support - [x]
+new Rest api for lavalink support - [x] connection handler - [x] Support
+youtube playlist - [x] Add example for other discord wrapper library #
+Installation ```shell # Linux/OS X $ pip3 install -U lavaplay.py # Windows $
+pip install -U lavaplay.py ```
```

### Comparing `lavaplay.py-1.0.11a0/README.md` & `lavaplay.py-1.0.12a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,40 +39,44 @@
     port=2333,
     password="youshallnotpass",
     user_id=123
 )
 
 @bot.listen()
 async def on_ready(event: hikari.ShardReadyEvent) -> None:
-    await node.connect()
+    node.connect()
 
 bot.run()
 ```
 
 examples for some methods.
 ```python
+# Player object
+player = node.get_player(guild_id)
+
 # Auto search mix with track or query
-await lavalink.auto_search_tracks("Rick Astley")
+await player.auto_search_tracks("Rick Astley")
 
 # Play track
-await lavalink.play(guild_id, track)
+await player.play(track)
 
 # Skip
-await lavalink.skip(guild_id)
+await player.skip()
 
 # Pause
-await lavalink.pause(guild_id, stats)
+await player.pause(stats)
 
 # Volume
-await lavalink.volume(guild_id, volume)
+await player.volume(volume)
 ```
 
 # Features
 
 - [ ] Spotify support
+- [x] new Rest api for lavalink support
 - [x] connection handler
 - [x] Support youtube playlist
 - [x] Add example for other discord wrapper library
 
 # Installation
 
 ```shell
```

#### html2text {}

```diff
@@ -5,15 +5,16 @@
 About lavaplay.py is a nodes manager to connection with discord voice gateway,
 easy to create a music bot, you can use to anything async discord wrapper
 library # Usage example for create connecting with lavalink server using
 [hikari](https://github.com/hikari-py/hikari). ```python import hikari import
 lavaplay bot = hikari.GatewayBot("token") lavalink = lavaplay.Lavalink() node =
 lavalink.create_node( host="localhost", port=2333, password="youshallnotpass",
 user_id=123 ) @bot.listen() async def on_ready(event: hikari.ShardReadyEvent) -
-> None: await node.connect() bot.run() ``` examples for some methods. ```python
-# Auto search mix with track or query await lavalink.auto_search_tracks("Rick
-Astley") # Play track await lavalink.play(guild_id, track) # Skip await
-lavalink.skip(guild_id) # Pause await lavalink.pause(guild_id, stats) # Volume
-await lavalink.volume(guild_id, volume) ``` # Features - [ ] Spotify support -
-[x] connection handler - [x] Support youtube playlist - [x] Add example for
-other discord wrapper library # Installation ```shell # Linux/OS X $ pip3
-install -U lavaplay.py # Windows $ pip install -U lavaplay.py ```
+> None: node.connect() bot.run() ``` examples for some methods. ```python #
+Player object player = node.get_player(guild_id) # Auto search mix with track
+or query await player.auto_search_tracks("Rick Astley") # Play track await
+player.play(track) # Skip await player.skip() # Pause await player.pause(stats)
+# Volume await player.volume(volume) ``` # Features - [ ] Spotify support - [x]
+new Rest api for lavalink support - [x] connection handler - [x] Support
+youtube playlist - [x] Add example for other discord wrapper library #
+Installation ```shell # Linux/OS X $ pip3 install -U lavaplay.py # Windows $
+pip install -U lavaplay.py ```
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/client.py` & `lavaplay.py-1.0.12a0/lavaplay/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import typing as t
 import logging
 from .node_manager import Node
 import asyncio
 
-_LOG = logging.getLogger("lavaplayer.client")
+_LOG = logging.getLogger("lavaplay.client")
 
 class Lavalink:
     """
     The main class for managing nodes.
     side note: to make connection must be use :meth:`Lavalink.create_node` or :meth:`Lavalink.destroy_node`.
     """
     def __init__(self) -> None:
         self._nodes: t.List[Node] = []
 
-    def create_node(self, host: str, port: int, password: str, user_id: int, *, name: str = None, shard_count: int = None, resume_key: str = None, resume_timeout: int = None, loop: t.Optional[asyncio.AbstractEventLoop] = None) -> Node:
+    def create_node(self, host: str, port: int, password: str, user_id: int, *, name: str = None, shard_count: int = None, ssl: bool = False, resume_key: str = None, resume_timeout: int = None, loop: t.Optional[asyncio.AbstractEventLoop] = None) -> Node:
         """
         Create a node for lavalink.
 
         Parameters
         ---------
         host: :class:`str`
             ip address for lavalink server, default ip address for lavalink is `
@@ -25,22 +25,24 @@
             The port to use for websocket and REST connections.
         password: :class:`str`
             The password used for authentication.
         name: :class:`str`
             The name for the node.
         shard_count: :class:`int`
             The shard count for the node.
+        ssl: :class:`bool`
+            Is server using ssl
         resume_key: :class:`str`
             The resume key for the node.
         resume_timeout: :class:`int`
             The resume timeout for the node.
         loop: :class:`asyncio.AbstractEventLoop`
             The event loop for the node.
         """
-        node = Node(host=host, port=port, password=password, user_id=user_id, name=name, shard_count=shard_count, resume_key=resume_key, resume_timeout=resume_timeout, loop=loop)
+        node = Node(host=host, port=port, password=password, user_id=user_id, name=name, shard_count=shard_count, resume_key=resume_key, resume_timeout=resume_timeout, is_ssl=ssl, loop=loop)
         self._nodes.append(node)
         return node
     
     def destroy_node(self, node: Node):
         """
         Destroy a node for lavalink.
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/emitter.py` & `lavaplay.py-1.0.12a0/lavaplay/emitter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import asyncio
-import typing as t
-from collections import deque
-import logging
-from .events import Event
-
-_LOGGER = logging.getLogger("lavaplayer.event_manger")
-
-class Emitter:
-    """
-    The class is a manger event from websocket.
-
-    Parameters
-    ---------
-    loop: :class:`AbstractEventLoop`
-        a loop event from asyncio
-    """
-    def __init__(self, loop: asyncio.AbstractEventLoop) -> None:
-        self._loop = loop
-        self.listeners = deque()
-    
-    def add_listener(self, event: t.Union[str, Event], func: t.Callable):
-        """
-        Add listener for listeners list.
-
-        Parameters
-        ---------
-        event: :class:`str` | :class:`Any`
-            event name or class for event
-        func: :class:`function`
-            the function to callback event
-        """
-        _LOGGER.debug(f"add listener {event}")
-        event = event if isinstance(event, str) else event.__name__
-        self.listeners.append({"event": event, "func": func})
-
-    def remove_listener(self, event: t.Union[str, Event], func: t.Callable):
-        """
-        Remove listener for listeners list.
-
-        Parameters
-        ---------
-        event: :class:`str` | :class:`Any`
-            event name or class for event
-        func: :class:`function`
-            the function to callback event
-        """
-        _LOGGER.debug(f"remove listener {event}")
-        event = event if isinstance(event, str) else event.__name__
-        self.listeners.remove([i for i in self.listeners if i["event"] == event and i["func"] == func])
-
-    def emit(self, event: t.Union[str, t.Any], data: t.Any):
-        """
-        Emit for event dont use this.
-
-        Parameters
-        ---------
-        event: :class:`str` | :class:`Any`
-            event name or class for event
-        data: :class:`function`
-            the data is revers to function callback
-        """
-        event_name = event if isinstance(event, str) else event.__name__
-        events = [i for i in self.listeners if i["event"] == event_name]
-        for event in events:
-            _LOGGER.debug(f"dispatch {event} for {len(events)} listeners")
-            if asyncio.iscoroutinefunction(event["func"]):
-                self._loop.create_task(event["func"](data))
-            else:
-                _LOGGER.error("Events only async function")
+import asyncio
+import typing as t
+from collections import deque
+import logging
+from .events import Event
+
+_LOG = logging.getLogger("lavaplay.emitter")
+
+class Emitter:
+    """
+    The class is a manger event from websocket.
+
+    Parameters
+    ---------
+    loop: :class:`AbstractEventLoop`
+        a loop event from asyncio
+    """
+    def __init__(self, loop: asyncio.AbstractEventLoop) -> None:
+        self._loop = loop
+        self.listeners = deque()
+    
+    def add_listener(self, event: t.Union[str, Event], func: t.Callable):
+        """
+        Add listener for listeners list.
+
+        Parameters
+        ---------
+        event: :class:`str` | :class:`Any`
+            event name or class for event
+        func: :class:`function`
+            the function to callback event
+        """
+        _LOG.debug(f"add listener {event}")
+        event = event if isinstance(event, str) else event.__name__
+        self.listeners.append({"event": event, "func": func})
+
+    def remove_listener(self, event: t.Union[str, Event], func: t.Callable):
+        """
+        Remove listener for listeners list.
+
+        Parameters
+        ---------
+        event: :class:`str` | :class:`Any`
+            event name or class for event
+        func: :class:`function`
+            the function to callback event
+        """
+        _LOG.debug(f"remove listener {event}")
+        event = event if isinstance(event, str) else event.__name__
+        self.listeners.remove([i for i in self.listeners if i["event"] == event and i["func"] == func])
+
+    def emit(self, event: t.Union[str, t.Any], data: t.Any):
+        """
+        Emit for event dont use this.
+
+        Parameters
+        ---------
+        event: :class:`str` | :class:`Any`
+            event name or class for event
+        data: :class:`function`
+            the data is revers to function callback
+        """
+        event_name = event if isinstance(event, str) else event.__name__
+        events = [i for i in self.listeners if i["event"] == event_name]
+        for event in events:
+            _LOG.debug(f"dispatch {event} for {len(events)} listeners")
+            if asyncio.iscoroutinefunction(event["func"]):
+                self._loop.create_task(event["func"](data))
+            else:
+                _LOG.error("Events only async function")
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/events.py` & `lavaplay.py-1.0.12a0/lavaplay/events.py`

 * *Files identical despite different names*

### Comparing `lavaplay.py-1.0.11a0/lavaplay/node_manager.py` & `lavaplay.py-1.0.12a0/lavaplay/node_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .objects import Stats, Track, ConnectionInfo, PlayList
 from .events import Event
 from . import __version__
 from .utlits import get_event_loop, prossing_tracks
 import logging
 from .player import Player
 
-_LOG = logging.getLogger("lavaplayer.node")
+_LOG = logging.getLogger("lavaplay.node")
 
 class Node:
     """
     Represents a Lavalink client used to manage nodes and connections.
 
     Parameters
     ---------
@@ -38,31 +38,33 @@
         host: t.Optional[str] = "127.0.0.1",
         port: int,
         password: str,
         user_id: t.Optional[int],
         resume_key: str = None, 
         resume_timeout: int = 180,
         shards_count: int = 1,
-        is_ssl: bool = False,
+        ssl: bool = False,
         loop: t.Optional[asyncio.AbstractEventLoop] = None,
         **kwargs
     ) -> None:
         self.host = host
         self.port = port
         self.password = password
         self.user_id = user_id
         self.shards_count = shards_count
-        self.is_ssl = is_ssl
+        self.ssl = ssl
         
         self.loop = loop or get_event_loop()
         self.event_manager = Emitter(self.loop)
         self._ws: t.Optional[WS] = None
+        self._resume_key = resume_key
+        self._resume_timeout = resume_timeout
 
         # Unique identifier for the client.
-        self.rest = RestApi(host=self.host, port=self.port, password=self.password, is_ssl=self.is_ssl)
+        self.rest = RestApi(host=self.host, port=self.port, password=self.password, ssl=self.ssl)
         self.stats: Stats = None
         self._voice_handlers: t.Dict[int, ConnectionInfo] = {}
 
         self.session_id: t.Optional[str] = None
 
         self.players: t.Dict[int, Player] = {}
     
@@ -71,15 +73,15 @@
         Set the event loop for the client requird set after call :meth:`connect`,
 
         Parameters
         ---------
         loop: :class:`asyncio.AbstractEventLoop`
             The event loop to use.
         """
-        asyncio.set_event_loop(loop)
+        # asyncio.set_event_loop(loop)
         self.loop = loop
         self.event_manager._loop = loop
 
     def create_player(self, guild_id: int) -> Player:
         """
         Create a player for guild id.
 
@@ -254,19 +256,19 @@
         """
         Connect to the lavalink websocket
         """
         self._ws = WS(
             node=self, 
             host=self.host, 
             port=self.port, 
-            is_ssl=self.is_ssl, 
+            ssl=self.ssl, 
             password=self.password, 
             user_id=self.user_id, 
             shards_count=self.shards_count,
         )
-        asyncio.run_coroutine_threadsafe(self._ws._connect(), self.loop)
+        asyncio.ensure_future(self._ws._connect(), loop=self.loop)
 
     async def close(self):
         """
         Disconnect from the lavalink websocket
         """
         await self._ws.ws.close()
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/objects.py` & `lavaplay.py-1.0.12a0/lavaplay/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,30 +119,29 @@
     ---------
     volume: :class:`int` | :class:`float`
         Float value where 1.0 is 100%. Values >1.0 may cause clipping
     """
     def __init__(self, volume: t.Union[int, float] = 1.0) -> None:
         self._payload: dict = {"op": "filters", "volume": volume}
     
-    def equalizer(self, bands: t.List[t.Dict[int, t.Union[float, int]]]):
+    def equalizer(self, bands: t.List[t.Tuple[int, t.Union[float, int]]]):
         """
         There are 15 bands (0-14) that can be changed.
 
         "gain" is the multiplier for the given band. The default value is 0. Valid values range from -0.25 to 1.0,
         where -0.25 means the given band is completely muted, and 0.25 means it is doubled. Modifying the gain could
         also change the volume of the output.
         """
         update_list = []
-        for x in range(0, len(bands)):
-            for key, value in bands[x].items():
-                if not -1 < key < 15:
-                    raise FiltersError("Invalid band, must be 0-14")
-                gain = max(min(float(value), 1.0), -0.25)
-                band = key
-                update_list.append({'band': band, 'gain': gain})
+        for v in bands:
+            if not -1 < v[0] < 15:
+                raise FiltersError("Invalid band, must be 0-14")
+            gain = max(min(float(v[1]), 1.0), -0.25)
+            band = v[1]
+            update_list.append({'band': band, 'gain': gain})
         self._payload["equalizer"] = update_list
     
     def karaoke(self, level: t.Union[int, float], mono_level: t.Union[int, float], filter_band: t.Union[int, float], filter_width: t.Union[int, float]):
         """
         Uses equalization to eliminate part of a band, usually targeting vocals.
         """
         self._payload["karaoke"] = {"level": level, "monoLevel": mono_level, "filterBand": filter_band, "filterWidth": filter_width}
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/player.py` & `lavaplay.py-1.0.12a0/lavaplay/player.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import typing as t
 import asyncio
 from .objects import Track, Filters, ConnectionInfo
 from .exceptions import VolumeError
 import random
+import logging
 if t.TYPE_CHECKING:
     from .node_manager import Node
 
+_LOG = logging.getLogger("lavaplay.player")
+
+
 class Player:
     def __init__(self, node: "Node", guild_id: int) -> None:
         self.guild_id = guild_id
         self.node = node
         self.rest = node.rest
         self._voice_state: t.Optional[dict] = None
         self.user_id: int = node.user_id
         self._voice_handlers: t.Dict[int, ConnectionInfo] = {}
 
         self._volume: int = 100
         self._filters: Filters = Filters()
         self.queue: t.List[Track] = []
         self.loop: asyncio.AbstractEventLoop = node.loop
+
         self._repeat = False
         self._queue_repeat = False
         self._is_connected = False
-    
+        self._ping = 0
 
     def add_to_queue(self, tracks: t.List[Track], requester: t.Optional[int] = None) -> None:
         """
         Add tracks to queue. use to load a playlist result.
 
         >>> playlist = lavaplayer.search_youtube("playlist url")
         >>> lavaplayer.add_to_queue(playlist.tracks)
@@ -35,37 +40,36 @@
         ---------
         tracks: :class:`list`
             tracks to add to queue
         """
         for track in tracks:
             self.loop.create_task(self.play(self.guild_id, track, requester))
 
-    async def play(self, track: Track, requester: t.Optional[int] = None, start: int = 0) -> None:
+    async def play(self, track: Track, requester: t.Optional[int] = None, start: bool = False) -> None:
         """
         Play track or add to the queue list.
 
         Parameters
         ---------
         requester: :class:`bool`
             user id for requester the play track
         start: :class:`bool`
             force play queue is ignored
         """
-        if len(self.queue) == 0:
+        if len(self.queue) == 0 or start:
             await self.rest.update_player(
                 session_id=self.node.session_id, 
                 guild_id=self.guild_id,
                 data={
                     "encodedTrack": track.track,
-                    "position": 0 or start, 
-                    "volume": 50
                 }
             )
-        track.requester = requester
-        self.queue.append(track)
+        if not start:
+            track.requester = requester
+            self.queue.append(track)
 
     def repeat(self, stats: bool) -> None:
         """
         Repeat the track for every.
 
         Parameters
         ---------
@@ -281,15 +285,16 @@
                 "voice": {
                     "token": token,
                     "sessionId": session_id,
                     "endpoint": endpoint.replace("wss://", "")
                 }
             }
         )
-        self._is_connected = True
+        self._is_connected = res["voice"]["connected"]
+        self._ping = res["voice"]["ping"]
 
     async def raw_voice_state_update(self, user_id: int, session_id: str, channel_id: t.Optional[int]) -> None:
         """
         A voice state update has been received from Discord.
         
         Parameters
         ---------
@@ -325,7 +330,21 @@
 
     @property
     def is_connected(self) -> bool:
         """
         Return if the player is connected to voice channel.
         """
         return self._is_connected
+
+    @property
+    def ping(self) -> int:
+        """
+        Return the ping of the player.
+        """
+        return self._ping
+    
+    @property
+    def is_playing(self) -> bool:
+        """
+        Return if the player is playing.
+        """
+        return len(self.queue) > 0
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/rest.py` & `lavaplay.py-1.0.12a0/lavaplay/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import aiohttp
 from . import routes
 import logging
 
-_LOG = logging.getLogger("lavaplayer.rest")
+_LOG = logging.getLogger("lavaplay.rest")
 
 class RestApi:
     """
     The class make a request to the rest api for lavalink.
 
     Parameters
     ---------
@@ -15,16 +15,16 @@
     port: :class:`int`
         The port to use for websocket and REST connections.
     password: :class:`str`
         The password used for authentication.
     is_ssl: :class:`bool`
         Is server using ssl.
     """
-    def __init__(self, *, host: str = "127.0.0.1", port: int, password: str, is_ssl: bool = False) -> None:
-        self.rest_uri = f"{'https' if is_ssl else 'http'}://{host}:{port}"
+    def __init__(self, *, host: str = "127.0.0.1", port: int, password: str, ssl: bool = False) -> None:
+        self.rest_uri = f"{'https' if ssl else 'http'}://{host}:{port}"
         self.headers = {
             "Host": f"{host}:{port}",
             "Authorization": password
         }
 
     async def request(self, method: str, rout: str, data: dict = {}) -> dict:
         """
@@ -43,14 +43,16 @@
         -------
         :class:`dict`
             The response from the request.
         """
         async with aiohttp.ClientSession() as session:
             async with session.request(method, self.rest_uri + rout, headers=self.headers, json=data) as response:
                 _LOG.debug(f"{method} {self.rest_uri + rout}")
+                if method == "DELETE":
+                    return
                 return await response.json()
     
     async def load_tracks(self, identifier: str) -> dict:
         """
         This function makes a request to the rest api for lavalink
 
         Parameters
@@ -197,15 +199,15 @@
         -------
         :class:`dict`
             The response from the request.
         """
         res = await self.request("GET", routes.GET_PLAYER.format(sessionId=session_id, guildId=guild_id))
         return res
     
-    async def update_player(self, session_id: str, guild_id: int, noReplace: bool = True, data: dict = {}) -> dict:
+    async def update_player(self, session_id: str, guild_id: int, noReplace: bool = False, data: dict = {}) -> dict:
         """
         This function makes a request to the rest api for lavalink
 
         Parameters
         ---------
         session_id: :class:`str`
             The session id for update player.
@@ -215,15 +217,15 @@
             The noReplace for update player.
 
         Returns
         -------
         :class:`dict`
             The response from the request.
         """
-        res = await self.request("PATCH", routes.UPDATE_PLAYER.format(sessionId=session_id, guildId=guild_id), data=data)
+        res = await self.request("PATCH", routes.UPDATE_PLAYER.format(sessionId=session_id, guildId=guild_id, noReplace="true" if noReplace else "false"), data=data)
         return res
     
     async def destroy_player(self, session_id: str, guild_id: int) -> None:
         """
         This function makes a request to the rest api for lavalink
 
         Parameters
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/routes.py` & `lavaplay.py-1.0.12a0/lavaplay/routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 GET_PLAYERS = "/v3/sessions/{sessionId}/players"  # GET
 GET_PLAYER = "/v3/sessions/{sessionId}/players/{guildId}"  # GET
-UPDATE_PLAYER = "/v3/sessions/{sessionId}/players/{guildId}"  # PATCH
+UPDATE_PLAYER = "/v3/sessions/{sessionId}/players/{guildId}?noReplace={noReplace}"  # PATCH
 """Whether to replace the current track with the new track. Defaults to `false`"""
 DESTROY_PLAYER = "/v3/sessions/{sessionId}/players/{guildId}"  # DELETE
 UPDATE_SESSION = "/v3/sessions/{sessionId}"  # PATCH
 TRACK_LOADING = "/loadtracks?identifier={identifier}"  # GET
 TRACK_DECODEING = "/decodetrack?encodedTrack={encodedTrack}"  # GET
 TRACKS_DECODEING = "/decodetracks"  # POST
 INFO = "/v3/info"  # GET
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/utlits.py` & `lavaplay.py-1.0.12a0/lavaplay/utlits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import random
 import asyncio
 import typing as t
 from .objects import Track
 
-
-
 def generate_resume_key():
     return "".join(random.choice("0123456789abcdef") for _ in range(16))
 
 
 def get_event_loop() -> asyncio.AbstractEventLoop:
     try:
         loop = asyncio.get_running_loop()
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay/ws.py` & `lavaplay.py-1.0.12a0/lavaplay/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,42 +13,42 @@
 )
 from .emitter import Emitter
 import typing as t
 from . import __version__
 if t.TYPE_CHECKING:
     from .node_manager import Node
 
-_LOG = logging.getLogger("lavaplayer.ws")
+_LOG = logging.getLogger("lavaplay.ws")
 
 class WS:
     def __init__(
         self,
         node: "Node",
         host: str,
         port: int,
-        is_ssl: bool = False,
+        ssl: bool = False,
         password: str = None,
         user_id: int = None,
         shards_count: int = None,
         resume_key: t.Optional[str] = None,
         loop: t.Optional[asyncio.AbstractEventLoop] = None,
     ) -> None:
         self.ws = None
-        self.ws_url = f"{'wss' if is_ssl else 'ws'}://{host}:{port}/v3/websocket"
+        self.ws_url = f"{'wss' if ssl else 'ws'}://{host}:{port}/v3/websocket"
         self.node = node
         self._headers = {
             "Authorization": password,
             "User-Id": str(user_id),
-            "Client-Name": f"Lavaplayer-py/{__version__}",
+            "Client-Name": f"Lavaplay.py/{__version__}",
             "Num-Shards": str(shards_count)
         }
         self._loop = loop or node.loop
         self.emitter: Emitter = node.event_manager
         self.is_connect: bool = False
-        self.resume_key = resume_key
+        self.resume_key = resume_key or self.node._resume_key or generate_resume_key()
         self._session_id: str = None
     
     @property
     def session_id(self) -> str:
         return self._session_id
 
     async def _connect(self):
@@ -71,21 +71,14 @@
                 elif isinstance(error, aiohttp.WSServerHandshakeError):
                     if error.status in (403, 401):  # Unauthorized or Forbidden
                         _LOG.warning("Password authentication failed - closing websocket")
                         return
                     _LOG.warning("Please check your websocket port - closing websocket")
             self.is_connect = True
 
-            # self.resume_key = generate_resume_key()
-            # await self.send({
-            #     "op": "configureResuming",
-            #     "key": self.resume_key,
-            #     "timeout": 60
-            # })
-
             async for msg in self.ws:
                 if msg.type == aiohttp.WSMsgType.TEXT:
                     self._loop.create_task(self.callback(msg.json()))
                 elif msg.type in (aiohttp.WSMsgType.CLOSE, aiohttp.WSMsgType.CLOSING, aiohttp.WSMsgType.CLOSED):
                     _LOG.error("Websocket closed")
                     break
                 elif msg.type == aiohttp.WSMsgType.ERROR:
@@ -102,14 +95,23 @@
 
     async def callback(self, payload: dict):
         # https://github.com/freyacodes/Lavalink/blob/master/IMPLEMENTATION.md#ready-op
         if payload["op"] == "ready":
             _LOG.info("Lavalink client is ready")
             self._session_id = payload["sessionId"]
             self.node.session_id = self._session_id
+            await self.node.rest.update_session(
+                self._session_id,
+                data={
+                    "resumingKey": self.resume_key,
+                    "timeout": self.node._resume_timeout or 180
+                }
+            )
+            if payload["resumed"] is True:
+                _LOG.info("Lavalink client resumed session successfully")
             self.emitter.emit("ready", data=ReadyEvent.from_kwargs(**payload))
         
         # https://github.com/freyacodes/Lavalink/blob/master/IMPLEMENTATION.md#player-update-op
         elif payload["op"] == "playerUpdate":
             payload.pop("op")
             guild_id = int(payload["guildId"])
             player = self.node.get_player(guild_id)
@@ -165,15 +167,15 @@
                 if len(player.queue) == 0:
                     return
                 await player.play(player.queue[0], player.queue[0].requester, True)
                 return
             if player._repeat:
                 await player.play(track, player.queue[0].requester, True)
                 return
-            del player.queue[0]
+            player.queue.pop(0)
             if len(player.queue) != 0:
                 await player.play(player.queue[0], player.queue[0].requester, True)
 
         elif event == "TrackExceptionEvent":
             payload["exception"] = TrackException.from_kwargs(**payload["exception"])
             self.emitter.emit("TrackExceptionEvent", TrackExceptionEvent.from_kwargs(**payload))
```

### Comparing `lavaplay.py-1.0.11a0/lavaplay.py.egg-info/PKG-INFO` & `lavaplay.py-1.0.12a0/lavaplay.py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavaplay.py
-Version: 1.0.11a0
+Version: 1.0.12a0
 Summary: Its a lavalink nodes manger to make a music bots for discord with python.
 Home-page: https://github.com/HazemMeqdad/lavaplay.py
 Author: HazemMeqdad
 Author-email: hazemmeqdad@outlook.com
 Project-URL: Bug Reports, https://github.com/HazemMeqdad/lavaplay.py/issues
 Project-URL: Source, https://github.com/HazemMeqdad/lavaplay.py/
 Project-URL: Documentation, https://lavaplay.readthedocs.io/en/latest
@@ -63,40 +63,44 @@
     port=2333,
     password="youshallnotpass",
     user_id=123
 )
 
 @bot.listen()
 async def on_ready(event: hikari.ShardReadyEvent) -> None:
-    await node.connect()
+    node.connect()
 
 bot.run()
 ```
 
 examples for some methods.
 ```python
+# Player object
+player = node.get_player(guild_id)
+
 # Auto search mix with track or query
-await lavalink.auto_search_tracks("Rick Astley")
+await player.auto_search_tracks("Rick Astley")
 
 # Play track
-await lavalink.play(guild_id, track)
+await player.play(track)
 
 # Skip
-await lavalink.skip(guild_id)
+await player.skip()
 
 # Pause
-await lavalink.pause(guild_id, stats)
+await player.pause(stats)
 
 # Volume
-await lavalink.volume(guild_id, volume)
+await player.volume(volume)
 ```
 
 # Features
 
 - [ ] Spotify support
+- [x] new Rest api for lavalink support
 - [x] connection handler
 - [x] Support youtube playlist
 - [x] Add example for other discord wrapper library
 
 # Installation
 
 ```shell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lavaplay.py Version: 1.0.11a0 Summary: Its a
+Metadata-Version: 2.1 Name: lavaplay.py Version: 1.0.12a0 Summary: Its a
 lavalink nodes manger to make a music bots for discord with python. Home-page:
 https://github.com/HazemMeqdad/lavaplay.py Author: HazemMeqdad Author-email:
 hazemmeqdad@outlook.com Project-URL: Bug Reports, https://github.com/
 HazemMeqdad/lavaplay.py/issues Project-URL: Source, https://github.com/
 HazemMeqdad/lavaplay.py/ Project-URL: Documentation, https://
 lavaplay.readthedocs.io/en/latest Keywords: lavalink,discord,discord-
 lavalink,lavaplay,lavaplay.py Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,16 @@
 About lavaplay.py is a nodes manager to connection with discord voice gateway,
 easy to create a music bot, you can use to anything async discord wrapper
 library # Usage example for create connecting with lavalink server using
 [hikari](https://github.com/hikari-py/hikari). ```python import hikari import
 lavaplay bot = hikari.GatewayBot("token") lavalink = lavaplay.Lavalink() node =
 lavalink.create_node( host="localhost", port=2333, password="youshallnotpass",
 user_id=123 ) @bot.listen() async def on_ready(event: hikari.ShardReadyEvent) -
-> None: await node.connect() bot.run() ``` examples for some methods. ```python
-# Auto search mix with track or query await lavalink.auto_search_tracks("Rick
-Astley") # Play track await lavalink.play(guild_id, track) # Skip await
-lavalink.skip(guild_id) # Pause await lavalink.pause(guild_id, stats) # Volume
-await lavalink.volume(guild_id, volume) ``` # Features - [ ] Spotify support -
-[x] connection handler - [x] Support youtube playlist - [x] Add example for
-other discord wrapper library # Installation ```shell # Linux/OS X $ pip3
-install -U lavaplay.py # Windows $ pip install -U lavaplay.py ```
+> None: node.connect() bot.run() ``` examples for some methods. ```python #
+Player object player = node.get_player(guild_id) # Auto search mix with track
+or query await player.auto_search_tracks("Rick Astley") # Play track await
+player.play(track) # Skip await player.skip() # Pause await player.pause(stats)
+# Volume await player.volume(volume) ``` # Features - [ ] Spotify support - [x]
+new Rest api for lavalink support - [x] connection handler - [x] Support
+youtube playlist - [x] Add example for other discord wrapper library #
+Installation ```shell # Linux/OS X $ pip3 install -U lavaplay.py # Windows $
+pip install -U lavaplay.py ```
```

### Comparing `lavaplay.py-1.0.11a0/setup.py` & `lavaplay.py-1.0.12a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='lavaplay.py',
-    version='1.0.11a',
+    version='1.0.12a',
     description='Its a lavalink nodes manger to make a music bots for discord with python.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/HazemMeqdad/lavaplay.py',
     author='HazemMeqdad',
     author_email='hazemmeqdad@outlook.com',
     classifiers=[
```


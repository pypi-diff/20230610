# Comparing `tmp/nextguild-1.1.7.tar.gz` & `tmp/nextguild-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.1.7.tar", last modified: Thu Jun  8 18:03:44 2023, max compression
+gzip compressed data, was "nextguild-1.2.0.tar", last modified: Sat Jun 10 21:34:25 2023, max compression
```

## Comparing `nextguild-1.1.7.tar` & `nextguild-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:03:44.568209 nextguild-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 18:03:31.000000 nextguild-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-08 18:03:44.568209 nextguild-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-08 18:03:31.000000 nextguild-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:03:44.568209 nextguild-1.1.7/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    41069 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/reaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:03:44.568209 nextguild-1.1.7/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-08 18:03:31.000000 nextguild-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:03:44.568209 nextguild-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:34:25.306409 nextguild-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 21:34:13.000000 nextguild-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 21:34:25.306409 nextguild-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-10 21:34:13.000000 nextguild-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:34:25.306409 nextguild-1.2.0/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-10 21:34:13.000000 nextguild-1.2.0/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-06-10 21:34:13.000000 nextguild-1.2.0/nextguild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41038 2023-06-10 21:34:13.000000 nextguild-1.2.0/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-10 21:34:13.000000 nextguild-1.2.0/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48069 2023-06-10 21:34:13.000000 nextguild-1.2.0/nextguild/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:34:25.306409 nextguild-1.2.0/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 21:34:25.000000 nextguild-1.2.0/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 21:34:25.000000 nextguild-1.2.0/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 21:34:25.000000 nextguild-1.2.0/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 21:34:25.000000 nextguild-1.2.0/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 21:34:13.000000 nextguild-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 21:34:25.306409 nextguild-1.2.0/setup.cfg
```

### Comparing `nextguild-1.1.7/LICENSE` & `nextguild-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.7/PKG-INFO` & `nextguild-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.7
+Version: 1.2.0
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,14 +56,19 @@
 pip install nextguild
 ```
 
 ## Documentation
 
 For NextGuild's official documentation, click [this link](https://github.com/ArjunSharda/nextguild/tree/main/docs)
 
+## Founders
+
+[Arjun Sharda](https://github.com/ArjunSharda)<br>
+[Erik Thorsell](https://github.com/erik-thorsell)
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 ## License
```

### Comparing `nextguild-1.1.7/README.md` & `nextguild-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 pip install nextguild
 ```
 
 ## Documentation
 
 For NextGuild's official documentation, click [this link](https://github.com/ArjunSharda/nextguild/tree/main/docs)
 
+## Founders
+
+[Arjun Sharda](https://github.com/ArjunSharda)<br>
+[Erik Thorsell](https://github.com/erik-thorsell)
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 ## License
```

### Comparing `nextguild-1.1.7/nextguild/client.py` & `nextguild-1.2.0/nextguild/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import time
 from datetime import datetime
 
 import requests
 
 from .embed import Embed
-from .message import Message
+from .classes import Data
 
 
 class Client:
     def __init__(self, token: str) -> None:
         self.token = token
         self.headers = {
             'Authorization': f'Bearer {self.token}',
@@ -52,15 +52,15 @@
             payload['embeds'] = [embed.to_dict]
 
         response = self.request(
             method='POST',
             url=f'{self.base_url}/channels/{channel_id}/messages',
             json=payload
         )
-        return Message(response)
+        return Data(response)
 
     def edit_message(
             self,
             channel_id: str,
             message_id: str,
             content: str = None,
             *,
@@ -77,15 +77,15 @@
             payload['embeds'] = [embed.to_dict]
 
         response = self.request(
             'PUT',
             f'{self.base_url}/channels/{channel_id}/messages/{message_id}',
             json=payload
         )
-        return Message(response)
+        return Data()
 
     def delete_message(
             self,
             channel_id: str,
             message_id: str
     ):
         response = self.request(
@@ -101,15 +101,15 @@
     ):
         """Docs: https://www.guilded.gg/docs/api/chat/ChannelMessageRead
         """
         response = self.request(
             'GET',
             f'{self.base_url}/channels/{channel_id}/messages/{message_id}'
         )
-        return Message(response)
+        return Data()
 
     def get_channel_messages(
             self,
             channel_id,
             limit=None,
             before=None,
             after=None,
@@ -133,15 +133,15 @@
 
         response = self.request(
             'GET',
             f'{self.base_url}/channels/{channel_id}/messages',
             params=params
         )
         return list(map(
-            lambda msg: Message(msg),
+            lambda msg: Data(msg),
             response.get('messages', [])
         ))
 
     def purge(
             self,
             channel_id: str,
             amount: int
```

### Comparing `nextguild-1.1.7/nextguild/embed.py` & `nextguild-1.2.0/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.7/nextguild/events.py` & `nextguild-1.2.0/nextguild/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import json
 from functools import wraps
 
 import websockets
 
-from .channel import Channel
-from .message import Message, Webhook
-from .reaction import Reaction, CalendarReaction, ForumTopicCommentReaction
+from .classes import Data
 
 
 class Events:
     def __init__(self, client):
         self._message_create_handlers = []
         self._message_update_handlers = []
         self._message_delete_handlers = []
@@ -90,14 +88,22 @@
         self._announcement_reaction_create_handlers = []
         self._announcement_reaction_delete_handlers = []
         self._announcement_comment_create_handlers = []
         self._announcement_comment_update_handlers = []
         self._announcement_comment_delete_handlers = []
         self._announcement_comment_reaction_create_handlers = []
         self._announcement_comment_reaction_delete_handlers = []
+        self._group_create_handlers = []
+        self._group_update_handlers = []
+        self._group_delete_handlers = []
+        self.on_user_status_create_handlers = []
+        self.on_user_status_delete_handlers = []
+        self.on_role_create_handlers = []
+        self.on_role_update_handlers = []
+        self.on_role_delete_handlers = []
         self.client = client
     
     def on_bot_membership_created(self, func):
         @wraps(func)
         def wrapper(server):
             return func(server)
 
@@ -108,23 +114,23 @@
         @wraps(func)
         def wrapper(server):
             return func(server)
 
         self._bot_server_leave_handlers.append(wrapper)
         return wrapper
     
-    def on_member_update(self, func):
+    def on_member_updated(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._member_update_handlers.append(wrapper)
         return wrapper
     
-    def on_roles_update(self, func):
+    def on_roles_updated(self, func):
         @wraps(func)
         def wrapper(member):
             return func(member)
 
         self._roles_update_handlers.append(wrapper)
         return wrapper
     
@@ -734,355 +740,518 @@
         @wraps(func)
         def wrapper(event):
             return func(event)
 
         self._announcement_comment_reaction_delete_handlers.append(wrapper)
         return wrapper
     
+    def on_group_create(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._group_create_handlers.append(wrapper)
+        return wrapper
+    
+    def on_group_update(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._group_update_handlers.append(wrapper)
+        return wrapper
+    
+    def on_group_delete(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._group_delete_handlers.append(wrapper)
+        return wrapper
+    
+    def on_user_status_create(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._user_status_create_handlers.append(wrapper)
+        return wrapper
+    
+    def on_user_status_delete(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._user_status_delete_handlers.append(wrapper)
+        return wrapper
+    
+    def on_role_create(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._role_create_handlers.append(wrapper)
+        return wrapper
+    
+    def on_role_update(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._role_update_handlers.append(wrapper)
+        return wrapper
+    
+    def on_role_delete(self, func):
+        @wraps(func)
+        def wrapper(event):
+            return func(event)
+
+        self._role_delete_handlers.append(wrapper)
+        return wrapper
+    
 
 
     async def _handle_bot_server_membership_created(self, event_data):
+        event = Data(event_data)
         for handler in self._bot_server_join_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_bot_server_membership_deleted(self, event_data):
-        # TODO: server class
+        event = Data(event_data)
         for handler in self._bot_server_leave_handlers:
-            await handler(event_data)
+            await handler(event)
         
     async def _handle_server_member_updated(self, event_data):
-        # TODO: member class
+        event = Data(event_data)
         for handler in self._member_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_server_roles_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._roles_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_server_member_social_links_created(self, event_data):
+        event = Data(event_data)
         for handler in self._member_social_create_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_server_member_social_links_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._member_social_update_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_server_member_social_links_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._member_social_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_doc_created(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_create_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_doc_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_update_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_doc_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_doc_comment_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_comment_update_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_doc_comment_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_comment_delete_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_doc_comment_created(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_comment_create_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_calendar_event_created(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_create_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_calendar_event_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_update_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_calendar_event_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_delete_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_forum_topic_created(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_create_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_forum_topic_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_update_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_forum_topic_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_server_member_banned(self, event_data):
-        # TODO: member class
+        event = Data(event_data)
         for handler in self._member_banned_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_create_message(self, event_data):
-        message = Message(event_data)
+        event = Data(event_data)
         for handler in self._message_create_handlers:
-            await handler(message)
+            await handler(event)
 
     async def _handle_update_message(self, event_data):
-        message = Message(event_data)
+        event = Data(event_data)
         for handler in self._message_update_handlers:
-            await handler(message)
+            await handler(event)
 
     async def _handle_delete_message(self, event_data):
-        message = Message(event_data)
+        event = Data(event_data)
         for handler in self._message_delete_handlers:
-            await handler(message)
+            await handler(event)
 
     async def _handle_member_join(self, event_data):
+        event = Data(event_data)
         for handler in self._member_join_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_member_leave(self, event_data):
+        event = Data(event_data)
         for handler in self._member_leave_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_member_banned(self, event_data):
+        event = Data(event_data)
         for handler in self._member_banned_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_member_unbanned(self, event_data):
+        event = Data(event_data)
         for handler in self._member_unbanned_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_ready(self):
         for handler in self._ready_handlers:
             await handler()
 
     async def _handle_create_reaction(self, event_data):
-        reaction = Reaction(event_data)
+        event = Data(event_data)
         for handler in self._reaction_create_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_delete_reaction(self, event_data):
-        reaction = Reaction(event_data)
+        event = Data(event_data)
         for handler in self._reaction_delete_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_forum_topic_comment_reaction_create(self, event_data):
-        reaction = ForumTopicCommentReaction(event_data)
+        event = Data(event_data)
         for handler in self._forum_topic_comment_reaction_create_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_forum_topic_comment_reaction_delete(self, event_data):
-        reaction = ForumTopicCommentReaction(event_data)
+        event = Data(event_data)
         for handler in self._forum_topic_comment_reaction_delete_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_calendar_event_reaction_create(self, event_data):
-        reaction = CalendarReaction(event_data)
+        event = Data(event_data)
         for handler in self._calendar_event_reaction_create_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_calendar_event_reaction_delete(self, event_data):
-        reaction = CalendarReaction(event_data)
+        event = Data(event_data)
         for handler in self._calendar_event_reaction_delete_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_create_channel(self, event_data):
-        channel = Channel(event_data)
+        event = Data(event_data)
         for handler in self._channel_create_handlers:
-            await handler(channel)
+            await handler(event)
 
     async def _handle_delete_channel(self, event_data):
-        channel = Channel(event_data)
+        event = Data(event_data)
         for handler in self._channel_delete_handlers:
-            await handler(channel)
+            await handler(event)
     
     async def _handle_update_channel(self, event_data):
-        channel = Channel(event_data)
+        event = Data(event_data)
         for handler in self._channel_update_handlers:
-            await handler(channel)
+            await handler(event)
     
     async def _handle_create_webhook(self, event_data):
-        webhook = Webhook(event_data)
+        event = Data(event_data)
         for handler in self._webhook_create_handlers:
-            await handler(webhook)
+            await handler(event)
 
     async def _handle_update_webhook(self, event_data):
-        webhook = Webhook(event_data)
+        event = Data(event_data)
         for handler in self._webhook_update_handlers:
-            await handler(webhook)
+            await handler(event)
 
     async def _handle_forum_topic_pinned(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_pinned_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_forum_topic_unpinned(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_unpinned_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_forum_topic_reaction_created(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_reaction_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_forum_topic_reaction_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_reaction_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_forum_topic_locked(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_lock_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_forum_topic_unlocked(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_unlock_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_forum_topic_comment_created(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_comment_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_forum_topic_comment_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_comment_update_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_forum_topic_comment_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._forum_topic_comment_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_rsvp_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_rsvp_update_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_calendar_event_rsvp_many_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_rsvp_many_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_rsvp_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_rsvp_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_list_item_created(self, event_data):
+        event = Data(event_data)
         for handler in self._list_item_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_list_item_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._list_item_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_list_item_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._list_item_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_list_item_completed(self, event_data):
+        event = Data(event_data)
         for handler in self._list_item_complete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_list_item_uncompleted(self, event_data):
+        event = Data(event_data)
         for handler in self._list_item_uncomplete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_channel_message_reaction_created(self, event_data):
-        reaction = Reaction(event_data)
+        event = Data(event_data)
         for handler in self._channel_message_reaction_create_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_channel_message_reaction_deleted(self, event_data):
-        reaction = Reaction(event_data)
+        event = Data(event_data)
         for handler in self._channel_message_reaction_delete_handlers:
-            await handler(reaction)
+            await handler(event)
 
     async def _handle_channel_message_reaction_many_deleted(self, event_data):
-        reaction = Reaction(event_data)
+        event = Data(event_data)
         for handler in self._channel_message_reaction_many_delete_handlers:
-            await handler(reaction)
+            await handler(event)
     
     async def _handle_calendar_event_comment_created(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_comment_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_comment_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_comment_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_comment_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_comment_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_comment_reaction_created(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_comment_reaction_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_comment_reaction_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_comment_reaction_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_doc_reaction_created(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_reaction_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_doc_reaction_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_reaction_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_doc_comment_reaction_created(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_comment_reaction_create_handlers:
-            await handler(event_data)
+            await handler(event)
     
     async def _handle_doc_comment_reaction_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._doc_comment_reaction_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_series_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_series_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_calendar_event_series_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._calendar_event_series_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_created(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_reaction_created(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_reaction_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_reaction_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_reaction_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_comment_created(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_comment_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_comment_updated(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_comment_update_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_comment_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_comment_delete_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_comment_reaction_created(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_comment_reaction_create_handlers:
-            await handler(event_data)
+            await handler(event)
 
     async def _handle_announcement_comment_reaction_deleted(self, event_data):
+        event = Data(event_data)
         for handler in self._announcement_comment_reaction_delete_handlers:
-            await handler(event_data)
+            await handler(event)
+
+    async def _handle_group_created(self, event_data):
+        event = Data(event_data)
+        for handler in self._group_create_handlers:
+            await handler(event)
+
+    async def _handle_group_updated(self, event_data):
+        event = Data(event_data)
+        for handler in self._group_update_handlers:
+            await handler(event)
+
+    async def _handle_group_deleted(self, event_data):
+        event = Data(event_data)
+        for handler in self._group_delete_handlers:
+            await handler(event)
+    
+    async def _handle_user_status_created(self, event_data):
+        event = Data(event_data)
+        for handler in self._user_status_create_handlers:
+            await handler(event)
+
+    async def _handle_user_status_deleted(self, event_data):
+        event = Data(event_data)
+        for handler in self._user_status_delete_handlers:
+            await handler(event)
+
+    async def _handle_role_created(self, event_data):
+        event = Data(event_data)
+        for handler in self._role_create_handlers:
+            await handler(event)
+
+    async def _handle_role_updated(self, event_data):
+        event = Data(event_data)
+        for handler in self._role_update_handlers:
+            await handler(event)
+
+    async def _handle_role_deleted(self, event_data):
+        event = Data(event_data)
+        for handler in self._role_delete_handlers:
+            await handler(event)
 
     async def start(self):
         async with websockets.connect(
                 'wss://www.guilded.gg/websocket/v1',
                 extra_headers={
                     'Authorization': f'Bearer {self.client.token}'
                 }
@@ -1172,14 +1341,22 @@
                     'AnnouncementReactionCreated': self._handle_announcement_reaction_created,
                     'AnnouncementReactionDeleted': self._handle_announcement_reaction_deleted,
                     'AnnouncementCommentCreated': self._handle_announcement_comment_created,
                     'AnnouncementCommentUpdated': self._handle_announcement_comment_updated,
                     'AnnouncementCommentDeleted': self._handle_announcement_comment_deleted,
                     'AnnouncementCommentReactionCreated': self._handle_announcement_comment_reaction_created,
                     'AnnouncementCommentReactionDeleted': self._handle_announcement_comment_reaction_deleted,
+                    'GroupCreated': self._handle_group_created,
+                    'GroupUpdated': self._handle_group_updated,
+                    'GroupDeleted': self._handle_group_deleted,
+                    'UserStatusCreated': self._handle_user_status_created,
+                    'UserStatusDeleted': self._handle_user_status_deleted,
+                    'RoleCreated': self._handle_role_created,
+                    'RoleUpdated': self._handle_role_updated,
+                    'RoleDeleted': self._handle_role_deleted,
 
 
                 }
                 handler = event_handlers.get(event_type)
                 if handler:
                     await handler(event_data)
```

### Comparing `nextguild-1.1.7/nextguild.egg-info/PKG-INFO` & `nextguild-1.2.0/nextguild.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.7
+Version: 1.2.0
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,14 +56,19 @@
 pip install nextguild
 ```
 
 ## Documentation
 
 For NextGuild's official documentation, click [this link](https://github.com/ArjunSharda/nextguild/tree/main/docs)
 
+## Founders
+
+[Arjun Sharda](https://github.com/ArjunSharda)<br>
+[Erik Thorsell](https://github.com/erik-thorsell)
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 ## License
```

### Comparing `nextguild-1.1.7/pyproject.toml` & `nextguild-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.1.7"
+version = "1.2.0"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```


# Comparing `tmp/multibot-1.9.2.tar.gz` & `tmp/multibot-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multibot-1.9.2.tar", last modified: Sat May 20 04:32:50 2023, max compression
+gzip compressed data, was "multibot-1.9.3.tar", last modified: Sat Jun 10 03:39:18 2023, max compression
```

## Comparing `multibot-1.9.2.tar` & `multibot-1.9.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 04:32:36.000000 multibot-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-20 04:32:50.096953 multibot-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-05-20 04:32:36.000000 multibot-1.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.092953 multibot-1.9.2/multibot/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/multibot/bots/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/discord_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    41554 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/multi_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26591 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/telegram_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/twitch_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/multibot/models/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/event_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/registered_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/multibot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-20 04:32:36.000000 multibot-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-20 04:32:50.096953 multibot-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:39:18.464932 multibot-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-10 03:39:00.000000 multibot-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-10 03:39:18.464932 multibot-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-06-10 03:39:00.000000 multibot-1.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:39:18.460932 multibot-1.9.3/multibot/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:39:18.464932 multibot-1.9.3/multibot/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28825 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/bots/discord_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41554 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/bots/multi_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26591 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/bots/telegram_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/bots/twitch_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:39:18.464932 multibot-1.9.3/multibot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/event_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/registered_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-10 03:39:00.000000 multibot-1.9.3/multibot/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:39:18.460932 multibot-1.9.3/multibot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-10 03:39:18.000000 multibot-1.9.3/multibot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-10 03:39:18.000000 multibot-1.9.3/multibot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:39:18.000000 multibot-1.9.3/multibot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-10 03:39:18.000000 multibot-1.9.3/multibot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 03:39:18.000000 multibot-1.9.3/multibot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-10 03:39:00.000000 multibot-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-10 03:39:18.468932 multibot-1.9.3/setup.cfg
```

### Comparing `multibot-1.9.2/LICENSE` & `multibot-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/PKG-INFO` & `multibot-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multibot
-Version: 1.9.2
+Version: 1.9.3
 Summary: Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 Home-page: https://github.com/AlberLC/multibot
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/multibot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multibot-1.9.2/README.rst` & `multibot-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/bots/discord_bot.py` & `multibot-1.9.3/multibot/bots/discord_bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,31 +602,31 @@
                 error_message = f'El archivo pesa más de {constants.DISCORD_MEDIA_MAX_BYTES // 1000000} MB.'
             else:
                 error_message = 'El archivo pesa mas que tu madre'
             await self._manage_exceptions(SendError(error_message), chat)
 
         text = self._parse_html_to_discord_markdown(text)
         if (
-                media
-                and
-                media.url
-                and
-                media.type_ is MediaType.GIF
-                and
-                any(domain.lower() in media.url for domain in constants.GIF_DOMAINS)
+            media
+            and
+            media.url
+            and
+            media.type_ is MediaType.GIF
+            and
+            any(domain.lower() in media.url for domain in constants.GIF_DOMAINS)
         ):
             text = f'{text} {media.url}' if text else media.url
             file = None
         else:
             try:
                 file = await self._prepare_media_to_send(media)
             except LimitError:
                 await file_too_large()
                 return
-            if not text and not file:
+            if not any((text, file, buttons, edit)):
                 return
 
         view = None
         if buttons:
             view = discord.ui.View(timeout=None)
             for i, row in enumerate(buttons):
                 for button in row:
```

### Comparing `multibot-1.9.2/multibot/bots/multi_bot.py` & `multibot-1.9.3/multibot/bots/multi_bot.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/bots/telegram_bot.py` & `multibot-1.9.3/multibot/bots/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/bots/twitch_bot.py` & `multibot-1.9.3/multibot/bots/twitch_bot.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/constants.py` & `multibot-1.9.3/multibot/constants.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/models/buttons.py` & `multibot-1.9.3/multibot/models/buttons.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,8 @@
         return [button for row in self.buttons for button in row if button.is_checked]
 
     def find_button(self, text: str) -> Button:
         return self[text]
 
     @property
     def pressed_button(self) -> Button | None:
-        return self.find_button(self.pressed_text)
+        return self[self.pressed_text]
```

### Comparing `multibot-1.9.2/multibot/models/chat.py` & `multibot-1.9.3/multibot/models/chat.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/models/event_component.py` & `multibot-1.9.3/multibot/models/event_component.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/models/message.py` & `multibot-1.9.3/multibot/models/message.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/models/penalties.py` & `multibot-1.9.3/multibot/models/penalties.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/models/registered_callback.py` & `multibot-1.9.3/multibot/models/registered_callback.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot/models/user.py` & `multibot-1.9.3/multibot/models/user.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/multibot.egg-info/PKG-INFO` & `multibot-1.9.3/multibot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multibot
-Version: 1.9.2
+Version: 1.9.3
 Summary: Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 Home-page: https://github.com/AlberLC/multibot
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/multibot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multibot-1.9.2/multibot.egg-info/SOURCES.txt` & `multibot-1.9.3/multibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multibot-1.9.2/setup.cfg` & `multibot-1.9.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multibot
-version = v1.9.2
+version = v1.9.3
 author = AlberLC
 description = Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 long_description = file: README.rst
 url = https://github.com/AlberLC/multibot
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/multibot/issues
 classifiers =
```


# Comparing `tmp/chrono_chatgpt-0.2.tar.gz` & `tmp/chrono_chatgpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrono_chatgpt-0.2.tar", last modified: Fri Jun  9 16:09:07 2023, max compression
+gzip compressed data, was "chrono_chatgpt-0.2.1.tar", last modified: Sat Jun 10 00:12:22 2023, max compression
```

## Comparing `chrono_chatgpt-0.2.tar` & `chrono_chatgpt-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 16:09:07.873323 chrono_chatgpt-0.2/
--rw-rw-rw-   0        0        0      226 2023-06-09 16:09:07.873323 chrono_chatgpt-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-09 06:11:46.000000 chrono_chatgpt-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 16:09:07.858323 chrono_chatgpt-0.2/chrono_chatgpt/
--rw-rw-rw-   0        0        0        0 2023-03-24 04:29:09.000000 chrono_chatgpt-0.2/chrono_chatgpt/__init__.py
--rw-rw-rw-   0        0        0      419 2023-03-24 21:07:32.000000 chrono_chatgpt-0.2/chrono_chatgpt/bot_initializer.py
--rw-rw-rw-   0        0        0     4094 2023-06-09 16:05:40.000000 chrono_chatgpt-0.2/chrono_chatgpt/chatbot_core.py
--rw-rw-rw-   0        0        0     3319 2023-03-24 21:07:27.000000 chrono_chatgpt-0.2/chrono_chatgpt/internet_module.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:42:11.000000 chrono_chatgpt-0.2/chrono_chatgpt/version0.1.1.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:09:07.871326 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/
--rw-rw-rw-   0        0        0      226 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-09 16:09:07.000000 chrono_chatgpt-0.2/chrono_chatgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 16:09:07.873323 chrono_chatgpt-0.2/setup.cfg
--rw-rw-rw-   0        0        0      504 2023-06-09 16:07:22.000000 chrono_chatgpt-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 00:12:22.125764 chrono_chatgpt-0.2.1/
+-rw-rw-rw-   0        0        0      228 2023-06-10 00:12:22.125764 chrono_chatgpt-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:11:46.000000 chrono_chatgpt-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 00:12:22.109765 chrono_chatgpt-0.2.1/chrono_chatgpt/
+-rw-rw-rw-   0        0        0        0 2023-03-24 04:29:09.000000 chrono_chatgpt-0.2.1/chrono_chatgpt/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-03-24 21:07:32.000000 chrono_chatgpt-0.2.1/chrono_chatgpt/bot_initializer.py
+-rw-rw-rw-   0        0        0     4119 2023-06-10 00:11:09.000000 chrono_chatgpt-0.2.1/chrono_chatgpt/chatbot_core.py
+-rw-rw-rw-   0        0        0     3319 2023-03-24 21:07:27.000000 chrono_chatgpt-0.2.1/chrono_chatgpt/internet_module.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:42:11.000000 chrono_chatgpt-0.2.1/chrono_chatgpt/version0.1.1.py
+drwxrwxrwx   0        0        0        0 2023-06-10 00:12:22.124765 chrono_chatgpt-0.2.1/chrono_chatgpt.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-06-10 00:12:21.000000 chrono_chatgpt-0.2.1/chrono_chatgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-10 00:12:22.000000 chrono_chatgpt-0.2.1/chrono_chatgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 00:12:21.000000 chrono_chatgpt-0.2.1/chrono_chatgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-10 00:12:21.000000 chrono_chatgpt-0.2.1/chrono_chatgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 00:12:22.125764 chrono_chatgpt-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      506 2023-06-10 00:11:43.000000 chrono_chatgpt-0.2.1/setup.py
```

### Comparing `chrono_chatgpt-0.2/chrono_chatgpt/chatbot_core.py` & `chrono_chatgpt-0.2.1/chrono_chatgpt/chatbot_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from chrono_chatgpt.internet_module import InternetModule
 import settings.setting_loader as setting_loader
 import chrono_chatgpt.bot_initializer as bot_initializer
 import logging
-
+import os
 
 class ChatBotCore:
     def __init__(self):
         bot_settings = setting_loader.load()
         self.bot = bot_initializer.initialize(bot_settings)
         self.chatbot = self.bot
         #self.mode_path = "C:\\Users\\Terre\\Development\\_Experiments\\ChatGPT\\src\\revChatGPT\\config\\modes.json"
-        self.mode_path = "settings\\modes.json"
+        self.mode_path = os.path.join('settings', 'modes.json')
         self.internet_module = InternetModule(self.bot)
         self.prompt_wrapper = lambda s: s
 
         self.internet_enabled = False
         self.is_internet_config_loaded = False
 
     def load_process_file_config(self):
```

### Comparing `chrono_chatgpt-0.2/chrono_chatgpt/internet_module.py` & `chrono_chatgpt-0.2.1/chrono_chatgpt/internet_module.py`

 * *Files identical despite different names*


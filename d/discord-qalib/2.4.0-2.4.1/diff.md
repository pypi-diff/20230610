# Comparing `tmp/discord-qalib-2.4.0.tar.gz` & `tmp/discord-qalib-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.4.0.tar", last modified: Sat Jun 10 16:54:32 2023, max compression
+gzip compressed data, was "discord-qalib-2.4.1.tar", last modified: Sat Jun 10 19:57:52 2023, max compression
```

## Comparing `discord-qalib-2.4.0.tar` & `discord-qalib-2.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.563566 discord-qalib-2.4.0/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-10 16:54:19.000000 discord-qalib-2.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.563566 discord-qalib-2.4.0/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-10 16:54:19.000000 discord-qalib-2.4.0/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.563566 discord-qalib-2.4.0/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    29579 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/templater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-10 16:54:19.000000 discord-qalib-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:52.530897 discord-qalib-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-10 19:57:52.530897 discord-qalib-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:52.526897 discord-qalib-2.4.1/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-10 19:57:52.000000 discord-qalib-2.4.1/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-10 19:57:52.000000 discord-qalib-2.4.1/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:57:52.000000 discord-qalib-2.4.1/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 19:57:52.000000 discord-qalib-2.4.1/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 19:57:52.000000 discord-qalib-2.4.1/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-10 19:57:39.000000 discord-qalib-2.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:52.526897 discord-qalib-2.4.1/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-10 19:57:39.000000 discord-qalib-2.4.1/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:52.530897 discord-qalib-2.4.1/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:52.530897 discord-qalib-2.4.1/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29579 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/templater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 19:57:14.000000 discord-qalib-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:57:52.530897 discord-qalib-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-10 19:57:39.000000 discord-qalib-2.4.1/setup.py
```

### Comparing `discord-qalib-2.4.0/LICENSE` & `discord-qalib-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/PKG-INFO` & `discord-qalib-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.4.0
+Version: 2.4.1
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.4.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.4.1 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.4.0/README.md` & `discord-qalib-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.4.1/discord_qalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.4.0
+Version: 2.4.1
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.4.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.4.1 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.4.0/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.4.1/discord_qalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/pyproject.toml` & `discord-qalib-2.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.4.0"
+version = "2.4.1"
 authors = [
     { name = "YousefEZ", email = "syberprojects@gmail.com" },
 ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.poetry]
 name = "discord-qalib"
-version = "2.4.0"
+version = "2.4.1"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.4.0/qalib/__init__.py` & `discord-qalib-2.4.1/qalib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .renderer import Renderer, RenderingOptions
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
         template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
```

### Comparing `discord-qalib-2.4.0/qalib/context.py` & `discord-qalib-2.4.1/qalib/context.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/interaction.py` & `discord-qalib-2.4.1/qalib/interaction.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/renderer.py` & `discord-qalib-2.4.1/qalib/renderer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/template_engines/formatter.py` & `discord-qalib-2.4.1/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/template_engines/jinja2.py` & `discord-qalib-2.4.1/qalib/template_engines/jinja2.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/__init__.py` & `discord-qalib-2.4.1/qalib/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/deserializer.py` & `discord-qalib-2.4.1/qalib/translators/deserializer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/factory.py` & `discord-qalib-2.4.1/qalib/translators/factory.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/json.py` & `discord-qalib-2.4.1/qalib/translators/json.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/menu.py` & `discord-qalib-2.4.1/qalib/translators/menu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from enum import Enum
-from typing import List, Optional, Dict, Any, Callable, TYPE_CHECKING
+from typing import List, Optional, Dict, Any, Callable, TYPE_CHECKING, Coroutine
 
 import discord.ui.button
 
 from qalib.translators import Message, Callback
 
 if TYPE_CHECKING:
     from qalib.translators.events import EventCallbacks
@@ -49,25 +49,25 @@
         self._timeout = timeout
         self._arrows = arrows
         self._events = {} if events is None else events
         self._active_page = 0
         self._front_page = 0
         self._link()
 
-    def add_event(self, event: MenuEvents, callback: Callable[[Menu], Any]) -> None:
+    def add_event(self, event: MenuEvents, callback: MenuChangeEvent) -> None:
         """This method is used to add an event to the menu.
 
         Args:
             event (MenuEvents): event that is added
             callback (Callable[[Menu], Any]): callback that is called when the event is triggered
         """
         self._events[event] = callback
 
-    def call_event(self, event: MenuEvents) -> None:
-        self._events[event](self)
+    async def call_event(self, event: MenuEvents) -> None:
+        await self._events[event](self)
 
     def _create_arrows(
             self,
             left: Optional[int] = None,
             right: Optional[int] = None
     ) -> List[discord.ui.Button]:
         """This function creates the arrow buttons that are used to navigate between the pages.
@@ -82,15 +82,15 @@
         def create_view(index: int) -> Callback:
             async def callback(interaction: discord.Interaction):
                 await interaction.response.edit_message(
                     **self._pages[index].convert_to_interaction_message().as_edit().dict()
                 )
 
                 self._active_page = index
-                self.call_event(MenuEvents.ON_CHANGE)
+                await self.call_event(MenuEvents.ON_CHANGE)
 
             return callback
 
         buttons: List[discord.ui.Button] = []
 
         def construct_button(display: Optional[int], action: MenuActions) -> None:
             if display is None:
@@ -136,8 +136,8 @@
     @front.setter
     def front(self, index: int) -> None:
         if index >= len(self._pages):
             raise IndexError("Index out of bounds")
         self._front_page = index
 
 
-MenuChangeEvent = Callable[[Menu], None]
+MenuChangeEvent = Callable[[Menu], Coroutine[Any, Any, None]]
```

### Comparing `discord-qalib-2.4.0/qalib/translators/message_parsing.py` & `discord-qalib-2.4.1/qalib/translators/message_parsing.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/modal.py` & `discord-qalib-2.4.1/qalib/translators/modal.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/templater.py` & `discord-qalib-2.4.1/qalib/translators/templater.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/view.py` & `discord-qalib-2.4.1/qalib/translators/view.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/qalib/translators/xml.py` & `discord-qalib-2.4.1/qalib/translators/xml.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.4.0/setup.py` & `discord-qalib-2.4.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.4.0",
+    version="2.4.1",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
     package_data={"qalib": ["py.typed"]},
 )
```


# Comparing `tmp/discord-qalib-2.3.0.tar.gz` & `tmp/discord-qalib-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.3.0.tar", last modified: Sat May 20 18:43:58 2023, max compression
+gzip compressed data, was "discord-qalib-2.4.0.tar", last modified: Sat Jun 10 16:54:32 2023, max compression
```

## Comparing `discord-qalib-2.3.0.tar` & `discord-qalib-2.4.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 18:43:58.000000 discord-qalib-2.3.0/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-20 18:43:48.000000 discord-qalib-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-20 18:43:48.000000 discord-qalib-2.3.0/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    28623 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/templater.py
--rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 18:43:32.000000 discord-qalib-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:43:58.788205 discord-qalib-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-20 18:43:48.000000 discord-qalib-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.563566 discord-qalib-2.4.0/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 16:54:32.000000 discord-qalib-2.4.0/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-10 16:54:19.000000 discord-qalib-2.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.563566 discord-qalib-2.4.0/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-10 16:54:19.000000 discord-qalib-2.4.0/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.563566 discord-qalib-2.4.0/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29579 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/templater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 16:54:01.000000 discord-qalib-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:54:32.567566 discord-qalib-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-10 16:54:19.000000 discord-qalib-2.4.0/setup.py
```

### Comparing `discord-qalib-2.3.0/LICENSE` & `discord-qalib-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.3.0/PKG-INFO` & `discord-qalib-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.3.0
+Version: 2.4.0
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
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.3.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.4.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.3.0/README.md` & `discord-qalib-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.3.0/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.4.0/discord_qalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.3.0
+Version: 2.4.0
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
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.3.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.4.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.3.0/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.4.0/discord_qalib.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -15,13 +15,16 @@
 qalib/renderer.py
 qalib/template_engines/__init__.py
 qalib/template_engines/formatter.py
 qalib/template_engines/jinja2.py
 qalib/template_engines/template_engine.py
 qalib/translators/__init__.py
 qalib/translators/deserializer.py
+qalib/translators/events.py
 qalib/translators/factory.py
 qalib/translators/json.py
 qalib/translators/menu.py
 qalib/translators/message_parsing.py
+qalib/translators/modal.py
 qalib/translators/templater.py
+qalib/translators/view.py
 qalib/translators/xml.py
```

### Comparing `discord-qalib-2.3.0/pyproject.toml` & `discord-qalib-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.3.0"
+version = "2.4.0"
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
-version = "2.3.0"
+version = "2.4.0"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.3.0/qalib/__init__.py` & `discord-qalib-2.4.0/qalib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .renderer import Renderer, RenderingOptions
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
         template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
```

### Comparing `discord-qalib-2.3.0/qalib/context.py` & `discord-qalib-2.4.0/qalib/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import discord.ext.commands
 import discord.message
 from deprecated import deprecated
 
 from qalib.renderer import Renderer
 from qalib.translators import Callback, Message
-from qalib.translators.deserializer import K_contra, EventCallback
+from qalib.translators.events import EventCallback, EventCallbacks
+from qalib.translators.deserializer import K_contra
 from qalib.translators.menu import Menu
 
 
 class QalibContext(discord.ext.commands.context.Context, Generic[K_contra]):
     """QalibContext object is responsible for handling messages that are to be sent to the client."""
 
     def __init__(self, ctx: discord.ext.commands.context.Context, renderer: Renderer[K_contra]):
@@ -58,15 +59,15 @@
         return confirm.content if confirm is not None else None
 
     async def rendered_send(
             self,
             identifier: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            events: Optional[EventCallback] = None,
+            events: Optional[EventCallbacks] = None,
             **kwargs,
     ) -> discord.message.Message:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
@@ -87,15 +88,15 @@
         return await self.send(**{**message.convert_to_context_message().dict(), **kwargs})
 
     async def display(
             self,
             key: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            events: Optional[EventCallback] = None,
+            events: Optional[EventCallbacks] = None,
             **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
             key (str): identifies the embed in the route file
```

### Comparing `discord-qalib-2.3.0/qalib/interaction.py` & `discord-qalib-2.4.0/qalib/interaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import discord
 from deprecated import deprecated
 from discord.interactions import InteractionResponse
 from discord.ui import Modal
 
 from qalib.renderer import Renderer
 from qalib.translators import Callback, Message
-from qalib.translators.deserializer import K_contra, EventCallback
+from qalib.translators.deserializer import K_contra
+from qalib.translators.events import EventCallbacks
 from qalib.translators.menu import Menu
 
 if TYPE_CHECKING:
     from discord.types.interactions import Interaction as InteractionPayload
 
 
 def create_interaction_payload(interaction: discord.Interaction) -> Dict[str, Any]:
@@ -57,15 +58,15 @@
         self._displayed = False
 
     async def rendered_send(
             self,
             identifier: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            events: Optional[EventCallback] = None,
+            events: Optional[EventCallbacks] = None,
             **kwargs,
     ) -> None:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
@@ -93,15 +94,15 @@
             return await self.response.send_modal(message)  # pyright: ignore [reportGeneralTypeIssues]
 
     async def display(
             self,
             key: K_contra,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            events: Optional[EventCallback] = None,
+            events: Optional[EventCallbacks] = None,
             **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
             key (K): identifies the message in the template file
```

### Comparing `discord-qalib-2.3.0/qalib/renderer.py` & `discord-qalib-2.4.0/qalib/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from enum import Enum, auto
 from typing import Any, Dict, Generic, Optional, cast
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback
-from qalib.translators.deserializer import ReturnType, K_contra, Deserializer, EventCallbacks
+from qalib.translators.events import EventCallbacks
+from qalib.translators.deserializer import ReturnType, K_contra, Deserializer
 from qalib.translators.factory import DeserializerFactory, TemplaterFactory
 from qalib.translators.templater import Templater
 
 
 class RenderingOptions(Enum):
     """Options for the renderer."""
```

### Comparing `discord-qalib-2.3.0/qalib/template_engines/formatter.py` & `discord-qalib-2.4.0/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.3.0/qalib/template_engines/jinja2.py` & `discord-qalib-2.4.0/qalib/template_engines/jinja2.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.3.0/qalib/translators/__init__.py` & `discord-qalib-2.4.0/qalib/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.3.0/qalib/translators/deserializer.py` & `discord-qalib-2.4.0/qalib/translators/deserializer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Dict, Protocol, Optional, Literal, TypeVar, Union, Callable
+from typing import Dict, Protocol, Optional, Literal, TypeVar, Union
 
 from discord.ui import Modal
 
 from qalib.translators import Callback, Message
-from qalib.translators.menu import Menu, MenuEvents
+from qalib.translators.events import EventCallbacks
+from qalib.translators.menu import Menu
 
 Types = Literal["message", "menu", "modal", "expansive"]
 
 ReturnType = Union[Message, Modal, Menu]
 
 K_contra = TypeVar("K_contra", bound=str, contravariant=True)
-Events = MenuEvents
-EventCallback = Callable[[Menu], None]
-EventCallbacks = Dict[Events, EventCallback]
 
 
 class ElementTypes(Enum):
     """Enum that represents the types of elements that can be deserialized."""
 
     MESSAGE = "message"
     MENU = "menu"
```

### Comparing `discord-qalib-2.3.0/qalib/translators/factory.py` & `discord-qalib-2.4.0/qalib/translators/factory.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.3.0/qalib/translators/json.py` & `discord-qalib-2.4.0/qalib/translators/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import discord.types.embed
 from discord import ui
 from discord.abc import Snowflake
 from typing_extensions import NotRequired
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback, DiscordIdentifier, Message
-from qalib.translators.deserializer import Deserializer, ElementTypes, Types, ReturnType, K_contra, EventCallbacks
+from qalib.translators.deserializer import Deserializer, ElementTypes, Types, ReturnType, K_contra
+from qalib.translators.events import EventCallbacks
 from qalib.translators.menu import MenuActions, Menu
 from qalib.translators.message_parsing import (
     ButtonComponent,
     ButtonStyle,
     ChannelType,
     CustomSelects,
     Emoji,
@@ -33,15 +34,17 @@
     Field,
     Footer,
     Author,
     TextInputRaw,
     TextInputComponent,
     make_expansive_embeds, apply
 )
+from qalib.translators.modal import QalibModal
 from qalib.translators.templater import Templater
+from qalib.translators.view import QalibView
 
 OBJ = TypeVar("OBJ")
 
 ComponentTypes = Literal[
     "button",
     "select",
     "channel_select",
@@ -222,14 +225,16 @@
     timeout: NotRequired[Optional[float]]
     pages: List[Union[str, Page]]
     arrows: NotRequired[Arrows]
 
 
 class Modal(Element):
     title: str
+    timeout: NotRequired[Optional[float]]
+    custom_id: NotRequired[str]
     components: Components
 
 
 Elements = Union[RegularMessage, ExpansiveMessage, MenuMessage, Modal]
 Document = Dict[str, Elements]
 
 
@@ -318,36 +323,38 @@
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
             events (EventCallbacks): A dictionary containing the event callbacks.
 
         Returns (ReturnType): All possible deserialized objects.
         """
         element_type: Optional[ElementTypes] = ElementTypes.from_str(element["type"])
 
-        deserializers: Dict[ElementTypes, Callable[[Elements, Dict[str, Callback]], ReturnType]] = {
+        deserializers: Dict[ElementTypes, Callable[[Elements, Dict[str, Callback], EventCallbacks], ReturnType]] = {
             ElementTypes.MESSAGE: self.deserialize_message,
-            ElementTypes.EXPANSIVE: partial(self.deserialize_expansive_into_menu, events=events),
-            ElementTypes.MENU: partial(self.deserialize_menu, document=document, events=events),
+            ElementTypes.EXPANSIVE: self.deserialize_expansive_into_menu,
+            ElementTypes.MENU: partial(self.deserialize_menu, document=document),
             ElementTypes.MODAL: self.deserialize_modal,
         }
         if element_type is None:
             raise KeyError(f"Element type {element['type']} not found")
-        return deserializers[element_type](element, callables)
+        return deserializers[element_type](element, callables, events)
 
     # pylint: disable= too-many-locals
     def deserialize_message(
             self,
             message_tree: Union[RegularMessage, ExpansiveMessage],
             callables: Dict[str, Callback],
+            events: EventCallbacks,
             **overrides: Any
     ) -> Message:
         """Method to deserialize an embed into a Display NamedTuple containing the embed and the view
 
         Args:
             message_tree (Dict[str, Any]): The embed to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
             **overrides (Any): keyword arguments that override the messages
 
         Returns (Display): A Display NamedTuple containing the embed and the view
         """
 
         def render(embeds: List[Embed]) -> Sequence[discord.Embed]:
             return [self._render_embed(embed) for embed in embeds]
@@ -365,15 +372,15 @@
             allowed_mentions=apply(message_tree.get("allowed_mentions"), self._render_allowed_mentions),
             reference=apply(message_tree.get("message_reference"), lambda reference: discord.MessageReference(
                 message_id=reference["message_id"],
                 channel_id=reference["channel_id"],
                 guild_id=reference.get("guild_id"),
             )),
             mention_author=message_tree.get("mention_author"),
-            view=apply(message_tree.get("view"), self._render_view, callables),
+            view=apply(message_tree.get("view"), self._render_view, callables, events),
             stickers=None,
             ephemeral=message_tree.get("ephemeral"),
             silent=message_tree.get("silent"),
         )
 
         for key, value in overrides.items():
             setattr(message, key, value)
@@ -391,15 +398,15 @@
         Args:
             message_tree (ExpansiveMessage): The ExpansiveMessage of the message_tree
             callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
             events (EventCallbacks): A dictionary containing the event callbacks.
 
         Returns (Menu): A Menu object
         """
-        pages = self.deserialize_expansive(message_tree, callbacks)
+        pages = self.deserialize_expansive(message_tree, callbacks, events)
         timeout = message_tree.get("timeout", 180.0)
         if "arrows" not in message_tree:
             return Menu(pages, timeout, events=events)
 
         arrows: Dict[MenuActions, ButtonComponent] = self._deserialize_menu_arrows(message_tree["arrows"])
         return Menu(pages, timeout, arrows, events)
 
@@ -417,52 +424,56 @@
             MenuActions.NEXT: cast(ButtonComponent, arrows["next"]),
         }
 
     def deserialize_expansive(
             self,
             message_tree: ExpansiveMessage,
             callbacks: Dict[str, Callback],
+            events: EventCallbacks
     ) -> List[Message]:
         """Method to deserialize a source into a list of Display objects
 
         Args:
             message_tree (ExpansiveMessage): The ExpansiveMessage of the message_tree
             callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
 
         Returns (List[Display]): A list of Display objects
         """
-        return [self.deserialize_message(message_tree, callbacks, embed=embed)
+        return [self.deserialize_message(message_tree, callbacks, events=events, embed=embed)
                 for embed in self._separate_embed(message_tree["embed"], message_tree.get("page_number_key"))]
 
     def deserialize_page(
             self,
             document: Document,
             raw_page: Union[str, Page],
-            callables: Dict[str, Callback]
+            callables: Dict[str, Callback],
+            events: EventCallbacks
     ) -> List[Message]:
         """Method to deserialize a page into a Display object
 
         Args:
             document (Document): the original document containing all the keys.
             raw_page (Page): The page to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
 
         Returns (List[Message]): List of pages
         """
         page = document[raw_page] if isinstance(raw_page, str) else raw_page
         element_type = ElementTypes.from_str(page["type"])
 
         page_deserializers: Dict[
-            ElementTypes, Callable[[BaseMessage, Dict[str, Callback]], List[Message]]] = {
-            ElementTypes.MESSAGE: lambda msg, callback: [self.deserialize_message(msg, callback)],
+            ElementTypes, Callable[[BaseMessage, Dict[str, Callback], EventCallbacks], List[Message]]] = {
+            ElementTypes.MESSAGE: lambda msg, callback, m_events: [self.deserialize_message(msg, callback, m_events)],
             ElementTypes.EXPANSIVE: self.deserialize_expansive,
         }
         if element_type is None:
             raise TypeError(f"Unknown Element type {page['type']}")
-        return page_deserializers[element_type](page, callables)
+        return page_deserializers[element_type](page, callables, events)
 
     def deserialize_menu(
             self,
             menu: MenuMessage,
             callables: Dict[str, Callback],
             events: EventCallbacks,
             *,
@@ -474,35 +485,47 @@
             menu (MenuMessage): The Menu Dictionary to deserialize into a List of Messages
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
             events (EventCallbacks): A dictionary containing the event callbacks.
             document (Document): the original document containing all the keys.
 
         Returns (List[Message]): A list of Display objects
         """
-        pages: List[Message] = sum((self.deserialize_page(document, page, callables) for page in menu["pages"]), [])
+        pages: List[Message] = sum((self.deserialize_page(document, page, callables, events) for page in menu["pages"]),
+                                   [])
         timeout: Optional[float] = menu.get("timeout", 180.0)
 
         if "arrows" not in menu:
             return Menu(pages, timeout, events=events)
 
         arrows: Dict[MenuActions, ButtonComponent] = self._deserialize_menu_arrows(menu["arrows"])
         return Menu(pages, timeout, arrows, events)
 
-    def deserialize_modal(self, tree: Modal, methods: Dict[str, Callback]) -> discord.ui.Modal:
+    def deserialize_modal(
+            self,
+            tree: Modal,
+            callables: Dict[str, Callback],
+            events: EventCallbacks,
+            **kwargs
+    ) -> discord.ui.Modal:
         """Method to deserialize a modal into a discord.ui.Modal object
 
         Args:
             tree (Modal): The Modal Dictionary to deserialize into a discord.ui.Modal object
-            methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            events (EventCallbacks): A dictionary containing the event callbacks.
+            **kwargs
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
-        modal = type(f"{tree['title']} Modal", (discord.ui.Modal,), methods)(title=tree["title"])
+        modal = QalibModal(title=tree["title"],
+                           events=events,
+                           timeout=tree.get("timeout", 180.0),
+                           custom_id=tree.get("custom_id", None))
 
-        components = self.render_components(tree["components"]) if "components" in tree else []
+        components = self.render_components(tree["components"], callables) if "components" in tree else []
 
         for component in components:
             modal.add_item(component)
 
         return modal
 
     def _separate_embed(self, raw_embed: ExpansiveEmbed, replacement_key: Optional[str]) -> List[discord.Embed]:
@@ -547,24 +570,25 @@
         """
         return discord.File(
             fp=raw_file["filename"],
             description=raw_file["description"] if "description" in raw_file else None,
             spoiler=raw_file["spoiler"] if "spoiler" in raw_file else False,
         )
 
-    def _render_view(self, raw_view: View, callables: Dict[str, Callback]) -> ui.View:
+    def _render_view(self, raw_view: View, callables: Dict[str, Callback], events: EventCallbacks) -> ui.View:
         """Method to render a view element into a discord.ui.View object
 
         Args:
             raw_view (View) The view element to render
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
 
         Returns (ui.View): A discord.ui.View object
         """
-        view = ui.View()
+
+        view = QalibView(events)
         if "timeout" in raw_view:
             view.timeout = raw_view["timeout"]
         for component in self.render_components(raw_view["components"], callables):
             view.add_item(component)
         return view
 
     @staticmethod
@@ -716,26 +740,24 @@
         item_renderer = component_renderer[component_type]
 
         return item_renderer(component, callback)
 
     def render_components(
             self,
             components: Components,
-            callables: Optional[Dict[str, Callback]] = None
+            callables: Dict[str, Callback]
     ) -> List[ui.Item]:
         """Renders the components specified by the identifier
 
         Args:
             components (Components): the dictionary containing the view component.
             callables (Dict[str, Callback]): the callbacks to be called when the user interacts with the components
 
         Returns (List[ui.Item]): the rendered components
         """
-        if callables is None:
-            callables = {}
         return [self.render_component(component, callables.get(key)) for key, component in components.items()]
 
     def _render_embed(self, raw_embed: Embed, *replacements: Tuple[str, str]) -> discord.Embed:
         """Render the desired templated embed in discord.Embed instance
 
         Args:
            raw_embed (Embed): the dictionary containing the required key, values needed to render the embed.
```

### Comparing `discord-qalib-2.3.0/qalib/translators/menu.py` & `discord-qalib-2.4.0/qalib/translators/menu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from enum import Enum
-from typing import List, Optional, Dict, Any, Callable
+from typing import List, Optional, Dict, Any, Callable, TYPE_CHECKING
 
 import discord.ui.button
-from discord import ui
 
 from qalib.translators import Message, Callback
-from qalib.translators.message_parsing import ButtonComponent, create_button
-
 
-class MenuEvents(Enum):
-    ON_CHANGE = "on_change"
+if TYPE_CHECKING:
+    from qalib.translators.events import EventCallbacks
+from qalib.translators.view import QalibView
+from qalib.translators.message_parsing import ButtonComponent, create_button
 
 
 class MenuActions(Enum):
     """Enum that represents the types of actions that can be performed by the buttons."""
 
     NEXT = "next"
     PREVIOUS = "previous"
@@ -26,49 +25,49 @@
 NextButton: ButtonComponent = {"emoji": "➡️", "style": "primary"}
 DefaultButtons: Dict[MenuActions, ButtonComponent] = {
     MenuActions.NEXT: NextButton,
     MenuActions.PREVIOUS: PreviousButton
 }
 
 
+class MenuEvents(Enum):
+    ON_CHANGE = "on_change"
+
+
 class Menu:
     """Class that represents a menu. It is used to store the pages of the menu, as well as the buttons that are used"""
 
     __slots__ = "_pages", "_timeout", "_arrows", "_events", "_active_page", "_front_page", "_linked"
 
     def __init__(
             self,
             pages: List[Message],
             timeout: Optional[float] = None,
             arrows: Optional[Dict[MenuActions, ButtonComponent]] = None,
-            events: Optional[Dict[MenuEvents, Callable[[Menu], Any]]] = None
+            events: Optional[EventCallbacks] = None
     ) -> None:
         self._pages = pages
         self._timeout = timeout
         self._arrows = arrows
-        self._events = {} if events is None else {event_type: [callback] for event_type, callback in events.items()}
+        self._events = {} if events is None else events
         self._active_page = 0
         self._front_page = 0
         self._link()
 
     def add_event(self, event: MenuEvents, callback: Callable[[Menu], Any]) -> None:
         """This method is used to add an event to the menu.
 
         Args:
             event (MenuEvents): event that is added
             callback (Callable[[Menu], Any]): callback that is called when the event is triggered
         """
-        if event not in self._events:
-            self._events[event] = [callback]
-            return
-        self._events[event].append(callback)
+        self._events[event] = callback
 
     def call_event(self, event: MenuEvents) -> None:
-        for action in self._events[event]:
-            action(self)
+        self._events[event](self)
 
     def _create_arrows(
             self,
             left: Optional[int] = None,
             right: Optional[int] = None
     ) -> List[discord.ui.Button]:
         """This function creates the arrow buttons that are used to navigate between the pages.
@@ -108,15 +107,15 @@
 
     def _link(self) -> None:
         for i, message in enumerate(self._pages):
             left = i - 1 if i > 0 else None
             right = i + 1 if i + 1 < len(self._pages) else None
 
             if message.view is None:
-                message.view = ui.View(timeout=self._timeout)
+                message.view = QalibView(self._events, timeout=self._timeout)
 
             for arrow in self._create_arrows(left, right):
                 message.view.add_item(arrow)
 
     def __len__(self) -> int:
         return len(self._pages)
 
@@ -135,7 +134,10 @@
         return self._pages[self._front_page]
 
     @front.setter
     def front(self, index: int) -> None:
         if index >= len(self._pages):
             raise IndexError("Index out of bounds")
         self._front_page = index
+
+
+MenuChangeEvent = Callable[[Menu], None]
```

### Comparing `discord-qalib-2.3.0/qalib/translators/message_parsing.py` & `discord-qalib-2.4.0/qalib/translators/message_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import discord
 import discord.emoji
 import discord.partial_emoji
 import emoji
 from discord import ui, utils
 from typing_extensions import NotRequired, Concatenate, ParamSpec
 
-from qalib.translators import Callback, CallbackMethod, Message, M, N
+from qalib.translators import Callback, CallbackMethod, M, N
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 __all__ = (
     "CustomSelects",
     "make_channel_types",
```

### Comparing `discord-qalib-2.3.0/qalib/translators/templater.py` & `discord-qalib-2.4.0/qalib/translators/templater.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.3.0/qalib/translators/xml.py` & `discord-qalib-2.4.0/qalib/translators/xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import discord
 import discord.types.embed as embed_types
 from discord import ui
 from discord.abc import Snowflake
 
 from qalib.template_engines.template_engine import TemplateEngine
 from qalib.translators import Callback, DiscordIdentifier, Message
-from qalib.translators.deserializer import Deserializer, ElementTypes, ReturnType, K_contra, EventCallbacks
+from qalib.translators.deserializer import Deserializer, ElementTypes, ReturnType, K_contra
+from qalib.translators.events import EventCallbacks
 from qalib.translators.menu import MenuActions, Menu
 from qalib.translators.message_parsing import (
     ButtonComponent,
     ChannelType,
     Emoji,
     create_button,
     create_channel_select,
@@ -27,15 +28,17 @@
     make_colour,
     make_emoji,
     Field,
     Footer,
     Author,
     TextInputComponent,
     make_expansive_embeds, apply, )
+from qalib.translators.modal import ModalEvents, ModalEventsCallbacks, QalibModal
 from qalib.translators.templater import Templater
+from qalib.translators.view import QalibView
 
 
 def get_text(element_tree: ElementTree.Element, child: str) -> Optional[str]:
     element = element_tree.find(child)
     if element is None:
         return None
     return None if element.text is None else element.text
@@ -112,56 +115,58 @@
             callables (Dict[str, Callback]): dictionary containing the callables to use for the components
             events (EventCallbacks): dictionary containing the events to use for the components
 
         Returns (ReturnType): all possible deserialized objects.
         """
         element_type = ElementTypes.from_str(element.tag)
 
-        deserializers: Dict[ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback]], ReturnType]] = {
+        deserializers: Dict[
+            ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback], EventCallbacks], ReturnType]] = {
             ElementTypes.MESSAGE: self.deserialize_message,
-            ElementTypes.EXPANSIVE: partial(self.deserialize_expansive_into_menu, events=events),
-            ElementTypes.MENU: partial(self.deserialize_menu, document=document, events=events),
+            ElementTypes.EXPANSIVE: self.deserialize_expansive_into_menu,
+            ElementTypes.MENU: partial(self.deserialize_menu, document=document),
             ElementTypes.MODAL: self.deserialize_modal,
         }
         assert element_type is not None, f"Element type {element.tag} not found"
-        return deserializers[element_type](element, callables)
+        return deserializers[element_type](element, callables, events)
 
     def deserialize_expansive_into_menu(
             self,
             element: ElementTree.Element,
             callbacks: Dict[str, Callback],
             events: EventCallbacks
     ) -> Menu:
-        pages = self.deserialize_expansive(element, callbacks)
-        print(element)
+        pages = self.deserialize_expansive(element, callbacks, events)
         timeout_element = element.find("timeout")
         timeout: Optional[float] = 180.0
         if timeout_element is not None:
             timeout = None if timeout_element.text is None else float(timeout_element.text)
 
         arrows: Dict[MenuActions, ButtonComponent] = self.deserialize_menu_arrows(element)
         return Menu(pages, timeout, arrows, events)
 
     def deserialize_expansive(
             self,
             element: ElementTree.Element,
             callbacks: Dict[str, Callback],
+            events: EventCallbacks
     ) -> List[Message]:
         """Deserializes an embed from an XML file, and returns it as a Display object.
 
         Args:
             element (ElementTree.Element): templated document contents to deserialize.
             callbacks (Dict[str, Callback]): A dictionary containing the callables to use for the components.
+            events (EventCallbacks): A dictionary containing the events to use for the components.
 
         Returns (List[Message]): A list of messages containing the embed and its view.
         """
         raw_embed = element.find("embed")
         assert raw_embed is not None, "Embed not found"
 
-        return [self.deserialize_message(element, callbacks, embed=embed)
+        return [self.deserialize_message(element, callbacks, events, embed=embed)
                 for embed in self._separate_embed(raw_embed, element.get("page_number_key"))]
 
     def deserialize_menu_arrows(self, arrows_view: ElementTree.Element) -> Dict[MenuActions, ButtonComponent]:
         """Deserializes the arrows of a menu from an XML file, and returns it as a dictionary.
 
         Args:
             arrows_view (ElementTree.Element): templated document contents to deserialize.
@@ -178,32 +183,34 @@
 
         return arrows
 
     def deserialize_message(
             self,
             message_tree: ElementTree.Element,
             callables: Dict[str, Callback],
+            events: EventCallbacks,
             **overrides: Any
     ) -> Message:
         """Deserializes an embed from an ElementTree.Element, and returns it as a Display object.
 
         Args:
             message_tree (ElementTree.Element): The element to deserialize the embed from.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
+            events (EventCallbacks): A dictionary containing the events to use for the components.
             **overrides (Any): any overrides to apply to the Message
 
         Returns (Message): A display object containing the embed and its view.
         """
         message = Message(
             embed=apply(get_element(message_tree, "embed"), self._render_embed),
             embeds=apply(
                 get_element(message_tree, "embeds"),
                 lambda raw_tree: list(map(self._render_embed, raw_tree)),
             ),
-            view=apply(get_element(message_tree, "view"), self._render_view, callables),
+            view=apply(get_element(message_tree, "view"), self._render_view, callables, events),
             content=get_text(message_tree, "content"),
             tts=apply(get_text(message_tree, "tts"), lambda string: string.lower() == "true"),
             nonce=apply(get_text(message_tree, "nonce"), int),
             delete_after=apply(get_text(message_tree, "delete_after"), float),
             suppress_embeds=apply(
                 get_element(message_tree, "suppress_embeds"),
                 lambda tree: self.get_attribute(tree, "value") in ("", "true"),
@@ -233,27 +240,28 @@
             setattr(message, key, value)
         return message
 
     def deserialize_page(
             self,
             document: ElementTree.Element,
             element: ElementTree.Element,
-            callables: Dict[str, Callback]
+            callables: Dict[str, Callback],
+            events: EventCallbacks,
     ) -> List[Message]:
         if element.tag == "page":
             element = self._get_element(document, self.get_attribute(element, "key"))
         element_type = ElementTypes.from_str(element.tag)
 
         page_deserializers: Dict[
-            ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback]], List[Message]]] = {
-            ElementTypes.MESSAGE: lambda page, callback: [self.deserialize_message(page, callback)],
+            ElementTypes, Callable[[ElementTree.Element, Dict[str, Callback], EventCallbacks], List[Message]]] = {
+            ElementTypes.MESSAGE: lambda page, callback, m_events: [self.deserialize_message(page, callback, m_events)],
             ElementTypes.EXPANSIVE: self.deserialize_expansive,
         }
         assert element_type is not None, f"Element type {element.tag} not found"
-        return page_deserializers[element_type](element, callables)
+        return page_deserializers[element_type](element, callables, events)
 
     def deserialize_menu(
             self,
             element: ElementTree.Element,
             callables: Dict[str, Callback],
             events: EventCallbacks,
             *,
@@ -269,45 +277,52 @@
             document (ElementTree.Element): The entire document
 
         Returns (List[Display]): List of displays that are connected by buttons in their views to navigate between them.
         """
         raw_pages = element.find("pages")
         assert raw_pages is not None, "pages is not present"
 
-        pages: List[Message] = sum([self.deserialize_page(document, page, callables) for page in raw_pages], [])
+        pages: List[Message] = sum([self.deserialize_page(document, page, callables, events) for page in raw_pages], [])
 
         timeout_ele = element.find("timeout")
         timeout = float(timeout_ele.text) if timeout_ele is not None and timeout_ele.text is not None else None
 
         view = element.find("arrows")
         if view is None:
             return Menu(pages, timeout, events=events)
 
         arrows: Dict[MenuActions, ButtonComponent] = self.deserialize_menu_arrows(view)
         return Menu(pages, timeout, arrows, events)
 
     def deserialize_modal(
             self,
             element: ElementTree.Element,
-            methods: Dict[str, Callback],
+            callables: Dict[str, Callback],
+            events: Dict[ModalEvents, ModalEventsCallbacks],
             **kwargs: Any
     ) -> discord.ui.Modal:
         """Method to deserialize a modal into a discord.ui.Modal object
 
         Args:
             element (ElementTree.Element): The element to deserialize into a modal
-            methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
+            callables (Dict[str, Callback]): A dictionary containing the callables to use for the components
+            events (Dict[ModalEvents, ModalEventsCallbacks]): A dictionary containing the events to callback on
             kwargs (Dict[str, Any]): A dictionary containing the keywords to use for the view
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
         title = self.get_attribute(element, "title")
-        modal = type(f"{title} Modal", (discord.ui.Modal,), {**methods, **kwargs})(title=title)
+        timeout_element = element.find("timeout")
+        if timeout_element is not None:
+            timeout = float(timeout_element.text) if timeout_element.text is not None else None
+            modal = QalibModal(title=title, events=events, timeout=timeout, custom_id=element.get("custom_id"))
+        else:
+            modal = QalibModal(title=title, events=events, custom_id=element.get("custom_id"))
 
-        for component in self.render_components(element):
+        for component in self.render_components(element, callables):
             modal.add_item(component)
 
         return modal
 
     def _separate_embed(self, raw_embed: ElementTree.Element, replacement_key: Optional[str]) -> List[discord.Embed]:
         """Separates the embeds from the raw embed element.
 
@@ -400,25 +415,25 @@
             description=self.get_element_text(raw_file.find("description")),
         )
 
     def _render_view(
             self,
             raw_view: ElementTree.Element,
             callables: Dict[str, Callback],
+            events: EventCallbacks,
     ) -> ui.View:
         """Renders a view from an ElementTree.Element.
 
         Args:
             raw_view (ElementTree.Element): The element to render the view from.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
 
         Returns (ui.View): A view object containing the components.
         """
-        view = ui.View()
-
+        view = QalibView(events)
         timeout = raw_view.find("timeout")
         if timeout is not None:
             view.timeout = None if timeout.text is None else float(timeout.text)
         for component in self.render_components(raw_view, callables):
             view.add_item(component)
         return view
 
@@ -700,27 +715,24 @@
             "mentionable_select": partial(self._render_type_select, select_base=ui.MentionableSelect),
             "user_select": partial(self._render_type_select, select_base=ui.UserSelect),
         }
         renderer: Callable[[ElementTree.Element, Optional[Callback]], ui.Item] = components[component.tag]
         return renderer(component, callback)
 
     def render_components(
-            self, view: ElementTree.Element, callables: Optional[Dict[str, Callback]] = None
+            self, view: ElementTree.Element, callables: Dict[str, Callback]
     ) -> List[ui.Item]:
         """Renders a list of components based on the identifier given.
 
         Args:
             view (ui.View): The raw view.
             callables (Dict[str, Callback]): The callbacks to use if the user interacts with the components.
 
         Returns (Optional[List[discord.ui.Item]]): The rendered components.
         """
-        if callables is None:
-            callables = {}
-
         components = view.find("components")
         if components is None:
             return []
         return [
             self.render_component(
                 component,
                 callables.get(self.get_attribute(component, "key")),
```

### Comparing `discord-qalib-2.3.0/setup.py` & `discord-qalib-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.3.0",
+    version="2.4.0",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
     package_data={"qalib": ["py.typed"]},
 )
```


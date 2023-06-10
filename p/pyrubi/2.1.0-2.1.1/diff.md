# Comparing `tmp/pyrubi-2.1.0.tar.gz` & `tmp/pyrubi-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubi-2.1.0.tar", last modified: Wed Jun  7 14:39:14 2023, max compression
+gzip compressed data, was "pyrubi-2.1.1.tar", last modified: Sat Jun 10 10:56:52 2023, max compression
```

## Comparing `pyrubi-2.1.0.tar` & `pyrubi-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.662299 pyrubi-2.1.0/
--rw-rw-rw-   0        0        0     2204 2023-06-07 14:39:14.662299 pyrubi-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2023-06-07 14:35:32.000000 pyrubi-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.622603 pyrubi-2.1.0/pyrubi/
--rw-rw-rw-   0        0        0      246 2023-06-07 14:36:26.000000 pyrubi-2.1.0/pyrubi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.646796 pyrubi-2.1.0/pyrubi/cryption/
--rw-rw-rw-   0        0        0     1194 2023-02-10 12:30:31.000000 pyrubi-2.1.0/pyrubi/cryption/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.647798 pyrubi-2.1.0/pyrubi/handler/
--rw-rw-rw-   0        0        0     1243 2023-06-07 06:58:02.000000 pyrubi-2.1.0/pyrubi/handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.649004 pyrubi-2.1.0/pyrubi/maker/
--rw-rw-rw-   0        0        0     3164 2023-06-07 09:01:39.000000 pyrubi-2.1.0/pyrubi/maker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.655895 pyrubi-2.1.0/pyrubi/message/
--rw-rw-rw-   0        0        0     4687 2023-04-20 12:26:50.000000 pyrubi-2.1.0/pyrubi/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.657895 pyrubi-2.1.0/pyrubi/methods/
--rw-rw-rw-   0        0        0    43655 2023-06-07 09:00:36.000000 pyrubi-2.1.0/pyrubi/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.659127 pyrubi-2.1.0/pyrubi/servers/
--rw-rw-rw-   0        0        0      334 2023-05-26 15:37:31.000000 pyrubi-2.1.0/pyrubi/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.660136 pyrubi-2.1.0/pyrubi/tools/
--rw-rw-rw-   0        0        0     7027 2023-06-07 09:00:54.000000 pyrubi-2.1.0/pyrubi/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:39:14.638957 pyrubi-2.1.0/pyrubi.egg-info/
--rw-rw-rw-   0        0        0     2204 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 14:39:14.000000 pyrubi-2.1.0/pyrubi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:39:14.662299 pyrubi-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-06-07 13:59:20.000000 pyrubi-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.158610 pyrubi-2.1.1/
+-rw-rw-rw-   0        0        0     1935 2023-06-10 10:56:52.157610 pyrubi-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1103 2023-06-10 10:50:53.000000 pyrubi-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.126635 pyrubi-2.1.1/pyrubi/
+-rw-rw-rw-   0        0        0      246 2023-06-10 10:46:07.000000 pyrubi-2.1.1/pyrubi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.143609 pyrubi-2.1.1/pyrubi/cryption/
+-rw-rw-rw-   0        0        0     1194 2023-02-10 12:30:31.000000 pyrubi-2.1.1/pyrubi/cryption/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.144614 pyrubi-2.1.1/pyrubi/handler/
+-rw-rw-rw-   0        0        0     1243 2023-06-07 06:58:02.000000 pyrubi-2.1.1/pyrubi/handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.145614 pyrubi-2.1.1/pyrubi/maker/
+-rw-rw-rw-   0        0        0     3164 2023-06-07 09:01:39.000000 pyrubi-2.1.1/pyrubi/maker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.145614 pyrubi-2.1.1/pyrubi/message/
+-rw-rw-rw-   0        0        0     4687 2023-04-20 12:26:50.000000 pyrubi-2.1.1/pyrubi/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.146613 pyrubi-2.1.1/pyrubi/methods/
+-rw-rw-rw-   0        0        0    43655 2023-06-07 09:00:36.000000 pyrubi-2.1.1/pyrubi/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.148612 pyrubi-2.1.1/pyrubi/servers/
+-rw-rw-rw-   0        0        0      334 2023-05-26 15:37:31.000000 pyrubi-2.1.1/pyrubi/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.156611 pyrubi-2.1.1/pyrubi/tools/
+-rw-rw-rw-   0        0        0     7100 2023-06-10 10:43:44.000000 pyrubi-2.1.1/pyrubi/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:56:52.141380 pyrubi-2.1.1/pyrubi.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 10:56:52.000000 pyrubi-2.1.1/pyrubi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:56:52.158610 pyrubi-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2023-06-10 10:55:08.000000 pyrubi-2.1.1/setup.py
```

### Comparing `pyrubi-2.1.0/PKG-INFO` & `pyrubi-2.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,52 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.1.0
+Version: 2.1.1
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat
+Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir,bot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.1.0</h1>
+<h1>Pyrubi 2.1.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
-<style>
-    .image {
-        border-radius: 12px
-    }
-    h1 {
-        text-align: center;
-        color: dodgerblue;
-        font-size: 25px;
-        border-radius: 3px
-    }
-    a{
-        margin: 1px;
-        color: white;
-        background-image: linear-gradient(to right, rgb(0, 89, 255), rgb(0, 166, 255));
-        font-size: 18px;
-        border-radius: 3px
-    }
-</style>
-
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.1' width='356' class="image">
 </p>
+
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
+    •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
 <hr>
 
 **Example:**
 ``` python
 from pyrubi import Bot, Message
 
 bot = Bot("TOKEN")
 
 for update in bot.on_message():
     message = Message(update)
-    if m.text() == 'Hello':
-        bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --I'm Ali--.", message.message_id())
+    if message.text() == 'hello':
+        bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://example.com).", message.message_id())
 ```
 
 <hr>
 
 ### Features:
     
 - **Fast** : *The requests are very fast.*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.1.0 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.1.1 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
-ali.ganji.za@gmail.com Keywords:
-rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
-Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
-markdown
-****** Pyrubi 2.1.0 ******
+ali.ganji.za@gmail.com Keywords: rubika,rubika-
+bot,pyrubi,rubx,rubino,rubika.ir,bot Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
+Python: ~=3.6 Description-Content-Type: text/markdown
+****** Pyrubi 2.1.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.1.0]
-                               GitHub Documents
+                            [Pyrubi Library 2.1.1]
+                             GitHub â¢ Documents
 ===============================================================================
 **Example:** ``` python from pyrubi import Bot, Message bot = Bot("TOKEN") for
-update in bot.on_message(): message = Message(update) if m.text() == 'Hello':
-bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --
-I'm Ali--.", message.message_id()) ```
+update in bot.on_message(): message = Message(update) if message.text() ==
+'hello': bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title
+()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://
+example.com).", message.message_id()) ```
 ===============================================================================
 ### Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
 ## Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
```

### Comparing `pyrubi-2.1.0/pyrubi/cryption/__init__.py` & `pyrubi-2.1.1/pyrubi/cryption/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.1.0/pyrubi/handler/__init__.py` & `pyrubi-2.1.1/pyrubi/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.1.0/pyrubi/maker/__init__.py` & `pyrubi-2.1.1/pyrubi/maker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.1.0/pyrubi/message/__init__.py` & `pyrubi-2.1.1/pyrubi/message/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.1.0/pyrubi/methods/__init__.py` & `pyrubi-2.1.1/pyrubi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.1.0/pyrubi/tools/__init__.py` & `pyrubi-2.1.1/pyrubi/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
         if '.' in url:
             mime = url.split('.')[-1]
             if len(mime) <= 4:
                 return mime
         return 'pyrubi'
     
     def check_metadata(text):
+        if text is None:
+            return [], text
+
         real_text = text.replace('``', '').replace('**', '').replace('__', '').replace('~~', '').replace('--', '').replace('@@', '')
         metadata = []
         conflict = 0
         mention_object_index = 0
         result = []
 
         for i in [(i.start(), len(i.group(1)), "mono") for i in finditer(r'\`\`([^``]*)\`\`', text)]:
@@ -161,15 +164,15 @@
                             'mention_text_object_guid': mention_objects[mention_object_index],
                             'mention_text_object_type': mention_type
                         }
                     )
                 real_text = real_text.replace(f'({mention_objects[mention_object_index]})', '')
                 conflict += 6 + len(mention_objects[mention_object_index])
                 mention_object_index += 1
-
+                
         return result, real_text
 
     def get_chat_type_by_id(chat_id):
         if chat_id.startswith('u'): data = 'User'
         elif chat_id.startswith('g'): data = 'Group'
         elif chat_id.startswith('c'): data = 'Channel'
         elif chat_id.startswith('b'): data = 'Bot'
```

### Comparing `pyrubi-2.1.0/pyrubi.egg-info/PKG-INFO` & `pyrubi-2.1.1/pyrubi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,52 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.1.0
+Version: 2.1.1
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat
+Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir,bot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.1.0</h1>
+<h1>Pyrubi 2.1.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
-<style>
-    .image {
-        border-radius: 12px
-    }
-    h1 {
-        text-align: center;
-        color: dodgerblue;
-        font-size: 25px;
-        border-radius: 3px
-    }
-    a{
-        margin: 1px;
-        color: white;
-        background-image: linear-gradient(to right, rgb(0, 89, 255), rgb(0, 166, 255));
-        font-size: 18px;
-        border-radius: 3px
-    }
-</style>
-
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.1.1' width='356' class="image">
 </p>
+
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
+    •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
 <hr>
 
 **Example:**
 ``` python
 from pyrubi import Bot, Message
 
 bot = Bot("TOKEN")
 
 for update in bot.on_message():
     message = Message(update)
-    if m.text() == 'Hello':
-        bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --I'm Ali--.", message.message_id())
+    if message.text() == 'hello':
+        bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://example.com).", message.message_id())
 ```
 
 <hr>
 
 ### Features:
     
 - **Fast** : *The requests are very fast.*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.1.0 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.1.1 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
-ali.ganji.za@gmail.com Keywords:
-rubika,rubino,pyrubi,pyrubika,rubx,rubika.ir,bot,chat Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
-Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
-markdown
-****** Pyrubi 2.1.0 ******
+ali.ganji.za@gmail.com Keywords: rubika,rubika-
+bot,pyrubi,rubx,rubino,rubika.ir,bot Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
+Python: ~=3.6 Description-Content-Type: text/markdown
+****** Pyrubi 2.1.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.1.0]
-                               GitHub Documents
+                            [Pyrubi Library 2.1.1]
+                             GitHub â¢ Documents
 ===============================================================================
 **Example:** ``` python from pyrubi import Bot, Message bot = Bot("TOKEN") for
-update in bot.on_message(): message = Message(update) if m.text() == 'Hello':
-bot.send_text(message.chat_id(), "``Hello`` **from** __Pyrubi__ ~~Library~~, --
-I'm Ali--.", message.message_id()) ```
+update in bot.on_message(): message = Message(update) if message.text() ==
+'hello': bot.send_text(message.chat_id(), f"**Hello** ``{message.author_title
+()}`` ! __This is a__ --test-- ~~message from~~ @@Pyrubi Library@@(https://
+example.com).", message.message_id()) ```
 ===============================================================================
 ### Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
 ## Rubika : @pyrubika ### Install or Update: ``` bash pip install -U pyrubi ```
```

### Comparing `pyrubi-2.1.0/setup.py` & `pyrubi-2.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pyrubi',
-    version = '2.1.0',
+    version = '2.1.1',
     author='Ali Ganji zadeh',
     author_email = 'ali.ganji.za@gmail.com',
     description = 'This is a powerful and easy library for building self Bots in Rubika',
-    keywords = ['rubika', 'rubino', 'pyrubi', 'pyrubika', 'rubx', 'rubika.ir', 'bot', 'chat'],
+    keywords = ['rubika', 'rubika-bot', 'pyrubi', 'rubx', 'rubino', 'rubika.ir', 'bot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/AliGanji1/pyrubi',
     packages = find_packages(),
-    install_requires = ['pycryptodome', 'websocket-client', 'requests', 'aiohttp', 'urllib3', 'pillow', 'mutagen', 'tinytag'],
+    install_requires = ['pycryptodome', 'websocket-client', 'requests', 'urllib3', 'pillow', 'mutagen', 'tinytag'],
     classifiers = [
     	"Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ]
 )
```


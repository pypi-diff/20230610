# Comparing `tmp/promptengine_catapult-0.0.9.tar.gz` & `tmp/promptengine_catapult-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptengine_catapult-0.0.9.tar", last modified: Sat Jun 10 08:33:56 2023, max compression
+gzip compressed data, was "promptengine_catapult-0.1.0.tar", last modified: Sat Jun 10 08:51:15 2023, max compression
```

## Comparing `promptengine_catapult-0.0.9.tar` & `promptengine_catapult-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.0.9/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.0.9/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/promptengine_catapult/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       66 2023-06-10 08:22:59.000000 promptengine_catapult-0.0.9/promptengine_catapult/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.0.9/promptengine_catapult/config.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6390 2023-06-08 05:51:13.000000 promptengine_catapult-0.0.9/promptengine_catapult/prompt_engine.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      805 2023-06-08 06:01:44.000000 promptengine_catapult-0.0.9/promptengine_catapult/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-06-10 08:32:58.000000 promptengine_catapult-0.0.9/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:51:15.408736 promptengine_catapult-0.1.0/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.1.0/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-10 08:51:15.408736 promptengine_catapult-0.1.0/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.1.0/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:51:15.408736 promptengine_catapult-0.1.0/promptengine_catapult/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       39 2023-06-10 08:48:22.000000 promptengine_catapult-0.1.0/promptengine_catapult/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.1.0/promptengine_catapult/config.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6398 2023-06-10 08:49:31.000000 promptengine_catapult-0.1.0/promptengine_catapult/prompt_engine.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      805 2023-06-08 06:01:44.000000 promptengine_catapult-0.1.0/promptengine_catapult/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:51:15.408736 promptengine_catapult-0.1.0/promptengine_catapult.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-10 08:51:15.000000 promptengine_catapult-0.1.0/promptengine_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-10 08:51:15.000000 promptengine_catapult-0.1.0/promptengine_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-10 08:51:15.000000 promptengine_catapult-0.1.0/promptengine_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-06-10 08:51:15.000000 promptengine_catapult-0.1.0/promptengine_catapult.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-10 08:51:15.000000 promptengine_catapult-0.1.0/promptengine_catapult.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-10 08:51:15.408736 promptengine_catapult-0.1.0/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-06-10 08:50:08.000000 promptengine_catapult-0.1.0/setup.py
```

### Comparing `promptengine_catapult-0.0.9/LICENSE` & `promptengine_catapult-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.9/PKG-INFO` & `promptengine_catapult-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine_catapult
-Version: 0.0.9
+Version: 0.1.0
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.9/README.md` & `promptengine_catapult-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.9/promptengine_catapult/config.py` & `promptengine_catapult-0.1.0/promptengine_catapult/config.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.9/promptengine_catapult/prompt_engine.py` & `promptengine_catapult-0.1.0/promptengine_catapult/prompt_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 os.chdir(os.path.dirname(os.path.abspath(__file__)))
 import openai
 import redis
 import json
 import tiktoken
 import requests
 import config
-import utils
+from .utils import *
 import logging
 
 from dotenv import load_dotenv
 import io
 import openai
 from pydub import AudioSegment
 from pydub.playback import play
```

### Comparing `promptengine_catapult-0.0.9/promptengine_catapult/utils.py` & `promptengine_catapult-0.1.0/promptengine_catapult/utils.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.9/promptengine_catapult.egg-info/PKG-INFO` & `promptengine_catapult-0.1.0/promptengine_catapult.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine-catapult
-Version: 0.0.9
+Version: 0.1.0
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.9/setup.py` & `promptengine_catapult-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.9"
+VERSION = "0.1.0"
 DESCRIPTION = "PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model."
 LONG_DESCRIPTION = """
 PromptEngine is a Python library that provides an interface for conducting interview sessions using OpenAI's ChatGPT model. It allows you to interact with the AI assistant to simulate interview conversations and generate responses based on candidate input.
 """
 
 # Setting up
 setup(
```


# Comparing `tmp/promptengine_catapult-0.0.8.tar.gz` & `tmp/promptengine_catapult-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptengine_catapult-0.0.8.tar", last modified: Thu Jun  8 05:56:04 2023, max compression
+gzip compressed data, was "promptengine_catapult-0.0.9.tar", last modified: Sat Jun 10 08:33:56 2023, max compression
```

## Comparing `promptengine_catapult-0.0.8.tar` & `promptengine_catapult-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:56:04.626788 promptengine_catapult-0.0.8/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.0.8/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-08 05:56:04.626788 promptengine_catapult-0.0.8/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.0.8/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:56:04.626788 promptengine_catapult-0.0.8/promptengine_catapult/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-06-04 19:15:11.000000 promptengine_catapult-0.0.8/promptengine_catapult/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.0.8/promptengine_catapult/config.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6390 2023-06-08 05:51:13.000000 promptengine_catapult-0.0.8/promptengine_catapult/prompt_engine.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      805 2023-06-08 05:55:42.000000 promptengine_catapult-0.0.8/promptengine_catapult/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:56:04.626788 promptengine_catapult-0.0.8/promptengine_catapult.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-08 05:56:04.000000 promptengine_catapult-0.0.8/promptengine_catapult.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-08 05:56:04.000000 promptengine_catapult-0.0.8/promptengine_catapult.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-08 05:56:04.000000 promptengine_catapult-0.0.8/promptengine_catapult.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-06-08 05:56:04.000000 promptengine_catapult-0.0.8/promptengine_catapult.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-08 05:56:04.000000 promptengine_catapult-0.0.8/promptengine_catapult.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-08 05:56:04.626788 promptengine_catapult-0.0.8/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-06-08 05:55:56.000000 promptengine_catapult-0.0.8/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.0.9/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.0.9/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/promptengine_catapult/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       66 2023-06-10 08:22:59.000000 promptengine_catapult-0.0.9/promptengine_catapult/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.0.9/promptengine_catapult/config.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6390 2023-06-08 05:51:13.000000 promptengine_catapult-0.0.9/promptengine_catapult/prompt_engine.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      805 2023-06-08 06:01:44.000000 promptengine_catapult-0.0.9/promptengine_catapult/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-10 08:33:56.000000 promptengine_catapult-0.0.9/promptengine_catapult.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-10 08:33:56.948814 promptengine_catapult-0.0.9/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-06-10 08:32:58.000000 promptengine_catapult-0.0.9/setup.py
```

### Comparing `promptengine_catapult-0.0.8/LICENSE` & `promptengine_catapult-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.8/PKG-INFO` & `promptengine_catapult-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine_catapult
-Version: 0.0.8
+Version: 0.0.9
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.8/README.md` & `promptengine_catapult-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.8/promptengine_catapult/config.py` & `promptengine_catapult-0.0.9/promptengine_catapult/config.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.8/promptengine_catapult/prompt_engine.py` & `promptengine_catapult-0.0.9/promptengine_catapult/prompt_engine.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.8/promptengine_catapult/utils.py` & `promptengine_catapult-0.0.9/promptengine_catapult/utils.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.8/promptengine_catapult.egg-info/PKG-INFO` & `promptengine_catapult-0.0.9/promptengine_catapult.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine-catapult
-Version: 0.0.8
+Version: 0.0.9
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.8/setup.py` & `promptengine_catapult-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model."
 LONG_DESCRIPTION = """
 PromptEngine is a Python library that provides an interface for conducting interview sessions using OpenAI's ChatGPT model. It allows you to interact with the AI assistant to simulate interview conversations and generate responses based on candidate input.
 """
 
 # Setting up
 setup(
```


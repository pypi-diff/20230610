# Comparing `tmp/term-chatgpt-1.1.tar.gz` & `tmp/term-chatgpt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-chatgpt-1.1.tar", last modified: Sat Jun 10 14:44:24 2023, max compression
+gzip compressed data, was "term-chatgpt-1.1.1.tar", last modified: Sat Jun 10 15:03:25 2023, max compression
```

## Comparing `term-chatgpt-1.1.tar` & `term-chatgpt-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 14:44:24.858622 term-chatgpt-1.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     3410 2023-06-10 14:44:24.858622 term-chatgpt-1.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      683 2023-06-10 14:44:15.000000 term-chatgpt-1.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-10 14:44:24.858622 term-chatgpt-1.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      711 2023-06-10 14:43:45.000000 term-chatgpt-1.1/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 14:44:24.858622 term-chatgpt-1.1/term_chatgpt.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3410 2023-06-10 14:44:24.000000 term-chatgpt-1.1/term_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:44:24.000000 term-chatgpt-1.1/term_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-10 14:44:24.000000 term-chatgpt-1.1/term_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       51 2023-06-10 14:44:24.000000 term-chatgpt-1.1/term_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-10 14:44:24.000000 term-chatgpt-1.1/term_chatgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 14:44:24.858622 term-chatgpt-1.1/termgpt/
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:02:02.000000 term-chatgpt-1.1/termgpt/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1/termgpt/cmd.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1/termgpt/copilot.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2123 2023-06-10 14:11:05.000000 term-chatgpt-1.1/termgpt/main.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1/termgpt/term.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     3412 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1.1/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      685 2023-06-10 15:03:04.000000 term-chatgpt-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      713 2023-06-10 15:03:06.000000 term-chatgpt-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 15:03:25.429526 term-chatgpt-1.1.1/term_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3412 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       51 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-10 15:03:24.000000 term-chatgpt-1.1.1/term_chatgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-10 15:03:25.433526 term-chatgpt-1.1.1/termgpt/
+-rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:02:02.000000 term-chatgpt-1.1.1/termgpt/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1.1/termgpt/cmd.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1.1/termgpt/copilot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2123 2023-06-10 14:11:05.000000 term-chatgpt-1.1.1/termgpt/main.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1.1/termgpt/term.py
```

### Comparing `term-chatgpt-1.1/LICENSE` & `term-chatgpt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1/PKG-INFO` & `term-chatgpt-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-chatgpt
-Version: 1.1
+Version: 1.1.1
 Summary: Ask ChatGPT directly on your terminal! Fast & Free.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
         
         Copyright (c) 2023 AWeirdDev @ tw
```

### Comparing `term-chatgpt-1.1/README.md` & `term-chatgpt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1/pyproject.toml` & `term-chatgpt-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "term-chatgpt"
-version = "1.1"
+version = "1.1.1"
 description = "Ask ChatGPT directly on your terminal! Fast & Free."
 authors = [{"name"="AWeirdDev"}]
 keywords=["chatgpt", "gpt", "free", "terminal", "textual", "rich", "chat-gpt", "ai"]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `term-chatgpt-1.1/setup.py` & `term-chatgpt-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
   name="term-chatgpt",
   authors="AWeirdDev",
-  version="1.1",
+  version="1.1.1",
   license="MIT License",
   description="Ask ChatGPT directly on your terminal! Fast & Free.",
   long_description=open("README.md", "r", encoding="utf-8").read(),
   author_email="aweirdscratcher@gmail.com",
   packages=['termgpt'],
   classifiers=[
     "Programming Language :: Python :: 3.10",
```

### Comparing `term-chatgpt-1.1/term_chatgpt.egg-info/PKG-INFO` & `term-chatgpt-1.1.1/term_chatgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-chatgpt
-Version: 1.1
+Version: 1.1.1
 Summary: Ask ChatGPT directly on your terminal! Fast & Free.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
         
         Copyright (c) 2023 AWeirdDev @ tw
```

### Comparing `term-chatgpt-1.1/termgpt/cmd.py` & `term-chatgpt-1.1.1/termgpt/cmd.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1/termgpt/copilot.py` & `term-chatgpt-1.1.1/termgpt/copilot.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1/termgpt/main.py` & `term-chatgpt-1.1.1/termgpt/main.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1/termgpt/term.py` & `term-chatgpt-1.1.1/termgpt/term.py`

 * *Files identical despite different names*


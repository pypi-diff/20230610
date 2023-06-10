# Comparing `tmp/pair_ai-0.5.8.tar.gz` & `tmp/pair_ai-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pair_ai-0.5.8.tar", last modified: Sat Mar 25 21:00:48 2023, max compression
+gzip compressed data, was "pair_ai-0.5.9.tar", last modified: Sat Mar 25 21:25:44 2023, max compression
```

## Comparing `pair_ai-0.5.8.tar` & `pair_ai-0.5.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 amy        (501) staff       (20)        0 2023-03-25 21:00:48.237836 pair_ai-0.5.8/
--rw-r--r--   0 amy        (501) staff       (20)    11357 2023-03-21 18:18:58.000000 pair_ai-0.5.8/LICENSE
--rw-r--r--   0 amy        (501) staff       (20)       73 2023-03-25 21:00:48.238042 pair_ai-0.5.8/PKG-INFO
--rw-r--r--   0 amy        (501) staff       (20)     2678 2023-03-25 20:42:21.000000 pair_ai-0.5.8/README.md
-drwxr-xr-x   0 amy        (501) staff       (20)        0 2023-03-25 21:00:48.225912 pair_ai-0.5.8/pair_ai/
--rw-r--r--   0 amy        (501) staff       (20)        0 2023-03-21 18:18:58.000000 pair_ai-0.5.8/pair_ai/__init__.py
--rw-r--r--   0 amy        (501) staff       (20)      750 2023-03-25 20:24:19.000000 pair_ai-0.5.8/pair_ai/exceptions.py
--rw-r--r--   0 amy        (501) staff       (20)     3036 2023-03-25 20:21:11.000000 pair_ai-0.5.8/pair_ai/extract.py
--rw-r--r--   0 amy        (501) staff       (20)     1212 2023-03-25 20:30:18.000000 pair_ai-0.5.8/pair_ai/github_api.py
--rwxr-xr-x   0 amy        (501) staff       (20)     7533 2023-03-25 20:40:54.000000 pair_ai-0.5.8/pair_ai/pair.py
--rw-r--r--   0 amy        (501) staff       (20)      509 2023-03-25 20:22:43.000000 pair_ai-0.5.8/pair_ai/pdf_text.py
--rw-r--r--   0 amy        (501) staff       (20)     1786 2023-03-25 20:56:11.000000 pair_ai-0.5.8/pair_ai/retry.py
-drwxr-xr-x   0 amy        (501) staff       (20)        0 2023-03-25 21:00:48.237247 pair_ai-0.5.8/pair_ai.egg-info/
--rw-r--r--   0 amy        (501) staff       (20)       73 2023-03-25 21:00:48.000000 pair_ai-0.5.8/pair_ai.egg-info/PKG-INFO
--rw-r--r--   0 amy        (501) staff       (20)      366 2023-03-25 21:00:48.000000 pair_ai-0.5.8/pair_ai.egg-info/SOURCES.txt
--rw-r--r--   0 amy        (501) staff       (20)        1 2023-03-25 21:00:48.000000 pair_ai-0.5.8/pair_ai.egg-info/dependency_links.txt
--rw-r--r--   0 amy        (501) staff       (20)       43 2023-03-25 21:00:48.000000 pair_ai-0.5.8/pair_ai.egg-info/entry_points.txt
--rw-r--r--   0 amy        (501) staff       (20)      176 2023-03-25 21:00:48.000000 pair_ai-0.5.8/pair_ai.egg-info/requires.txt
--rw-r--r--   0 amy        (501) staff       (20)        8 2023-03-25 21:00:48.000000 pair_ai-0.5.8/pair_ai.egg-info/top_level.txt
--rw-r--r--   0 amy        (501) staff       (20)       90 2023-03-21 18:18:58.000000 pair_ai-0.5.8/pyproject.toml
--rw-r--r--   0 amy        (501) staff       (20)      419 2023-03-25 21:00:48.239167 pair_ai-0.5.8/setup.cfg
+drwxr-xr-x   0 amy        (501) staff       (20)        0 2023-03-25 21:25:44.489099 pair_ai-0.5.9/
+-rw-r--r--   0 amy        (501) staff       (20)    11357 2023-03-21 18:18:58.000000 pair_ai-0.5.9/LICENSE
+-rw-r--r--   0 amy        (501) staff       (20)       73 2023-03-25 21:25:44.489315 pair_ai-0.5.9/PKG-INFO
+-rw-r--r--   0 amy        (501) staff       (20)     2678 2023-03-25 20:42:21.000000 pair_ai-0.5.9/README.md
+drwxr-xr-x   0 amy        (501) staff       (20)        0 2023-03-25 21:25:44.407356 pair_ai-0.5.9/pair_ai/
+-rw-r--r--   0 amy        (501) staff       (20)        0 2023-03-21 18:18:58.000000 pair_ai-0.5.9/pair_ai/__init__.py
+-rw-r--r--   0 amy        (501) staff       (20)      750 2023-03-25 20:24:19.000000 pair_ai-0.5.9/pair_ai/exceptions.py
+-rw-r--r--   0 amy        (501) staff       (20)     3038 2023-03-25 21:22:27.000000 pair_ai-0.5.9/pair_ai/extract.py
+-rw-r--r--   0 amy        (501) staff       (20)     1212 2023-03-25 20:30:18.000000 pair_ai-0.5.9/pair_ai/github_api.py
+-rwxr-xr-x   0 amy        (501) staff       (20)     7534 2023-03-25 21:21:32.000000 pair_ai-0.5.9/pair_ai/pair.py
+-rw-r--r--   0 amy        (501) staff       (20)      509 2023-03-25 20:22:43.000000 pair_ai-0.5.9/pair_ai/pdf_text.py
+-rw-r--r--   0 amy        (501) staff       (20)     1786 2023-03-25 20:56:11.000000 pair_ai-0.5.9/pair_ai/retry.py
+drwxr-xr-x   0 amy        (501) staff       (20)        0 2023-03-25 21:25:44.483738 pair_ai-0.5.9/pair_ai.egg-info/
+-rw-r--r--   0 amy        (501) staff       (20)       73 2023-03-25 21:25:44.000000 pair_ai-0.5.9/pair_ai.egg-info/PKG-INFO
+-rw-r--r--   0 amy        (501) staff       (20)      366 2023-03-25 21:25:44.000000 pair_ai-0.5.9/pair_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 amy        (501) staff       (20)        1 2023-03-25 21:25:44.000000 pair_ai-0.5.9/pair_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 amy        (501) staff       (20)       43 2023-03-25 21:25:44.000000 pair_ai-0.5.9/pair_ai.egg-info/entry_points.txt
+-rw-r--r--   0 amy        (501) staff       (20)      176 2023-03-25 21:25:44.000000 pair_ai-0.5.9/pair_ai.egg-info/requires.txt
+-rw-r--r--   0 amy        (501) staff       (20)        8 2023-03-25 21:25:44.000000 pair_ai-0.5.9/pair_ai.egg-info/top_level.txt
+-rw-r--r--   0 amy        (501) staff       (20)       90 2023-03-21 18:18:58.000000 pair_ai-0.5.9/pyproject.toml
+-rw-r--r--   0 amy        (501) staff       (20)      419 2023-03-25 21:25:44.519697 pair_ai-0.5.9/setup.cfg
```

### Comparing `pair_ai-0.5.8/LICENSE` & `pair_ai-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pair_ai-0.5.8/README.md` & `pair_ai-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pair_ai-0.5.8/pair_ai/exceptions.py` & `pair_ai-0.5.9/pair_ai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pair_ai-0.5.8/pair_ai/extract.py` & `pair_ai-0.5.9/pair_ai/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 
 from loguru import logger
 from bs4 import BeautifulSoup, NavigableString, Tag
 from readability import Document    # https://github.com/buriy/python-readability
 import requests
 import urllib.parse
 
-from github_api import github_readme_text
-from pdf_text import pdf_text
-
-from exceptions import *
+from .github_api import github_readme_text
+from .pdf_text import pdf_text
+from .exceptions import *
     
 user_agent = "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"
 
 headers = {'User-Agent': user_agent}
 
 def extract_text_from_html(content):
     soup = BeautifulSoup(content, 'html.parser')
```

### Comparing `pair_ai-0.5.8/pair_ai/github_api.py` & `pair_ai-0.5.9/pair_ai/github_api.py`

 * *Files identical despite different names*

### Comparing `pair_ai-0.5.8/pair_ai/pair.py` & `pair_ai-0.5.9/pair_ai/pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from prompt_toolkit.completion import Completer, Completion, PathCompleter, NestedCompleter, WordCompleter
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit import print_formatted_text
 import re
 import subprocess
-from extract import url_to_text
+from .extract import url_to_text
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
 
 BASE_PROMPT = "You are a programming assistant. "
 BASE_PROMPT += "The below are portions of code the user is working on as well as questions from the user. "
 BASE_PROMPT += "Provide helpful answers to the user. If you need more information on code that is not included, "
```

### Comparing `pair_ai-0.5.8/pair_ai/retry.py` & `pair_ai-0.5.9/pair_ai/retry.py`

 * *Files identical despite different names*


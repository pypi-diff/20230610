# Comparing `tmp/FLOBOT-0.1.117.tar.gz` & `tmp/FLOBOT-0.1.118.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLOBOT-0.1.117.tar", last modified: Sat Jun 10 12:58:26 2023, max compression
+gzip compressed data, was "FLOBOT-0.1.118.tar", last modified: Sat Jun 10 19:47:55 2023, max compression
```

## Comparing `FLOBOT-0.1.117.tar` & `FLOBOT-0.1.118.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:58:26.655565 FLOBOT-0.1.117/
-drwxrwxrwx   0        0        0        0 2023-06-10 12:58:26.591938 FLOBOT-0.1.117/FLOBOT/
--rw-rw-rw-   0        0        0    54302 2023-06-10 12:56:55.000000 FLOBOT-0.1.117/FLOBOT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 12:58:26.639858 FLOBOT-0.1.117/FLOBOT.egg-info/
--rw-rw-rw-   0        0        0      277 2023-06-10 12:58:24.000000 FLOBOT-0.1.117/FLOBOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-10 12:58:24.000000 FLOBOT-0.1.117/FLOBOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:58:24.000000 FLOBOT-0.1.117/FLOBOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-06-10 12:58:24.000000 FLOBOT-0.1.117/FLOBOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 12:58:24.000000 FLOBOT-0.1.117/FLOBOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-06-10 12:58:26.639858 FLOBOT-0.1.117/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-10 12:58:26.655565 FLOBOT-0.1.117/setup.cfg
--rw-rw-rw-   0        0        0      590 2023-06-10 12:56:53.000000 FLOBOT-0.1.117/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:47:55.895128 FLOBOT-0.1.118/
+drwxrwxrwx   0        0        0        0 2023-06-10 19:47:55.825838 FLOBOT-0.1.118/FLOBOT/
+-rw-rw-rw-   0        0        0    54303 2023-06-10 19:46:39.000000 FLOBOT-0.1.118/FLOBOT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:47:55.879017 FLOBOT-0.1.118/FLOBOT.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-06-10 19:47:55.000000 FLOBOT-0.1.118/FLOBOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-10 19:47:55.000000 FLOBOT-0.1.118/FLOBOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 19:47:55.000000 FLOBOT-0.1.118/FLOBOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-06-10 19:47:55.000000 FLOBOT-0.1.118/FLOBOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 19:47:55.000000 FLOBOT-0.1.118/FLOBOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      277 2023-06-10 19:47:55.888080 FLOBOT-0.1.118/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-10 19:47:55.895128 FLOBOT-0.1.118/setup.cfg
+-rw-rw-rw-   0        0        0      590 2023-06-10 19:46:48.000000 FLOBOT-0.1.118/setup.py
```

### Comparing `FLOBOT-0.1.117/FLOBOT/__init__.py` & `FLOBOT-0.1.118/FLOBOT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-try:
+atry:
     # System imports.
     from typing import Tuple, Any, Union, Optional
 
     import asyncio
     import sys
     import datetime
     import json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-try: # System imports. from typing import Tuple, Any, Union, Optional import
+atry: # System imports. from typing import Tuple, Any, Union, Optional import
 asyncio import sys import datetime import json import functools import os
 import random as py_random import logging import uuid import json import
 subprocess # Third party imports. from fortnitepy.ext import commands from
 colorama import Fore, Back, Style, init init(autoreset=True) from functools
 import partial from datetime import timedelta import crayons try: import
 PirxcyPinger except: pass import fortnitepy import BenBotAsync import
 FortniteAPIAsync import sanic import aiohttp import uvloop import requests
```

### Comparing `FLOBOT-0.1.117/setup.py` & `FLOBOT-0.1.118/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
     
 setuptools.setup(
     name="FLOBOT",
-    version="0.1.117",
+    version="0.1.118",
     author="Sekkay",
     description="Lobby bot.",
     url="https://www.youtube.com",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```


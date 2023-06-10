# Comparing `tmp/SEKKAYBOT-0.22.266.tar.gz` & `tmp/SEKKAYBOT-0.22.267.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SEKKAYBOT-0.22.266.tar", last modified: Fri Jun  9 11:57:10 2023, max compression
+gzip compressed data, was "SEKKAYBOT-0.22.267.tar", last modified: Sat Jun 10 12:58:26 2023, max compression
```

## Comparing `SEKKAYBOT-0.22.266.tar` & `SEKKAYBOT-0.22.267.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 11:57:10.681608 SEKKAYBOT-0.22.266/
--rw-rw-rw-   0        0        0      281 2023-06-09 11:57:10.649732 SEKKAYBOT-0.22.266/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 11:57:10.586023 SEKKAYBOT-0.22.266/SEKKAYBOT/
--rw-rw-rw-   0        0        0    54304 2023-06-09 11:55:55.000000 SEKKAYBOT-0.22.266/SEKKAYBOT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:57:10.649732 SEKKAYBOT-0.22.266/SEKKAYBOT.egg-info/
--rw-rw-rw-   0        0        0      281 2023-06-09 11:57:10.000000 SEKKAYBOT-0.22.266/SEKKAYBOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-09 11:57:10.000000 SEKKAYBOT-0.22.266/SEKKAYBOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 11:57:10.000000 SEKKAYBOT-0.22.266/SEKKAYBOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-09 11:57:10.000000 SEKKAYBOT-0.22.266/SEKKAYBOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 11:57:10.000000 SEKKAYBOT-0.22.266/SEKKAYBOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 11:57:10.681608 SEKKAYBOT-0.22.266/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-06-09 11:56:11.000000 SEKKAYBOT-0.22.266/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:58:26.862714 SEKKAYBOT-0.22.267/
+-rw-rw-rw-   0        0        0      281 2023-06-10 12:58:26.830830 SEKKAYBOT-0.22.267/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 12:58:26.727258 SEKKAYBOT-0.22.267/SEKKAYBOT/
+-rw-rw-rw-   0        0        0    54303 2023-06-10 12:56:56.000000 SEKKAYBOT-0.22.267/SEKKAYBOT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:58:26.830830 SEKKAYBOT-0.22.267/SEKKAYBOT.egg-info/
+-rw-rw-rw-   0        0        0      281 2023-06-10 12:58:25.000000 SEKKAYBOT-0.22.267/SEKKAYBOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-06-10 12:58:26.000000 SEKKAYBOT-0.22.267/SEKKAYBOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 12:58:25.000000 SEKKAYBOT-0.22.267/SEKKAYBOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-10 12:58:26.000000 SEKKAYBOT-0.22.267/SEKKAYBOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-10 12:58:26.000000 SEKKAYBOT-0.22.267/SEKKAYBOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 12:58:26.862714 SEKKAYBOT-0.22.267/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-06-10 12:56:54.000000 SEKKAYBOT-0.22.267/setup.py
```

### Comparing `SEKKAYBOT-0.22.266/SEKKAYBOT/__init__.py` & `SEKKAYBOT-0.22.267/SEKKAYBOT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-atry:
+try:
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
-atry: # System imports. from typing import Tuple, Any, Union, Optional import
+try: # System imports. from typing import Tuple, Any, Union, Optional import
 asyncio import sys import datetime import json import functools import os
 import random as py_random import logging import uuid import json import
 subprocess # Third party imports. from fortnitepy.ext import commands from
 colorama import Fore, Back, Style, init init(autoreset=True) from functools
 import partial from datetime import timedelta import crayons try: import
 PirxcyPinger except: pass import fortnitepy import BenBotAsync import
 FortniteAPIAsync import sanic import aiohttp import uvloop import requests
```

### Comparing `SEKKAYBOT-0.22.266/setup.py` & `SEKKAYBOT-0.22.267/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
     
 setuptools.setup(
     name="SEKKAYBOT",
-    version="0.22.266",
+    version="0.22.267",
     author="Sekkay",
     description="Lobby bot.",
     url="https://www.youtube.com",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```


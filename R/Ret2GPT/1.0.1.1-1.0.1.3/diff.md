# Comparing `tmp/Ret2GPT-1.0.1.1.tar.gz` & `tmp/Ret2GPT-1.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ret2GPT-1.0.1.1.tar", last modified: Sat Jun 10 02:31:04 2023, max compression
+gzip compressed data, was "Ret2GPT-1.0.1.3.tar", last modified: Sat Jun 10 02:40:35 2023, max compression
```

## Comparing `Ret2GPT-1.0.1.1.tar` & `Ret2GPT-1.0.1.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:31:04.710000 Ret2GPT-1.0.1.1/
--rwxrwxrwx   0 retr0      (501) staff       (20)       33 2023-06-10 02:30:19.000000 Ret2GPT-1.0.1.1/MANIFEST.in
--rwxrwxrwx   0 retr0      (501) staff       (20)      379 2023-06-10 02:31:04.720000 Ret2GPT-1.0.1.1/PKG-INFO
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:31:04.710000 Ret2GPT-1.0.1.1/Ret2GPT/
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:31:04.710000 Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/
--rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:22:26.000000 Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/__init__.py
--rwxrwxrwx   0 retr0      (501) staff       (20)     3503 2023-06-10 01:25:02.000000 Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/check_for_command.py
--rwxrwxrwx   0 retr0      (501) staff       (20)     4764 2023-06-10 02:28:55.000000 Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/command_line.py
--rwxrwxrwx   0 retr0      (501) staff       (20)      599 2023-06-10 01:25:02.000000 Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/decompile.py
--rwxrwxrwx   0 retr0      (501) staff       (20)     9607 2023-06-10 01:40:24.000000 Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/prompt_builder.py
--rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 01:49:08.000000 Ret2GPT-1.0.1.1/Ret2GPT/__init__.py
--rwxrwxrwx   0 retr0      (501) staff       (20)       89 2023-06-10 01:49:15.000000 Ret2GPT-1.0.1.1/Ret2GPT/main.py
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:31:04.710000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/
--rwxrwxrwx   0 retr0      (501) staff       (20)      379 2023-06-10 02:31:04.000000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/PKG-INFO
--rwxrwxrwx   0 retr0      (501) staff       (20)      434 2023-06-10 02:31:04.000000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/SOURCES.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:31:04.000000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/dependency_links.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)       46 2023-06-10 02:31:04.000000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/entry_points.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:01:44.000000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/not-zip-safe
--rwxrwxrwx   0 retr0      (501) staff       (20)       64 2023-06-10 02:31:04.000000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/requires.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)        8 2023-06-10 02:31:04.000000 Ret2GPT-1.0.1.1/Ret2GPT.egg-info/top_level.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)       38 2023-06-10 02:31:04.720000 Ret2GPT-1.0.1.1/setup.cfg
--rwxrwxrwx   0 retr0      (501) staff       (20)      884 2023-06-10 02:30:35.000000 Ret2GPT-1.0.1.1/setup.py
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:40:35.650000 Ret2GPT-1.0.1.3/
+-rwxrwxrwx   0 retr0      (501) staff       (20)      379 2023-06-10 02:40:35.670000 Ret2GPT-1.0.1.3/PKG-INFO
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:40:35.650000 Ret2GPT-1.0.1.3/Ret2GPT/
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:40:35.660000 Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/
+-rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:22:26.000000 Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/__init__.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)     3503 2023-06-10 01:25:02.000000 Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/check_for_command.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)     4753 2023-06-10 02:35:21.000000 Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/command_line.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)      599 2023-06-10 01:25:02.000000 Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/decompile.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)     9607 2023-06-10 01:40:24.000000 Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/prompt_builder.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 01:49:08.000000 Ret2GPT-1.0.1.3/Ret2GPT/__init__.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)       89 2023-06-10 01:49:15.000000 Ret2GPT-1.0.1.3/Ret2GPT/main.py
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:40:35.650000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/
+-rwxrwxrwx   0 retr0      (501) staff       (20)      379 2023-06-10 02:40:35.000000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/PKG-INFO
+-rwxrwxrwx   0 retr0      (501) staff       (20)      422 2023-06-10 02:40:35.000000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/SOURCES.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:40:35.000000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/dependency_links.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)       46 2023-06-10 02:40:35.000000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/entry_points.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:01:44.000000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/not-zip-safe
+-rwxrwxrwx   0 retr0      (501) staff       (20)       64 2023-06-10 02:40:35.000000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/requires.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)        8 2023-06-10 02:40:35.000000 Ret2GPT-1.0.1.3/Ret2GPT.egg-info/top_level.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)       38 2023-06-10 02:40:35.670000 Ret2GPT-1.0.1.3/setup.cfg
+-rwxrwxrwx   0 retr0      (501) staff       (20)      884 2023-06-10 02:39:46.000000 Ret2GPT-1.0.1.3/setup.py
```

### Comparing `Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/check_for_command.py` & `Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/check_for_command.py`

 * *Files identical despite different names*

### Comparing `Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/command_line.py` & `Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from Ret2GPT import prompt_builder as pwnchain
-from Ret2GPT import decompile as retdec
+from . import prompt_builder as pwnchain
+from . import decompile as retdec
+
 import builtins
 import logging
 
 from rich.console import Console
 from rich import print
 from enrich.console import Console
```

### Comparing `Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/decompile.py` & `Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/decompile.py`

 * *Files identical despite different names*

### Comparing `Ret2GPT-1.0.1.1/Ret2GPT/Ret2GPT/prompt_builder.py` & `Ret2GPT-1.0.1.3/Ret2GPT/Ret2GPT/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `Ret2GPT-1.0.1.1/setup.py` & `Ret2GPT-1.0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-str_version = '1.0.1.1'
+str_version = '1.0.1.3'
 name = 'Ret2GPT'
 requires_list = open(f'{name}/requirements.txt', 'r', encoding='utf8').readlines()
 requires_list = [i.strip() for i in requires_list]
 
 setup(name='Ret2GPT',
       version=str_version,
       description='Ret2GPT: Advanced AI-powered binary analysis tool leveraging OpenAI\'s LangChain technology, revolutionizing CTF Pwners\' experience in binary file interpretation and vulnerability detection.',
```


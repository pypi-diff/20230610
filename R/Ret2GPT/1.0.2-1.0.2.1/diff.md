# Comparing `tmp/Ret2GPT-1.0.2.tar.gz` & `tmp/Ret2GPT-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ret2GPT-1.0.2.tar", last modified: Sat Jun 10 02:54:19 2023, max compression
+gzip compressed data, was "Ret2GPT-1.0.2.1.tar", last modified: Sat Jun 10 02:58:53 2023, max compression
```

## Comparing `Ret2GPT-1.0.2.tar` & `Ret2GPT-1.0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:54:19.970000 Ret2GPT-1.0.2/
--rwxrwxrwx   0 retr0      (501) staff       (20)      380 2023-06-10 02:54:19.980000 Ret2GPT-1.0.2/PKG-INFO
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:54:19.970000 Ret2GPT-1.0.2/Ret2GPT/
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:54:19.970000 Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/
--rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:22:26.000000 Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/__init__.py
--rwxrwxrwx   0 retr0      (501) staff       (20)     3503 2023-06-10 01:25:02.000000 Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/check_for_command.py
--rwxrwxrwx   0 retr0      (501) staff       (20)     4789 2023-06-10 02:44:39.000000 Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/command_line.py
--rwxrwxrwx   0 retr0      (501) staff       (20)      599 2023-06-10 01:25:02.000000 Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/decompile.py
--rwxrwxrwx   0 retr0      (501) staff       (20)     9607 2023-06-10 01:40:24.000000 Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/prompt_builder.py
--rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 01:49:08.000000 Ret2GPT-1.0.2/Ret2GPT/__init__.py
--rwxrwxrwx   0 retr0      (501) staff       (20)      120 2023-06-10 02:43:14.000000 Ret2GPT-1.0.2/Ret2GPT/main.py
-drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:54:19.970000 Ret2GPT-1.0.2/Ret2GPT.egg-info/
--rwxrwxrwx   0 retr0      (501) staff       (20)      380 2023-06-10 02:54:19.000000 Ret2GPT-1.0.2/Ret2GPT.egg-info/PKG-INFO
--rwxrwxrwx   0 retr0      (501) staff       (20)      422 2023-06-10 02:54:19.000000 Ret2GPT-1.0.2/Ret2GPT.egg-info/SOURCES.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:54:19.000000 Ret2GPT-1.0.2/Ret2GPT.egg-info/dependency_links.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)       46 2023-06-10 02:54:19.000000 Ret2GPT-1.0.2/Ret2GPT.egg-info/entry_points.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:01:44.000000 Ret2GPT-1.0.2/Ret2GPT.egg-info/not-zip-safe
--rwxrwxrwx   0 retr0      (501) staff       (20)       77 2023-06-10 02:54:19.000000 Ret2GPT-1.0.2/Ret2GPT.egg-info/requires.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)        8 2023-06-10 02:54:19.000000 Ret2GPT-1.0.2/Ret2GPT.egg-info/top_level.txt
--rwxrwxrwx   0 retr0      (501) staff       (20)       38 2023-06-10 02:54:19.980000 Ret2GPT-1.0.2/setup.cfg
--rwxrwxrwx   0 retr0      (501) staff       (20)      885 2023-06-10 02:54:16.000000 Ret2GPT-1.0.2/setup.py
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:58:53.750000 Ret2GPT-1.0.2.1/
+-rwxrwxrwx   0 retr0      (501) staff       (20)      382 2023-06-10 02:58:53.750000 Ret2GPT-1.0.2.1/PKG-INFO
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:58:53.750000 Ret2GPT-1.0.2.1/Ret2GPT/
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:58:53.750000 Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/
+-rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:22:26.000000 Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/__init__.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)     3503 2023-06-10 01:25:02.000000 Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/check_for_command.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)     4789 2023-06-10 02:44:39.000000 Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/command_line.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)      599 2023-06-10 01:25:02.000000 Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/decompile.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)     9607 2023-06-10 01:40:24.000000 Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/prompt_builder.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 01:49:08.000000 Ret2GPT-1.0.2.1/Ret2GPT/__init__.py
+-rwxrwxrwx   0 retr0      (501) staff       (20)      120 2023-06-10 02:43:14.000000 Ret2GPT-1.0.2.1/Ret2GPT/main.py
+drwxrwxrwx   0 retr0      (501) staff       (20)        0 2023-06-10 02:58:53.750000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/
+-rwxrwxrwx   0 retr0      (501) staff       (20)      382 2023-06-10 02:58:53.000000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/PKG-INFO
+-rwxrwxrwx   0 retr0      (501) staff       (20)      422 2023-06-10 02:58:53.000000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/SOURCES.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:58:53.000000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/dependency_links.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)       46 2023-06-10 02:58:53.000000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/entry_points.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)        1 2023-06-10 02:01:44.000000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/not-zip-safe
+-rwxrwxrwx   0 retr0      (501) staff       (20)       77 2023-06-10 02:58:53.000000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/requires.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)        8 2023-06-10 02:58:53.000000 Ret2GPT-1.0.2.1/Ret2GPT.egg-info/top_level.txt
+-rwxrwxrwx   0 retr0      (501) staff       (20)       38 2023-06-10 02:58:53.750000 Ret2GPT-1.0.2.1/setup.cfg
+-rwxrwxrwx   0 retr0      (501) staff       (20)      887 2023-06-10 02:58:39.000000 Ret2GPT-1.0.2.1/setup.py
```

### Comparing `Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/check_for_command.py` & `Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/check_for_command.py`

 * *Files identical despite different names*

### Comparing `Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/command_line.py` & `Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/command_line.py`

 * *Files identical despite different names*

### Comparing `Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/decompile.py` & `Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/decompile.py`

 * *Files identical despite different names*

### Comparing `Ret2GPT-1.0.2/Ret2GPT/Ret2GPT/prompt_builder.py` & `Ret2GPT-1.0.2.1/Ret2GPT/Ret2GPT/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `Ret2GPT-1.0.2/setup.py` & `Ret2GPT-1.0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-str_version = '1.0.2'
+str_version = '1.0.2.1'
 name = 'Ret2GPT'
 requires_list = open(f'{name}/requirements.txt', 'r', encoding='utf8').readlines()
 requires_list = [i.strip() for i in requires_list]
 
 setup(name='Ret2GPT',
       version=str_version,
       description='Ret2GPT: Advanced AI-powered binary analysis tool leveraging OpenAI\'s LangChain technology, revolutionizing CTF Pwners\' experience in binary file interpretation and vulnerability detection.',
```


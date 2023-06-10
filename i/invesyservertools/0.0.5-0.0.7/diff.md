# Comparing `tmp/invesyservertools-0.0.5.tar.gz` & `tmp/invesyservertools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invesyservertools-0.0.5.tar", last modified: Fri Dec  9 17:52:15 2022, max compression
+gzip compressed data, was "dist/invesyservertools-0.0.7.tar", last modified: Sat Jun 10 12:08:02 2023, max compression
```

## Comparing `invesyservertools-0.0.5.tar` & `invesyservertools-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2022-12-09 17:52:15.107336 invesyservertools-0.0.5/
--rw-r--r--   0 georg      (502) staff       (20)     1050 2022-04-20 10:44:14.000000 invesyservertools-0.0.5/LICENSE.txt
--rw-r--r--   0 georg      (502) staff       (20)     2257 2022-12-09 17:52:15.107660 invesyservertools-0.0.5/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)      971 2022-06-13 09:19:16.000000 invesyservertools-0.0.5/README.md
--rw-r--r--   0 georg      (502) staff       (20)      823 2022-12-09 17:52:15.108528 invesyservertools-0.0.5/setup.cfg
--rw-r--r--   0 georg      (502) staff       (20)       69 2022-06-08 20:27:46.000000 invesyservertools-0.0.5/setup.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2022-12-09 17:52:15.097967 invesyservertools-0.0.5/src/
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2022-12-09 17:52:15.102152 invesyservertools-0.0.5/src/invesyservertools/
--rw-r--r--   0 georg      (502) staff       (20)      363 2022-12-09 16:17:01.000000 invesyservertools-0.0.5/src/invesyservertools/__init__.py
--rw-r--r--   0 georg      (502) staff       (20)     1060 2022-12-09 14:04:09.000000 invesyservertools-0.0.5/src/invesyservertools/interactive_tools.py
--rw-r--r--   0 georg      (502) staff       (20)     5109 2022-12-09 14:04:17.000000 invesyservertools-0.0.5/src/invesyservertools/print_tools.py
--rw-r--r--   0 georg      (502) staff       (20)      966 2022-12-09 14:04:01.000000 invesyservertools-0.0.5/src/invesyservertools/system_tools.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2022-12-09 17:52:15.104480 invesyservertools-0.0.5/src/invesyservertools.egg-info/
--rw-r--r--   0 georg      (502) staff       (20)     2257 2022-12-09 17:52:14.000000 invesyservertools-0.0.5/src/invesyservertools.egg-info/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)      487 2022-12-09 17:52:15.000000 invesyservertools-0.0.5/src/invesyservertools.egg-info/SOURCES.txt
--rw-r--r--   0 georg      (502) staff       (20)        1 2022-12-09 17:52:14.000000 invesyservertools-0.0.5/src/invesyservertools.egg-info/dependency_links.txt
--rw-r--r--   0 georg      (502) staff       (20)        9 2022-12-09 17:52:14.000000 invesyservertools-0.0.5/src/invesyservertools.egg-info/requires.txt
--rw-r--r--   0 georg      (502) staff       (20)       24 2022-12-09 17:52:14.000000 invesyservertools-0.0.5/src/invesyservertools.egg-info/top_level.txt
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2022-12-09 17:52:15.106457 invesyservertools-0.0.5/src/tests/
--rw-r--r--   0 georg      (502) staff       (20)        1 2022-06-09 11:45:01.000000 invesyservertools-0.0.5/src/tests/__init__.py
--rwxr--r--   0 georg      (502) staff       (20)      843 2022-08-23 12:05:52.000000 invesyservertools-0.0.5/src/tests/test_print.py
--rwxr--r--   0 georg      (502) staff       (20)     1178 2022-08-23 12:03:07.000000 invesyservertools-0.0.5/src/tests/test_system.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.856760 invesyservertools-0.0.7/
+-rw-r--r--   0 georg      (502) staff       (20)     1050 2022-04-20 10:44:14.000000 invesyservertools-0.0.7/LICENSE.txt
+-rw-r--r--   0 georg      (502) staff       (20)     2403 2023-06-10 12:08:02.856948 invesyservertools-0.0.7/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)      971 2022-06-13 09:19:16.000000 invesyservertools-0.0.7/README.md
+-rw-r--r--   0 georg      (502) staff       (20)      823 2023-06-10 12:08:02.857884 invesyservertools-0.0.7/setup.cfg
+-rw-r--r--   0 georg      (502) staff       (20)       69 2022-06-08 20:27:46.000000 invesyservertools-0.0.7/setup.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.846997 invesyservertools-0.0.7/src/
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.852165 invesyservertools-0.0.7/src/invesyservertools/
+-rw-r--r--   0 georg      (502) staff       (20)      363 2022-12-09 16:17:01.000000 invesyservertools-0.0.7/src/invesyservertools/__init__.py
+-rw-r--r--   0 georg      (502) staff       (20)     1114 2023-06-10 11:56:34.000000 invesyservertools-0.0.7/src/invesyservertools/interactive_tools.py
+-rw-r--r--   0 georg      (502) staff       (20)     5739 2023-06-10 12:07:11.000000 invesyservertools-0.0.7/src/invesyservertools/print_tools.py
+-rw-r--r--   0 georg      (502) staff       (20)      987 2023-06-10 11:48:16.000000 invesyservertools-0.0.7/src/invesyservertools/system_tools.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.854382 invesyservertools-0.0.7/src/invesyservertools.egg-info/
+-rw-r--r--   0 georg      (502) staff       (20)     2403 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)      487 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/SOURCES.txt
+-rw-r--r--   0 georg      (502) staff       (20)        1 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/dependency_links.txt
+-rw-r--r--   0 georg      (502) staff       (20)        9 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/requires.txt
+-rw-r--r--   0 georg      (502) staff       (20)       24 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/top_level.txt
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.856193 invesyservertools-0.0.7/src/tests/
+-rw-r--r--   0 georg      (502) staff       (20)        1 2022-06-09 11:45:01.000000 invesyservertools-0.0.7/src/tests/__init__.py
+-rwxr--r--   0 georg      (502) staff       (20)      849 2023-06-10 12:05:24.000000 invesyservertools-0.0.7/src/tests/test_print.py
+-rwxr--r--   0 georg      (502) staff       (20)     1178 2022-08-23 12:03:07.000000 invesyservertools-0.0.7/src/tests/test_system.py
```

### Comparing `invesyservertools-0.0.5/LICENSE.txt` & `invesyservertools-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invesyservertools-0.0.5/PKG-INFO` & `invesyservertools-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invesyservertools
-Version: 0.0.5
+Version: 0.0.7
 Summary: Tools for Python scripts or terminal
 Home-page: https://gitlab.com/Rastaf/invesyservertools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/Rastaf/invesyservertools/-/issues
 Platform: UNKNOWN
@@ -35,14 +35,20 @@
 - **format_filesize**: return a human-readable filesize, like `31.9 GiB`.
 
 ## system_tools
 - **get_username**: get the username in the operating system
 - **get\_home\_dir**
 - **find\_file\_with\_path**: provide a filename and a start path to begin searching recursively, get the complete path including the filename
 # History
+## 0.0.7
+- **print_** checks for terminal (-> no colors, no wrapper)
+
+## 0.0.6
+- fixed IndexError in **print_** (for line ending in last string)
+
 ## 0.0.5 (2022-12-09)
 - fixed import of submodules
 
 ## 0.0.4 (2022-12-09)
 - *wait_for_key* gets a "indent" argument
 - Sphinx documentation
```

### Comparing `invesyservertools-0.0.5/README.md` & `invesyservertools-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `invesyservertools-0.0.5/setup.cfg` & `invesyservertools-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = invesyservertools
-version = 0.0.5
+version = 0.0.7
 author = Georg Pfolz
 author_email = georg.pfolz@invesy.at
 description = Tools for Python scripts or terminal
 long_description = file: README.md,HISTORY.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE.txt
```

### Comparing `invesyservertools-0.0.5/src/invesyservertools/interactive_tools.py` & `invesyservertools-0.0.7/src/invesyservertools/interactive_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 """
 =================
 interactive_tools
 =================
 """
 
 import sys
+from typing import Union, List, Tuple, Dict, Any
 from .print_tools import print_
 
 
 ## Wait for a key press on the console and return it
 def wait_for_key(
     text: str = 'continue: press any button',
+    list_bullet: Union(bool, str) = False,
     color: str = None,
-    list_bullet: (bool, str) = False,
     indent: int = None
 ) -> 'None or str':
     ''' Wait for a key press on the console and return it.'''
 
     if text:
         print_(
             text,
```

### Comparing `invesyservertools-0.0.5/src/invesyservertools/print_tools.py` & `invesyservertools-0.0.7/src/invesyservertools/print_tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 """
 ===========
 print_tools
 ===========
 """
 
 import os
+import sys
 import re
 import textwrap
 from colorama import Fore, Style
+from typing import Union, List, Tuple, Dict, Any
 
 LIST_BULLET = '-'
 COLOR_RESET = getattr(Style, 'RESET_ALL')
 
 INDENT_MULT = 4
 INDENT_BASE = 4 * ' '
 
@@ -66,52 +68,67 @@
 #   @param style
 #   @param sep: as in print function
 #   @param end: as in print function
 #   @param ignore: don't print (but possibly log)
 #   @param flush: as in print function
 #   @param nowrapper: don't use textwrap
 def print_(
-    *texts: list,
+    *texts: List[str],
     logging: bool = False,
     indent: int = 0,
-    list_bullet: (bool, str) = '',
-    color: (str, dict) = '',
+    list_bullet: Union[bool, str] = '',
+    color: Union[str, Dict[int, str]] = '',
     style: str = '',
     sep: str = ' ',
     end: str = '\n',
     ignore: bool = False,
-    flush: bool = False,
-    nowrapper: bool = False
+    flush: bool = None,
+    nowrapper: bool = None
 ) -> None:
     """Enhanced print function"""
+    
+    # are we in a tty?
+    is_a_tty = sys.stdout.isatty()
+
+    if nowrapper is None:
+        nowrapper = not is_a_tty
+    if flush is None:
+        flush = not is_a_tty
 
     texts = [str(t) for t in texts]
 
     # we have line endings
     if any(
         ['\n' in t for t in texts]
     ):
         for i, t in enumerate(texts):
             if t.endswith('\n'):
-                texts[i + 1] = '\n' + texts[i + 1]  # update next string by adding line end
-                texts[i] = t[:-1]  # remove line end from current string
+                try:
+                    texts[i + 1] = '\n' + texts[i + 1]  # update next string by adding line end
+                    texts[i] = t[:-1]  # remove line end from current string
+                except IndexError:
+                    pass
+
         nowrapper = True
 
         texts = list(filter(None, texts))  # remove empty strings
 
     if logging:
         logging.info(sep.join(texts))
 
     if ignore:
         return
 
     colors = None
-    if isinstance(color, dict):
-        colors = color
-        color = None
+
+    # only use colors if stdout is a tty
+    if is_a_tty:
+        if isinstance(color, dict):
+            colors = color
+            color = None
 
     if len(texts):
         try:
             prefix = ' ' * indent
         except TypeError:
             prefix = indent or ''
 
@@ -145,26 +162,29 @@
                 list_bullet = LIST_BULLET
             else:
                 list_bullet = ''
 
         bullet_sep = ' '
         prefix += list_bullet + bullet_sep if list_bullet else ''
 
-        try:  # when there is no terminal, i.e. cron-job
-            term_rows, term_columns = map(
-                int,
-                os.popen('stty size', 'r').read().split()
-            )
-            wrapper = textwrap.TextWrapper(
-                initial_indent=prefix,
-                width=term_columns,
-                subsequent_indent=' ' * (len(prefix) - prefix_len_subtract)
-            )
-        except ValueError:
-            nowrapper = True
+        if is_a_tty:
+            # in case there is no terminal, i.e. cron-job
+            # not sure if this is still needed with the is_a_tty condition
+            try:
+                term_rows, term_columns = map(
+                    int,
+                    os.popen('stty size', 'r').read().split()
+                )
+                wrapper = textwrap.TextWrapper(
+                    initial_indent=prefix,
+                    width=term_columns,
+                    subsequent_indent=' ' * (len(prefix) - prefix_len_subtract)
+                )
+            except ValueError:
+                nowrapper = True
 
         if flush or nowrapper:
             print(
                 prefix + texts[0],
                 *texts[1:],
                 suffix,
                 sep=sep,
@@ -182,15 +202,19 @@
         print()
 
 
 ##  format file size
 #
 #   inspired by Fred Cirera, https://stackoverflow.com/a/1094933/1690805
 #   @param IEC: use binary prefixes as established by the International Electrotechnical Commission
-def format_filesize(num, suffix="B", prefix_type='binary'):
+def format_filesize(
+    num: Union[int, float],
+    suffix: str = "B",
+    prefix_type: str = 'binary'
+) -> str:
     divider = 1024.0 if prefix_type == 'binary' else 1000.0
 
     for unit in UNIT_PREFIXES.get(prefix_type):
         if abs(num) < 1024.0:
             return f"{num:3.1f} {unit}{suffix}"
 
         num /= divider
```

### Comparing `invesyservertools-0.0.5/src/invesyservertools/system_tools.py` & `invesyservertools-0.0.7/src/invesyservertools/system_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 """
 
 import pwd
 import os
 from pathlib import Path
 
 
-def get_username():
+def get_username() -> str:
     return pwd.getpwuid(os.getuid())[0]
 
 
-def get_home_dir():
+def get_home_dir() -> str:
     return str(Path.home())
 
 
 ##  find the complete path for a file
 #
 #   return value is usually str, but any value can
 #   be returned as specified in not_found
 def find_file_path(
     filename: str,
     rootpath: str,
     path_only: bool = False,
-    not_found='{filename} not found in {rootpath}',
+    not_found: str = '{filename} not found in {rootpath}',
     verbose=False
 ) -> str:
 
     if rootpath.startswith('~'):
         rootpath = get_home_dir() + rootpath[1:]
 
     for root, dirs, files in os.walk(rootpath):
```

### Comparing `invesyservertools-0.0.5/src/invesyservertools.egg-info/PKG-INFO` & `invesyservertools-0.0.7/src/invesyservertools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invesyservertools
-Version: 0.0.5
+Version: 0.0.7
 Summary: Tools for Python scripts or terminal
 Home-page: https://gitlab.com/Rastaf/invesyservertools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/Rastaf/invesyservertools/-/issues
 Platform: UNKNOWN
@@ -35,14 +35,20 @@
 - **format_filesize**: return a human-readable filesize, like `31.9 GiB`.
 
 ## system_tools
 - **get_username**: get the username in the operating system
 - **get\_home\_dir**
 - **find\_file\_with\_path**: provide a filename and a start path to begin searching recursively, get the complete path including the filename
 # History
+## 0.0.7
+- **print_** checks for terminal (-> no colors, no wrapper)
+
+## 0.0.6
+- fixed IndexError in **print_** (for line ending in last string)
+
 ## 0.0.5 (2022-12-09)
 - fixed import of submodules
 
 ## 0.0.4 (2022-12-09)
 - *wait_for_key* gets a "indent" argument
 - Sphinx documentation
```

### Comparing `invesyservertools-0.0.5/src/tests/test_print.py` & `invesyservertools-0.0.7/src/tests/test_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 """
 
 import sys
 import unittest
 
 sys.path.append(".")
 
-from print_tools import \
-    format_filesize, print_
+from print_tools import (
+    format_filesize,
+    print_
+)
 
 
 class TestSystem(unittest.TestCase):
     def test_format_filesize(self):
         for prefix_type in ('binary', 'decimal'):
             for nb in (1, 40000, 23456, 34234234234):
                 print(format_filesize(
```

### Comparing `invesyservertools-0.0.5/src/tests/test_system.py` & `invesyservertools-0.0.7/src/tests/test_system.py`

 * *Files identical despite different names*


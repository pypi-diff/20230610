# Comparing `tmp/invesyservertools-0.0.7.tar.gz` & `tmp/invesyservertools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invesyservertools-0.0.7.tar", last modified: Sat Jun 10 12:08:02 2023, max compression
+gzip compressed data, was "dist/invesyservertools-0.0.8.tar", last modified: Sat Jun 10 12:23:32 2023, max compression
```

## Comparing `invesyservertools-0.0.7.tar` & `invesyservertools-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.856760 invesyservertools-0.0.7/
--rw-r--r--   0 georg      (502) staff       (20)     1050 2022-04-20 10:44:14.000000 invesyservertools-0.0.7/LICENSE.txt
--rw-r--r--   0 georg      (502) staff       (20)     2403 2023-06-10 12:08:02.856948 invesyservertools-0.0.7/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)      971 2022-06-13 09:19:16.000000 invesyservertools-0.0.7/README.md
--rw-r--r--   0 georg      (502) staff       (20)      823 2023-06-10 12:08:02.857884 invesyservertools-0.0.7/setup.cfg
--rw-r--r--   0 georg      (502) staff       (20)       69 2022-06-08 20:27:46.000000 invesyservertools-0.0.7/setup.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.846997 invesyservertools-0.0.7/src/
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.852165 invesyservertools-0.0.7/src/invesyservertools/
--rw-r--r--   0 georg      (502) staff       (20)      363 2022-12-09 16:17:01.000000 invesyservertools-0.0.7/src/invesyservertools/__init__.py
--rw-r--r--   0 georg      (502) staff       (20)     1114 2023-06-10 11:56:34.000000 invesyservertools-0.0.7/src/invesyservertools/interactive_tools.py
--rw-r--r--   0 georg      (502) staff       (20)     5739 2023-06-10 12:07:11.000000 invesyservertools-0.0.7/src/invesyservertools/print_tools.py
--rw-r--r--   0 georg      (502) staff       (20)      987 2023-06-10 11:48:16.000000 invesyservertools-0.0.7/src/invesyservertools/system_tools.py
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.854382 invesyservertools-0.0.7/src/invesyservertools.egg-info/
--rw-r--r--   0 georg      (502) staff       (20)     2403 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/PKG-INFO
--rw-r--r--   0 georg      (502) staff       (20)      487 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/SOURCES.txt
--rw-r--r--   0 georg      (502) staff       (20)        1 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/dependency_links.txt
--rw-r--r--   0 georg      (502) staff       (20)        9 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/requires.txt
--rw-r--r--   0 georg      (502) staff       (20)       24 2023-06-10 12:08:02.000000 invesyservertools-0.0.7/src/invesyservertools.egg-info/top_level.txt
-drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:08:02.856193 invesyservertools-0.0.7/src/tests/
--rw-r--r--   0 georg      (502) staff       (20)        1 2022-06-09 11:45:01.000000 invesyservertools-0.0.7/src/tests/__init__.py
--rwxr--r--   0 georg      (502) staff       (20)      849 2023-06-10 12:05:24.000000 invesyservertools-0.0.7/src/tests/test_print.py
--rwxr--r--   0 georg      (502) staff       (20)     1178 2022-08-23 12:03:07.000000 invesyservertools-0.0.7/src/tests/test_system.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:23:32.873239 invesyservertools-0.0.8/
+-rw-r--r--   0 georg      (502) staff       (20)     1050 2022-04-20 10:44:14.000000 invesyservertools-0.0.8/LICENSE.txt
+-rw-r--r--   0 georg      (502) staff       (20)     2450 2023-06-10 12:23:32.873427 invesyservertools-0.0.8/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)      971 2022-06-13 09:19:16.000000 invesyservertools-0.0.8/README.md
+-rw-r--r--   0 georg      (502) staff       (20)      823 2023-06-10 12:23:32.874206 invesyservertools-0.0.8/setup.cfg
+-rw-r--r--   0 georg      (502) staff       (20)       69 2022-06-08 20:27:46.000000 invesyservertools-0.0.8/setup.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:23:32.863448 invesyservertools-0.0.8/src/
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:23:32.868347 invesyservertools-0.0.8/src/invesyservertools/
+-rw-r--r--   0 georg      (502) staff       (20)      363 2022-12-09 16:17:01.000000 invesyservertools-0.0.8/src/invesyservertools/__init__.py
+-rw-r--r--   0 georg      (502) staff       (20)     1114 2023-06-10 12:13:58.000000 invesyservertools-0.0.8/src/invesyservertools/interactive_tools.py
+-rw-r--r--   0 georg      (502) staff       (20)     5739 2023-06-10 12:07:11.000000 invesyservertools-0.0.8/src/invesyservertools/print_tools.py
+-rw-r--r--   0 georg      (502) staff       (20)      987 2023-06-10 11:48:16.000000 invesyservertools-0.0.8/src/invesyservertools/system_tools.py
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:23:32.870535 invesyservertools-0.0.8/src/invesyservertools.egg-info/
+-rw-r--r--   0 georg      (502) staff       (20)     2450 2023-06-10 12:23:32.000000 invesyservertools-0.0.8/src/invesyservertools.egg-info/PKG-INFO
+-rw-r--r--   0 georg      (502) staff       (20)      487 2023-06-10 12:23:32.000000 invesyservertools-0.0.8/src/invesyservertools.egg-info/SOURCES.txt
+-rw-r--r--   0 georg      (502) staff       (20)        1 2023-06-10 12:23:32.000000 invesyservertools-0.0.8/src/invesyservertools.egg-info/dependency_links.txt
+-rw-r--r--   0 georg      (502) staff       (20)        9 2023-06-10 12:23:32.000000 invesyservertools-0.0.8/src/invesyservertools.egg-info/requires.txt
+-rw-r--r--   0 georg      (502) staff       (20)       24 2023-06-10 12:23:32.000000 invesyservertools-0.0.8/src/invesyservertools.egg-info/top_level.txt
+drwxr-xr-x   0 georg      (502) staff       (20)        0 2023-06-10 12:23:32.872652 invesyservertools-0.0.8/src/tests/
+-rw-r--r--   0 georg      (502) staff       (20)        1 2022-06-09 11:45:01.000000 invesyservertools-0.0.8/src/tests/__init__.py
+-rwxr--r--   0 georg      (502) staff       (20)      849 2023-06-10 12:15:59.000000 invesyservertools-0.0.8/src/tests/test_print.py
+-rwxr--r--   0 georg      (502) staff       (20)     1178 2022-08-23 12:03:07.000000 invesyservertools-0.0.8/src/tests/test_system.py
```

### Comparing `invesyservertools-0.0.7/LICENSE.txt` & `invesyservertools-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invesyservertools-0.0.7/PKG-INFO` & `invesyservertools-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invesyservertools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools for Python scripts or terminal
 Home-page: https://gitlab.com/Rastaf/invesyservertools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/Rastaf/invesyservertools/-/issues
 Platform: UNKNOWN
@@ -35,17 +35,20 @@
 - **format_filesize**: return a human-readable filesize, like `31.9 GiB`.
 
 ## system_tools
 - **get_username**: get the username in the operating system
 - **get\_home\_dir**
 - **find\_file\_with\_path**: provide a filename and a start path to begin searching recursively, get the complete path including the filename
 # History
-## 0.0.7
+## 0.0.8 (2023-06-10)
 - **print_** checks for terminal (-> no colors, no wrapper)
 
+## 0.0.7 (2023-06-10)
+- (broken)
+
 ## 0.0.6
 - fixed IndexError in **print_** (for line ending in last string)
 
 ## 0.0.5 (2022-12-09)
 - fixed import of submodules
 
 ## 0.0.4 (2022-12-09)
```

### Comparing `invesyservertools-0.0.7/README.md` & `invesyservertools-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `invesyservertools-0.0.7/setup.cfg` & `invesyservertools-0.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = invesyservertools
-version = 0.0.7
+version = 0.0.8
 author = Georg Pfolz
 author_email = georg.pfolz@invesy.at
 description = Tools for Python scripts or terminal
 long_description = file: README.md,HISTORY.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE.txt
```

### Comparing `invesyservertools-0.0.7/src/invesyservertools/interactive_tools.py` & `invesyservertools-0.0.8/src/invesyservertools/interactive_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Union, List, Tuple, Dict, Any
 from .print_tools import print_
 
 
 ## Wait for a key press on the console and return it
 def wait_for_key(
     text: str = 'continue: press any button',
-    list_bullet: Union(bool, str) = False,
+    list_bullet: Union[bool, str] = False,
     color: str = None,
     indent: int = None
 ) -> 'None or str':
     ''' Wait for a key press on the console and return it.'''
 
     if text:
         print_(
```

### Comparing `invesyservertools-0.0.7/src/invesyservertools/print_tools.py` & `invesyservertools-0.0.8/src/invesyservertools/print_tools.py`

 * *Files identical despite different names*

### Comparing `invesyservertools-0.0.7/src/invesyservertools/system_tools.py` & `invesyservertools-0.0.8/src/invesyservertools/system_tools.py`

 * *Files identical despite different names*

### Comparing `invesyservertools-0.0.7/src/invesyservertools.egg-info/PKG-INFO` & `invesyservertools-0.0.8/src/invesyservertools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invesyservertools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools for Python scripts or terminal
 Home-page: https://gitlab.com/Rastaf/invesyservertools
 Author: Georg Pfolz
 Author-email: georg.pfolz@invesy.at
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/Rastaf/invesyservertools/-/issues
 Platform: UNKNOWN
@@ -35,17 +35,20 @@
 - **format_filesize**: return a human-readable filesize, like `31.9 GiB`.
 
 ## system_tools
 - **get_username**: get the username in the operating system
 - **get\_home\_dir**
 - **find\_file\_with\_path**: provide a filename and a start path to begin searching recursively, get the complete path including the filename
 # History
-## 0.0.7
+## 0.0.8 (2023-06-10)
 - **print_** checks for terminal (-> no colors, no wrapper)
 
+## 0.0.7 (2023-06-10)
+- (broken)
+
 ## 0.0.6
 - fixed IndexError in **print_** (for line ending in last string)
 
 ## 0.0.5 (2022-12-09)
 - fixed import of submodules
 
 ## 0.0.4 (2022-12-09)
```

### Comparing `invesyservertools-0.0.7/src/tests/test_print.py` & `invesyservertools-0.0.8/src/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `invesyservertools-0.0.7/src/tests/test_system.py` & `invesyservertools-0.0.8/src/tests/test_system.py`

 * *Files identical despite different names*


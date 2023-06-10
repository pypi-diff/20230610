# Comparing `tmp/rubyvenv-1.2.0.tar.gz` & `tmp/rubyvenv-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubyvenv-1.2.0.tar", last modified: Mon May 22 23:09:50 2023, max compression
+gzip compressed data, was "rubyvenv-1.2.1.tar", last modified: Sat Jun 10 20:01:55 2023, max compression
```

## Comparing `rubyvenv-1.2.0.tar` & `rubyvenv-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-22 22:56:01.000000 rubyvenv-1.2.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1050 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      416 2023-05-22 22:56:01.000000 rubyvenv-1.2.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/rubyvenv.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1050 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      242 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        7 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8611 2023-05-22 23:09:49.000000 rubyvenv-1.2.0/rubyvenv.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1142 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-22 22:56:01.000000 rubyvenv-1.2.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:01:55.638187 rubyvenv-1.2.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 19:40:08.000000 rubyvenv-1.2.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1050 2023-06-10 20:01:55.638187 rubyvenv-1.2.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      416 2023-06-10 19:40:08.000000 rubyvenv-1.2.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:01:55.638187 rubyvenv-1.2.1/rubyvenv.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1050 2023-06-10 20:01:55.000000 rubyvenv-1.2.1/rubyvenv.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      242 2023-06-10 20:01:55.000000 rubyvenv-1.2.1/rubyvenv.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 20:01:55.000000 rubyvenv-1.2.1/rubyvenv.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2023-06-10 20:01:55.000000 rubyvenv-1.2.1/rubyvenv.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        7 2023-06-10 20:01:55.000000 rubyvenv-1.2.1/rubyvenv.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2023-06-10 20:01:55.000000 rubyvenv-1.2.1/rubyvenv.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8611 2023-06-10 20:01:55.000000 rubyvenv-1.2.1/rubyvenv.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1142 2023-06-10 20:01:55.642186 rubyvenv-1.2.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 19:40:08.000000 rubyvenv-1.2.1/setup.py
```

### Comparing `rubyvenv-1.2.0/LICENSE` & `rubyvenv-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubyvenv-1.2.0/PKG-INFO` & `rubyvenv-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubyvenv
-Version: 1.2.0
+Version: 1.2.1
 Summary: Create no-hassle ruby "virtualenvs".  No .bashrc, no shims, no cd-magic.
 Home-page: https://github.com/asottile/rubyvenv
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rubyvenv-1.2.0/rubyvenv.egg-info/PKG-INFO` & `rubyvenv-1.2.1/rubyvenv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubyvenv
-Version: 1.2.0
+Version: 1.2.1
 Summary: Create no-hassle ruby "virtualenvs".  No .bashrc, no shims, no cd-magic.
 Home-page: https://github.com/asottile/rubyvenv
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rubyvenv-1.2.0/rubyvenv.py` & `rubyvenv-1.2.1/rubyvenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import argparse
 import functools
 import gzip
 import html.parser
 import io
 import os.path
-import pipes
 import platform
+import shlex
 import shutil
 import tarfile
 import tempfile
 import urllib.parse
 import urllib.request
 from typing import Callable
 from typing import ContextManager
@@ -218,15 +218,15 @@
         return get_prebuilt_versions(platform_info)[-1]
     else:
         return Version(version, _download_url(platform_info, version))
 
 
 def _write_activate(dest: str, more: str = '') -> None:
     with open(os.path.join(dest, 'bin', 'activate'), 'w') as activate:
-        activate.write(ACTIVATE.replace('DIRECTORY', pipes.quote(dest)))
+        activate.write(ACTIVATE.replace('DIRECTORY', shlex.quote(dest)))
         activate.write(more)
 
 
 def _write_gitignore(dest: str) -> None:
     with open(os.path.join(dest, '.gitignore'), 'w') as gitignore:
         gitignore.write('# created by rubyvenv automatically\n*\n')
```

### Comparing `rubyvenv-1.2.0/setup.cfg` & `rubyvenv-1.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rubyvenv
-version = 1.2.0
+version = 1.2.1
 description = Create no-hassle ruby "virtualenvs".  No .bashrc, no shims, no cd-magic.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/rubyvenv
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```


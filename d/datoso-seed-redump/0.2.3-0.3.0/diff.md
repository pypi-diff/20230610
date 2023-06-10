# Comparing `tmp/datoso_seed_redump-0.2.3.tar.gz` & `tmp/datoso_seed_redump-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_redump-0.2.3.tar", last modified: Fri May  5 04:16:44 2023, max compression
+gzip compressed data, was "datoso_seed_redump-0.3.0.tar", last modified: Sat Jun 10 20:50:22 2023, max compression
```

## Comparing `datoso_seed_redump-0.2.3.tar` & `datoso_seed_redump-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:16:44.897979 datoso_seed_redump-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.889979 datoso_seed_redump-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/src/datoso_seed_redump/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:50:22.872208 datoso_seed_redump-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-10 20:50:22.872208 datoso_seed_redump-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:50:22.872208 datoso_seed_redump-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:50:22.872208 datoso_seed_redump-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:50:22.872208 datoso_seed_redump-0.3.0/src/datoso_seed_redump/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-10 20:50:10.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:50:22.872208 datoso_seed_redump-0.3.0/src/datoso_seed_redump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-10 20:50:22.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-10 20:50:22.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:50:22.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 20:50:22.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 20:50:22.000000 datoso_seed_redump-0.3.0/src/datoso_seed_redump.egg-info/top_level.txt
```

### Comparing `datoso_seed_redump-0.2.3/LICENSE` & `datoso_seed_redump-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.3/PKG-INFO` & `datoso_seed_redump-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso_seed_redump
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_redump
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datoso_seed_redump-0.2.3/README.md` & `datoso_seed_redump-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.3/pyproject.toml` & `datoso_seed_redump-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 requires-python = ">=3.10"
 license     = {text = "MIT License"}
 authors     = [
     {name = 'Lacides Miranda', email = 'laromicas@hotmail.com'},
 ]
 keywords = ["emulators", "roms"]
 classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.3",
+    "datoso>=0.3.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_redump"
 
 [tool.setuptools]
```

### Comparing `datoso_seed_redump-0.2.3/src/datoso_seed_redump/actions.py` & `datoso_seed_redump-0.3.0/src/datoso_seed_redump/actions.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.3/src/datoso_seed_redump/dats.py` & `datoso_seed_redump-0.3.0/src/datoso_seed_redump/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.3/src/datoso_seed_redump/fetch.py` & `datoso_seed_redump-0.3.0/src/datoso_seed_redump/fetch.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import shutil
 import zipfile
 from datetime import datetime
 from html.parser import HTMLParser
 import urllib.request
 from concurrent.futures import ThreadPoolExecutor
 from datoso.configuration.folder_helper import Folders
+from datoso.helpers import Bcolors
 from datoso_seed_redump import __preffix__
+import logging
 
 MAIN_URL = 'http://redump.org'
 DOWNLOAD_URL = 'http://redump.org/downloads/'
 TYPES = ["datfile", "cues", "gdi", "sbi"]
 
 class MyHTMLParser(HTMLParser):
     dats = {}
@@ -31,29 +33,39 @@
                     self.add_to_dats(output, self.rootpath+href)
 
     def add_to_dats(self, folder, href):
         self.dats[href] = folder
 
 def download_dats(folder_helper):
     done = 0
-    def download_dat(href, folder):
+    def download_dat(href, folder): #TODO: change to asyncio
         nonlocal done
         # print(f'Downloading {href}')
-        tmp_filename, headers = urllib.request.urlretrieve(href)
+        try:
+            tmp_filename, headers = urllib.request.urlretrieve(href)
+        except Exception as e:
+            logging.error(f'Error downloading {DOWNLOAD_URL}: {e}')
+            print(f'Error downloading {href}')
+            return
         local_filename = os.path.join(folder_helper.dats, folder, headers.get_filename())
         shutil.move(tmp_filename, local_filename)
         if folder in ['datfile']:
             with zipfile.ZipFile(local_filename, 'r') as zip_ref:
                 zip_ref.extractall(os.path.join(folder_helper.dats, folder))
             os.remove(local_filename)
         done += 1
         print_progress(done)
 
     print('Downloading Redump HTML')
-    red = urllib.request.urlopen(DOWNLOAD_URL)
+    try:
+        red = urllib.request.urlopen(DOWNLOAD_URL)
+    except Exception as e:
+        logging.error(f'Error downloading {DOWNLOAD_URL}: {e}')
+        print(f'{Bcolors.ERROR}Error downloading {DOWNLOAD_URL}. Skipping redump.{Bcolors.ENDC}')
+        return
     redumphtml = red.read()
 
     print('Parsing Redump HTML')
     parser = MyHTMLParser()
     parser.feed(str(redumphtml))
 
     print('Downloading new dats')
```

### Comparing `datoso_seed_redump-0.2.3/src/datoso_seed_redump/rules.py` & `datoso_seed_redump-0.3.0/src/datoso_seed_redump/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/PKG-INFO` & `datoso_seed_redump-0.3.0/src/datoso_seed_redump.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso-seed-redump
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_redump
 Keywords: emulators,roms
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```


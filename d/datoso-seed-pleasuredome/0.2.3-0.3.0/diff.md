# Comparing `tmp/datoso_seed_pleasuredome-0.2.3.tar.gz` & `tmp/datoso_seed_pleasuredome-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_pleasuredome-0.2.3.tar", last modified: Fri May  5 04:16:01 2023, max compression
+gzip compressed data, was "datoso_seed_pleasuredome-0.3.0.tar", last modified: Sat Jun 10 20:48:39 2023, max compression
```

## Comparing `datoso_seed_pleasuredome-0.2.3.tar` & `datoso_seed_pleasuredome-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.942121 datoso_seed_pleasuredome-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.942121 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:48:39.639635 datoso_seed_pleasuredome-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-10 20:48:39.639635 datoso_seed_pleasuredome-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:48:39.639635 datoso_seed_pleasuredome-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:48:39.635635 datoso_seed_pleasuredome-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:48:39.639635 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-10 20:48:24.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:48:39.639635 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-10 20:48:39.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 20:48:39.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:48:39.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 20:48:39.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 20:48:39.000000 datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome.egg-info/top_level.txt
```

### Comparing `datoso_seed_pleasuredome-0.2.3/LICENSE` & `datoso_seed_pleasuredome-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.3/PKG-INFO` & `datoso_seed_pleasuredome-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso_seed_pleasuredome
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_pleasuredome
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

### Comparing `datoso_seed_pleasuredome-0.2.3/README.md` & `datoso_seed_pleasuredome-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.3/pyproject.toml` & `datoso_seed_pleasuredome-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

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
 "Source Code"       = "https://github.com/laromicas/datoso_seed_pleasuredome"
 
 [tool.setuptools]
```

### Comparing `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/actions.py` & `datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from datoso_seed_pleasuredome.dats import FruitMachinesDat, HomeBrewMameDat, mame_dat_factory
+from datoso_seed_pleasuredome.dats import FruitMachinesXMLDat, HomeBrewMameDat, mame_dat_factory, fruit_machine_factory
 
 actions = {
     '{dat_origin}/FruitMachines': [
         {
             'action': 'LoadDatFile',
-            '_class': FruitMachinesDat
+            '_factory': fruit_machine_factory
         },
         {
             'action': 'DeleteOld'
         },
         {
             'action': 'Copy',
             'folder': '{dat_destination}'
```

### Comparing `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/dats.py` & `datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/dats.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
     PleasureDome Dat class to parse different types of dat files.
 """
 import os
 import re
 import json
 from pathlib import Path
+import logging
+from datoso.helpers import FileHeaders
 
-from datoso.repositories.dat import XMLDatFile, DirMultiDatFile
+from datoso.repositories.dat import XMLDatFile, ClrMameProDatFile, DirMultiDatFile
 # pylint: disable=attribute-defined-outside-init,unsupported-membership-test
 
 
 def mame_dat_factory(file: str):
     """ Dat factory. """
     ext = Path(file).suffix
     if ext in ('.dat', '.xml'):
@@ -96,15 +98,65 @@
             self.name = remove_extra_spaces(self.name.replace(self.version, ''))
         if 'dir2dat' in self.file and 'dir2dat' not in self.name:
             self.name = f'{self.name} (dir2dat)'
 
         return [self.preffix, self.company, self.system, self.suffix, self.get_date()]
 
 
-class FruitMachinesDat(XMLDatFile):
+def fruit_machine_factory(file: str):
+    """ Fruit Dat factory. """
+    # Read first 5 chars of file to determine type
+    with open(file, 'r', encoding='utf-8') as file:
+        file_header = file.read(5)
+    if file_header == FileHeaders.XML.value:
+        return FruitMachinesXMLDat
+    if file_header == FileHeaders.CLRMAMEPRO.value:
+        return FruitMachinesClrMameDat
+    logging.error(f'Unknown Fruit Machine Dat file: {file}')
+    return None
+
+class FruitMachinesXMLDat(XMLDatFile):
+    """ Fruit Machines Dat class. """
+
+    def load_metadata_file(self):
+        """ Load the metadata file. """
+        basedir = Path(self.file).parents[0]
+        filename = os.path.join(basedir, 'metadata.txt')
+        if os.path.exists(filename):
+            with open(filename, encoding='utf-8') as file:
+                metadata = json.load(file)
+        return metadata
+
+
+    def initial_parse(self):
+        # pylint: disable=R0801
+        """ Parse the dat file. """
+        name = self.name
+        extra_data = self.load_metadata_file()
+
+        name = name.split('(')[0].strip()
+        if 'Layouts' in self.file:
+            self.suffix = 'Layouts'
+
+        self.company = 'Fruit'
+        self.system = extra_data['folder']
+
+        self.preffix = 'Arcade'
+
+        return [self.preffix, self.company, self.system, self.suffix, self.get_date()]
+
+
+    def get_date(self):
+        """ Get the date from the dat file. """
+        if self.file and '(' in self.file:
+            file = str(self.file)
+            self.date = file[file.find("(")+1:file.find(")")]
+        return self.date
+
+class FruitMachinesClrMameDat(ClrMameProDatFile):
     """ Fruit Machines Dat class. """
 
     def load_metadata_file(self):
         """ Load the metadata file. """
         basedir = Path(self.file).parents[0]
         filename = os.path.join(basedir, 'metadata.txt')
         if os.path.exists(filename):
```

### Comparing `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/fetch.py` & `datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/rules.py` & `datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/PKG-INFO` & `datoso_seed_pleasuredome-0.3.0/src/datoso_seed_pleasuredome.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datoso-seed-pleasuredome
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_pleasuredome
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


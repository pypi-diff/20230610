# Comparing `tmp/datoso_seed_sfc_speedhacks-0.2.3.tar.gz` & `tmp/datoso_seed_sfc_speedhacks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_sfc_speedhacks-0.2.3.tar", last modified: Fri May  5 04:29:24 2023, max compression
+gzip compressed data, was "datoso_seed_sfc_speedhacks-0.3.0.tar", last modified: Sat Jun 10 20:40:32 2023, max compression
```

## Comparing `datoso_seed_sfc_speedhacks-0.2.3.tar` & `datoso_seed_sfc_speedhacks-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:29:24.126819 datoso_seed_sfc_speedhacks-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-05 04:29:24.126819 datoso_seed_sfc_speedhacks-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:29:24.126819 datoso_seed_sfc_speedhacks-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:29:24.126819 datoso_seed_sfc_speedhacks-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:29:24.126819 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 04:29:11.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:29:24.126819 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-05 04:29:24.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-05 04:29:24.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:29:24.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 04:29:24.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 04:29:24.000000 datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:40:32.324948 datoso_seed_sfc_speedhacks-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-10 20:40:32.324948 datoso_seed_sfc_speedhacks-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 20:40:32.324948 datoso_seed_sfc_speedhacks-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:40:32.320948 datoso_seed_sfc_speedhacks-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:40:32.320948 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-10 20:40:17.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:40:32.324948 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-10 20:40:32.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-10 20:40:32.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:40:32.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 20:40:32.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 20:40:32.000000 datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/top_level.txt
```

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/LICENSE` & `datoso_seed_sfc_speedhacks-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/PKG-INFO` & `datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: datoso_seed_sfc_speedhacks
-Version: 0.2.3
+Name: datoso-seed-sfc-speedhacks
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_sfc_speedhacks
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
@@ -40,26 +40,14 @@
 ```
 
 ## Usage
 
 Check [Datoso](https://github.com/laromicas/datoso) for usage.
 
 
-## Developing a seed
-
-Clone this repository and execute init.sh
-``` bash
-$ git clone https://github.com/laromicas/datoso_seed_sfc_speedhacks
-
-$ cd datoso_seed_sfc_speedhacks
-$ ./init.sh [new_name]   #e.g. ./init.sh newnointro
-
-```
-This creates a new folder with the name `datoso_seed_newnointro` with a scaffold to begin.
-
 ## TODO
 
 -   Tests
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/README.md` & `datoso_seed_sfc_speedhacks-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -22,26 +22,14 @@
 ```
 
 ## Usage
 
 Check [Datoso](https://github.com/laromicas/datoso) for usage.
 
 
-## Developing a seed
-
-Clone this repository and execute init.sh
-``` bash
-$ git clone https://github.com/laromicas/datoso_seed_sfc_speedhacks
-
-$ cd datoso_seed_sfc_speedhacks
-$ ./init.sh [new_name]   #e.g. ./init.sh newnointro
-
-```
-This creates a new folder with the name `datoso_seed_newnointro` with a scaffold to begin.
-
 ## TODO
 
 -   Tests
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/pyproject.toml` & `datoso_seed_sfc_speedhacks-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

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
     "datoso-plugin-internetarchive>=0.2.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_sfc_speedhacks"
```

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/dats.py` & `datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks/rules.py` & `datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/PKG-INFO` & `datoso_seed_sfc_speedhacks-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: datoso-seed-sfc-speedhacks
-Version: 0.2.3
+Name: datoso_seed_sfc_speedhacks
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_sfc_speedhacks
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
@@ -40,26 +40,14 @@
 ```
 
 ## Usage
 
 Check [Datoso](https://github.com/laromicas/datoso) for usage.
 
 
-## Developing a seed
-
-Clone this repository and execute init.sh
-``` bash
-$ git clone https://github.com/laromicas/datoso_seed_sfc_speedhacks
-
-$ cd datoso_seed_sfc_speedhacks
-$ ./init.sh [new_name]   #e.g. ./init.sh newnointro
-
-```
-This creates a new folder with the name `datoso_seed_newnointro` with a scaffold to begin.
-
 ## TODO
 
 -   Tests
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `datoso_seed_sfc_speedhacks-0.2.3/src/datoso_seed_sfc_speedhacks.egg-info/SOURCES.txt` & `datoso_seed_sfc_speedhacks-0.3.0/src/datoso_seed_sfc_speedhacks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


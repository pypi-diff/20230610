# Comparing `tmp/datoso_seed_vpinmame-0.2.8.tar.gz` & `tmp/datoso_seed_vpinmame-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_vpinmame-0.2.8.tar", last modified: Sat May 13 00:08:29 2023, max compression
+gzip compressed data, was "datoso_seed_vpinmame-0.3.0.tar", last modified: Sat Jun 10 20:53:04 2023, max compression
```

## Comparing `datoso_seed_vpinmame-0.2.8.tar` & `datoso_seed_vpinmame-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:08:29.510221 datoso_seed_vpinmame-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-13 00:08:29.510221 datoso_seed_vpinmame-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-13 00:08:29.510221 datoso_seed_vpinmame-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:08:29.506220 datoso_seed_vpinmame-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:08:29.510221 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-13 00:08:17.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:08:29.510221 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-13 00:08:29.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-13 00:08:29.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 00:08:29.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-13 00:08:29.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-13 00:08:29.000000 datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:53:04.878638 datoso_seed_vpinmame-0.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-10 20:53:04.878638 datoso_seed_vpinmame-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-06-10 20:53:04.878638 datoso_seed_vpinmame-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:53:04.874638 datoso_seed_vpinmame-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:53:04.874638 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      430 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame/actions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame/dats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame/fetch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-06-10 20:52:45.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:53:04.878638 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-10 20:53:04.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-10 20:53:04.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:53:04.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 20:53:04.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-10 20:53:04.000000 datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame.egg-info/top_level.txt
```

### Comparing `datoso_seed_vpinmame-0.2.8/LICENSE` & `datoso_seed_vpinmame-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_vpinmame-0.2.8/PKG-INFO` & `datoso_seed_vpinmame-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso_seed_vpinmame
-Version: 0.2.8
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_vpinmame
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso_seed_vpinmame-0.2.8/README.md` & `datoso_seed_vpinmame-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_vpinmame-0.2.8/pyproject.toml` & `datoso_seed_vpinmame-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.8",
-    "datoso-plugin-internetarchive>=0.2.3",
+    "datoso>=0.3.1",
+    "datoso-plugin-internetarchive>=0.3.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_vpinmame"
 
 [tool.setuptools]
```

### Comparing `datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame/dats.py` & `datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_vpinmame-0.2.8/src/datoso_seed_vpinmame.egg-info/PKG-INFO` & `datoso_seed_vpinmame-0.3.0/src/datoso_seed_vpinmame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso-seed-vpinmame
-Version: 0.2.8
+Version: 0.3.0
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_vpinmame
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```


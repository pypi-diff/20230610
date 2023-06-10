# Comparing `tmp/evilHunter-0.1.6.tar.gz` & `tmp/evilHunter-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.6.tar", last modified: Sat Jun 10 09:29:15 2023, max compression
+gzip compressed data, was "evilHunter-0.1.7.tar", last modified: Sat Jun 10 09:34:38 2023, max compression
```

## Comparing `evilHunter-0.1.6.tar` & `evilHunter-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:29:15.403884 evilHunter-0.1.6/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:29:15.403884 evilHunter-0.1.6/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1440 2023-06-09 11:15:59.000000 evilHunter-0.1.6/README.md
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:29:15.403884 evilHunter-0.1.6/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15576 2023-06-09 22:58:05.000000 evilHunter-0.1.6/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-10 09:29:15.403884 evilHunter-0.1.6/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      520 2023-06-10 09:29:05.000000 evilHunter-0.1.6/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:34:38.524323 evilHunter-0.1.7/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:34:38.524323 evilHunter-0.1.7/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1440 2023-06-09 11:15:59.000000 evilHunter-0.1.7/README.md
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:34:38.524323 evilHunter-0.1.7/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15538 2023-06-10 09:31:04.000000 evilHunter-0.1.7/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-10 09:34:38.524323 evilHunter-0.1.7/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      520 2023-06-10 09:34:34.000000 evilHunter-0.1.7/setup.py
```

### Comparing `evilHunter-0.1.6/PKG-INFO` & `evilHunter-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.6/README.md` & `evilHunter-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.6/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.7/evilHunter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.6/evilHunter.py` & `evilHunter-0.1.7/evilHunter.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,16 +419,14 @@
             print(output.decode().strip())
         except KeyboardInterrupt:
             break
 
 
 def main():
     try:
-        delete_files()
-        exit()
         # Recogemos argumentos
         parser = argparse.ArgumentParser()
         parser.add_argument("-w", "--wordlist", help="Use an extern wordlists dictionary", required=True)
         args = parser.parse_args()
 
         # Somos root?
         am_i_root()
```

### Comparing `evilHunter-0.1.6/setup.py` & `evilHunter-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.6",
+    version="0.1.7",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```


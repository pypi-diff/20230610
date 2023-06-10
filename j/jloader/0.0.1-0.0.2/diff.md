# Comparing `tmp/jloader-0.0.1.tar.gz` & `tmp/jloader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jloader-0.0.1.tar", last modified: Sat Jun 10 15:15:16 2023, max compression
+gzip compressed data, was "jloader-0.0.2.tar", last modified: Sat Jun 10 15:38:49 2023, max compression
```

## Comparing `jloader-0.0.1.tar` & `jloader-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:15:16.724230 jloader-0.0.1/
--rw-r--r--   0 loj       (1000) users      (984)     1075 2023-06-10 14:25:35.000000 jloader-0.0.1/LICENSE
--rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:15:16.724230 jloader-0.0.1/PKG-INFO
--rw-r--r--   0 loj       (1000) users      (984)       52 2023-06-10 12:41:36.000000 jloader-0.0.1/README.md
-drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:15:16.724230 jloader-0.0.1/jloader.egg-info/
--rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:15:16.000000 jloader-0.0.1/jloader.egg-info/PKG-INFO
--rw-r--r--   0 loj       (1000) users      (984)      195 2023-06-10 15:15:16.000000 jloader-0.0.1/jloader.egg-info/SOURCES.txt
--rw-r--r--   0 loj       (1000) users      (984)        1 2023-06-10 15:15:16.000000 jloader-0.0.1/jloader.egg-info/dependency_links.txt
--rw-r--r--   0 loj       (1000) users      (984)       17 2023-06-10 15:15:16.000000 jloader-0.0.1/jloader.egg-info/requires.txt
--rw-r--r--   0 loj       (1000) users      (984)        1 2023-06-10 15:15:16.000000 jloader-0.0.1/jloader.egg-info/top_level.txt
--rw-r--r--   0 loj       (1000) users      (984)      289 2023-06-10 14:30:21.000000 jloader-0.0.1/pyproject.toml
--rw-r--r--   0 loj       (1000) users      (984)       38 2023-06-10 15:15:16.724230 jloader-0.0.1/setup.cfg
--rw-r--r--   0 loj       (1000) users      (984)      702 2023-06-10 14:28:23.000000 jloader-0.0.1/setup.py
+drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:38:49.504273 jloader-0.0.2/
+-rw-r--r--   0 loj       (1000) users      (984)     1075 2023-06-10 14:25:35.000000 jloader-0.0.2/LICENSE
+-rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:38:49.504273 jloader-0.0.2/PKG-INFO
+-rw-r--r--   0 loj       (1000) users      (984)       52 2023-06-10 12:41:36.000000 jloader-0.0.2/README.md
+drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:38:49.504273 jloader-0.0.2/jloader/
+-rw-r--r--   0 loj       (1000) users      (984)       19 2023-06-10 15:30:36.000000 jloader-0.0.2/jloader/__init__.py
+-rw-r--r--   0 loj       (1000) users      (984)     2038 2023-06-10 15:13:17.000000 jloader-0.0.2/jloader/main.py
+drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:38:49.504273 jloader-0.0.2/jloader.egg-info/
+-rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/PKG-INFO
+-rw-r--r--   0 loj       (1000) users      (984)      231 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/SOURCES.txt
+-rw-r--r--   0 loj       (1000) users      (984)        1 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/dependency_links.txt
+-rw-r--r--   0 loj       (1000) users      (984)       17 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/requires.txt
+-rw-r--r--   0 loj       (1000) users      (984)        8 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/top_level.txt
+-rw-r--r--   0 loj       (1000) users      (984)      289 2023-06-10 14:30:21.000000 jloader-0.0.2/pyproject.toml
+-rw-r--r--   0 loj       (1000) users      (984)       38 2023-06-10 15:38:49.504273 jloader-0.0.2/setup.cfg
+-rw-r--r--   0 loj       (1000) users      (984)      702 2023-06-10 15:38:21.000000 jloader-0.0.2/setup.py
```

### Comparing `jloader-0.0.1/LICENSE` & `jloader-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jloader-0.0.1/setup.py` & `jloader-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests>=2.31.0"]
 
 setuptools.setup(
     name="jloader",
-    version="0.0.1",
+    version="0.0.2",
     author="Lojaleto",
     author_email="lojaleto@yandex.ru",
     description="Downloader for jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lojaleto/jloader",
     packages=setuptools.find_packages(),
```


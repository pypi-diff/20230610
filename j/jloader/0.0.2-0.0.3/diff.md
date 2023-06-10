# Comparing `tmp/jloader-0.0.2.tar.gz` & `tmp/jloader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jloader-0.0.2.tar", last modified: Sat Jun 10 15:38:49 2023, max compression
+gzip compressed data, was "jloader-0.0.3.tar", last modified: Sat Jun 10 15:43:54 2023, max compression
```

## Comparing `jloader-0.0.2.tar` & `jloader-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:38:49.504273 jloader-0.0.2/
--rw-r--r--   0 loj       (1000) users      (984)     1075 2023-06-10 14:25:35.000000 jloader-0.0.2/LICENSE
--rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:38:49.504273 jloader-0.0.2/PKG-INFO
--rw-r--r--   0 loj       (1000) users      (984)       52 2023-06-10 12:41:36.000000 jloader-0.0.2/README.md
-drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:38:49.504273 jloader-0.0.2/jloader/
--rw-r--r--   0 loj       (1000) users      (984)       19 2023-06-10 15:30:36.000000 jloader-0.0.2/jloader/__init__.py
--rw-r--r--   0 loj       (1000) users      (984)     2038 2023-06-10 15:13:17.000000 jloader-0.0.2/jloader/main.py
-drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:38:49.504273 jloader-0.0.2/jloader.egg-info/
--rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/PKG-INFO
--rw-r--r--   0 loj       (1000) users      (984)      231 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/SOURCES.txt
--rw-r--r--   0 loj       (1000) users      (984)        1 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/dependency_links.txt
--rw-r--r--   0 loj       (1000) users      (984)       17 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/requires.txt
--rw-r--r--   0 loj       (1000) users      (984)        8 2023-06-10 15:38:49.000000 jloader-0.0.2/jloader.egg-info/top_level.txt
--rw-r--r--   0 loj       (1000) users      (984)      289 2023-06-10 14:30:21.000000 jloader-0.0.2/pyproject.toml
--rw-r--r--   0 loj       (1000) users      (984)       38 2023-06-10 15:38:49.504273 jloader-0.0.2/setup.cfg
--rw-r--r--   0 loj       (1000) users      (984)      702 2023-06-10 15:38:21.000000 jloader-0.0.2/setup.py
+drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:43:54.180949 jloader-0.0.3/
+-rw-r--r--   0 loj       (1000) users      (984)     1075 2023-06-10 14:25:35.000000 jloader-0.0.3/LICENSE
+-rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:43:54.180949 jloader-0.0.3/PKG-INFO
+-rw-r--r--   0 loj       (1000) users      (984)       52 2023-06-10 12:41:36.000000 jloader-0.0.3/README.md
+drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:43:54.177616 jloader-0.0.3/jloader/
+-rw-r--r--   0 loj       (1000) users      (984)       50 2023-06-10 15:43:38.000000 jloader-0.0.3/jloader/__init__.py
+-rw-r--r--   0 loj       (1000) users      (984)     2038 2023-06-10 15:13:17.000000 jloader-0.0.3/jloader/main.py
+drwxr-xr-x   0 loj       (1000) users      (984)        0 2023-06-10 15:43:54.180949 jloader-0.0.3/jloader.egg-info/
+-rw-r--r--   0 loj       (1000) users      (984)      467 2023-06-10 15:43:54.000000 jloader-0.0.3/jloader.egg-info/PKG-INFO
+-rw-r--r--   0 loj       (1000) users      (984)      231 2023-06-10 15:43:54.000000 jloader-0.0.3/jloader.egg-info/SOURCES.txt
+-rw-r--r--   0 loj       (1000) users      (984)        1 2023-06-10 15:43:54.000000 jloader-0.0.3/jloader.egg-info/dependency_links.txt
+-rw-r--r--   0 loj       (1000) users      (984)       17 2023-06-10 15:43:54.000000 jloader-0.0.3/jloader.egg-info/requires.txt
+-rw-r--r--   0 loj       (1000) users      (984)        8 2023-06-10 15:43:54.000000 jloader-0.0.3/jloader.egg-info/top_level.txt
+-rw-r--r--   0 loj       (1000) users      (984)      289 2023-06-10 14:30:21.000000 jloader-0.0.3/pyproject.toml
+-rw-r--r--   0 loj       (1000) users      (984)       38 2023-06-10 15:43:54.180949 jloader-0.0.3/setup.cfg
+-rw-r--r--   0 loj       (1000) users      (984)      702 2023-06-10 15:43:47.000000 jloader-0.0.3/setup.py
```

### Comparing `jloader-0.0.2/LICENSE` & `jloader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jloader-0.0.2/jloader/main.py` & `jloader-0.0.3/jloader/main.py`

 * *Files identical despite different names*

### Comparing `jloader-0.0.2/setup.py` & `jloader-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests>=2.31.0"]
 
 setuptools.setup(
     name="jloader",
-    version="0.0.2",
+    version="0.0.3",
     author="Lojaleto",
     author_email="lojaleto@yandex.ru",
     description="Downloader for jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lojaleto/jloader",
     packages=setuptools.find_packages(),
```


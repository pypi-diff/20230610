# Comparing `tmp/somnium-8.9.8.tar.gz` & `tmp/somnium-9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somnium-8.9.8.tar", last modified: Mon May 15 10:49:37 2023, max compression
+gzip compressed data, was "somnium-9.9.1.tar", last modified: Sat Jun 10 21:12:51 2023, max compression
```

## Comparing `somnium-8.9.8.tar` & `somnium-9.9.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.173350 somnium-8.9.8/
--rw-r--r--   0 kali      (1000) kali      (1000)       19 2022-07-25 10:16:20.000000 somnium-8.9.8/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 10:49:37.173350 somnium-8.9.8/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      412 2023-05-15 07:58:19.000000 somnium-8.9.8/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      103 2022-07-25 10:16:08.000000 somnium-8.9.8/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)      687 2023-05-15 10:49:37.173350 somnium-8.9.8/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.169350 somnium-8.9.8/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.173350 somnium-8.9.8/src/somnium/
--rw-r--r--   0 kali      (1000) kali      (1000)       30 2023-04-14 11:43:25.000000 somnium-8.9.8/src/somnium/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4909 2023-05-15 10:48:07.000000 somnium-8.9.8/src/somnium/__main__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-15 10:49:37.173350 somnium-8.9.8/src/somnium.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      264 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       22 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-05-15 10:49:37.000000 somnium-8.9.8/src/somnium.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-10 21:12:51.264951 somnium-9.9.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)       19 2022-07-25 10:16:20.000000 somnium-9.9.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     1453 2023-06-10 21:12:51.264951 somnium-9.9.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      939 2023-06-10 21:01:47.000000 somnium-9.9.1/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      103 2022-07-25 10:16:08.000000 somnium-9.9.1/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)      687 2023-06-10 21:12:51.264951 somnium-9.9.1/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-10 21:12:51.264951 somnium-9.9.1/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-10 21:12:51.264951 somnium-9.9.1/src/somnium/
+-rw-r--r--   0 kali      (1000) kali      (1000)       30 2023-04-14 11:43:25.000000 somnium-9.9.1/src/somnium/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4909 2023-05-15 10:48:07.000000 somnium-9.9.1/src/somnium/__main__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-10 21:12:51.264951 somnium-9.9.1/src/somnium/sync/
+-rw-r--r--   0 kali      (1000) kali      (1000)       30 2023-04-14 11:43:25.000000 somnium-9.9.1/src/somnium/sync/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5606 2023-06-10 20:58:42.000000 somnium-9.9.1/src/somnium/sync/__main__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-10 21:12:51.264951 somnium-9.9.1/src/somnium.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1453 2023-06-10 21:12:51.000000 somnium-9.9.1/src/somnium.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      322 2023-06-10 21:12:51.000000 somnium-9.9.1/src/somnium.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-10 21:12:51.000000 somnium-9.9.1/src/somnium.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       22 2023-06-10 21:12:51.000000 somnium-9.9.1/src/somnium.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-06-10 21:12:51.000000 somnium-9.9.1/src/somnium.egg-info/top_level.txt
```

### Comparing `somnium-8.9.8/setup.cfg` & `somnium-9.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = somnium
-version = 8.9.8
+version = 9.9.1
 author = odi
 author_email = ivuxey@gmail.com
 description = Create beautiful artwork using the power of AI.
 keywords = ai, stablediffusion, dream, somnium
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://odium.us
```

### Comparing `somnium-8.9.8/src/somnium/__main__.py` & `somnium-9.9.1/src/somnium/__main__.py`

 * *Files identical despite different names*


# Comparing `tmp/kdslibs-0.0.5.tar.gz` & `tmp/kdslibs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdslibs-0.0.5.tar", last modified: Sat Jun 10 16:12:40 2023, max compression
+gzip compressed data, was "kdslibs-0.0.6.tar", last modified: Sat Jun 10 16:59:33 2023, max compression
```

## Comparing `kdslibs-0.0.5.tar` & `kdslibs-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:12:40.452834 kdslibs-0.0.5/
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.5/LICENSE
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 16:12:40.452834 kdslibs-0.0.5/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.5/README.md
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:12:40.452834 kdslibs-0.0.5/kdslibs/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      379 2023-06-10 16:09:52.000000 kdslibs-0.0.5/kdslibs/__init__.py
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:12:40.452834 kdslibs-0.0.5/kdslibs.egg-info/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 16:12:40.000000 kdslibs-0.0.5/kdslibs.egg-info/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-10 16:12:40.000000 kdslibs-0.0.5/kdslibs.egg-info/SOURCES.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-10 16:12:40.000000 kdslibs-0.0.5/kdslibs.egg-info/dependency_links.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-10 16:12:40.000000 kdslibs-0.0.5/kdslibs.egg-info/top_level.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-10 16:12:40.452834 kdslibs-0.0.5/setup.cfg
--rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-10 16:06:57.000000 kdslibs-0.0.5/setup.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:59:33.162751 kdslibs-0.0.6/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.6/LICENSE
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 16:59:33.162751 kdslibs-0.0.6/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.6/README.md
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:59:33.152751 kdslibs-0.0.6/kdslibs/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      701 2023-06-10 16:58:59.000000 kdslibs-0.0.6/kdslibs/__init__.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 16:59:33.162751 kdslibs-0.0.6/kdslibs.egg-info/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-10 16:59:33.000000 kdslibs-0.0.6/kdslibs.egg-info/top_level.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-10 16:59:33.162751 kdslibs-0.0.6/setup.cfg
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-10 16:59:22.000000 kdslibs-0.0.6/setup.py
```


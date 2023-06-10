# Comparing `tmp/kdslibs-0.0.1.tar.gz` & `tmp/kdslibs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdslibs-0.0.1.tar", last modified: Sat Jun 10 10:58:24 2023, max compression
+gzip compressed data, was "kdslibs-0.0.2.tar", last modified: Sat Jun 10 11:10:23 2023, max compression
```

## Comparing `kdslibs-0.0.1.tar` & `kdslibs-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 10:58:24.405658 kdslibs-0.0.1/
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.1/LICENSE
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 10:58:24.405658 kdslibs-0.0.1/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.1/README.md
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 10:58:24.405658 kdslibs-0.0.1/kdslib/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      100 2023-06-10 08:35:04.000000 kdslibs-0.0.1/kdslib/__init__.py
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 10:58:24.405658 kdslibs-0.0.1/kdslibs.egg-info/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 10:58:24.000000 kdslibs-0.0.1/kdslibs.egg-info/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)      169 2023-06-10 10:58:24.000000 kdslibs-0.0.1/kdslibs.egg-info/SOURCES.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-10 10:58:24.000000 kdslibs-0.0.1/kdslibs.egg-info/dependency_links.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        7 2023-06-10 10:58:24.000000 kdslibs-0.0.1/kdslibs.egg-info/top_level.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-10 10:58:24.405658 kdslibs-0.0.1/setup.cfg
--rw-r--r--   0 diwa      (1000) diwa      (1000)      431 2023-06-10 10:58:19.000000 kdslibs-0.0.1/setup.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:10:23.395638 kdslibs-0.0.2/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.2/LICENSE
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 11:10:23.395638 kdslibs-0.0.2/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.2/README.md
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:10:23.395638 kdslibs-0.0.2/kdslibs/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      100 2023-06-10 08:35:04.000000 kdslibs-0.0.2/kdslibs/__init__.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:10:23.395638 kdslibs-0.0.2/kdslibs.egg-info/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 11:10:23.000000 kdslibs-0.0.2/kdslibs.egg-info/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-10 11:10:23.000000 kdslibs-0.0.2/kdslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-10 11:10:23.000000 kdslibs-0.0.2/kdslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-10 11:10:23.000000 kdslibs-0.0.2/kdslibs.egg-info/top_level.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-10 11:10:23.395638 kdslibs-0.0.2/setup.cfg
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-10 11:09:23.000000 kdslibs-0.0.2/setup.py
```


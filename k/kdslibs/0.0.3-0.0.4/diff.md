# Comparing `tmp/kdslibs-0.0.3.tar.gz` & `tmp/kdslibs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdslibs-0.0.3.tar", last modified: Sat Jun 10 11:25:13 2023, max compression
+gzip compressed data, was "kdslibs-0.0.4.tar", last modified: Sat Jun 10 11:38:04 2023, max compression
```

## Comparing `kdslibs-0.0.3.tar` & `kdslibs-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:25:13.045612 kdslibs-0.0.3/
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.3/LICENSE
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 11:25:13.045612 kdslibs-0.0.3/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.3/README.md
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:25:13.045612 kdslibs-0.0.3/kdslibs/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      280 2023-06-10 11:24:44.000000 kdslibs-0.0.3/kdslibs/__init__.py
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:25:13.045612 kdslibs-0.0.3/kdslibs.egg-info/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 11:25:13.000000 kdslibs-0.0.3/kdslibs.egg-info/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-10 11:25:13.000000 kdslibs-0.0.3/kdslibs.egg-info/SOURCES.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-10 11:25:13.000000 kdslibs-0.0.3/kdslibs.egg-info/dependency_links.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-10 11:25:13.000000 kdslibs-0.0.3/kdslibs.egg-info/top_level.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-10 11:25:13.045612 kdslibs-0.0.3/setup.cfg
--rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-10 11:25:04.000000 kdslibs-0.0.3/setup.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:38:04.805593 kdslibs-0.0.4/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.4/LICENSE
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 11:38:04.805593 kdslibs-0.0.4/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.4/README.md
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:38:04.805593 kdslibs-0.0.4/kdslibs/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      379 2023-06-10 11:35:42.000000 kdslibs-0.0.4/kdslibs/__init__.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-10 11:38:04.805593 kdslibs-0.0.4/kdslibs.egg-info/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-10 11:38:04.000000 kdslibs-0.0.4/kdslibs.egg-info/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-10 11:38:04.000000 kdslibs-0.0.4/kdslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-10 11:38:04.000000 kdslibs-0.0.4/kdslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-10 11:38:04.000000 kdslibs-0.0.4/kdslibs.egg-info/top_level.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-10 11:38:04.805593 kdslibs-0.0.4/setup.cfg
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-10 11:37:32.000000 kdslibs-0.0.4/setup.py
```


# Comparing `tmp/psychom-scanner-0.1.tar.gz` & `tmp/psychom-scanner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychom-scanner-0.1.tar", last modified: Sat Jun 10 15:37:08 2023, max compression
+gzip compressed data, was "psychom-scanner-0.1.1.tar", last modified: Sat Jun 10 16:17:24 2023, max compression
```

## Comparing `psychom-scanner-0.1.tar` & `psychom-scanner-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 kcd       (1000) kcd       (1000)        0 2023-06-10 15:37:08.249427 psychom-scanner-0.1/
--rw-rw-r--   0 kcd       (1000) kcd       (1000)      257 2023-06-10 15:37:08.249427 psychom-scanner-0.1/PKG-INFO
--rw-rw-r--   0 kcd       (1000) kcd       (1000)      519 2023-06-10 14:37:10.000000 psychom-scanner-0.1/README.md
-drwxrwxr-x   0 kcd       (1000) kcd       (1000)        0 2023-06-10 15:37:08.249427 psychom-scanner-0.1/psychom_scanner/
--rw-rw-r--   0 kcd       (1000) kcd       (1000)        0 2023-06-09 15:54:35.000000 psychom-scanner-0.1/psychom_scanner/__init__.py
-drwxrwxr-x   0 kcd       (1000) kcd       (1000)        0 2023-06-10 15:37:08.249427 psychom-scanner-0.1/psychom_scanner.egg-info/
--rw-rw-r--   0 kcd       (1000) kcd       (1000)      257 2023-06-10 15:37:08.000000 psychom-scanner-0.1/psychom_scanner.egg-info/PKG-INFO
--rw-rw-r--   0 kcd       (1000) kcd       (1000)      202 2023-06-10 15:37:08.000000 psychom-scanner-0.1/psychom_scanner.egg-info/SOURCES.txt
--rw-rw-r--   0 kcd       (1000) kcd       (1000)        1 2023-06-10 15:37:08.000000 psychom-scanner-0.1/psychom_scanner.egg-info/dependency_links.txt
--rw-rw-r--   0 kcd       (1000) kcd       (1000)       16 2023-06-10 15:37:08.000000 psychom-scanner-0.1/psychom_scanner.egg-info/top_level.txt
--rw-rw-r--   0 kcd       (1000) kcd       (1000)       38 2023-06-10 15:37:08.249427 psychom-scanner-0.1/setup.cfg
--rw-rw-r--   0 kcd       (1000) kcd       (1000)      282 2023-06-10 15:37:02.000000 psychom-scanner-0.1/setup.py
+drwxrwxr-x   0 kcd       (1000) kcd       (1000)        0 2023-06-10 16:17:24.762509 psychom-scanner-0.1.1/
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)      259 2023-06-10 16:17:24.762509 psychom-scanner-0.1.1/PKG-INFO
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)      520 2023-06-10 15:42:34.000000 psychom-scanner-0.1.1/README.md
+drwxrwxr-x   0 kcd       (1000) kcd       (1000)        0 2023-06-10 16:17:24.762509 psychom-scanner-0.1.1/psychom_scanner/
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)        0 2023-06-09 15:54:35.000000 psychom-scanner-0.1.1/psychom_scanner/__init__.py
+drwxrwxr-x   0 kcd       (1000) kcd       (1000)        0 2023-06-10 16:17:24.762509 psychom-scanner-0.1.1/psychom_scanner.egg-info/
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)      259 2023-06-10 16:17:24.000000 psychom-scanner-0.1.1/psychom_scanner.egg-info/PKG-INFO
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)      202 2023-06-10 16:17:24.000000 psychom-scanner-0.1.1/psychom_scanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)        1 2023-06-10 16:17:24.000000 psychom-scanner-0.1.1/psychom_scanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)       16 2023-06-10 16:17:24.000000 psychom-scanner-0.1.1/psychom_scanner.egg-info/top_level.txt
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)       38 2023-06-10 16:17:24.762509 psychom-scanner-0.1.1/setup.cfg
+-rw-rw-r--   0 kcd       (1000) kcd       (1000)      284 2023-06-10 16:17:21.000000 psychom-scanner-0.1.1/setup.py
```


# Comparing `tmp/brainfk-0.0.2.tar.gz` & `tmp/brainfk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainfk-0.0.2.tar", last modified: Sat Jun 10 17:59:45 2023, max compression
+gzip compressed data, was "brainfk-1.0.0.tar", last modified: Thu Jun  8 14:26:31 2023, max compression
```

## Comparing `brainfk-0.0.2.tar` & `brainfk-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 17:59:45.339216 brainfk-0.0.2/
--rw-rw-rw-   0        0        0     2031 2023-06-10 17:59:45.338200 brainfk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-10 16:44:33.000000 brainfk-0.0.2/README.md
--rw-rw-rw-   0        0        0     1729 2023-06-10 17:53:16.000000 brainfk-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 17:59:45.306210 brainfk-0.0.2/brainfk/
--rw-rw-rw-   0        0        0        0 2023-06-08 13:59:59.000000 brainfk-0.0.2/brainfk/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-06-10 17:29:03.000000 brainfk-0.0.2/brainfk/interpreter.py
-drwxrwxrwx   0        0        0        0 2023-06-10 17:59:45.336169 brainfk-0.0.2/brainfk.egg-info/
--rw-rw-rw-   0        0        0     2031 2023-06-10 17:59:45.000000 brainfk-0.0.2/brainfk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-10 17:59:45.000000 brainfk-0.0.2/brainfk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 17:59:45.000000 brainfk-0.0.2/brainfk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-10 17:59:45.000000 brainfk-0.0.2/brainfk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 17:59:45.000000 brainfk-0.0.2/brainfk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 17:59:45.000000 brainfk-0.0.2/brainfk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      535 2023-06-10 17:59:00.000000 brainfk-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 17:59:45.340212 brainfk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      686 2023-06-10 17:59:04.000000 brainfk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 14:26:31.069764 brainfk-1.0.0/
+-rw-rw-rw-   0        0        0      169 2023-06-08 14:26:31.067809 brainfk-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 14:26:31.025765 brainfk-1.0.0/brainfk/
+-rw-rw-rw-   0        0        0        0 2023-06-08 13:59:59.000000 brainfk-1.0.0/brainfk/__init__.py
+-rw-rw-rw-   0        0        0     1715 2023-06-08 13:59:41.000000 brainfk-1.0.0/brainfk/interpreter.py
+drwxrwxrwx   0        0        0        0 2023-06-08 14:26:31.065766 brainfk-1.0.0/brainfk.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-06-08 14:26:30.000000 brainfk-1.0.0/brainfk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-06-08 14:26:30.000000 brainfk-1.0.0/brainfk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 14:26:30.000000 brainfk-1.0.0/brainfk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-08 14:26:30.000000 brainfk-1.0.0/brainfk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 14:26:30.000000 brainfk-1.0.0/brainfk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-08 14:26:30.000000 brainfk-1.0.0/brainfk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 14:26:31.069764 brainfk-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      359 2023-06-08 14:08:02.000000 brainfk-1.0.0/setup.py
```


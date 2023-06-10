# Comparing `tmp/brainfk-0.0.3.tar.gz` & `tmp/brainfk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainfk-0.0.3.tar", last modified: Sat Jun 10 18:25:54 2023, max compression
+gzip compressed data, was "brainfk-1.0.0.tar", last modified: Thu Jun  8 14:26:31 2023, max compression
```

## Comparing `brainfk-0.0.3.tar` & `brainfk-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 18:25:54.658868 brainfk-0.0.3/
--rw-rw-rw-   0        0        0     2297 2023-06-10 18:25:54.657866 brainfk-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1729 2023-06-10 17:53:16.000000 brainfk-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 18:25:54.623860 brainfk-0.0.3/brainfk/
--rw-rw-rw-   0        0        0        0 2023-06-08 13:59:59.000000 brainfk-0.0.3/brainfk/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-06-10 17:29:03.000000 brainfk-0.0.3/brainfk/interpreter.py
-drwxrwxrwx   0        0        0        0 2023-06-10 18:25:54.653871 brainfk-0.0.3/brainfk.egg-info/
--rw-rw-rw-   0        0        0     2297 2023-06-10 18:25:54.000000 brainfk-0.0.3/brainfk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-10 18:25:54.000000 brainfk-0.0.3/brainfk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 18:25:54.000000 brainfk-0.0.3/brainfk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-10 18:25:54.000000 brainfk-0.0.3/brainfk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 18:25:54.000000 brainfk-0.0.3/brainfk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 18:25:54.000000 brainfk-0.0.3/brainfk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-06-10 18:25:11.000000 brainfk-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 18:25:54.659869 brainfk-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-10 18:25:47.000000 brainfk-0.0.3/setup.py
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


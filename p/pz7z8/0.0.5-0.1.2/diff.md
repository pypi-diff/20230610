# Comparing `tmp/pz7z8-0.0.5.tar.gz` & `tmp/pz7z8-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pz7z8-0.0.5.tar", last modified: Sat Jun 18 09:19:36 2022, max compression
+gzip compressed data, was "pz7z8-0.1.2.tar", last modified: Sat Jun 10 08:44:48 2023, max compression
```

## Comparing `pz7z8-0.0.5.tar` & `pz7z8-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 oracle    (1001) oracle    (1001)        0 2022-06-18 09:19:36.000000 pz7z8-0.0.5/
--rwxrwxrwx   0 oracle    (1001) oracle    (1001)     1074 2022-03-26 03:22:28.000000 pz7z8-0.0.5/LICENSE
--rw-r--r--   0 oracle    (1001) oracle    (1001)       38 2022-06-18 09:19:36.000000 pz7z8-0.0.5/setup.cfg
--rwxrwxrwx   0 oracle    (1001) oracle    (1001)       26 2022-03-26 03:24:29.000000 pz7z8-0.0.5/README.md
-drwxr-xr-x   0 oracle    (1001) oracle    (1001)        0 2022-06-18 09:19:36.000000 pz7z8-0.0.5/z7z8/
--rwxrw-rw-   0 oracle    (1001) oracle    (1001)     2830 2021-12-14 03:02:47.000000 pz7z8-0.0.5/z7z8/smod.py
--rwxrwxrwx   0 oracle    (1001) oracle    (1001)        0 2020-03-05 08:42:50.000000 pz7z8-0.0.5/z7z8/__init__.py
--rwxrwxrwx   0 oracle    (1001) oracle    (1001)     1205 2022-04-11 03:00:33.000000 pz7z8-0.0.5/z7z8/dsync.py
--rwxrwxrwx   0 oracle    (1001) oracle    (1001)      544 2022-06-18 09:08:51.000000 pz7z8-0.0.5/z7z8/dfslow.py
--rw-r--r--   0 oracle    (1001) oracle    (1001)      453 2022-06-18 09:19:36.000000 pz7z8-0.0.5/PKG-INFO
--rwxrwxrwx   0 oracle    (1001) oracle    (1001)      931 2022-06-18 09:11:22.000000 pz7z8-0.0.5/setup.py
-drwxr-xr-x   0 oracle    (1001) oracle    (1001)        0 2022-06-18 09:19:36.000000 pz7z8-0.0.5/pz7z8.egg-info/
--rw-r--r--   0 oracle    (1001) oracle    (1001)       94 2022-06-18 09:19:36.000000 pz7z8-0.0.5/pz7z8.egg-info/entry_points.txt
--rw-r--r--   0 oracle    (1001) oracle    (1001)      261 2022-06-18 09:19:36.000000 pz7z8-0.0.5/pz7z8.egg-info/SOURCES.txt
--rw-r--r--   0 oracle    (1001) oracle    (1001)        1 2022-03-26 04:05:10.000000 pz7z8-0.0.5/pz7z8.egg-info/not-zip-safe
--rw-r--r--   0 oracle    (1001) oracle    (1001)        1 2022-06-18 09:19:36.000000 pz7z8-0.0.5/pz7z8.egg-info/dependency_links.txt
--rw-r--r--   0 oracle    (1001) oracle    (1001)        5 2022-06-18 09:19:36.000000 pz7z8-0.0.5/pz7z8.egg-info/top_level.txt
--rw-r--r--   0 oracle    (1001) oracle    (1001)      453 2022-06-18 09:19:36.000000 pz7z8-0.0.5/pz7z8.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 08:44:48.000000 pz7z8-0.1.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1074 2022-03-26 03:22:28.000000 pz7z8-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-10 08:44:48.000000 pz7z8-0.1.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       26 2022-03-26 03:24:29.000000 pz7z8-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 08:44:48.000000 pz7z8-0.1.2/pz7z8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-26 04:05:10.000000 pz7z8-0.1.2/pz7z8.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-10 08:44:47.000000 pz7z8-0.1.2/pz7z8.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 08:44:48.000000 pz7z8-0.1.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2081 2023-06-10 08:43:46.000000 pz7z8-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 08:44:48.000000 pz7z8-0.1.2/z7z8/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 pz7z8-0.1.2/z7z8/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      544 2022-06-18 09:08:51.000000 pz7z8-0.1.2/z7z8/dfslow.py
+-rwxrwxrwx   0 root         (0) root         (0)     1205 2022-04-11 03:00:33.000000 pz7z8-0.1.2/z7z8/dsync.py
+-rwxrw-rw-   0 root         (0) root         (0)      683 2023-06-10 08:40:49.000000 pz7z8-0.1.2/z7z8/md2pdf.py
+-rwxrw-rw-   0 root         (0) root         (0)     2830 2021-12-14 03:02:47.000000 pz7z8-0.1.2/z7z8/smod.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pz7z8-0.0.5/LICENSE` & `pz7z8-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz7z8-0.0.5/z7z8/smod.py` & `pz7z8-0.1.2/z7z8/smod.py`

 * *Files identical despite different names*

### Comparing `pz7z8-0.0.5/z7z8/dsync.py` & `pz7z8-0.1.2/z7z8/dsync.py`

 * *Files identical despite different names*

### Comparing `pz7z8-0.0.5/z7z8/dfslow.py` & `pz7z8-0.1.2/z7z8/dfslow.py`

 * *Files identical despite different names*


# Comparing `tmp/needed-libs-0.1.tar.gz` & `tmp/needed-libs-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "needed-libs-0.1.tar", last modified: Sat Jun 10 18:24:39 2023, max compression
+gzip compressed data, was "needed-libs-0.2.tar", last modified: Sat Jun 10 18:45:25 2023, max compression
```

## Comparing `needed-libs-0.1.tar` & `needed-libs-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 18:24:39.300797 needed-libs-0.1/
--rw-rw-rw-   0        0        0       56 2023-06-10 18:24:39.301797 needed-libs-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-10 18:24:39.300797 needed-libs-0.1/needed_libs.egg-info/
--rw-rw-rw-   0        0        0       56 2023-06-10 18:24:38.000000 needed-libs-0.1/needed_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-10 18:24:39.000000 needed-libs-0.1/needed_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 18:24:38.000000 needed-libs-0.1/needed_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-10 18:24:38.000000 needed-libs-0.1/needed_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-10 18:24:38.000000 needed-libs-0.1/needed_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-10 18:24:39.301797 needed-libs-0.1/setup.cfg
--rw-rw-rw-   0        0        0      210 2023-06-10 18:23:31.000000 needed-libs-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:45:25.975804 needed-libs-0.2/
+-rw-rw-rw-   0        0        0       56 2023-06-10 18:45:25.975804 needed-libs-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 18:45:25.974803 needed-libs-0.2/needed_libs.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-06-10 18:45:25.000000 needed-libs-0.2/needed_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-10 18:45:25.000000 needed-libs-0.2/needed_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 18:45:25.000000 needed-libs-0.2/needed_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      364 2023-06-10 18:45:25.000000 needed-libs-0.2/needed_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-10 18:45:25.000000 needed-libs-0.2/needed_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-10 18:45:25.976802 needed-libs-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-06-10 18:45:22.000000 needed-libs-0.2/setup.py
```


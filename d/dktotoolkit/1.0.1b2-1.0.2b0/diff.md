# Comparing `tmp/dktotoolkit-1.0.1b2.tar.gz` & `tmp/dktotoolkit-1.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktotoolkit-1.0.1b2.tar", last modified: Fri Jun  2 12:29:18 2023, max compression
+gzip compressed data, was "dktotoolkit-1.0.2b0.tar", last modified: Sat Jun 10 18:20:48 2023, max compression
```

## Comparing `dktotoolkit-1.0.1b2.tar` & `dktotoolkit-1.0.2b0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2071 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1286 2023-06-02 11:45:29.000000 dktotoolkit-1.0.1b2/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2071 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      202 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       64 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-06-02 12:29:18.000000 dktotoolkit-1.0.1b2/dktotoolkit.egg-info/top_level.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)      195 2023-06-02 12:29:18.603287 dktotoolkit-1.0.1b2/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3493 2023-06-02 12:18:24.000000 dktotoolkit-1.0.1b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 18:20:48.520110 dktotoolkit-1.0.2b0/
+-rw-rw-rw-   0 root         (0) root         (0)    34469 2023-06-10 18:14:09.000000 dktotoolkit-1.0.2b0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-06-10 18:20:48.520110 dktotoolkit-1.0.2b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-06-10 18:14:09.000000 dktotoolkit-1.0.2b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 18:20:48.520110 dktotoolkit-1.0.2b0/dktotoolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-06-10 18:20:48.000000 dktotoolkit-1.0.2b0/dktotoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-10 18:20:48.000000 dktotoolkit-1.0.2b0/dktotoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 18:20:48.000000 dktotoolkit-1.0.2b0/dktotoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2023-06-10 18:20:48.000000 dktotoolkit-1.0.2b0/dktotoolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 18:20:48.000000 dktotoolkit-1.0.2b0/dktotoolkit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-10 18:20:48.520110 dktotoolkit-1.0.2b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4951 2023-06-10 18:14:09.000000 dktotoolkit-1.0.2b0/setup.py
```


# Comparing `tmp/arithmetica-py-1.0.219.tar.gz` & `tmp/arithmetica-py-1.0.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.219.tar", last modified: Fri Jun  9 12:58:27 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.221.tar", last modified: Sat Jun 10 08:43:40 2023, max compression
```

## Comparing `arithmetica-py-1.0.219.tar` & `arithmetica-py-1.0.221.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.712378 arithmetica-py-1.0.219/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   187086 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:43:40.026999 arithmetica-py-1.0.221/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-10 08:43:20.000000 arithmetica-py-1.0.221/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 08:43:40.026999 arithmetica-py-1.0.221/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-10 08:43:20.000000 arithmetica-py-1.0.221/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:43:40.026999 arithmetica-py-1.0.221/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 08:43:39.000000 arithmetica-py-1.0.221/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-10 08:43:39.000000 arithmetica-py-1.0.221/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 08:43:39.000000 arithmetica-py-1.0.221/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-10 08:43:39.000000 arithmetica-py-1.0.221/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 08:43:40.026999 arithmetica-py-1.0.221/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-10 08:43:20.000000 arithmetica-py-1.0.221/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:43:40.022999 arithmetica-py-1.0.221/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:43:40.026999 arithmetica-py-1.0.221/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   187086 2023-06-10 08:43:39.000000 arithmetica-py-1.0.221/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-06-10 08:43:39.000000 arithmetica-py-1.0.221/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-10 08:43:20.000000 arithmetica-py-1.0.221/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 08:43:39.000000 arithmetica-py-1.0.221/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.219/LICENSE` & `arithmetica-py-1.0.221/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.219/README.md` & `arithmetica-py-1.0.221/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.219/setup.py` & `arithmetica-py-1.0.221/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.219/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.221/src/python-module/libarithmetica.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.219/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.221/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.219/src/python-module/module.c` & `arithmetica-py-1.0.221/src/python-module/module.c`

 * *Files identical despite different names*


# Comparing `tmp/irvy-0.0.1.tar.gz` & `tmp/irvy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irvy-0.0.1.tar", last modified: Sat Jun 10 17:31:17 2023, max compression
+gzip compressed data, was "irvy-1.0.0.tar", last modified: Sat Jun 10 17:33:19 2023, max compression
```

## Comparing `irvy-0.0.1.tar` & `irvy-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:17.146306 irvy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-10 17:31:17.146306 irvy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-10 17:31:04.000000 irvy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:17.142306 irvy-0.0.1/irvy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:04.000000 irvy-0.0.1/irvy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:17.146306 irvy-0.0.1/irvy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-10 17:31:04.000000 irvy-0.0.1/irvy/generators/PlaywrightGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-10 17:31:04.000000 irvy-0.0.1/irvy/generators/SeleniumGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:04.000000 irvy-0.0.1/irvy/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-10 17:31:04.000000 irvy-0.0.1/irvy/irvy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:17.146306 irvy-0.0.1/irvy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:04.000000 irvy-0.0.1/irvy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:04.000000 irvy-0.0.1/irvy/utils/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:31:17.142306 irvy-0.0.1/irvy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-10 17:31:17.000000 irvy-0.0.1/irvy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-10 17:31:17.000000 irvy-0.0.1/irvy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:31:17.000000 irvy-0.0.1/irvy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-10 17:31:17.000000 irvy-0.0.1/irvy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 17:31:17.000000 irvy-0.0.1/irvy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:31:17.146306 irvy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 17:31:04.000000 irvy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:19.629505 irvy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-10 17:33:19.629505 irvy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-10 17:33:08.000000 irvy-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:19.625505 irvy-1.0.0/irvy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:08.000000 irvy-1.0.0/irvy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:19.625505 irvy-1.0.0/irvy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-10 17:33:08.000000 irvy-1.0.0/irvy/generators/PlaywrightGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-10 17:33:08.000000 irvy-1.0.0/irvy/generators/SeleniumGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:08.000000 irvy-1.0.0/irvy/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-10 17:33:08.000000 irvy-1.0.0/irvy/irvy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:19.625505 irvy-1.0.0/irvy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:08.000000 irvy-1.0.0/irvy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:08.000000 irvy-1.0.0/irvy/utils/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:33:19.625505 irvy-1.0.0/irvy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-10 17:33:19.000000 irvy-1.0.0/irvy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-10 17:33:19.000000 irvy-1.0.0/irvy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:33:19.000000 irvy-1.0.0/irvy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-10 17:33:19.000000 irvy-1.0.0/irvy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 17:33:19.000000 irvy-1.0.0/irvy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:33:19.629505 irvy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 17:33:08.000000 irvy-1.0.0/setup.py
```

### Comparing `irvy-0.0.1/PKG-INFO` & `irvy-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irvy
-Version: 0.0.1
+Version: 1.0.0
 Summary: A brief description of your project
 Description-Content-Type: text/markdown
 
 # Irvy
 
 Irvy is a command-line tool to setup projects for Selenium and Playwright in different languages.
```

### Comparing `irvy-0.0.1/README.md` & `irvy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `irvy-0.0.1/irvy/generators/PlaywrightGenerator.py` & `irvy-1.0.0/irvy/generators/PlaywrightGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-0.0.1/irvy/generators/SeleniumGenerator.py` & `irvy-1.0.0/irvy/generators/SeleniumGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-0.0.1/irvy/irvy.py` & `irvy-1.0.0/irvy/irvy.py`

 * *Files identical despite different names*

### Comparing `irvy-0.0.1/irvy.egg-info/PKG-INFO` & `irvy-1.0.0/irvy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irvy
-Version: 0.0.1
+Version: 1.0.0
 Summary: A brief description of your project
 Description-Content-Type: text/markdown
 
 # Irvy
 
 Irvy is a command-line tool to setup projects for Selenium and Playwright in different languages.
```


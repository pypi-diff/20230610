# Comparing `tmp/numtoname-0.2.2.tar.gz` & `tmp/numtoname-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numtoname-0.2.2.tar", last modified: Thu Jun  1 07:21:07 2023, max compression
+gzip compressed data, was "numtoname-0.3.1.tar", last modified: Sat Jun 10 00:27:52 2023, max compression
```

## Comparing `numtoname-0.2.2.tar` & `numtoname-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 07:21:07.927036 numtoname-0.2.2/
--rw-rw-rw-   0        0        0     1088 2023-05-25 23:57:32.000000 numtoname-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-06-01 07:21:07.927036 numtoname-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-05-26 00:55:44.000000 numtoname-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 07:21:07.902015 numtoname-0.2.2/numtoname/
--rw-rw-rw-   0        0        0     1092 2023-05-31 19:21:40.000000 numtoname-0.2.2/numtoname/__init__.py
--rw-rw-rw-   0        0        0    17206 2023-06-01 07:19:40.000000 numtoname-0.2.2/numtoname/functions.py
--rw-rw-rw-   0        0        0    12926 2023-06-01 07:08:40.000000 numtoname-0.2.2/numtoname/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:21:07.924031 numtoname-0.2.2/numtoname.egg-info/
--rw-rw-rw-   0        0        0      693 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-01 07:21:07.930034 numtoname-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-06-01 07:16:56.000000 numtoname-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 00:27:52.542741 numtoname-0.3.1/
+-rw-rw-rw-   0        0        0     1088 2023-05-25 23:57:32.000000 numtoname-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      742 2023-06-10 00:27:52.542741 numtoname-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-06-08 23:30:13.000000 numtoname-0.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-10 00:27:52.494740 numtoname-0.3.1/numtoname/
+-rw-rw-rw-   0        0        0     1092 2023-06-10 00:22:09.000000 numtoname-0.3.1/numtoname/__init__.py
+-rw-rw-rw-   0        0        0    25854 2023-06-09 17:31:42.000000 numtoname-0.3.1/numtoname/functions.py
+-rw-rw-rw-   0        0        0     3131 2023-06-08 08:45:23.000000 numtoname-0.3.1/numtoname/helpers.py
+-rw-rw-rw-   0        0        0    20126 2023-06-09 21:09:52.000000 numtoname-0.3.1/numtoname/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-10 00:27:52.539737 numtoname-0.3.1/numtoname.egg-info/
+-rw-rw-rw-   0        0        0      742 2023-06-10 00:27:52.000000 numtoname-0.3.1/numtoname.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-10 00:27:52.000000 numtoname-0.3.1/numtoname.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 00:27:52.000000 numtoname-0.3.1/numtoname.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-10 00:27:52.000000 numtoname-0.3.1/numtoname.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1639 2023-06-10 00:27:52.547746 numtoname-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      292 2023-06-10 00:19:50.000000 numtoname-0.3.1/setup.py
```

### Comparing `numtoname-0.2.2/LICENSE.txt` & `numtoname-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numtoname-0.2.2/numtoname/__init__.py` & `numtoname-0.3.1/numtoname/__init__.py`

 * *Files identical despite different names*


# Comparing `tmp/krx_holidays-0.0.1.tar.gz` & `tmp/krx_holidays-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krx_holidays-0.0.1.tar", last modified: Sat Jun 10 07:12:36 2023, max compression
+gzip compressed data, was "dist/krx_holidays-0.0.2.tar", last modified: Sat Jun 10 07:38:31 2023, max compression
```

## Comparing `krx_holidays-0.0.1.tar` & `krx_holidays-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:12:36.000000 krx_holidays-0.0.1/
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:12:36.000000 krx_holidays-0.0.1/krxholidays/
--rw-r--r--   0 nezah      (501) staff       (20)      648 2023-06-10 07:06:47.000000 krx_holidays-0.0.1/krxholidays/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)    10784 2023-06-10 07:10:31.000000 krx_holidays-0.0.1/krxholidays/data.py
--rw-r--r--   0 nezah      (501) staff       (20)      739 2023-06-10 07:12:36.000000 krx_holidays-0.0.1/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 krx_holidays-0.0.1/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:12:36.000000 krx_holidays-0.0.1/test/
--rw-r--r--   0 nezah      (501) staff       (20)      192 2023-06-10 07:06:47.000000 krx_holidays-0.0.1/test/test_holiday.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:12:36.000000 krx_holidays-0.0.1/krx_holidays.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      739 2023-06-10 07:12:35.000000 krx_holidays-0.0.1/krx_holidays.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      235 2023-06-10 07:12:35.000000 krx_holidays-0.0.1/krx_holidays.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       12 2023-06-10 07:12:35.000000 krx_holidays-0.0.1/krx_holidays.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-10 07:12:35.000000 krx_holidays-0.0.1/krx_holidays.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)      356 2023-06-10 07:12:10.000000 krx_holidays-0.0.1/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      506 2023-06-10 06:34:43.000000 krx_holidays-0.0.1/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-10 07:12:36.000000 krx_holidays-0.0.1/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/krxholidays/
+-rw-r--r--   0 nezah      (501) staff       (20)     1146 2023-06-10 07:38:02.000000 krx_holidays-0.0.2/krxholidays/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)    14450 2023-06-10 07:33:10.000000 krx_holidays-0.0.2/krxholidays/data.py
+-rw-r--r--   0 nezah      (501) staff       (20)      739 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 krx_holidays-0.0.2/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/test/
+-rw-r--r--   0 nezah      (501) staff       (20)     1606 2023-06-10 07:37:10.000000 krx_holidays-0.0.2/test/test_holiday.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/krx_holidays.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      739 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/krx_holidays.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      235 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/krx_holidays.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       12 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/krx_holidays.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/krx_holidays.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)      356 2023-06-10 07:12:10.000000 krx_holidays-0.0.2/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      506 2023-06-10 07:38:30.000000 krx_holidays-0.0.2/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-10 07:38:31.000000 krx_holidays-0.0.2/setup.cfg
```

### Comparing `krx_holidays-0.0.1/PKG-INFO` & `krx_holidays-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krx_holidays
-Version: 0.0.1
+Version: 0.0.2
 Summary: KRX Holidays
 Home-page: https://github.com/cheddars/krx_holidays
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krx_holidays-0.0.1/LICENSE` & `krx_holidays-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `krx_holidays-0.0.1/krx_holidays.egg-info/PKG-INFO` & `krx_holidays-0.0.2/krx_holidays.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krx-holidays
-Version: 0.0.1
+Version: 0.0.2
 Summary: KRX Holidays
 Home-page: https://github.com/cheddars/krx_holidays
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/once-utils-0.0.5.tar.gz` & `tmp/once-utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "once-utils-0.0.5.tar", last modified: Sun Jun  4 14:42:52 2023, max compression
+gzip compressed data, was "once-utils-0.0.6.tar", last modified: Sat Jun 10 10:54:26 2023, max compression
```

## Comparing `once-utils-0.0.5.tar` & `once-utils-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/
--rw-rw-rw-   0        0        0      852 2023-06-04 14:42:52.041295 once-utils-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       56 2022-09-25 12:18:04.000000 once-utils-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.029190 once-utils-0.0.5/once_utils.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/onceutils/
--rw-rw-rw-   0        0        0      184 2023-04-16 05:52:44.000000 once-utils-0.0.5/onceutils/__init__.py
--rw-rw-rw-   0        0        0     3805 2023-06-04 14:37:47.000000 once-utils-0.0.5/onceutils/_cmd.py
--rw-rw-rw-   0        0        0     1115 2022-09-10 06:29:17.000000 once-utils-0.0.5/onceutils/_convert.py
--rw-rw-rw-   0        0        0      436 2022-09-24 05:27:27.000000 once-utils-0.0.5/onceutils/_iter.py
--rw-rw-rw-   0        0        0      629 2022-08-26 16:47:36.000000 once-utils-0.0.5/onceutils/_pymodule.py
--rw-rw-rw-   0        0        0     6652 2022-09-25 11:20:31.000000 once-utils-0.0.5/onceutils/_random.py
--rw-rw-rw-   0        0        0      618 2022-09-24 13:55:11.000000 once-utils-0.0.5/onceutils/const.py
--rw-rw-rw-   0        0        0      322 2023-04-16 05:49:32.000000 once-utils-0.0.5/onceutils/ex_dict.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/onceutils/github/
--rw-rw-rw-   0        0        0        0 2022-08-28 14:34:38.000000 once-utils-0.0.5/onceutils/github/__init__.py
--rw-rw-rw-   0        0        0     4764 2022-08-29 14:40:26.000000 once-utils-0.0.5/onceutils/github/personal_token.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/onceutils/xjson/
--rw-rw-rw-   0        0        0      125 2022-08-28 14:34:36.000000 once-utils-0.0.5/onceutils/xjson/__init__.py
--rw-rw-rw-   0        0        0      736 2022-08-28 14:34:36.000000 once-utils-0.0.5/onceutils/xjson/encoder.py
--rw-rw-rw-   0        0        0       42 2023-06-04 14:42:52.041295 once-utils-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-06-04 14:40:21.000000 once-utils-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.915557 once-utils-0.0.6/
+-rw-rw-rw-   0        0        0      852 2023-06-10 10:54:26.915557 once-utils-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2022-09-25 12:18:04.000000 once-utils-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.890558 once-utils-0.0.6/once_utils.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.905573 once-utils-0.0.6/onceutils/
+-rw-rw-rw-   0        0        0      184 2023-04-16 05:52:44.000000 once-utils-0.0.6/onceutils/__init__.py
+-rw-rw-rw-   0        0        0     3805 2023-06-04 14:37:47.000000 once-utils-0.0.6/onceutils/_cmd.py
+-rw-rw-rw-   0        0        0     1115 2022-09-10 06:29:17.000000 once-utils-0.0.6/onceutils/_convert.py
+-rw-rw-rw-   0        0        0      436 2022-09-24 05:27:27.000000 once-utils-0.0.6/onceutils/_iter.py
+-rw-rw-rw-   0        0        0      629 2022-08-26 16:47:36.000000 once-utils-0.0.6/onceutils/_pymodule.py
+-rw-rw-rw-   0        0        0     6652 2022-09-25 11:20:31.000000 once-utils-0.0.6/onceutils/_random.py
+-rw-rw-rw-   0        0        0      618 2022-09-24 13:55:11.000000 once-utils-0.0.6/onceutils/const.py
+-rw-rw-rw-   0        0        0      322 2023-04-16 05:49:32.000000 once-utils-0.0.6/onceutils/ex_dict.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.909134 once-utils-0.0.6/onceutils/github/
+-rw-rw-rw-   0        0        0        0 2022-08-28 14:34:38.000000 once-utils-0.0.6/onceutils/github/__init__.py
+-rw-rw-rw-   0        0        0     4764 2022-08-29 14:40:26.000000 once-utils-0.0.6/onceutils/github/personal_token.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.913560 once-utils-0.0.6/onceutils/xjson/
+-rw-rw-rw-   0        0        0      164 2023-06-10 10:01:41.000000 once-utils-0.0.6/onceutils/xjson/__init__.py
+-rw-rw-rw-   0        0        0     1680 2023-06-10 10:00:10.000000 once-utils-0.0.6/onceutils/xjson/_common.py
+-rw-rw-rw-   0        0        0     1048 2023-06-10 07:17:05.000000 once-utils-0.0.6/onceutils/xjson/encoder.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:54:26.916558 once-utils-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-06-10 10:51:54.000000 once-utils-0.0.6/setup.py
```

### Comparing `once-utils-0.0.5/PKG-INFO` & `once-utils-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: once-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simplest utils.
 Home-page: https://github.com/Mingyueyixi/once-utils
 Author: Lu
 Author-email: Mingyueyixi@hotmail.com
 License: MIT Licence
 Keywords: pip,once-utils
 Platform: any
```

### Comparing `once-utils-0.0.5/once_utils.egg-info/PKG-INFO` & `once-utils-0.0.6/once_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: once-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simplest utils.
 Home-page: https://github.com/Mingyueyixi/once-utils
 Author: Lu
 Author-email: Mingyueyixi@hotmail.com
 License: MIT Licence
 Keywords: pip,once-utils
 Platform: any
```

### Comparing `once-utils-0.0.5/onceutils/_cmd.py` & `once-utils-0.0.6/onceutils/_cmd.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.5/onceutils/_convert.py` & `once-utils-0.0.6/onceutils/_convert.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.5/onceutils/_pymodule.py` & `once-utils-0.0.6/onceutils/_pymodule.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.5/onceutils/_random.py` & `once-utils-0.0.6/onceutils/_random.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.5/onceutils/const.py` & `once-utils-0.0.6/onceutils/const.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.5/onceutils/github/personal_token.py` & `once-utils-0.0.6/onceutils/github/personal_token.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.5/setup.py` & `once-utils-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open(readme_md_path) as f:
         ret = f.read()
     return ret
 
 
 setup(
     name="once-utils",
-    version="0.0.5",
+    version="0.0.6",
     keywords=["pip", "once-utils"],
     description="Simplest utils.",
     long_description=readme_md(),
     long_description_content_type='text/markdown',
     license="MIT Licence",
     classifiers=[
         'Programming Language :: Python :: 3',
```


# Comparing `tmp/cbpi4-PushOver-0.0.8.tar.gz` & `tmp/cbpi4-PushOver-0.0.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-PushOver-0.0.8.tar", last modified: Sat Jun 10 12:11:47 2023, max compression
+gzip compressed data, was "cbpi4-PushOver-0.0.8rc1.tar", last modified: Thu Jun  8 10:58:03 2023, max compression
```

## Comparing `cbpi4-PushOver-0.0.8.tar` & `cbpi4-PushOver-0.0.8rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:11:47.879222 cbpi4-PushOver-0.0.8/
--rw-rw-rw-   0        0        0    35149 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       76 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1252 2023-06-10 12:11:47.877238 cbpi4-PushOver-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-06-10 12:11:33.000000 cbpi4-PushOver-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:11:47.844219 cbpi4-PushOver-0.0.8/cbpi4-PushOver/
--rw-rw-rw-   0        0        0     4286 2023-04-05 17:22:51.000000 cbpi4-PushOver-0.0.8/cbpi4-PushOver/__init__.py
--rw-rw-rw-   0        0        0       31 2021-04-17 11:12:15.000000 cbpi4-PushOver-0.0.8/cbpi4-PushOver/config.yaml
-drwxrwxrwx   0        0        0        0 2023-06-10 12:11:47.875238 cbpi4-PushOver-0.0.8/cbpi4_PushOver.egg-info/
--rw-rw-rw-   0        0        0     1252 2023-06-10 12:11:47.000000 cbpi4-PushOver-0.0.8/cbpi4_PushOver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-10 12:11:47.000000 cbpi4-PushOver-0.0.8/cbpi4_PushOver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:11:47.000000 cbpi4-PushOver-0.0.8/cbpi4_PushOver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-10 12:11:47.000000 cbpi4-PushOver-0.0.8/cbpi4_PushOver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-10 12:11:47.000000 cbpi4-PushOver-0.0.8/cbpi4_PushOver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:11:47.880226 cbpi4-PushOver-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1009 2023-06-10 12:10:16.000000 cbpi4-PushOver-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:58:03.070863 cbpi4-PushOver-0.0.8rc1/
+-rw-rw-rw-   0        0        0    35149 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.8rc1/LICENSE
+-rw-rw-rw-   0        0        0       76 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.8rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1210 2023-06-08 10:58:03.068868 cbpi4-PushOver-0.0.8rc1/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-06-02 15:25:09.000000 cbpi4-PushOver-0.0.8rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 10:58:03.023871 cbpi4-PushOver-0.0.8rc1/cbpi4-PushOver/
+-rw-rw-rw-   0        0        0     4286 2023-04-05 17:22:51.000000 cbpi4-PushOver-0.0.8rc1/cbpi4-PushOver/__init__.py
+-rw-rw-rw-   0        0        0       31 2021-04-17 11:12:15.000000 cbpi4-PushOver-0.0.8rc1/cbpi4-PushOver/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 10:58:03.066866 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/
+-rw-rw-rw-   0        0        0     1210 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:58:03.070863 cbpi4-PushOver-0.0.8rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-06-02 15:25:11.000000 cbpi4-PushOver-0.0.8rc1/setup.py
```

### Comparing `cbpi4-PushOver-0.0.8/LICENSE` & `cbpi4-PushOver-0.0.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-PushOver-0.0.8/PKG-INFO` & `cbpi4-PushOver-0.0.8rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-PushOver
-Version: 0.0.8
+Version: 0.0.8rc1
 Summary: CraftBeerPi4 Plugin to forward Notifications to Pushover Push Notifications
 Home-page: https://github.com/PiBrewing/cbpi4-PushOver
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -31,16 +31,15 @@
 - Parameters:
 
 	- pushover_token: your token for this service
 	- pushover_user: your user for this service
 
 ### Changelog:
 
-- 10.06.23: (0.0.8) bump version to release
-- 02.06.23: (0.0.8.rc1) added cbpi4 requirement
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
 - 05.04.23: (0.0.8.a2) test for plugin settings selection test branch
 - 10.05.22: (0.0.7) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 02.04.21:  Minor changes
 - 15.03.21: Initial Release.
```

### Comparing `cbpi4-PushOver-0.0.8/README.md` & `cbpi4-PushOver-0.0.8rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,13 @@
 - Parameters:
 
 	- pushover_token: your token for this service
 	- pushover_user: your user for this service
 
 ### Changelog:
 
-- 10.06.23: (0.0.8) bump version to release
-- 02.06.23: (0.0.8.rc1) added cbpi4 requirement
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
 - 05.04.23: (0.0.8.a2) test for plugin settings selection test branch
 - 10.05.22: (0.0.7) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 02.04.21:  Minor changes
 - 15.03.21: Initial Release.
```

### Comparing `cbpi4-PushOver-0.0.8/cbpi4-PushOver/__init__.py` & `cbpi4-PushOver-0.0.8rc1/cbpi4-PushOver/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-PushOver-0.0.8/cbpi4_PushOver.egg-info/PKG-INFO` & `cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-PushOver
-Version: 0.0.8
+Version: 0.0.8rc1
 Summary: CraftBeerPi4 Plugin to forward Notifications to Pushover Push Notifications
 Home-page: https://github.com/PiBrewing/cbpi4-PushOver
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -31,16 +31,15 @@
 - Parameters:
 
 	- pushover_token: your token for this service
 	- pushover_user: your user for this service
 
 ### Changelog:
 
-- 10.06.23: (0.0.8) bump version to release
-- 02.06.23: (0.0.8.rc1) added cbpi4 requirement
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
 - 05.04.23: (0.0.8.a2) test for plugin settings selection test branch
 - 10.05.22: (0.0.7) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 02.04.21:  Minor changes
 - 15.03.21: Initial Release.
```

### Comparing `cbpi4-PushOver-0.0.8/setup.py` & `cbpi4-PushOver-0.0.8rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-PushOver',
-      version='0.0.8',
+      version='0.0.8.rc1',
       description='CraftBeerPi4 Plugin to forward Notifications to Pushover Push Notifications',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-PushOver',
       license='GPLv3',
       include_package_data=True,
       keywords='globalsettings',
```


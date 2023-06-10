# Comparing `tmp/cbpi4-Flowmeter-0.0.6.tar.gz` & `tmp/cbpi4-Flowmeter-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-Flowmeter-0.0.6.tar", last modified: Sat Jun 10 12:16:47 2023, max compression
+gzip compressed data, was "cbpi4-Flowmeter-0.0.6rc1.tar", last modified: Thu Jun  8 11:02:51 2023, max compression
```

## Comparing `cbpi4-Flowmeter-0.0.6.tar` & `cbpi4-Flowmeter-0.0.6rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:16:47.227060 cbpi4-Flowmeter-0.0.6/
--rw-rw-rw-   0        0        0    35149 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       78 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4361 2023-06-10 12:16:47.226058 cbpi4-Flowmeter-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4000 2023-06-10 12:16:18.000000 cbpi4-Flowmeter-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:16:47.189060 cbpi4-Flowmeter-0.0.6/cbpi4-Flowmeter/
--rw-rw-rw-   0        0        0    16141 2023-06-02 15:20:10.000000 cbpi4-Flowmeter-0.0.6/cbpi4-Flowmeter/__init__.py
--rw-rw-rw-   0        0        0       32 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6/cbpi4-Flowmeter/config.yaml
-drwxrwxrwx   0        0        0        0 2023-06-10 12:16:47.223058 cbpi4-Flowmeter-0.0.6/cbpi4_Flowmeter.egg-info/
--rw-rw-rw-   0        0        0     4361 2023-06-10 12:16:47.000000 cbpi4-Flowmeter-0.0.6/cbpi4_Flowmeter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-06-10 12:16:47.000000 cbpi4-Flowmeter-0.0.6/cbpi4_Flowmeter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:16:47.000000 cbpi4-Flowmeter-0.0.6/cbpi4_Flowmeter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-10 12:16:47.000000 cbpi4-Flowmeter-0.0.6/cbpi4_Flowmeter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-10 12:16:47.000000 cbpi4-Flowmeter-0.0.6/cbpi4_Flowmeter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:16:47.227060 cbpi4-Flowmeter-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-06-10 12:15:49.000000 cbpi4-Flowmeter-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.037570 cbpi4-Flowmeter-0.0.6rc1/
+-rw-rw-rw-   0        0        0    35149 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6rc1/LICENSE
+-rw-rw-rw-   0        0        0       78 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4317 2023-06-08 11:02:51.036568 cbpi4-Flowmeter-0.0.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     3953 2023-06-02 15:22:20.000000 cbpi4-Flowmeter-0.0.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:50.994571 cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/
+-rw-rw-rw-   0        0        0    16141 2023-06-02 15:20:10.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/__init__.py
+-rw-rw-rw-   0        0        0       32 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.033568 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/
+-rw-rw-rw-   0        0        0     4317 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:02:51.038567 cbpi4-Flowmeter-0.0.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0      982 2023-06-02 15:22:12.000000 cbpi4-Flowmeter-0.0.6rc1/setup.py
```

### Comparing `cbpi4-Flowmeter-0.0.6/LICENSE` & `cbpi4-Flowmeter-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-Flowmeter-0.0.6/PKG-INFO` & `cbpi4-Flowmeter-0.0.6rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-Flowmeter
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Flowsensor / Step Plugin 
 Home-page: https://github.com/PiBrewing/cbpi4-Flowmeter
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -75,16 +75,14 @@
 Actions:
  - Reset Sensor: resets the countet impulses and volume to 0
  - Fake Impulse: fakes the detection of an impulse (i used this for testing because i dont have a flow sensor)
 
 
 
 ## Changelog:
-
-- 10.06.23: (0.0.6) bump version to release
 - 14.05.23: (0.0.6.rc1) added simple VolumeSensor and cbpi4 requirement
 - 14.04.23: (0.0.5.a2) fixed bug in parameter generation
 - 08.04.23: (0.0.5.a1) added test support for plugin settings selection branch
 - 11.05.22: (0.0.4) Updated README (removed cbpi add)
 - 10.05.22: (0.0.3) removed cbpi dependency
 - 27.04.22: (0.0.2) Added MQTT based flowsensor with reset topic
 - 02.10.21: (0.0.1) Initial Release
```

### Comparing `cbpi4-Flowmeter-0.0.6/README.md` & `cbpi4-Flowmeter-0.0.6rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,14 @@
 Actions:
  - Reset Sensor: resets the countet impulses and volume to 0
  - Fake Impulse: fakes the detection of an impulse (i used this for testing because i dont have a flow sensor)
 
 
 
 ## Changelog:
-
-- 10.06.23: (0.0.6) bump version to release
 - 14.05.23: (0.0.6.rc1) added simple VolumeSensor and cbpi4 requirement
 - 14.04.23: (0.0.5.a2) fixed bug in parameter generation
 - 08.04.23: (0.0.5.a1) added test support for plugin settings selection branch
 - 11.05.22: (0.0.4) Updated README (removed cbpi add)
 - 10.05.22: (0.0.3) removed cbpi dependency
 - 27.04.22: (0.0.2) Added MQTT based flowsensor with reset topic
 - 02.10.21: (0.0.1) Initial Release
```

### Comparing `cbpi4-Flowmeter-0.0.6/cbpi4-Flowmeter/__init__.py` & `cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-Flowmeter-0.0.6/cbpi4_Flowmeter.egg-info/PKG-INFO` & `cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-Flowmeter
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Flowsensor / Step Plugin 
 Home-page: https://github.com/PiBrewing/cbpi4-Flowmeter
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -75,16 +75,14 @@
 Actions:
  - Reset Sensor: resets the countet impulses and volume to 0
  - Fake Impulse: fakes the detection of an impulse (i used this for testing because i dont have a flow sensor)
 
 
 
 ## Changelog:
-
-- 10.06.23: (0.0.6) bump version to release
 - 14.05.23: (0.0.6.rc1) added simple VolumeSensor and cbpi4 requirement
 - 14.04.23: (0.0.5.a2) fixed bug in parameter generation
 - 08.04.23: (0.0.5.a1) added test support for plugin settings selection branch
 - 11.05.22: (0.0.4) Updated README (removed cbpi add)
 - 10.05.22: (0.0.3) removed cbpi dependency
 - 27.04.22: (0.0.2) Added MQTT based flowsensor with reset topic
 - 02.10.21: (0.0.1) Initial Release
```

### Comparing `cbpi4-Flowmeter-0.0.6/setup.py` & `cbpi4-Flowmeter-0.0.6rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-Flowmeter',
-      version='0.0.6',
+      version='0.0.6.rc1',
       description='CraftBeerPi4 Flowsensor / Step Plugin ',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-Flowmeter',
       include_package_data=True,
       keywords='globalsettings',
       package_data={
```


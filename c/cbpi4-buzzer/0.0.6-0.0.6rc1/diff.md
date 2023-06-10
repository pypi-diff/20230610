# Comparing `tmp/cbpi4-buzzer-0.0.6.tar.gz` & `tmp/cbpi4-buzzer-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-buzzer-0.0.6.tar", last modified: Sat Jun 10 12:09:39 2023, max compression
+gzip compressed data, was "cbpi4-buzzer-0.0.6rc1.tar", last modified: Thu Jun  8 11:04:56 2023, max compression
```

## Comparing `cbpi4-buzzer-0.0.6.tar` & `cbpi4-buzzer-0.0.6rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:09:39.479455 cbpi4-buzzer-0.0.6/
--rw-rw-rw-   0        0        0    35129 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       33 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1166 2023-06-10 12:09:39.478452 cbpi4-buzzer-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      825 2023-06-10 12:09:16.000000 cbpi4-buzzer-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:09:39.435453 cbpi4-buzzer-0.0.6/cbpi4-buzzer/
--rw-rw-rw-   0        0        0    16128 2023-04-16 15:31:44.000000 cbpi4-buzzer-0.0.6/cbpi4-buzzer/__init__.py
--rw-rw-rw-   0        0        0       29 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.6/cbpi4-buzzer/config.yaml
-drwxrwxrwx   0        0        0        0 2023-06-10 12:09:39.476459 cbpi4-buzzer-0.0.6/cbpi4_buzzer.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-06-10 12:09:39.000000 cbpi4-buzzer-0.0.6/cbpi4_buzzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-10 12:09:39.000000 cbpi4-buzzer-0.0.6/cbpi4_buzzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:09:39.000000 cbpi4-buzzer-0.0.6/cbpi4_buzzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-10 12:09:39.000000 cbpi4-buzzer-0.0.6/cbpi4_buzzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 12:09:39.000000 cbpi4-buzzer-0.0.6/cbpi4_buzzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:09:39.480454 cbpi4-buzzer-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1314 2023-06-02 15:09:01.000000 cbpi4-buzzer-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:56.711928 cbpi4-buzzer-0.0.6rc1/
+-rw-rw-rw-   0        0        0    35129 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.6rc1/LICENSE
+-rw-rw-rw-   0        0        0       33 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.6rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1124 2023-06-08 11:04:56.709928 cbpi4-buzzer-0.0.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-02 15:00:18.000000 cbpi4-buzzer-0.0.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:56.654927 cbpi4-buzzer-0.0.6rc1/cbpi4-buzzer/
+-rw-rw-rw-   0        0        0    16128 2023-04-16 15:31:44.000000 cbpi4-buzzer-0.0.6rc1/cbpi4-buzzer/__init__.py
+-rw-rw-rw-   0        0        0       29 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.6rc1/cbpi4-buzzer/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:56.707925 cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/
+-rw-rw-rw-   0        0        0     1124 2023-06-08 11:04:56.000000 cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-08 11:04:56.000000 cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:04:56.000000 cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 11:04:56.000000 cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 11:04:56.000000 cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:04:56.711928 cbpi4-buzzer-0.0.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1314 2023-06-02 15:09:01.000000 cbpi4-buzzer-0.0.6rc1/setup.py
```

### Comparing `cbpi4-buzzer-0.0.6/LICENSE` & `cbpi4-buzzer-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-buzzer-0.0.6/PKG-INFO` & `cbpi4-buzzer-0.0.6rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-buzzer
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Buzzer Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-buzzer
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -19,15 +19,14 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
-- 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) added cbpi version requirement
 - 16.04.23: (0.0.6.a4) bug fix for parameter generation
 - 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
 - 01.04.21: Initial release
```

### Comparing `cbpi4-buzzer-0.0.6/README.md` & `cbpi4-buzzer-0.0.6rc1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,13 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
-- 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) added cbpi version requirement
 - 16.04.23: (0.0.6.a4) bug fix for parameter generation
 - 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
 - 01.04.21: Initial release
```

### Comparing `cbpi4-buzzer-0.0.6/cbpi4-buzzer/__init__.py` & `cbpi4-buzzer-0.0.6rc1/cbpi4-buzzer/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-buzzer-0.0.6/cbpi4_buzzer.egg-info/PKG-INFO` & `cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-buzzer
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Buzzer Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-buzzer
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -19,15 +19,14 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
-- 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) added cbpi version requirement
 - 16.04.23: (0.0.6.a4) bug fix for parameter generation
 - 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
 - 01.04.21: Initial release
```

### Comparing `cbpi4-buzzer-0.0.6/setup.py` & `cbpi4-buzzer-0.0.6rc1/setup.py`

 * *Files identical despite different names*


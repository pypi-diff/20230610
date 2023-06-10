# Comparing `tmp/cbpi4-buzzer-0.0.4.tar.gz` & `tmp/cbpi4-buzzer-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-buzzer-0.0.4.tar", last modified: Mon Mar 13 19:14:45 2023, max compression
+gzip compressed data, was "cbpi4-buzzer-0.0.6rc1.tar", last modified: Thu Jun  8 11:04:56 2023, max compression
```

## Comparing `cbpi4-buzzer-0.0.4.tar` & `cbpi4-buzzer-0.0.6rc1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 19:14:45.338117 cbpi4-buzzer-0.0.4/
--rw-rw-rw-   0        0        0    35129 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       33 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      903 2023-03-13 19:14:45.336114 cbpi4-buzzer-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-03-13 19:14:13.000000 cbpi4-buzzer-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 19:14:45.307115 cbpi4-buzzer-0.0.4/cbpi4-buzzer/
--rw-rw-rw-   0        0        0     9415 2023-03-13 19:14:13.000000 cbpi4-buzzer-0.0.4/cbpi4-buzzer/__init__.py
--rw-rw-rw-   0        0        0       29 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.4/cbpi4-buzzer/config.yaml
-drwxrwxrwx   0        0        0        0 2023-03-13 19:14:45.333114 cbpi4-buzzer-0.0.4/cbpi4_buzzer.egg-info/
--rw-rw-rw-   0        0        0      903 2023-03-13 19:14:44.000000 cbpi4-buzzer-0.0.4/cbpi4_buzzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-03-13 19:14:44.000000 cbpi4-buzzer-0.0.4/cbpi4_buzzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 19:14:44.000000 cbpi4-buzzer-0.0.4/cbpi4_buzzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-13 19:14:44.000000 cbpi4-buzzer-0.0.4/cbpi4_buzzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 19:14:45.339118 cbpi4-buzzer-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-03-13 19:14:13.000000 cbpi4-buzzer-0.0.4/setup.py
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

### Comparing `cbpi4-buzzer-0.0.4/LICENSE` & `cbpi4-buzzer-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-buzzer-0.0.4/PKG-INFO` & `cbpi4-buzzer-0.0.6rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cbpi4-buzzer
-Version: 0.0.4
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Buzzer Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-buzzer
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CBPi4 Buzzer Plugin
 
 ## Buzzer Plugin calls buzzer on cbpi notifications
@@ -18,12 +19,15 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
+- 02.06.23: (0.0.6.rc1) added cbpi version requirement
+- 16.04.23: (0.0.6.a4) bug fix for parameter generation
+- 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
 - 01.04.21: Initial release
```

### Comparing `cbpi4-buzzer-0.0.4/README.md` & `cbpi4-buzzer-0.0.6rc1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -6,10 +6,13 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
+- 02.06.23: (0.0.6.rc1) added cbpi version requirement
+- 16.04.23: (0.0.6.a4) bug fix for parameter generation
+- 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
 - 01.04.21: Initial release
```

### Comparing `cbpi4-buzzer-0.0.4/cbpi4_buzzer.egg-info/PKG-INFO` & `cbpi4-buzzer-0.0.6rc1/cbpi4_buzzer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cbpi4-buzzer
-Version: 0.0.4
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Buzzer Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-buzzer
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CBPi4 Buzzer Plugin
 
 ## Buzzer Plugin calls buzzer on cbpi notifications
@@ -18,12 +19,15 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
+- 02.06.23: (0.0.6.rc1) added cbpi version requirement
+- 16.04.23: (0.0.6.a4) bug fix for parameter generation
+- 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
 - 01.04.21: Initial release
```

### Comparing `cbpi4-buzzer-0.0.4/setup.py` & `cbpi4-buzzer-0.0.6rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 from setuptools import setup
 
 # read the contents of your README file
 from os import path
+import re
+
+
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
+
+with open(path.join(this_directory, 'version.py'), encoding='latin1') as fp:
+    #long_description = fp.read()
+    try:
+        match = re.search('.*\"(.*)\"', fp.readline())
+        print(match)
+        version = match.group(1)
+    except IndexError:
+        raise RuntimeError('Unable to determine version.')
+
 setup(name='cbpi4-buzzer',
-      version='0.0.4',
+      version=version,
       description='CraftBeerPi4 Buzzer Plugin',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-buzzer',
       license='GPLv3',
+      keywords='globalsettings',
       include_package_data=True,
       package_data={
         # If any package contains *.txt or *.rst files, include them:
       '': ['*.txt', '*.rst', '*.yaml'],
       'cbpi4-buzzer': ['*','*.txt', '*.rst', '*.yaml']},
       packages=['cbpi4-buzzer'],
+      install_requires=[
+      'cbpi4>=4.1.10.rc2'
+      ],
       long_description=long_description,
       long_description_content_type='text/markdown'
      )
```


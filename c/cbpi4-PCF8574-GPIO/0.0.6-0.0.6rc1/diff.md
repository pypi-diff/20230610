# Comparing `tmp/cbpi4-PCF8574-GPIO-0.0.6.tar.gz` & `tmp/cbpi4-PCF8574-GPIO-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-PCF8574-GPIO-0.0.6.tar", last modified: Sat Jun 10 12:14:53 2023, max compression
+gzip compressed data, was "cbpi4-PCF8574-GPIO-0.0.6rc1.tar", last modified: Thu Jun  8 11:04:17 2023, max compression
```

## Comparing `cbpi4-PCF8574-GPIO-0.0.6.tar` & `cbpi4-PCF8574-GPIO-0.0.6rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:14:53.473547 cbpi4-PCF8574-GPIO-0.0.6/
--rw-rw-rw-   0        0        0    35149 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       84 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2285 2023-06-10 12:14:53.471540 cbpi4-PCF8574-GPIO-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1885 2023-06-10 12:13:56.000000 cbpi4-PCF8574-GPIO-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:14:53.451547 cbpi4-PCF8574-GPIO-0.0.6/cbpi4-PCF8574-GPIO/
--rw-rw-rw-   0        0        0     6519 2023-04-07 15:05:20.000000 cbpi4-PCF8574-GPIO-0.0.6/cbpi4-PCF8574-GPIO/__init__.py
--rw-rw-rw-   0        0        0       35 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6/cbpi4-PCF8574-GPIO/config.yaml
-drwxrwxrwx   0        0        0        0 2023-06-10 12:14:53.468561 cbpi4-PCF8574-GPIO-0.0.6/cbpi4_PCF8574_GPIO.egg-info/
--rw-rw-rw-   0        0        0     2285 2023-06-10 12:14:53.000000 cbpi4-PCF8574-GPIO-0.0.6/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-06-10 12:14:53.000000 cbpi4-PCF8574-GPIO-0.0.6/cbpi4_PCF8574_GPIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:14:53.000000 cbpi4-PCF8574-GPIO-0.0.6/cbpi4_PCF8574_GPIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-10 12:14:53.000000 cbpi4-PCF8574-GPIO-0.0.6/cbpi4_PCF8574_GPIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-10 12:14:53.000000 cbpi4-PCF8574-GPIO-0.0.6/cbpi4_PCF8574_GPIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:14:53.474542 cbpi4-PCF8574-GPIO-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      992 2023-06-10 12:14:03.000000 cbpi4-PCF8574-GPIO-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:17.115646 cbpi4-PCF8574-GPIO-0.0.6rc1/
+-rw-rw-rw-   0        0        0    35149 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/LICENSE
+-rw-rw-rw-   0        0        0       84 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2243 2023-06-08 11:04:17.114643 cbpi4-PCF8574-GPIO-0.0.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1841 2023-06-02 15:13:11.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:17.079641 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/
+-rw-rw-rw-   0        0        0     6519 2023-04-07 15:05:20.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/__init__.py
+-rw-rw-rw-   0        0        0       35 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:17.112640 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/
+-rw-rw-rw-   0        0        0     2243 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:04:17.115646 cbpi4-PCF8574-GPIO-0.0.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-06-02 15:12:44.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/setup.py
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.6/LICENSE` & `cbpi4-PCF8574-GPIO-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-PCF8574-GPIO-0.0.6/PKG-INFO` & `cbpi4-PCF8574-GPIO-0.0.6rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-PCF8574-GPIO
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 PCF8574 Actor Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-PCF8574-GPIO
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -37,15 +37,14 @@
 
 Some information can be found here: https://www.instructables.com/PCF8574-GPIO-Extender-With-Arduino-and-NodeMCU/
 Connect the device to 5 Volt, GND and your I2C bus. Check the Address ans set it to a different address if required
 According to the datasheet, the pins can handle up to 25 mA. If you want to trigger an SSR or a relais, it is recommended to add a darlington array like the ULN2308
 
 ### Changelog:
 
-- 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) Added cbpi4 version requirement
 - 07.04.23: (0.0.6.a1) Added fucntions for plugins settings selection branches of server and ui
 - 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 10.12.21: (0.0.3) Updated README
 - 09.12.21: (0.0.2) Bug Fix for power
 - 09-12-21: (0.0.1) Initial release
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.6/README.md` & `cbpi4-PCF8574-GPIO-0.0.6rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 Some information can be found here: https://www.instructables.com/PCF8574-GPIO-Extender-With-Arduino-and-NodeMCU/
 Connect the device to 5 Volt, GND and your I2C bus. Check the Address ans set it to a different address if required
 According to the datasheet, the pins can handle up to 25 mA. If you want to trigger an SSR or a relais, it is recommended to add a darlington array like the ULN2308
 
 ### Changelog:
 
-- 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) Added cbpi4 version requirement
 - 07.04.23: (0.0.6.a1) Added fucntions for plugins settings selection branches of server and ui
 - 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 10.12.21: (0.0.3) Updated README
 - 09.12.21: (0.0.2) Bug Fix for power
 - 09-12-21: (0.0.1) Initial release
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.6/cbpi4-PCF8574-GPIO/__init__.py` & `cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-PCF8574-GPIO-0.0.6/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO` & `cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-PCF8574-GPIO
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 PCF8574 Actor Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-PCF8574-GPIO
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -37,15 +37,14 @@
 
 Some information can be found here: https://www.instructables.com/PCF8574-GPIO-Extender-With-Arduino-and-NodeMCU/
 Connect the device to 5 Volt, GND and your I2C bus. Check the Address ans set it to a different address if required
 According to the datasheet, the pins can handle up to 25 mA. If you want to trigger an SSR or a relais, it is recommended to add a darlington array like the ULN2308
 
 ### Changelog:
 
-- 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) Added cbpi4 version requirement
 - 07.04.23: (0.0.6.a1) Added fucntions for plugins settings selection branches of server and ui
 - 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 10.12.21: (0.0.3) Updated README
 - 09.12.21: (0.0.2) Bug Fix for power
 - 09-12-21: (0.0.1) Initial release
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.6/setup.py` & `cbpi4-PCF8574-GPIO-0.0.6rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-PCF8574-GPIO',
-      version='0.0.6',
+      version='0.0.6.rc1',
       description='CraftBeerPi4 PCF8574 Actor Plugin',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-PCF8574-GPIO',
       include_package_data=True,
       keywords='globalsettings',
       package_data={
```


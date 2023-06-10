# Comparing `tmp/cbpi4-system-0.0.9.tar.gz` & `tmp/cbpi4-system-0.0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-system-0.0.9.tar", last modified: Sat Jun 10 12:07:07 2023, max compression
+gzip compressed data, was "cbpi4-system-0.0.9rc1.tar", last modified: Thu Jun  8 11:03:36 2023, max compression
```

## Comparing `cbpi4-system-0.0.9.tar` & `cbpi4-system-0.0.9rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:07:07.985144 cbpi4-system-0.0.9/
--rw-rw-rw-   0        0        0    35149 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       72 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2189 2023-06-10 12:07:07.983142 cbpi4-system-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1790 2023-06-10 12:06:44.000000 cbpi4-system-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:07:07.930155 cbpi4-system-0.0.9/cbpi4-system/
--rw-rw-rw-   0        0        0    13312 2023-04-16 15:17:45.000000 cbpi4-system-0.0.9/cbpi4-system/__init__.py
--rw-rw-rw-   0        0        0       29 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9/cbpi4-system/config.yaml
-drwxrwxrwx   0        0        0        0 2023-06-10 12:07:07.979139 cbpi4-system-0.0.9/cbpi4_system.egg-info/
--rw-rw-rw-   0        0        0     2189 2023-06-10 12:07:07.000000 cbpi4-system-0.0.9/cbpi4_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-10 12:07:07.000000 cbpi4-system-0.0.9/cbpi4_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:07:07.000000 cbpi4-system-0.0.9/cbpi4_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-10 12:07:07.000000 cbpi4-system-0.0.9/cbpi4_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 12:07:07.000000 cbpi4-system-0.0.9/cbpi4_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:07:07.986143 cbpi4-system-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1029 2023-06-10 12:06:22.000000 cbpi4-system-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:03:36.217127 cbpi4-system-0.0.9rc1/
+-rw-rw-rw-   0        0        0    35149 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9rc1/LICENSE
+-rw-rw-rw-   0        0        0       72 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2145 2023-06-08 11:03:36.216126 cbpi4-system-0.0.9rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1744 2023-06-02 15:17:20.000000 cbpi4-system-0.0.9rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:03:36.178124 cbpi4-system-0.0.9rc1/cbpi4-system/
+-rw-rw-rw-   0        0        0    13312 2023-04-16 15:17:45.000000 cbpi4-system-0.0.9rc1/cbpi4-system/__init__.py
+-rw-rw-rw-   0        0        0       29 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9rc1/cbpi4-system/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:03:36.214129 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/
+-rw-rw-rw-   0        0        0     2145 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:03:36.218123 cbpi4-system-0.0.9rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-06-02 15:16:49.000000 cbpi4-system-0.0.9rc1/setup.py
```

### Comparing `cbpi4-system-0.0.9/LICENSE` & `cbpi4-system-0.0.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-system-0.0.9/PKG-INFO` & `cbpi4-system-0.0.9rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-system
-Version: 0.0.9
+Version: 0.0.9rc1
 Summary: CraftBeerPi4 Plugin for system fucntions
 Home-page: https://github.com/PiBrewing/cbpi4-system
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -13,41 +13,40 @@
 
 # CraftBeerPi4 System Functions Plugin
 
 ### Functions:
 
 - Plugin has capability to reboot Pi every day at a time that can be specified in the settings.
 
-![Auto Reboot](https://github.com/PiBrewing/cbpi4-system/blob/main/AutoReboot.png?raw=true)
+![Auto Reboot](https://github.com/avollkopf/cbpi4-system/blob/main/AutoReboot.png?raw=true)
 
 ### Sensors	
 
 Plugin will add system 'sensors' to monitor some system parameters. The psutil package is currently used for that purpose:
 	
 - CPU Load: 		CPU load in % (psutil: cpu_perc)
 - Available Memory:	Available system memory in Mb (psutil: vitrual_memory -> available)
 - Used memory:		Used memory in percent (psutil: vitrual_memory -> percent)
 - CPU Temp:		CPU temperature (psutil: sensors_temperatures -> cpu_thermal)
 
 Each parameter has to be added as individual sensor.
 	
-![Sensor Config](https://github.com/PiBrewing/cbpi4-system/blob/main/SystemSensor.png?raw=true)
+![Sensor Config](https://github.com/avollkopf/cbpi4-system/blob/main/SystemSensor.png?raw=true)
 
 ### Installation: 
 - sudo pip3 install cbpi4-system
-- or install from repo: sudo pip3 install https://github.com/PiBrewing/cbpi4-system/archive/main.zip
+- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-system/archive/main.zip
 	
 ### Usage:
 
 - Add Hardware under Sensor and choose SystemSensor as Type
 - Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
 
 ### Changelog:
 
-- 10.06.23: (0.0.9) change version to release
 - 02.06.23: (0.0.9.rc1) add cbpi4 version requirements
 - 16.04.23: (0.0.9.a6) fixed bug with creation of parameters
 - 05.04.23: (0.0.9.a5) test for gloabl plugin settings selection branch
 - 08.01.23: (0.0.8) updated requirements
 - 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.4) Reduced amount of mqtt traffic
 - 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
```

### Comparing `cbpi4-system-0.0.9/README.md` & `cbpi4-system-0.0.9rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # CraftBeerPi4 System Functions Plugin
 
 ### Functions:
 
 - Plugin has capability to reboot Pi every day at a time that can be specified in the settings.
 
-![Auto Reboot](https://github.com/PiBrewing/cbpi4-system/blob/main/AutoReboot.png?raw=true)
+![Auto Reboot](https://github.com/avollkopf/cbpi4-system/blob/main/AutoReboot.png?raw=true)
 
 ### Sensors	
 
 Plugin will add system 'sensors' to monitor some system parameters. The psutil package is currently used for that purpose:
 	
 - CPU Load: 		CPU load in % (psutil: cpu_perc)
 - Available Memory:	Available system memory in Mb (psutil: vitrual_memory -> available)
 - Used memory:		Used memory in percent (psutil: vitrual_memory -> percent)
 - CPU Temp:		CPU temperature (psutil: sensors_temperatures -> cpu_thermal)
 
 Each parameter has to be added as individual sensor.
 	
-![Sensor Config](https://github.com/PiBrewing/cbpi4-system/blob/main/SystemSensor.png?raw=true)
+![Sensor Config](https://github.com/avollkopf/cbpi4-system/blob/main/SystemSensor.png?raw=true)
 
 ### Installation: 
 - sudo pip3 install cbpi4-system
-- or install from repo: sudo pip3 install https://github.com/PiBrewing/cbpi4-system/archive/main.zip
+- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-system/archive/main.zip
 	
 ### Usage:
 
 - Add Hardware under Sensor and choose SystemSensor as Type
 - Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
 
 ### Changelog:
 
-- 10.06.23: (0.0.9) change version to release
 - 02.06.23: (0.0.9.rc1) add cbpi4 version requirements
 - 16.04.23: (0.0.9.a6) fixed bug with creation of parameters
 - 05.04.23: (0.0.9.a5) test for gloabl plugin settings selection branch
 - 08.01.23: (0.0.8) updated requirements
 - 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.4) Reduced amount of mqtt traffic
 - 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
```

### Comparing `cbpi4-system-0.0.9/cbpi4-system/__init__.py` & `cbpi4-system-0.0.9rc1/cbpi4-system/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-system-0.0.9/cbpi4_system.egg-info/PKG-INFO` & `cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-system
-Version: 0.0.9
+Version: 0.0.9rc1
 Summary: CraftBeerPi4 Plugin for system fucntions
 Home-page: https://github.com/PiBrewing/cbpi4-system
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -13,41 +13,40 @@
 
 # CraftBeerPi4 System Functions Plugin
 
 ### Functions:
 
 - Plugin has capability to reboot Pi every day at a time that can be specified in the settings.
 
-![Auto Reboot](https://github.com/PiBrewing/cbpi4-system/blob/main/AutoReboot.png?raw=true)
+![Auto Reboot](https://github.com/avollkopf/cbpi4-system/blob/main/AutoReboot.png?raw=true)
 
 ### Sensors	
 
 Plugin will add system 'sensors' to monitor some system parameters. The psutil package is currently used for that purpose:
 	
 - CPU Load: 		CPU load in % (psutil: cpu_perc)
 - Available Memory:	Available system memory in Mb (psutil: vitrual_memory -> available)
 - Used memory:		Used memory in percent (psutil: vitrual_memory -> percent)
 - CPU Temp:		CPU temperature (psutil: sensors_temperatures -> cpu_thermal)
 
 Each parameter has to be added as individual sensor.
 	
-![Sensor Config](https://github.com/PiBrewing/cbpi4-system/blob/main/SystemSensor.png?raw=true)
+![Sensor Config](https://github.com/avollkopf/cbpi4-system/blob/main/SystemSensor.png?raw=true)
 
 ### Installation: 
 - sudo pip3 install cbpi4-system
-- or install from repo: sudo pip3 install https://github.com/PiBrewing/cbpi4-system/archive/main.zip
+- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-system/archive/main.zip
 	
 ### Usage:
 
 - Add Hardware under Sensor and choose SystemSensor as Type
 - Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
 
 ### Changelog:
 
-- 10.06.23: (0.0.9) change version to release
 - 02.06.23: (0.0.9.rc1) add cbpi4 version requirements
 - 16.04.23: (0.0.9.a6) fixed bug with creation of parameters
 - 05.04.23: (0.0.9.a5) test for gloabl plugin settings selection branch
 - 08.01.23: (0.0.8) updated requirements
 - 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.4) Reduced amount of mqtt traffic
 - 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
```

### Comparing `cbpi4-system-0.0.9/setup.py` & `cbpi4-system-0.0.9rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-system',
-      version='0.0.9',
+      version='0.0.9.rc1',
       description='CraftBeerPi4 Plugin for system fucntions',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-system',
       include_package_data=True,
       keywords='globalsettings',
       package_data={
```


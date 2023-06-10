# Comparing `tmp/cbpi4-scd30-CO2-Sensor-0.0.6.tar.gz` & `tmp/cbpi4-scd30-CO2-Sensor-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-scd30-CO2-Sensor-0.0.6.tar", last modified: Sat Jun 10 12:13:02 2023, max compression
+gzip compressed data, was "cbpi4-scd30-CO2-Sensor-0.0.6rc1.tar", last modified: Thu Jun  8 11:02:07 2023, max compression
```

## Comparing `cbpi4-scd30-CO2-Sensor-0.0.6.tar` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:13:02.102277 cbpi4-scd30-CO2-Sensor-0.0.6/
--rw-rw-rw-   0        0        0    35149 2021-11-29 14:48:50.000000 cbpi4-scd30-CO2-Sensor-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       92 2023-04-08 13:04:58.000000 cbpi4-scd30-CO2-Sensor-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2543 2023-06-10 12:13:02.100274 cbpi4-scd30-CO2-Sensor-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2116 2023-06-10 12:12:43.000000 cbpi4-scd30-CO2-Sensor-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:13:02.048977 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4-scd30-CO2-Sensor/
--rw-rw-rw-   0        0        0     8172 2023-04-16 15:20:12.000000 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4-scd30-CO2-Sensor/__init__.py
--rw-rw-rw-   0        0        0       39 2023-04-08 13:05:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4-scd30-CO2-Sensor/config.yaml
-drwxrwxrwx   0        0        0        0 2023-06-10 12:13:02.097270 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4_scd30_CO2_Sensor.egg-info/
--rw-rw-rw-   0        0        0     2543 2023-06-10 12:13:01.000000 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-06-10 12:13:01.000000 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4_scd30_CO2_Sensor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:13:01.000000 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4_scd30_CO2_Sensor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-10 12:13:01.000000 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4_scd30_CO2_Sensor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-10 12:13:01.000000 cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4_scd30_CO2_Sensor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:13:02.102277 cbpi4-scd30-CO2-Sensor-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-06-10 12:12:23.000000 cbpi4-scd30-CO2-Sensor-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:07.926223 cbpi4-scd30-CO2-Sensor-0.0.6rc1/
+-rw-rw-rw-   0        0        0    35149 2021-11-29 14:48:50.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/LICENSE
+-rw-rw-rw-   0        0        0       92 2023-04-08 13:04:58.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2501 2023-06-08 11:02:07.925168 cbpi4-scd30-CO2-Sensor-0.0.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     2072 2023-06-02 15:19:03.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:07.874807 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/
+-rw-rw-rw-   0        0        0     8172 2023-04-16 15:20:12.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-04-08 13:05:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:07.922487 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/
+-rw-rw-rw-   0        0        0     2501 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:02:07.926223 cbpi4-scd30-CO2-Sensor-0.0.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-06-02 15:19:08.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/setup.py
```

### Comparing `cbpi4-scd30-CO2-Sensor-0.0.6/LICENSE` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-scd30-CO2-Sensor-0.0.6/PKG-INFO` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-scd30-CO2-Sensor
-Version: 0.0.6
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Plugin for SCD30 based CO2 Sensor
 Home-page: https://github.com/PiBrewing/cbpi4-scd30-co2-sensor
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -45,15 +45,14 @@
 
 Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
 
 The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
 
 ### Changelog:
 
-- 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) added cbpi4 requirement
 - 16.04.23: (0.0.6.a6) fixed bug in parameter generation
 - 04.04.23: (0.0.6.a5) test for plugin settings selection branch
 - 10.05.22: (0.0.4) Removed cbpi requirement
 - 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.2) Reduction of mqtt traffic
 - 23.07.21: (0.0.1) Initial commit
```

### Comparing `cbpi4-scd30-CO2-Sensor-0.0.6/README.md` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,60 @@
-# CraftBeerPi4 SCD30 based CO2 Sensor Plugin
-
-### Sensors	
-
-Plugin will add system a sensor to monitor for instance CO2 monitoring in your fermentation room
-
-![Sensor Config](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings.png?raw=true)
-	
-- CO2: 					CO2 value in ppm
-- Relative Humidity:	Relative humidity in %
-- Temperatur:			Temperature
-
-Each parameter has to be added as individual sensor.
-	
-![Multiple Sensors](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-multiple-scd30.png?raw=true)
-
-### Installation: 
-- sudo pip3 install cbpi4-scd30_CO2_Sensor
-- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-scd30-co2-sensor/archive/main.zip
-	
-### Usage:
-
-- Configure the update interval of the sensor data in the cbpi global settings. Although shorter cycles ar possible, 30 or 60 seconds should be more than sufficient.
-
-![Global Sensor Interval Settings](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings-interval.png?raw=true)
-
-- Add Hardware under Sensor and choose SCD30 Sensor as Type and select the parameter you want to monitor.
-
-### Hardware requirements:
-
-A datasheet of the sensor can be found here: https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/9.5_CO2/Sensirion_CO2_Sensors_SCD30_Datasheet.pdf
-
-Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
-
-The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
-
-### Changelog:
-
-- 10.06.23: (0.0.6) bump version to release
-- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
-- 16.04.23: (0.0.6.a6) fixed bug in parameter generation
-- 04.04.23: (0.0.6.a5) test for plugin settings selection branch
-- 10.05.22: (0.0.4) Removed cbpi requirement
-- 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
-- 12.01.22: (0.0.2) Reduction of mqtt traffic
-- 23.07.21: (0.0.1) Initial commit
+Metadata-Version: 2.1
+Name: cbpi4-scd30-CO2-Sensor
+Version: 0.0.6rc1
+Summary: CraftBeerPi4 Plugin for SCD30 based CO2 Sensor
+Home-page: https://github.com/PiBrewing/cbpi4-scd30-co2-sensor
+Author: Alexander Vollkopf
+Author-email: avollkopf@web.de
+License: GPLv3
+Keywords: globalsettings
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CraftBeerPi4 SCD30 based CO2 Sensor Plugin
+
+### Sensors	
+
+Plugin will add system a sensor to monitor for instance CO2 monitoring in your fermentation room
+
+![Sensor Config](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings.png?raw=true)
+	
+- CO2: 					CO2 value in ppm
+- Relative Humidity:	Relative humidity in %
+- Temperatur:			Temperature
+
+Each parameter has to be added as individual sensor.
+	
+![Multiple Sensors](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-multiple-scd30.png?raw=true)
+
+### Installation: 
+- sudo pip3 install cbpi4-scd30_CO2_Sensor
+- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-scd30-co2-sensor/archive/main.zip
+	
+### Usage:
+
+- Configure the update interval of the sensor data in the cbpi global settings. Although shorter cycles ar possible, 30 or 60 seconds should be more than sufficient.
+
+![Global Sensor Interval Settings](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings-interval.png?raw=true)
+
+- Add Hardware under Sensor and choose SCD30 Sensor as Type and select the parameter you want to monitor.
+
+### Hardware requirements:
+
+A datasheet of the sensor can be found here: https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/9.5_CO2/Sensirion_CO2_Sensors_SCD30_Datasheet.pdf
+
+Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
+
+The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
+
+### Changelog:
+
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 16.04.23: (0.0.6.a6) fixed bug in parameter generation
+- 04.04.23: (0.0.6.a5) test for plugin settings selection branch
+- 10.05.22: (0.0.4) Removed cbpi requirement
+- 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
+- 12.01.22: (0.0.2) Reduction of mqtt traffic
+- 23.07.21: (0.0.1) Initial commit
+
+
```

### Comparing `cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4-scd30-CO2-Sensor/__init__.py` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-scd30-CO2-Sensor-0.0.6/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,45 @@
-Metadata-Version: 2.1
-Name: cbpi4-scd30-CO2-Sensor
-Version: 0.0.6
-Summary: CraftBeerPi4 Plugin for SCD30 based CO2 Sensor
-Home-page: https://github.com/PiBrewing/cbpi4-scd30-co2-sensor
-Author: Alexander Vollkopf
-Author-email: avollkopf@web.de
-License: GPLv3
-Keywords: globalsettings
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CraftBeerPi4 SCD30 based CO2 Sensor Plugin
-
-### Sensors	
-
-Plugin will add system a sensor to monitor for instance CO2 monitoring in your fermentation room
-
-![Sensor Config](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings.png?raw=true)
-	
-- CO2: 					CO2 value in ppm
-- Relative Humidity:	Relative humidity in %
-- Temperatur:			Temperature
-
-Each parameter has to be added as individual sensor.
-	
-![Multiple Sensors](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-multiple-scd30.png?raw=true)
-
-### Installation: 
-- sudo pip3 install cbpi4-scd30_CO2_Sensor
-- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-scd30-co2-sensor/archive/main.zip
-	
-### Usage:
-
-- Configure the update interval of the sensor data in the cbpi global settings. Although shorter cycles ar possible, 30 or 60 seconds should be more than sufficient.
-
-![Global Sensor Interval Settings](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings-interval.png?raw=true)
-
-- Add Hardware under Sensor and choose SCD30 Sensor as Type and select the parameter you want to monitor.
-
-### Hardware requirements:
-
-A datasheet of the sensor can be found here: https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/9.5_CO2/Sensirion_CO2_Sensors_SCD30_Datasheet.pdf
-
-Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
-
-The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
-
-### Changelog:
-
-- 10.06.23: (0.0.6) bump version to release
-- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
-- 16.04.23: (0.0.6.a6) fixed bug in parameter generation
-- 04.04.23: (0.0.6.a5) test for plugin settings selection branch
-- 10.05.22: (0.0.4) Removed cbpi requirement
-- 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
-- 12.01.22: (0.0.2) Reduction of mqtt traffic
-- 23.07.21: (0.0.1) Initial commit
-
-
+# CraftBeerPi4 SCD30 based CO2 Sensor Plugin
+
+### Sensors	
+
+Plugin will add system a sensor to monitor for instance CO2 monitoring in your fermentation room
+
+![Sensor Config](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings.png?raw=true)
+	
+- CO2: 					CO2 value in ppm
+- Relative Humidity:	Relative humidity in %
+- Temperatur:			Temperature
+
+Each parameter has to be added as individual sensor.
+	
+![Multiple Sensors](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-multiple-scd30.png?raw=true)
+
+### Installation: 
+- sudo pip3 install cbpi4-scd30_CO2_Sensor
+- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-scd30-co2-sensor/archive/main.zip
+	
+### Usage:
+
+- Configure the update interval of the sensor data in the cbpi global settings. Although shorter cycles ar possible, 30 or 60 seconds should be more than sufficient.
+
+![Global Sensor Interval Settings](https://github.com/avollkopf/cbpi4-scd30-co2-sensor/blob/main/cbpi4-scd30-settings-interval.png?raw=true)
+
+- Add Hardware under Sensor and choose SCD30 Sensor as Type and select the parameter you want to monitor.
+
+### Hardware requirements:
+
+A datasheet of the sensor can be found here: https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/9.5_CO2/Sensirion_CO2_Sensors_SCD30_Datasheet.pdf
+
+Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
+
+The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
+
+### Changelog:
+
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 16.04.23: (0.0.6.a6) fixed bug in parameter generation
+- 04.04.23: (0.0.6.a5) test for plugin settings selection branch
+- 10.05.22: (0.0.4) Removed cbpi requirement
+- 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
+- 12.01.22: (0.0.2) Reduction of mqtt traffic
+- 23.07.21: (0.0.1) Initial commit
```

### Comparing `cbpi4-scd30-CO2-Sensor-0.0.6/setup.py` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-scd30-CO2-Sensor',
-      version='0.0.6',
+      version='0.0.6.rc1',
       description='CraftBeerPi4 Plugin for SCD30 based CO2 Sensor',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-scd30-co2-sensor',
       license='GPLv3',
       include_package_data=True,
       keywords='globalsettings',
```


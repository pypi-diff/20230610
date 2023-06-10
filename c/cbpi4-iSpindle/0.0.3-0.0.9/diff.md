# Comparing `tmp/cbpi4-iSpindle-0.0.3.tar.gz` & `tmp/cbpi4-iSpindle-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cbpi4-iSpindle-0.0.3.tar", last modified: Fri Apr  2 11:49:11 2021, max compression
+gzip compressed data, was "cbpi4-iSpindle-0.0.9.tar", last modified: Tue May 10 16:29:43 2022, max compression
```

## Comparing `cbpi4-iSpindle-0.0.3.tar` & `cbpi4-iSpindle-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-02 11:49:11.000000 cbpi4-iSpindle-0.0.3/
--rw-r--r--   0 pi        (1000) pi        (1000)       76 2021-03-07 10:50:37.000000 cbpi4-iSpindle-0.0.3/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     2511 2021-04-02 11:49:11.000000 cbpi4-iSpindle-0.0.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1941 2021-03-15 06:21:56.000000 cbpi4-iSpindle-0.0.3/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-02 11:49:11.000000 cbpi4-iSpindle-0.0.3/cbpi4-iSpindle/
--rw-r--r--   0 pi        (1000) pi        (1000)     4297 2021-03-24 13:10:15.000000 cbpi4-iSpindle-0.0.3/cbpi4-iSpindle/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)       31 2021-03-07 10:50:37.000000 cbpi4-iSpindle-0.0.3/cbpi4-iSpindle/config.yaml
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-02 11:49:11.000000 cbpi4-iSpindle-0.0.3/cbpi4_iSpindle.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2511 2021-04-02 11:49:10.000000 cbpi4-iSpindle-0.0.3/cbpi4_iSpindle.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      273 2021-04-02 11:49:11.000000 cbpi4-iSpindle-0.0.3/cbpi4_iSpindle.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-04-02 11:49:10.000000 cbpi4-iSpindle-0.0.3/cbpi4_iSpindle.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2021-04-02 11:49:10.000000 cbpi4-iSpindle-0.0.3/cbpi4_iSpindle.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2021-04-02 11:49:10.000000 cbpi4-iSpindle-0.0.3/cbpi4_iSpindle.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2021-04-02 11:49:11.000000 cbpi4-iSpindle-0.0.3/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      940 2021-03-17 05:39:04.000000 cbpi4-iSpindle-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-10 16:29:43.885114 cbpi4-iSpindle-0.0.9/
+-rw-rw-rw-   0        0        0    35149 2021-11-29 14:46:13.000000 cbpi4-iSpindle-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       76 2021-11-29 14:46:13.000000 cbpi4-iSpindle-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2649 2022-05-10 16:29:43.884117 cbpi4-iSpindle-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2279 2022-05-10 15:29:35.000000 cbpi4-iSpindle-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-10 16:29:43.838114 cbpi4-iSpindle-0.0.9/cbpi4-iSpindle/
+-rw-rw-rw-   0        0        0     5984 2022-01-14 15:44:11.000000 cbpi4-iSpindle-0.0.9/cbpi4-iSpindle/__init__.py
+-rw-rw-rw-   0        0        0       31 2021-11-29 14:46:13.000000 cbpi4-iSpindle-0.0.9/cbpi4-iSpindle/config.yaml
+drwxrwxrwx   0        0        0        0 2022-05-10 16:29:43.881117 cbpi4-iSpindle-0.0.9/cbpi4_iSpindle.egg-info/
+-rw-rw-rw-   0        0        0     2649 2022-05-10 16:29:43.000000 cbpi4-iSpindle-0.0.9/cbpi4_iSpindle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2022-05-10 16:29:43.000000 cbpi4-iSpindle-0.0.9/cbpi4_iSpindle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-10 16:29:43.000000 cbpi4-iSpindle-0.0.9/cbpi4_iSpindle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2022-05-10 16:29:43.000000 cbpi4-iSpindle-0.0.9/cbpi4_iSpindle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-10 16:29:43.885114 cbpi4-iSpindle-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      876 2022-05-10 15:28:57.000000 cbpi4-iSpindle-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cbpi4-iSpindle-0.0.3/PKG-INFO` & `cbpi4-iSpindle-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,53 @@
-Metadata-Version: 2.1
-Name: cbpi4-iSpindle
-Version: 0.0.3
-Summary: CraftBeerPi4 iSpindle Sensor Plugin
-Home-page: https://github.com/avollkopf/cbpi4-iSpindle
-Author: Alexander Vollkopf
-Author-email: avollkopf@web.de
-License: GPLv 3.0
-Description: # CraftBeerPi4 iSpindle Sensor Plugin
-        
-        - Initial Version which has to be considered as beta
-            - Data Transfer is working from the SPindle itself and from the TCP server via forward-
-            - TCP Server does not require any changes. Only the port needs to be changed from 5000 to 8000
-            - The Spindel Connection needs to be changed from CraftbeerPi to HTTP as shown in the image below
-            - For Server, please enter the IP address of your CBPi4 Server.
-            - Enter 8000 for Port and '/api/hydrometer/v1/data' for path.
-        
-        ![iSpindle Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Spindle_Connection_Settings.png?raw=true)
-        
-        - Installation: 
-            - pip install cbpi4-iSpindle (or from the GIT repo)
-            - cbpi add cbpi4-iSpindle
-        - Usage:
-            - Add Hardware under Sensor and choose iSpindle as Type
-        
-        - Units are currently not displayed in CBPi4 for Sensors. You need to add that on you own in the Dashboard
-        - If you want to retrieve multiple parameters from one Spindle, you need to add the Spindle several times as sensor and choose different Types
-            - The Sensor name should be different for each of your sensors
-        - The settings are shown below.
-            - Name: This is the name of your sensor shown in CBPi4. e.g. iSpindleXXX - Angle
-            - iSpindle: Name of your Spindle that you entered in the Spindle setup page. This name must match to the Spindle. Otherwise no data will be collected.
-            - Type: Temperature, Gravity/Angle, Battery (Choose one type)
-                - If Gravity/Angle is choosen and the Polynomial field is left empty, the angle data is stored
-            - Polynomial: The polynomial to calculate gravity. '^' is not working. You need to uses tilt*tilt*tilt for '^3' and tilt*tilt for '^2'
-            - Units: Choose SG, Brix or °P. This has impact on the calculated digits
-        
-        ![CBPi4 Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Settings.png?raw=true)
-        
-        Changelog:
-        
-        15.03.21: Changes to suppoer cbpi >= 4.0.0.31
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: cbpi4-iSpindle
+Version: 0.0.9
+Summary: CraftBeerPi4 iSpindle Sensor Plugin
+Home-page: https://github.com/avollkopf/cbpi4-iSpindle
+Author: Alexander Vollkopf
+Author-email: avollkopf@web.de
+License: GPLv 3.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CraftBeerPi4 iSpindle Sensor Plugin
+
+- Initial Version which has to be considered as beta
+    - Data Transfer is working from the SPindle itself and from the TCP server via forward-
+    - TCP Server does not require any changes. Only the port needs to be changed from 5000 to 8000
+    - The Spindel Connection needs to be changed from CraftbeerPi to HTTP as shown in the image below
+    - For Server, please enter the IP address of your CBPi4 Server.
+    - Enter 8000 for Port and '/api/hydrometer/v1/data' for path.
+
+![iSpindle Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Spindle_Connection_Settings.png?raw=true)
+
+- Installation: 
+    - pip install cbpi4-iSpindle (or from the GIT repo)
+    - cbpi add cbpi4-iSpindle
+- Usage:
+    - Add Hardware under Sensor and choose iSpindle as Type
+
+- Units are currently not displayed in CBPi4 for Sensors. You need to add that on you own in the Dashboard
+- If you want to retrieve multiple parameters from one Spindle, you need to add the Spindle several times as sensor and choose different Types
+    - The Sensor name should be different for each of your sensors
+- The settings are shown below.
+    - Name: This is the name of your sensor shown in CBPi4. e.g. iSpindleXXX - Angle
+    - iSpindle: Name of your Spindle that you entered in the Spindle setup page. This name must match to the Spindle. Otherwise no data will be collected.
+    - Type: Temperature, Gravity/Angle, Battery (Choose one type)
+        - If Gravity/Angle is choosen and the Polynomial field is left empty, the angle data is stored
+    - Polynomial: The polynomial to calculate gravity. '^' is not working. You need to uses tilt*tilt*tilt for '^3' and tilt*tilt for '^2'
+    - Units: Choose SG, Brix or °P. This has impact on the calculated digits
+
+![CBPi4 Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Settings.png?raw=true)
+
+### Changelog:
+
+- 10.05.22: (0.0.9) Removed cbpi dependency
+- 16.01.22: (0.0.8) Adaption for cbpi 4.0.1.2
+- 13.01.22: (0.0.7) Reduced mqtt traffic -> update only for new value
+- 23.11.21: (0.0.6) Added RSSI to available parmeters
+- 10.06.21: (0.0.5) Fix to improve UI behavior with respect to frequency of value update
+- 17.04.21: Some small fixes
+- 15.03.21: Changes to suppoer cbpi >= 4.0.0.31
+
+
```

### Comparing `cbpi4-iSpindle-0.0.3/README.md` & `cbpi4-iSpindle-0.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -24,10 +24,16 @@
     - Type: Temperature, Gravity/Angle, Battery (Choose one type)
         - If Gravity/Angle is choosen and the Polynomial field is left empty, the angle data is stored
     - Polynomial: The polynomial to calculate gravity. '^' is not working. You need to uses tilt*tilt*tilt for '^3' and tilt*tilt for '^2'
     - Units: Choose SG, Brix or °P. This has impact on the calculated digits
 
 ![CBPi4 Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Settings.png?raw=true)
 
-Changelog:
+### Changelog:
 
-15.03.21: Changes to suppoer cbpi >= 4.0.0.31
+- 10.05.22: (0.0.9) Removed cbpi dependency
+- 16.01.22: (0.0.8) Adaption for cbpi 4.0.1.2
+- 13.01.22: (0.0.7) Reduced mqtt traffic -> update only for new value
+- 23.11.21: (0.0.6) Added RSSI to available parmeters
+- 10.06.21: (0.0.5) Fix to improve UI behavior with respect to frequency of value update
+- 17.04.21: Some small fixes
+- 15.03.21: Changes to suppoer cbpi >= 4.0.0.31
```

### Comparing `cbpi4-iSpindle-0.0.3/cbpi4-iSpindle/__init__.py` & `cbpi4-iSpindle-0.0.9/cbpi4-iSpindle/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import asyncio
 import random
 from cbpi.api import *
 from aiohttp import web
 from cbpi.api import *
 import re
 import time
+import json
 
 logger = logging.getLogger(__name__)
 
 cache = {}
 
 async def calcGravity(polynom, tilt, unitsGravity):
 	if unitsGravity == "SG":
@@ -25,104 +26,140 @@
 	# Calculate gravity from polynomial
 	tilt = float(tilt)
 	result = eval(polynom)
 	result = round(float(result),rounddec)
 	return result
 
 @parameters([Property.Text(label="iSpindle", configurable=True, description="Enter the name of your iSpindel"),
-             Property.Select("Type", options=["Temperature", "Gravity/Angle", "Battery"], description="Select which type of data to register for this sensor. For Angle, Polynomial has to be left empty"),
+             Property.Select("Type", options=["Temperature", "Gravity/Angle", "Battery", "RSSI"], description="Select which type of data to register for this sensor. For Angle, Polynomial has to be left empty"),
              Property.Text(label="Polynomial", configurable=True, description="Enter your iSpindel polynomial. Use the variable tilt for the angle reading from iSpindel. Does not support ^ character."),
-             Property.Select("Units", options=["SG", "Brix", "°P"], description="Displays gravity reading with this unit if the Data Type is set to Gravity. Does not convert between units, to do that modify your polynomial.")])
+             Property.Select("Units", options=["SG", "Brix", "°P"], description="Displays gravity reading with this unit if the Data Type is set to Gravity. Does not convert between units, to do that modify your polynomial."),
+             Property.Sensor("FermenterTemp",description="Select Fermenter Temp Sensor that you want to provide to TCP Server")])
 
 class iSpindle(CBPiSensor):
     
     def __init__(self, cbpi, id, props):
         super(iSpindle, self).__init__(cbpi, id, props)
         self.value = 0
-        self.key = self.props.iSpindle
-        self.Polynomial = 'tilt' if self.props.Polynomial == '' else self.props.Polynomial
+        self.key = self.props.get("iSpindle", None)
+        self.Polynomial = self.props.get("Polynomial", "tilt")
+        self.temp_sensor_id = self.props.get("FermenterTemp", None)
         self.time_old = 0
 
     def get_unit(self):
-        if self.props.Type == "Temperature":
+        if self.props.get("Type") == "Temperature":
             return "°C" if self.get_config_value("TEMP_UNIT", "C") == "C" else "°F"
-        elif self.props.Type == "Gravity/Angle":
+        elif self.props.get("Type") == "Gravity/Angle":
             return self.props.Units
-        elif self.props.Type == "Battery":
+        elif self.props.get("Type") == "Battery":
             return "V"
+        elif self.props.get("Type") == "RSSI":
+            return "dB"
         else:
             return " "
 
     async def run(self):
         global cache
+        global fermenter_temp
+        Spindle_name = self.props.get("iSpindle") 
         while self.running == True:
             try:
                 if (float(cache[self.key]['Time']) > float(self.time_old)):
                     self.time_old = float(cache[self.key]['Time'])
-                    if self.props.Type == "Gravity/Angle":
-                        self.value = await calcGravity(self.Polynomial, cache[self.key]['Angle'], self.props.Units)
+                    if self.props.get("Type") == "Gravity/Angle":
+                        self.value = await calcGravity(self.Polynomial, cache[self.key]['Angle'], self.props.get("Units"))
                     else:
                         self.value = float(cache[self.key][self.props.Type])
                     self.log_data(self.value)
                     self.push_update(self.value)
+                self.push_update(self.value,False)
+                #self.cbpi.ws.send(dict(topic="sensorstate", id=self.id, value=self.value))
+                
             except Exception as e:
                 pass
-            await asyncio.sleep(1)
+            await asyncio.sleep(2)
 
     def get_state(self):
         return dict(value=self.value)
 
 class iSpindleEndpoint(CBPiExtension):
     
     def __init__(self, cbpi):
         '''
         Initializer
         :param cbpi:
         '''
         self.pattern_check = re.compile("^[a-zA-Z0-9,.]{0,10}$")
         self.cbpi = cbpi
+        self.sensor_controller : SensorController = cbpi.sensor
         # register component for http, events
         # In addtion the sub folder static is exposed to access static content via http
         self.cbpi.register(self, "/api/hydrometer/v1/data")
 
+    async def run(self):
+        await self.get_spindle_sensor()
+
     @request_mapping(path='', method="POST", auth_required=False)
     async def http_new_value3(self, request):
         import time
         """
         ---
         description: Get iSpindle Value
         tags:
-        - iSpindle Sensor
-        consumes:
-        - application/json
+        - iSpindle 
         parameters:
         - name: "data"
           in: "body"
           description: "Data"
           required: "name"
           type: "object"
-          properties: 
-          name: 
           type: string
         responses:
             "204":
                 description: successful operation
         """
 
         global cache
         try:
             data = await request.json()
         except Exception as e:
             print(e)
+        logging.info(data)
         time = time.time()
         key = data['name']
         temp = round(float(data['temperature']), 2)
         angle = data['angle']
         battery = data['battery']
-        cache[key] = {'Time': time,'Temperature': temp, 'Angle': angle, 'Battery': battery}
-
-        return web.Response(status=204)
+        try:
+            rssi = data['RSSI']
+        except:
+            rssi = 0
+        cache[key] = {'Time': time,'Temperature': temp, 'Angle': angle, 'Battery': battery, 'RSSI': rssi}
+
+
+    @request_mapping(path='/gettemp/{SpindleID}', method="POST", auth_required=False)
+    async def get_fermenter_temp(self, request):
+        SpindleID = request.match_info['SpindleID']
+        sensor_value = await self.get_spindle_sensor(SpindleID)
+        data = {'Temp': sensor_value}
+        return  web.json_response(data=data)
+
+    async def get_spindle_sensor(self, iSpindleID = None):
+        self.sensor = self.sensor_controller.get_state()
+        for id in self.sensor['data']:
+            if id['type'] == 'iSpindle':
+                name= id['props']['iSpindle']
+                if name == iSpindleID:
+                    try:
+                        sensor= id['props']['FermenterTemp']
+                    except:
+                        sensor = None
+                    if sensor is not None:
+                        sensor_value = self.cbpi.sensor.get_sensor_value(sensor).get('value')
+                    else:
+                        sensor_value = None
+                    return sensor_value
 
 def setup(cbpi):
     cbpi.plugin.register("iSpindle", iSpindle)
     cbpi.plugin.register("iSpindleEndpoint", iSpindleEndpoint)
     pass
```

### Comparing `cbpi4-iSpindle-0.0.3/cbpi4_iSpindle.egg-info/PKG-INFO` & `cbpi4-iSpindle-0.0.9/cbpi4_iSpindle.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,53 @@
-Metadata-Version: 2.1
-Name: cbpi4-iSpindle
-Version: 0.0.3
-Summary: CraftBeerPi4 iSpindle Sensor Plugin
-Home-page: https://github.com/avollkopf/cbpi4-iSpindle
-Author: Alexander Vollkopf
-Author-email: avollkopf@web.de
-License: GPLv 3.0
-Description: # CraftBeerPi4 iSpindle Sensor Plugin
-        
-        - Initial Version which has to be considered as beta
-            - Data Transfer is working from the SPindle itself and from the TCP server via forward-
-            - TCP Server does not require any changes. Only the port needs to be changed from 5000 to 8000
-            - The Spindel Connection needs to be changed from CraftbeerPi to HTTP as shown in the image below
-            - For Server, please enter the IP address of your CBPi4 Server.
-            - Enter 8000 for Port and '/api/hydrometer/v1/data' for path.
-        
-        ![iSpindle Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Spindle_Connection_Settings.png?raw=true)
-        
-        - Installation: 
-            - pip install cbpi4-iSpindle (or from the GIT repo)
-            - cbpi add cbpi4-iSpindle
-        - Usage:
-            - Add Hardware under Sensor and choose iSpindle as Type
-        
-        - Units are currently not displayed in CBPi4 for Sensors. You need to add that on you own in the Dashboard
-        - If you want to retrieve multiple parameters from one Spindle, you need to add the Spindle several times as sensor and choose different Types
-            - The Sensor name should be different for each of your sensors
-        - The settings are shown below.
-            - Name: This is the name of your sensor shown in CBPi4. e.g. iSpindleXXX - Angle
-            - iSpindle: Name of your Spindle that you entered in the Spindle setup page. This name must match to the Spindle. Otherwise no data will be collected.
-            - Type: Temperature, Gravity/Angle, Battery (Choose one type)
-                - If Gravity/Angle is choosen and the Polynomial field is left empty, the angle data is stored
-            - Polynomial: The polynomial to calculate gravity. '^' is not working. You need to uses tilt*tilt*tilt for '^3' and tilt*tilt for '^2'
-            - Units: Choose SG, Brix or °P. This has impact on the calculated digits
-        
-        ![CBPi4 Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Settings.png?raw=true)
-        
-        Changelog:
-        
-        15.03.21: Changes to suppoer cbpi >= 4.0.0.31
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: cbpi4-iSpindle
+Version: 0.0.9
+Summary: CraftBeerPi4 iSpindle Sensor Plugin
+Home-page: https://github.com/avollkopf/cbpi4-iSpindle
+Author: Alexander Vollkopf
+Author-email: avollkopf@web.de
+License: GPLv 3.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CraftBeerPi4 iSpindle Sensor Plugin
+
+- Initial Version which has to be considered as beta
+    - Data Transfer is working from the SPindle itself and from the TCP server via forward-
+    - TCP Server does not require any changes. Only the port needs to be changed from 5000 to 8000
+    - The Spindel Connection needs to be changed from CraftbeerPi to HTTP as shown in the image below
+    - For Server, please enter the IP address of your CBPi4 Server.
+    - Enter 8000 for Port and '/api/hydrometer/v1/data' for path.
+
+![iSpindle Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Spindle_Connection_Settings.png?raw=true)
+
+- Installation: 
+    - pip install cbpi4-iSpindle (or from the GIT repo)
+    - cbpi add cbpi4-iSpindle
+- Usage:
+    - Add Hardware under Sensor and choose iSpindle as Type
+
+- Units are currently not displayed in CBPi4 for Sensors. You need to add that on you own in the Dashboard
+- If you want to retrieve multiple parameters from one Spindle, you need to add the Spindle several times as sensor and choose different Types
+    - The Sensor name should be different for each of your sensors
+- The settings are shown below.
+    - Name: This is the name of your sensor shown in CBPi4. e.g. iSpindleXXX - Angle
+    - iSpindle: Name of your Spindle that you entered in the Spindle setup page. This name must match to the Spindle. Otherwise no data will be collected.
+    - Type: Temperature, Gravity/Angle, Battery (Choose one type)
+        - If Gravity/Angle is choosen and the Polynomial field is left empty, the angle data is stored
+    - Polynomial: The polynomial to calculate gravity. '^' is not working. You need to uses tilt*tilt*tilt for '^3' and tilt*tilt for '^2'
+    - Units: Choose SG, Brix or °P. This has impact on the calculated digits
+
+![CBPi4 Settings](https://github.com/avollkopf/cbpi4-iSpindle/blob/main/Settings.png?raw=true)
+
+### Changelog:
+
+- 10.05.22: (0.0.9) Removed cbpi dependency
+- 16.01.22: (0.0.8) Adaption for cbpi 4.0.1.2
+- 13.01.22: (0.0.7) Reduced mqtt traffic -> update only for new value
+- 23.11.21: (0.0.6) Added RSSI to available parmeters
+- 10.06.21: (0.0.5) Fix to improve UI behavior with respect to frequency of value update
+- 17.04.21: Some small fixes
+- 15.03.21: Changes to suppoer cbpi >= 4.0.0.31
+
+
```

### Comparing `cbpi4-iSpindle-0.0.3/setup.py` & `cbpi4-iSpindle-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-iSpindle',
-      version='0.0.3',
+      version='0.0.9',
       description='CraftBeerPi4 iSpindle Sensor Plugin',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/avollkopf/cbpi4-iSpindle',
       license='GPLv 3.0',
       include_package_data=True,
       package_data={
         # If any package contains *.txt or *.rst files, include them:
       '': ['*.txt', '*.rst', '*.yaml'],
       'cbpi4-iSpindle': ['*','*.txt', '*.rst', '*.yaml']},
       packages=['cbpi4-iSpindle'],
-      install_requires=[
-            'cbpi>=4.0.0.31',
-      ],
       long_description=long_description,
       long_description_content_type='text/markdown'
       )
```


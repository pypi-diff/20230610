# Comparing `tmp/py-miraie-ac-0.0.8.tar.gz` & `tmp/py-miraie-ac-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.0.8.tar", last modified: Fri Jun  9 16:12:51 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.0.9.tar", last modified: Sat Jun 10 06:47:45 2023, max compression
```

## Comparing `py-miraie-ac-0.0.8.tar` & `py-miraie-ac-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.501058 py-miraie-ac-0.0.8/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1232 2023-06-09 16:12:51.512073 py-miraie-ac-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.8/README.md
--rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-09 16:12:51.512073 py-miraie-ac-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.394343 py-miraie-ac-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.411850 py-miraie-ac-0.0.8/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6172 2023-06-09 13:28:16.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0     6221 2023-06-09 13:28:36.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/broker.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4542 2023-06-09 13:28:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      857 2023-06-09 13:29:04.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.0.8/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:12:51.501058 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1232 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-09 16:12:51.000000 py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.873209 py-miraie-ac-0.0.9/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1232 2023-06-10 06:47:45.874328 py-miraie-ac-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.9/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-10 06:47:45.875331 py-miraie-ac-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.798210 py-miraie-ac-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.866206 py-miraie-ac-0.0.9/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6359 2023-06-10 06:47:06.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6252 2023-06-09 17:07:32.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4604 2023-06-10 06:43:16.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      857 2023-06-09 13:29:04.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.872205 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1232 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.0.8/LICENSE` & `py-miraie-ac-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.8/PKG-INFO` & `py-miraie-ac-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.0.8/README.md` & `py-miraie-ac-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.8/setup.cfg` & `py-miraie-ac-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e38  .version = 0.0.8
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e39  .version = 0.0.9
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.0.8/src/py_miraie_ac/api.py` & `py-miraie-ac-0.0.9/src/py_miraie_ac/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,19 @@
     __password: str
     __http_session: aiohttp.ClientSession
     __user: User
     __home: Home
     __topics: list[str] = []
     __broker: MirAIeBroker
 
+    @property
+    def devices(self) -> list[Device]:
+        """Returns a list of available devices."""
+        return list(self.__home.devices.values())
+    
     def __init__(self, auth_type: AuthType, login_id: str, password: str):
         self.__auth_type = str(auth_type.value)
         self.__login_id = login_id
         self.__password = password
         self.__http_session = aiohttp.ClientSession()
 
     async def __aenter__(self):
@@ -52,16 +57,14 @@
         self.__broker = MirAIeBroker()
 
         self.__home = await self.__get_home_details()
         self.__broker.set_topics(self.__topics)
         self.__broker.init_broker(self.__home.home_id, self.__user.access_token)
         self.__broker.connect()
 
-        return self.__home
-
     async def reconnect_broker(self):
         """Authenticates with MirAIe and reconnects to MQTT server with the new credentials"""
         self.__user = await self.__login()
         self.__broker.reconnect(self.__user.access_token)
 
     async def __login(self):
         data = {
@@ -112,17 +115,19 @@
                     mac_address=device_details["macAddress"],
                     category=device_details["category"],
                     brand=device_details["brand"],
                     firmware_version=device_details["firmwareVersion"],
                     serial_number=device_details["serialNumber"],
                     model_number=device_details["modelNumber"],
                     product_serial_number=device_details["productSerialNumber"],
+                    area_name=space["spaceName"],
                     status=device_status,
                     broker=self.__broker,
                 )
+
                 self.__topics.append(device.status_topic)
                 self.__topics.append(device.connection_status_topic)
                 devices.append(device)
 
         return Home(home_id=json_response["homeId"], devices=devices)
 
     async def __get_device_details(self, device_id: str):
```

### Comparing `py-miraie-ac-0.0.8/src/py_miraie_ac/broker.py` & `py-miraie-ac-0.0.9/src/py_miraie_ac/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
     __host: str = "mqtt.miraie.in"
     __port: int = 8883
     __username: str
     __password: str
     __topics: list[str] = []
     __callbacks: dict[str, list[callable]] = {}
-
+    __client: paho.Client
+    
     def init_broker(self, username: str, password: str):
         """Initializes the MQTT client"""
         self.__username = username
         self.__password = password
         self.__init_mqtt_client()
 
     def set_topics(self, topics: list[str]):
```

### Comparing `py-miraie-ac-0.0.8/src/py_miraie_ac/device.py` & `py-miraie-ac-0.0.9/src/py_miraie_ac/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         mac_address: str,
         category: str,
         brand: str,
         firmware_version: str,
         serial_number: str,
         model_number: str,
         product_serial_number: str,
+        area_name: str,
         status: DeviceStatus,
         broker: MirAIeBroker,
     ):
         self.device_id = device_id
         self.name = name
         self.friendly_name = friendly_name
         self.control_topic = control_topic
@@ -39,14 +40,15 @@
         self.mac_address = mac_address
         self.category = category
         self.brand = brand
         self.firmware_version = firmware_version
         self.serial_number = serial_number
         self.model_number = model_number
         self.product_serial_number = product_serial_number
+        self.area_name = area_name,
         self.status = status
 
         self.__broker = broker
         self.__callbacks = set()
         self.__broker.register_callback(self.status_topic, self.status_callback_handler)
         self.__broker.register_callback(
             self.connection_status_topic, self.connection_callback_handler
```

### Comparing `py-miraie-ac-0.0.8/src/py_miraie_ac/deviceStatus.py` & `py-miraie-ac-0.0.9/src/py_miraie_ac/deviceStatus.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.8/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.0.9/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.0.8/src/py_miraie_ac.egg-info/SOURCES.txt` & `py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/SOURCES.txt`

 * *Files identical despite different names*


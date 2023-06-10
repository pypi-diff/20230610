# Comparing `tmp/pyeasee-0.7.52.tar.gz` & `tmp/pyeasee-0.7.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasee-0.7.52.tar", last modified: Sat Apr 22 20:13:58 2023, max compression
+gzip compressed data, was "pyeasee-0.7.53.tar", last modified: Sat Jun 10 20:36:31 2023, max compression
```

## Comparing `pyeasee-0.7.52.tar` & `pyeasee-0.7.53.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-22 20:13:58.413156 pyeasee-0.7.52/
--rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-04-22 20:13:58.413156 pyeasee-0.7.52/PKG-INFO
--rw-rw-r--   0 olal      (1000) olal      (1000)     2299 2022-10-12 21:10:32.000000 pyeasee-0.7.52/README.md
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-22 20:13:58.409156 pyeasee-0.7.52/pyeasee/
--rw-rw-r--   0 olal      (1000) olal      (1000)      185 2022-12-18 22:29:13.000000 pyeasee-0.7.52/pyeasee/__init__.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    13505 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/__main__.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    19443 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/charger.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    29599 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/const.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    16785 2023-04-22 20:11:43.000000 pyeasee-0.7.52/pyeasee/easee.py
--rw-rw-r--   0 olal      (1000) olal      (1000)      776 2022-12-17 23:49:14.000000 pyeasee-0.7.52/pyeasee/exceptions.py
--rw-rw-r--   0 olal      (1000) olal      (1000)     8707 2023-04-06 21:27:23.000000 pyeasee-0.7.52/pyeasee/site.py
--rw-rw-r--   0 olal      (1000) olal      (1000)     2130 2022-12-18 22:29:13.000000 pyeasee-0.7.52/pyeasee/utils.py
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-04-22 20:13:58.413156 pyeasee-0.7.52/pyeasee.egg-info/
--rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/PKG-INFO
--rw-rw-r--   0 olal      (1000) olal      (1000)      364 2023-04-22 20:13:53.000000 pyeasee-0.7.52/pyeasee.egg-info/SOURCES.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)        1 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/dependency_links.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)       51 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/entry_points.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)       27 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/requires.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)        8 2023-04-22 20:13:52.000000 pyeasee-0.7.52/pyeasee.egg-info/top_level.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)      169 2023-04-22 20:13:58.413156 pyeasee-0.7.52/setup.cfg
--rw-rw-r--   0 olal      (1000) olal      (1000)      805 2023-04-22 20:11:43.000000 pyeasee-0.7.52/setup.py
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-06-10 20:36:31.710323 pyeasee-0.7.53/
+-rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-06-10 20:36:31.710323 pyeasee-0.7.53/PKG-INFO
+-rw-rw-r--   0 olal      (1000) olal      (1000)     2299 2023-06-05 09:52:50.000000 pyeasee-0.7.53/README.md
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-06-10 20:36:31.706323 pyeasee-0.7.53/pyeasee/
+-rw-rw-r--   0 olal      (1000) olal      (1000)      185 2022-12-18 22:29:13.000000 pyeasee-0.7.53/pyeasee/__init__.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    13505 2023-04-06 21:27:23.000000 pyeasee-0.7.53/pyeasee/__main__.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    20721 2023-06-10 20:31:11.000000 pyeasee-0.7.53/pyeasee/charger.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    29599 2023-04-06 21:27:23.000000 pyeasee-0.7.53/pyeasee/const.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    16669 2023-06-10 20:33:17.000000 pyeasee-0.7.53/pyeasee/easee.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)      776 2022-12-17 23:49:14.000000 pyeasee-0.7.53/pyeasee/exceptions.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)     8691 2023-06-10 20:31:11.000000 pyeasee-0.7.53/pyeasee/site.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)     2130 2022-12-18 22:29:13.000000 pyeasee-0.7.53/pyeasee/utils.py
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2023-06-10 20:36:31.710323 pyeasee-0.7.53/pyeasee.egg-info/
+-rw-rw-r--   0 olal      (1000) olal      (1000)     3319 2023-06-10 20:36:30.000000 pyeasee-0.7.53/pyeasee.egg-info/PKG-INFO
+-rw-rw-r--   0 olal      (1000) olal      (1000)      364 2023-06-10 20:36:30.000000 pyeasee-0.7.53/pyeasee.egg-info/SOURCES.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)        1 2023-06-10 20:36:30.000000 pyeasee-0.7.53/pyeasee.egg-info/dependency_links.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)       51 2023-06-10 20:36:30.000000 pyeasee-0.7.53/pyeasee.egg-info/entry_points.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)       27 2023-06-10 20:36:30.000000 pyeasee-0.7.53/pyeasee.egg-info/requires.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)        8 2023-06-10 20:36:30.000000 pyeasee-0.7.53/pyeasee.egg-info/top_level.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)      169 2023-06-10 20:36:31.710323 pyeasee-0.7.53/setup.cfg
+-rw-rw-r--   0 olal      (1000) olal      (1000)      805 2023-06-10 20:33:17.000000 pyeasee-0.7.53/setup.py
```

### Comparing `pyeasee-0.7.52/PKG-INFO` & `pyeasee-0.7.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyeasee
-Version: 0.7.52
+Version: 0.7.53
 Summary: Easee EV charger API library
 Home-page: https://github.com/fondberg/pyeasee
 Author: Niklas Fondberg
 Author-email: niklas.fondberg@gmail.com
 License: MIT
-Description: ![Maintenance](https://img.shields.io/maintenance/yes/2022.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
+Description: ![Maintenance](https://img.shields.io/maintenance/yes/2023.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
         
         [![Buy me a coffee](https://img.shields.io/static/v1.svg?label=Buy%20me%20a%20coffee&message=🥨&color=black&logo=buy%20me%20a%20coffee&logoColor=white&labelColor=6f4e37)](https://www.buymeacoffee.com/fondberg)
         
         # Easee EV Charger library
         
         This library is an async thin wrapper around [Easee's Rest API](https://api.easee.cloud/index.html)
```

### Comparing `pyeasee-0.7.52/README.md` & `pyeasee-0.7.53/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Maintenance](https://img.shields.io/maintenance/yes/2022.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
+![Maintenance](https://img.shields.io/maintenance/yes/2023.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
 
 [![Buy me a coffee](https://img.shields.io/static/v1.svg?label=Buy%20me%20a%20coffee&message=🥨&color=black&logo=buy%20me%20a%20coffee&logoColor=white&labelColor=6f4e37)](https://www.buymeacoffee.com/fondberg)
 
 # Easee EV Charger library
 
 This library is an async thin wrapper around [Easee's Rest API](https://api.easee.cloud/index.html)
```

### Comparing `pyeasee-0.7.52/pyeasee/__main__.py` & `pyeasee-0.7.53/pyeasee/__main__.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.52/pyeasee/charger.py` & `pyeasee-0.7.53/pyeasee/charger.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,37 +12,74 @@
     0: "OFFLINE",
     1: "DISCONNECTED",
     2: "AWAITING_START",
     3: "CHARGING",
     4: "COMPLETED",
     5: "ERROR",
     6: "READY_TO_CHARGE",
+    7: "AWAITING_AUTHORIZATION",
+    8: "DE_AUTHORIZING",
+    100: "START_CHARGING",
+    101: "STOP_CHARGING",
+    102: "OFFLINE",
+    103: "AWAITING_LOAD_BALANCING",
+    104: "AWAITING_AUTHORIZATION",
+    105: "AWAITING_SMART_START",
+    106: "AWAITING_SCHEDULED_START",
+    107: "AUTHENTICATING",
+    108: "PAUSED_DUE_TO_EQUALIZER",
+    109: "SEARCHING_FOR_MASTER",
+    157: "ERRATIC_EV",
+    158: "ERROR_TEMPERATURE_TOO_HIGH",
+    159: "ERROR_DEAD_POWERBOARD",
+    160: "ERROR_OVERCURRENT",
+    161: "ERROR_PEN_FAULT",
 }
 
 NODE_TYPE = {1: "Master", 2: "Extender"}
 
 PHASE_MODE = {1: "Locked to single phase", 2: "Auto", 3: "Locked to three phase"}
 
 REASON_FOR_NO_CURRENT = {
     # Work-in-progress, must be taken with a pinch of salt, as per now just reverse engineering of observations until API properly documented
     None: "No reason",
     0: "No reason, charging or ready to charge",
-    1: "Charger paused",
-    2: "Charger paused",
-    3: "Charger paused",
-    4: "Charger paused",
-    5: "Charger paused",
-    6: "Charger paused",
-    9: "Error no current",
+    1: "Max circuit limit too low",
+    2: "Max dynamic circuit limit too low",
+    3: "Max dynamic offline limit too low",
+    4: "Circuit fuse too low",
+    5: "Waiting in queue",
+    6: "Waiting in fully",
+    7: "Illegal grid type",
+    8: "No current request recieved",
+    9: "Not connected to master",
+    10: "EQ current too low",
+    11: "Phase not connected",
+    25: "Limited by circuit fuse",
+    26: "Limited by circuit max limit",
+    27: "Limited by circuit dynamic limit",
+    28: "Limited by equalizer",
+    29: "Limited by load balancing",
+    30: "Limited by offline settings",
     50: "Secondary unit not requesting current or no car connected",
-    51: "Charger paused",
-    52: "Charger paused",
+    51: "Max charger limit too low",
+    52: "Max dynamic charger limit too low",
     53: "Charger disabled",
     54: "Waiting for schedule/auth",
     55: "Pending auth",
+    56: "Charger in error state",
+    57: "EV erratic",
+    75: "Limited by cable rating",
+    76: "Limited by schedule",
+    77: "Limited by charger max limit",
+    78: "Limited by charger dynamic limit",
+    79: "EV is not charging",
+    80: "Limited by local adjustment",
+    81: "Limited by EV",
+    100: "Undefined",
 }
 
 
 class ChargerState(BaseDict):
     """Charger state with integer enum values converted to human readable string values"""
 
     def __init__(self, state: Dict[str, Any], raw=False):
@@ -190,15 +227,15 @@
         self.circuit = circuit
         self.easee = easee
 
     async def get_observations(self, *args):
         """Gets observation IDs"""
         observation_ids = ",".join(str(s) for s in args)
         try:
-            return await (await self.easee.get(f"/state/{self.id}/observations?ids={observation_ids}", base=1)).json()
+            return await (await self.easee.get(f"/state/{self.id}/observations?ids={observation_ids}")).json()
         except (ServerFailureException):
             return None
 
     async def get_consumption_between_dates(self, from_date: datetime, to_date):
         """Gets consumption between two dates"""
         try:
             value = await (
@@ -435,15 +472,15 @@
             return await self.easee.post(f"/api/chargers/{self.id}/commands/update_firmware")
         except (ServerFailureException):
             return None
 
     async def get_latest_firmware(self):
         """Get the latest released firmeware version"""
         try:
-            return await (await self.easee.get(f"/firmware/{self.id}/latest", base=1)).json()
+            return await (await self.easee.get(f"/firmware/{self.id}/latest")).json()
         except (ServerFailureException):
             return None
 
     async def set_dynamic_charger_circuit_current(
         self, currentP1: int, currentP2: int = None, currentP3: int = None, timeToLive: int = 0
     ):
         """Set dynamic current on circuit level. timeToLive specifies, in minutes, for how long the new dynamic current is valid. timeToLive = 0 means that the new dynamic current is valid until changed the next time. The dynamic current is always reset to default when the charger is restarted."""
```

### Comparing `pyeasee-0.7.52/pyeasee/const.py` & `pyeasee-0.7.53/pyeasee/const.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.52/pyeasee/easee.py` & `pyeasee-0.7.53/pyeasee/easee.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     NotFoundException,
     ServerFailureException,
     TooManyRequestsException,
 )
 from .site import Site, SiteState
 from .utils import convert_stream_data
 
-__VERSION__ = "0.7.52"
+__VERSION__ = "0.7.53"
 
 _LOGGER = logging.getLogger(__name__)
 
 SR_MIN_BACKOFF = 0
 SR_MAX_BACKOFF = 300
 SR_INC_BACKOFF = 30
 
@@ -77,15 +77,15 @@
     def __init__(self, username, password, session: aiohttp.ClientSession = None):
         self.username = username
         self.password = password
         self.external_session = True if session else False
 
         _LOGGER.info("Easee python library version: %s", __VERSION__)
 
-        self.base = ["https://api.easee.cloud", "https://api.easee.com"]
+        self.base = "https://api.easee.com"
         self.sr_base = "https://streams.easee.com/hubs/chargers"
         self.token = {}
         self.headers = {
             "User-Agent": f"pyeasee/{__VERSION__} REST client",
             "Accept": "application/json",
             "Content-Type": "application/json;charset=UTF-8",
         }
@@ -105,41 +105,41 @@
         self.sr_connected = False
         self.sr_connect_in_progress = False
         self.running_loop = None
         self.event_loop = None
         self._sr_backoff = SR_MIN_BACKOFF
 
     def base_uri(self):
-        return self.base[0]
+        return self.base
 
-    async def post(self, url, base=0, **kwargs):
+    async def post(self, url, **kwargs):
         _LOGGER.debug("POST: %s (%s)", url, kwargs)
         await self._verify_updated_token()
-        response = await self.session.post(f"{self.base[base]}{url}", headers=self.headers, **kwargs)
+        response = await self.session.post(f"{self.base}{url}", headers=self.headers, **kwargs)
         await self.check_status(response)
         return response
 
-    async def put(self, url, base=0, **kwargs):
+    async def put(self, url, **kwargs):
         _LOGGER.debug("PUT: %s (%s)", url, kwargs)
         await self._verify_updated_token()
-        response = await self.session.put(f"{self.base[base]}{url}", headers=self.headers, **kwargs)
+        response = await self.session.put(f"{self.base}{url}", headers=self.headers, **kwargs)
         await self.check_status(response)
         return response
 
-    async def get(self, url, base=0, **kwargs):
+    async def get(self, url, **kwargs):
         _LOGGER.debug("GET: %s (%s)", url, kwargs)
         await self._verify_updated_token()
-        response = await self.session.get(f"{self.base[base]}{url}", headers=self.headers, **kwargs)
+        response = await self.session.get(f"{self.base}{url}", headers=self.headers, **kwargs)
         await self.check_status(response)
         return response
 
-    async def delete(self, url, base=0, **kwargs):
+    async def delete(self, url, **kwargs):
         _LOGGER.debug("DELETE: %s (%s)", url, kwargs)
         await self._verify_updated_token()
-        response = await self.session.delete(f"{self.base[base]}{url}", headers=self.headers, **kwargs)
+        response = await self.session.delete(f"{self.base}{url}", headers=self.headers, **kwargs)
         await self.check_status(response)
         return response
 
     # TODO: Quick fix for the auth fail errors due to something wrong with refresh token logic
     async def check_status(self, response):
         try:
             await raise_for_status(response)
@@ -183,32 +183,30 @@
 
     async def connect(self):
         """
         Connect and gets initial token
         """
         data = {"userName": self.username, "password": self.password}
         _LOGGER.debug("getting token for user: %s", self.username)
-        response = await self.session.post(
-            f"{self.base[0]}/api/accounts/login", headers=self.minimal_headers, json=data
-        )
+        response = await self.session.post(f"{self.base}/api/accounts/login", headers=self.minimal_headers, json=data)
         await raise_for_status(response)
         await self._handle_token_response(response)
 
     async def _refresh_token(self):
         """
         Refresh token
         """
         data = {
             "accessToken": self.token["accessToken"],
             "refreshToken": self.token["refreshToken"],
         }
         _LOGGER.debug("Refreshing access token")
         try:
             res = await self.session.post(
-                f"{self.base[0]}/api/accounts/refresh_token", headers=self.minimal_headers, json=data
+                f"{self.base}/api/accounts/refresh_token", headers=self.minimal_headers, json=data
             )
             await self._handle_token_response(res)
         except (AuthorizationFailedException, BadRequestException):
             _LOGGER.debug("Could not get new access token from refresh token, getting new one")
             await self.connect()
 
     async def close(self):
```

### Comparing `pyeasee-0.7.52/pyeasee/exceptions.py` & `pyeasee-0.7.53/pyeasee/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.52/pyeasee/site.py` & `pyeasee-0.7.53/pyeasee/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.site = site
         self.easee = easee
 
     async def get_observations(self, *args):
         """Gets observation IDs"""
         observation_ids = ",".join(str(s) for s in args)
         try:
-            return await (await self.easee.get(f"/state/{self.id}/observations?ids={observation_ids}", base=1)).json()
+            return await (await self.easee.get(f"/state/{self.id}/observations?ids={observation_ids}")).json()
         except (ServerFailureException):
             return None
 
     async def get_state(self):
         """Get Equalizer state"""
         try:
             state = await (await self.easee.get(f"/api/equalizers/{self.id}/state")).json()
@@ -62,15 +62,15 @@
         """Crate an empty config data structure"""
         config = {}
         return EqualizerConfig(config)
 
     async def get_latest_firmware(self):
         """Get the latest released firmeware version"""
         try:
-            return await (await self.easee.get(f"/firmware/{self.id}/latest", base=1)).json()
+            return await (await self.easee.get(f"/firmware/{self.id}/latest")).json()
         except (ServerFailureException):
             return None
 
 
 class Circuit(BaseDict):
     """Represents a Circuit"""
```

### Comparing `pyeasee-0.7.52/pyeasee/utils.py` & `pyeasee-0.7.53/pyeasee/utils.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.7.52/pyeasee.egg-info/PKG-INFO` & `pyeasee-0.7.53/pyeasee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyeasee
-Version: 0.7.52
+Version: 0.7.53
 Summary: Easee EV charger API library
 Home-page: https://github.com/fondberg/pyeasee
 Author: Niklas Fondberg
 Author-email: niklas.fondberg@gmail.com
 License: MIT
-Description: ![Maintenance](https://img.shields.io/maintenance/yes/2022.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
+Description: ![Maintenance](https://img.shields.io/maintenance/yes/2023.svg) ![Easee library](https://github.com/fondberg/easee/workflows/Easee%20library/badge.svg)
         
         [![Buy me a coffee](https://img.shields.io/static/v1.svg?label=Buy%20me%20a%20coffee&message=🥨&color=black&logo=buy%20me%20a%20coffee&logoColor=white&labelColor=6f4e37)](https://www.buymeacoffee.com/fondberg)
         
         # Easee EV Charger library
         
         This library is an async thin wrapper around [Easee's Rest API](https://api.easee.cloud/index.html)
```

### Comparing `pyeasee-0.7.52/setup.py` & `pyeasee-0.7.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os.path
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="pyeasee",
-    version="0.7.52",
+    version="0.7.53",
     description="Easee EV charger API library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fondberg/pyeasee",
     author="Niklas Fondberg",
     author_email="niklas.fondberg@gmail.com",
     license="MIT",
```


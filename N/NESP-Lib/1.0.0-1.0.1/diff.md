# Comparing `tmp/NESP-Lib-1.0.0.tar.gz` & `tmp/NESP-Lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NESP-Lib-1.0.0.tar", last modified: Sun May 16 14:40:02 2021, max compression
+gzip compressed data, was "NESP-Lib-1.0.1.tar", last modified: Fri Jun  9 21:53:07 2023, max compression
```

## Comparing `NESP-Lib-1.0.0.tar` & `NESP-Lib-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-05-16 14:40:02.241460 NESP-Lib-1.0.0/
--rw-rw-rw-   0        0        0     1088 2021-05-14 18:40:17.000000 NESP-Lib-1.0.0/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2021-05-16 14:40:02.229491 NESP-Lib-1.0.0/NESP_Lib.egg-info/
--rw-rw-rw-   0        0        0     3555 2021-05-16 14:40:02.000000 NESP-Lib-1.0.0/NESP_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2021-05-16 14:40:02.000000 NESP-Lib-1.0.0/NESP_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-16 14:40:02.000000 NESP-Lib-1.0.0/NESP_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-05-16 14:40:02.000000 NESP-Lib-1.0.0/NESP_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-05-16 14:40:02.000000 NESP-Lib-1.0.0/NESP_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3555 2021-05-16 14:40:02.241460 NESP-Lib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2021-05-16 14:24:31.000000 NESP-Lib-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2021-05-16 14:40:02.239465 NESP-Lib-1.0.0/nesp_lib/
--rw-rw-rw-   0        0        0      300 2021-05-16 14:36:07.000000 NESP-Lib-1.0.0/nesp_lib/__init__.py
--rw-rw-rw-   0        0        0      439 2021-04-13 23:02:59.000000 NESP-Lib-1.0.0/nesp_lib/alarm_status.py
--rw-rw-rw-   0        0        0     2244 2021-04-13 23:05:40.000000 NESP-Lib-1.0.0/nesp_lib/exceptions.py
--rw-rw-rw-   0        0        0     1781 2021-04-09 18:40:21.000000 NESP-Lib-1.0.0/nesp_lib/port.py
--rw-rw-rw-   0        0        0    25444 2021-05-10 22:38:10.000000 NESP-Lib-1.0.0/nesp_lib/pump.py
--rw-rw-rw-   0        0        0      186 2021-04-13 21:06:27.000000 NESP-Lib-1.0.0/nesp_lib/pumping_direction.py
--rw-rw-rw-   0        0        0      506 2021-04-13 21:07:24.000000 NESP-Lib-1.0.0/nesp_lib/status.py
--rw-rw-rw-   0        0        0      739 2021-05-16 14:40:02.256417 NESP-Lib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-05-16 14:28:59.000000 NESP-Lib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 21:53:07.015717 NESP-Lib-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2021-05-14 18:40:17.000000 NESP-Lib-1.0.1/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 21:53:06.996790 NESP-Lib-1.0.1/NESP_Lib.egg-info/
+-rw-rw-rw-   0        0        0     2864 2023-06-09 21:53:06.000000 NESP-Lib-1.0.1/NESP_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-06-09 21:53:06.000000 NESP-Lib-1.0.1/NESP_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 21:53:06.000000 NESP-Lib-1.0.1/NESP_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 21:53:06.000000 NESP-Lib-1.0.1/NESP_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 21:53:06.000000 NESP-Lib-1.0.1/NESP_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2864 2023-06-09 21:53:07.016705 NESP-Lib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2234 2021-05-16 14:24:31.000000 NESP-Lib-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 21:53:07.013715 NESP-Lib-1.0.1/nesp_lib/
+-rw-rw-rw-   0        0        0      300 2023-06-09 21:14:48.000000 NESP-Lib-1.0.1/nesp_lib/__init__.py
+-rw-rw-rw-   0        0        0      439 2021-04-13 23:02:59.000000 NESP-Lib-1.0.1/nesp_lib/alarm_status.py
+-rw-rw-rw-   0        0        0     2244 2021-04-13 23:05:40.000000 NESP-Lib-1.0.1/nesp_lib/exceptions.py
+-rw-rw-rw-   0        0        0     1781 2021-04-09 18:40:21.000000 NESP-Lib-1.0.1/nesp_lib/port.py
+-rw-rw-rw-   0        0        0    25955 2023-06-09 20:35:43.000000 NESP-Lib-1.0.1/nesp_lib/pump.py
+-rw-rw-rw-   0        0        0      186 2021-04-13 21:06:27.000000 NESP-Lib-1.0.1/nesp_lib/pumping_direction.py
+-rw-rw-rw-   0        0        0      506 2021-04-13 21:07:24.000000 NESP-Lib-1.0.1/nesp_lib/status.py
+-rw-rw-rw-   0        0        0      740 2023-06-09 21:53:07.019697 NESP-Lib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2021-05-16 14:28:59.000000 NESP-Lib-1.0.1/setup.py
```

### Comparing `NESP-Lib-1.0.0/LICENSE.txt` & `NESP-Lib-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NESP-Lib-1.0.0/NESP_Lib.egg-info/PKG-INFO` & `NESP-Lib-1.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,104 +1,87 @@
-Metadata-Version: 2.1
-Name: NESP-Lib
-Version: 1.0.0
-Summary: New Era Syringe Pump Library for Python
-Home-page: https://github.com/florian-lapp/nesp-lib-py
-Author: Florian Lapp
-Author-email: e5abed0c@gmail.com
-License: MIT
-Description: # NESP-Lib – New Era Syringe Pump Library for Python
-        
-        This project aims to offer a clean high-level interface to the New Era syringe pumps by New Era Pump
-        Systems.
-        
-        These pumps are also distributed under different names, like Aladdin by World Precision Instruments
-        (WPI) and LA by Landgraf Laborsysteme.
-        
-        ## Features
-        
-        - Object-oriented design
-        - Documented public elements via type hints and docstrings
-        - Signaling errors via exceptions
-        - Blocking and non-blocking running
-        - Sending heartbeat messages automatically
-        
-        ## Installing
-        
-        ```
-        pip install NESP-Lib
-        ```
-        
-        ## Importing
-        
-        ``` python
-        import nesp_lib
-        ```
-        
-        ## Examples
-        
-        ### Configuring
-        
-        ``` python
-        from nesp_lib import Port, Pump, PumpingDirection
-        
-        # Constructs the port to which the pump is connected.
-        port = Port('COM1')
-        # Constructs the pump connected to the port.
-        pump = Pump(port)
-        # Sets the syringe diameter of the pump in units of millimeters.
-        pump.syringe_diameter = 30.0
-        # Sets the pumping direction of the pump.
-        pump.pumping_direction = PumpingDirection.INFUSE
-        # Sets the pumping volume of the pump in units of milliliters.
-        pump.pumping_volume = 1.0
-        # Sets the pumping rate of the pump in units of milliliters per minute.
-        pump.pumping_rate = 20.0
-        ```
-        
-        ### Identifying
-        
-        ``` python
-        # Prints the model number of the pump (e.g. "1000" for NE-1000).
-        print(pump.model_number)
-        # Prints the firmware version of the pump (e.g. "(3, 928)" for 3.928).
-        print(pump.firmware_version)
-        ```
-        
-        ### Running (Blocking)
-        
-        Blocking running waits while the pump is running.
-        
-        ``` python
-        # Runs the pump considering the direction, volume, and rate set.
-        pump.run()
-        ```
-        
-        ### Running (Non-blocking)
-        
-        Non-blocking running returns immediately after starting the running.
-        
-        ``` python
-        # Starts running the pump considering the direction, volume, and rate set.
-        pump.run(False)
-        # Waits while the pump is running.
-        pump.wait_while_running()
-        # Starts running the pump considering the direction, volume, and rate set.
-        pump.run(False)
-        # Waits while the pump is running.
-        while pump.running :
-            ...
-        # Starts running the pump considering the direction, volume, and rate set.
-        pump.run(False)
-        ...
-        # Stops the pump.
-        pump.stop()
-        ```
-Keywords: New-Era-Pump-Systems,Syringe-Pump
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
+# NESP-Lib – New Era Syringe Pump Library for Python
+
+This project aims to offer a clean high-level interface to the New Era syringe pumps by New Era Pump
+Systems.
+
+These pumps are also distributed under different names, like Aladdin by World Precision Instruments
+(WPI) and LA by Landgraf Laborsysteme.
+
+## Features
+
+- Object-oriented design
+- Documented public elements via type hints and docstrings
+- Signaling errors via exceptions
+- Blocking and non-blocking running
+- Sending heartbeat messages automatically
+
+## Installing
+
+```
+pip install NESP-Lib
+```
+
+## Importing
+
+``` python
+import nesp_lib
+```
+
+## Examples
+
+### Configuring
+
+``` python
+from nesp_lib import Port, Pump, PumpingDirection
+
+# Constructs the port to which the pump is connected.
+port = Port('COM1')
+# Constructs the pump connected to the port.
+pump = Pump(port)
+# Sets the syringe diameter of the pump in units of millimeters.
+pump.syringe_diameter = 30.0
+# Sets the pumping direction of the pump.
+pump.pumping_direction = PumpingDirection.INFUSE
+# Sets the pumping volume of the pump in units of milliliters.
+pump.pumping_volume = 1.0
+# Sets the pumping rate of the pump in units of milliliters per minute.
+pump.pumping_rate = 20.0
+```
+
+### Identifying
+
+``` python
+# Prints the model number of the pump (e.g. "1000" for NE-1000).
+print(pump.model_number)
+# Prints the firmware version of the pump (e.g. "(3, 928)" for 3.928).
+print(pump.firmware_version)
+```
+
+### Running (Blocking)
+
+Blocking running waits while the pump is running.
+
+``` python
+# Runs the pump considering the direction, volume, and rate set.
+pump.run()
+```
+
+### Running (Non-blocking)
+
+Non-blocking running returns immediately after starting the running.
+
+``` python
+# Starts running the pump considering the direction, volume, and rate set.
+pump.run(False)
+# Waits while the pump is running.
+pump.wait_while_running()
+# Starts running the pump considering the direction, volume, and rate set.
+pump.run(False)
+# Waits while the pump is running.
+while pump.running :
+    ...
+# Starts running the pump considering the direction, volume, and rate set.
+pump.run(False)
+...
+# Stops the pump.
+pump.stop()
+```
```

### Comparing `NESP-Lib-1.0.0/README.md` & `NESP-Lib-1.0.1/NESP_Lib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: NESP-Lib
+Version: 1.0.1
+Summary: New Era Syringe Pump Library for Python
+Home-page: https://github.com/florian-lapp/nesp-lib-py
+Author: Florian Lapp
+Author-email: e5abed0c@gmail.com
+License: MIT
+Keywords: New-Era-Pump-Systems,Syringe-Pump
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Typing :: Typed
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # NESP-Lib – New Era Syringe Pump Library for Python
 
 This project aims to offer a clean high-level interface to the New Era syringe pumps by New Era Pump
 Systems.
 
 These pumps are also distributed under different names, like Aladdin by World Precision Instruments
 (WPI) and LA by Landgraf Laborsysteme.
@@ -80,8 +98,8 @@
 while pump.running :
     ...
 # Starts running the pump considering the direction, volume, and rate set.
 pump.run(False)
 ...
 # Stops the pump.
 pump.stop()
-```
+```
```

### Comparing `NESP-Lib-1.0.0/nesp_lib/exceptions.py` & `NESP-Lib-1.0.1/nesp_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `NESP-Lib-1.0.0/nesp_lib/port.py` & `NESP-Lib-1.0.1/nesp_lib/port.py`

 * *Files identical despite different names*

### Comparing `NESP-Lib-1.0.0/nesp_lib/pump.py` & `NESP-Lib-1.0.1/nesp_lib/pump.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,22 @@
         self.__port_lock = threading.Lock()
         self.__address = address
         self.__safe_mode = False
         self.__heartbeat_thread : typing.Optional[threading.Thread] = None
         self.__heartbeat_event : typing.Optional[threading.Event] = None
         self.__heartbeat_event_timeout = 0.0
         self.__safe_mode_timeout_set(safe_mode_timeout, True)
-        model_number_port, firmware_version_port = self.__firmware_version_get()
+        model_number_port, firmware_version_port, firmware_upgrade_port = (
+            self.__firmware_version_get()
+        )
         if model_number != Pump.MODEL_NUMBER_IGNORE and model_number_port != model_number :
             raise ModelException()
         self.__model_number = model_number_port
         self.__firmware_version = firmware_version_port
+        self.__firmware_upgrade = firmware_upgrade
 
     @property
     def address(self) -> int :
         """
         Gets the address of the pump.
 
         Values: [`0`, `ADDRESS_LIMIT`]
@@ -99,14 +102,23 @@
 
     @property
     def firmware_version(self) -> typing.Tuple[int, int] :
         """Gets the firmware version of the pump as major version and minor version."""
         return self.__firmware_version
 
     @property
+    def firmware_upgrade(self) -> int :
+        """
+        Gets the firmware upgrade of the pump.
+
+        Zero if the pump has no firmware upgrade.
+        """
+        return self.__firmware_upgrade
+
+    @property
     def safe_mode_timeout(self) -> int :
         """
         Gets the safe mode timeout of the pump in units of seconds.
 
         Values: [`0`, `SAFE_MODE_TIMEOUT_LIMIT`]
         """
         _, match = self.__command_transceive(
@@ -368,17 +380,20 @@
     }
 
     # Regular expressions.
     __RE_INTEGER = r'(\d+)'
     __RE_FLOAT   = r'(\d+\.\d*)'
     __RE_SYMBOL  = '([A-Z]+)'
 
-    # Format: "NE" <Model number> "V" <Firmware major version> "." <Firmware minor version>
+    # Format: "NE" <Model number> ("X" (<Firmware upgrade>)?)? "V"
+    # <Firmware major version> "." <Firmware minor version>
     __RE_PATTERN_FIRMWARE_VERSION = re.compile(
-        'NE' + __RE_INTEGER + 'V' + __RE_INTEGER + r'\.' + __RE_INTEGER, re.ASCII
+        'NE' + __RE_INTEGER + '(X' + __RE_INTEGER + '?)?' + 'V' +
+        __RE_INTEGER + r'\.' + __RE_INTEGER,
+        re.ASCII
     )
     __RE_PATTERN_SAFE_MODE_TIMEOUT = re.compile(__RE_INTEGER, re.ASCII)
     __RE_PATTERN_SYRINGE_DIAMETER = re.compile(__RE_FLOAT, re.ASCII)
     # Format: <Pumping volume> <Units>
     __RE_PATTERN_PUMPING_VOLUME = re.compile(__RE_FLOAT + __RE_SYMBOL, re.ASCII)
     # Format: <Pumping rate> <Units>
     __RE_PATTERN_PUMPING_RATE = re.compile(__RE_FLOAT + __RE_SYMBOL, re.ASCII)
@@ -676,22 +691,23 @@
     def __heartbeat(self) -> None :
         while self.__heartbeat_event_timeout != 0.0 :
             if self.__heartbeat_event.wait(self.__heartbeat_event_timeout) :
                 self.__heartbeat_event.clear()
             else :
                 self.__command_transceive(Pump.__CommandName.STATUS)
 
-    def __firmware_version_get(self) -> typing.Tuple[int, typing.Tuple[int, int]] :
+    def __firmware_version_get(self) -> typing.Tuple[int, typing.Tuple[int, int], int] :
         _, match = self.__command_transceive(
             Pump.__CommandName.FIRMWARE_VERSION, [], Pump.__RE_PATTERN_FIRMWARE_VERSION
         )
         model_number = int(match[1])
-        version_major = int(match[2])
-        version_minor = int(match[3])
-        return model_number, (version_major, version_minor)
+        upgrade = 0 if match[2] is None else 1 if match[3] is None else int(match[3])
+        version_major = int(match[4])
+        version_minor = int(match[5])
+        return model_number, (version_major, version_minor), upgrade
 
     def __dispensation_get(self, withdrawn : bool) -> float :
         _, match = self.__command_transceive(
             Pump.__CommandName.DISPENSATION, [], Pump.__RE_PATTERN_DISPENSATION
         )
         value = float(match[1 + withdrawn])
         units = match[3]
```

### Comparing `NESP-Lib-1.0.0/setup.cfg` & `NESP-Lib-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 00000030: 7261 2053 7972 696e 6765 2050 756d 7020  ra Syringe Pump 
 00000040: 4c69 6272 6172 7920 666f 7220 5079 7468  Library for Pyth
 00000050: 6f6e 0d0a 6175 7468 6f72 203d 2046 6c6f  on..author = Flo
 00000060: 7269 616e 204c 6170 700d 0a61 7574 686f  rian Lapp..autho
 00000070: 725f 656d 6169 6c20 3d20 6535 6162 6564  r_email = e5abed
 00000080: 3063 4067 6d61 696c 2e63 6f6d 0d0a 6c69  0c@gmail.com..li
 00000090: 6365 6e73 6520 3d20 4d49 540d 0a6c 6963  cense = MIT..lic
-000000a0: 656e 7365 5f66 696c 6520 3d20 4c49 4345  ense_file = LICE
-000000b0: 4e53 452e 7478 740d 0a6b 6579 776f 7264  NSE.txt..keyword
-000000c0: 7320 3d20 4e65 772d 4572 612d 5075 6d70  s = New-Era-Pump
-000000d0: 2d53 7973 7465 6d73 2c20 5379 7269 6e67  -Systems, Syring
-000000e0: 652d 5075 6d70 0d0a 7572 6c20 3d20 6874  e-Pump..url = ht
-000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000100: 2f66 6c6f 7269 616e 2d6c 6170 702f 6e65  /florian-lapp/ne
-00000110: 7370 2d6c 6962 2d70 790d 0a6c 6f6e 675f  sp-lib-py..long_
-00000120: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000130: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000140: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000150: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000160: 6578 742f 6d61 726b 646f 776e 0d0a 7665  ext/markdown..ve
-00000170: 7273 696f 6e20 3d20 6174 7472 3a20 6e65  rsion = attr: ne
-00000180: 7370 5f6c 6962 2e56 4552 5349 4f4e 0d0a  sp_lib.VERSION..
-00000190: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001a0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
-000001b0: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
-000001c0: 6374 696f 6e2f 5374 6162 6c65 0d0a 0949  ction/Stable...I
-000001d0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-000001e0: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
-000001f0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
-00000200: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
-00000210: 7365 6172 6368 0d0a 094c 6963 656e 7365  search...License
-00000220: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000230: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-00000240: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000250: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000260: 6465 6e74 0d0a 0954 7970 696e 6720 3a3a  dent...Typing ::
-00000270: 2054 7970 6564 0d0a 0d0a 5b6f 7074 696f   Typed....[optio
-00000280: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-00000290: 6e65 7370 5f6c 6962 0d0a 696e 7374 616c  nesp_lib..instal
-000002a0: 6c5f 7265 7175 6972 6573 203d 2070 7973  l_requires = pys
-000002b0: 6572 6961 6c0d 0a0d 0a5b 6567 675f 696e  erial....[egg_in
-000002c0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000002d0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002e0: 0a0d 0a                                  ...
+000000a0: 656e 7365 5f66 696c 6573 203d 204c 4943  ense_files = LIC
+000000b0: 454e 5345 2e74 7874 0d0a 6b65 7977 6f72  ENSE.txt..keywor
+000000c0: 6473 203d 204e 6577 2d45 7261 2d50 756d  ds = New-Era-Pum
+000000d0: 702d 5379 7374 656d 732c 2053 7972 696e  p-Systems, Syrin
+000000e0: 6765 2d50 756d 700d 0a75 726c 203d 2068  ge-Pump..url = h
+000000f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000100: 6d2f 666c 6f72 6961 6e2d 6c61 7070 2f6e  m/florian-lapp/n
+00000110: 6573 702d 6c69 622d 7079 0d0a 6c6f 6e67  esp-lib-py..long
+00000120: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000130: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+00000140: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000150: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+00000160: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a76  text/markdown..v
+00000170: 6572 7369 6f6e 203d 2061 7474 723a 206e  ersion = attr: n
+00000180: 6573 705f 6c69 622e 5645 5253 494f 4e0d  esp_lib.VERSION.
+00000190: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+000001a0: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+000001b0: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
+000001c0: 7563 7469 6f6e 2f53 7461 626c 650d 0a09  uction/Stable...
+000001d0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000001e0: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
+000001f0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+00000200: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
+00000210: 6573 6561 7263 680d 0a09 4c69 6365 6e73  esearch...Licens
+00000220: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000230: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000240: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000250: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000260: 6e64 656e 740d 0a09 5479 7069 6e67 203a  ndent...Typing :
+00000270: 3a20 5479 7065 640d 0a0d 0a5b 6f70 7469  : Typed....[opti
+00000280: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
+00000290: 206e 6573 705f 6c69 620d 0a69 6e73 7461   nesp_lib..insta
+000002a0: 6c6c 5f72 6571 7569 7265 7320 3d20 7079  ll_requires = py
+000002b0: 7365 7269 616c 0d0a 0d0a 5b65 6767 5f69  serial....[egg_i
+000002c0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000002d0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000002e0: 0d0a 0d0a                                ....
```


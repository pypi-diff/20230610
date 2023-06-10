# Comparing `tmp/sinricpro-2.6.4.tar.gz` & `tmp/sinricpro-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinricpro-2.6.4.tar", last modified: Wed Feb 22 10:24:32 2023, max compression
+gzip compressed data, was "sinricpro-2.7.1.tar", last modified: Sat Jun 10 16:09:20 2023, max compression
```

## Comparing `sinricpro-2.6.4.tar` & `sinricpro-2.7.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 10:24:32.315211 sinricpro-2.6.4/
--rw-rw-rw-   0        0        0      116 2021-11-21 15:17:10.000000 sinricpro-2.6.4/.dockerignore
-drwxrwxrwx   0        0        0        0 2023-02-22 10:24:31.990211 sinricpro-2.6.4/.github/
-drwxrwxrwx   0        0        0        0 2023-02-22 10:24:32.065246 sinricpro-2.6.4/.github/workflows/
--rw-rw-rw-   0        0        0     1096 2022-06-20 09:22:30.000000 sinricpro-2.6.4/.github/workflows/python-publish.yml
--rw-rw-rw-   0        0        0      171 2021-11-21 15:17:10.000000 sinricpro-2.6.4/.gitignore
--rw-rw-rw-   0        0        0      712 2023-02-22 10:24:32.314247 sinricpro-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      781 2022-06-20 09:22:30.000000 sinricpro-2.6.4/README.md
--rw-rw-rw-   0        0        0      320 2022-06-20 09:22:30.000000 sinricpro-2.6.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-22 10:24:32.131210 sinricpro-2.6.4/examples/
--rw-rw-rw-   0        0        0      595 2022-10-08 01:06:54.000000 sinricpro-2.6.4/examples/blinds.py
--rw-rw-rw-   0        0        0      828 2022-10-08 01:06:57.000000 sinricpro-2.6.4/examples/custom_device.py
--rw-rw-rw-   0        0        0      710 2022-10-08 01:06:59.000000 sinricpro-2.6.4/examples/dim_switch.py
--rw-rw-rw-   0        0        0      669 2022-10-08 01:12:05.000000 sinricpro-2.6.4/examples/doorbell.py
--rw-rw-rw-   0        0        0      571 2022-10-08 01:07:06.000000 sinricpro-2.6.4/examples/garagedoor.py
--rw-rw-rw-   0        0        0     1802 2022-10-08 01:07:11.000000 sinricpro-2.6.4/examples/light.py
--rw-rw-rw-   0        0        0      628 2022-10-08 01:11:22.000000 sinricpro-2.6.4/examples/push_notification.py
--rw-rw-rw-   0        0        0      681 2022-10-08 01:07:14.000000 sinricpro-2.6.4/examples/smart_lock.py
--rw-rw-rw-   0        0        0     1399 2022-10-08 01:07:18.000000 sinricpro-2.6.4/examples/speaker.py
--rw-rw-rw-   0        0        0      729 2023-02-22 10:18:37.000000 sinricpro-2.6.4/examples/switch.py
--rw-rw-rw-   0        0        0     1150 2023-02-22 10:02:05.000000 sinricpro-2.6.4/examples/temperature_sensor.py
--rw-rw-rw-   0        0        0     1861 2022-10-08 01:07:28.000000 sinricpro-2.6.4/examples/tv.py
--rw-rw-rw-   0        0        0       42 2023-02-22 10:24:32.315211 sinricpro-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1012 2023-02-22 10:21:11.000000 sinricpro-2.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-22 10:24:32.259212 sinricpro-2.6.4/sinric/
--rw-rw-rw-   0        0        0      331 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/__init__.py
--rw-rw-rw-   0        0        0     1079 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_brightnessController.py
--rw-rw-rw-   0        0        0    29612 2022-10-08 01:11:22.000000 sinricpro-2.6.4/sinric/_cbhandler.py
--rw-rw-rw-   0        0        0      731 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_colorController.py
--rw-rw-rw-   0        0        0      990 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_colorTemperature.py
--rw-rw-rw-   0        0        0     7546 2022-10-08 01:11:22.000000 sinricpro-2.6.4/sinric/_events.py
--rw-rw-rw-   0        0        0     1678 2022-02-14 09:21:25.000000 sinricpro-2.6.4/sinric/_jsoncommands.py
--rw-rw-rw-   0        0        0     1207 2022-02-14 09:21:25.000000 sinricpro-2.6.4/sinric/_leakyBucket.py
--rw-rw-rw-   0        0        0      475 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_lockController.py
--rw-rw-rw-   0        0        0      256 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_mainqueue.py
--rw-rw-rw-   0        0        0      621 2022-02-14 09:21:25.000000 sinricpro-2.6.4/sinric/_modeController.py
--rw-rw-rw-   0        0        0      507 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_powerController.py
--rw-rw-rw-   0        0        0     1040 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_powerLevelController.py
--rw-rw-rw-   0        0        0     1111 2022-02-14 09:21:25.000000 sinricpro-2.6.4/sinric/_rangeValueController.py
--rw-rw-rw-   0        0        0      863 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_signature.py
--rw-rw-rw-   0        0        0     2620 2023-02-22 10:15:35.000000 sinricpro-2.6.4/sinric/_sinricpro.py
--rw-rw-rw-   0        0        0     3311 2022-10-08 01:11:22.000000 sinricpro-2.6.4/sinric/_sinricprosocket.py
--rw-rw-rw-   0        0        0     2261 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_sinricproudp.py
--rw-rw-rw-   0        0        0     1372 2022-02-14 09:21:25.000000 sinricpro-2.6.4/sinric/_speakerController.py
--rw-rw-rw-   0        0        0      950 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_temperatureController.py
--rw-rw-rw-   0        0        0      494 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_thermostatController.py
--rw-rw-rw-   0        0        0     1905 2021-11-21 15:17:10.000000 sinricpro-2.6.4/sinric/_tvcontorller.py
-drwxrwxrwx   0        0        0        0 2023-02-22 10:24:32.312249 sinricpro-2.6.4/sinricpro.egg-info/
--rw-rw-rw-   0        0        0      712 2023-02-22 10:24:31.000000 sinricpro-2.6.4/sinricpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2023-02-22 10:24:31.000000 sinricpro-2.6.4/sinricpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 10:24:31.000000 sinricpro-2.6.4/sinricpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-02-22 10:24:31.000000 sinricpro-2.6.4/sinricpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-22 10:24:31.000000 sinricpro-2.6.4/sinricpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 16:09:20.465545 sinricpro-2.7.1/
+-rw-rw-rw-   0        0        0      116 2021-11-21 15:17:10.000000 sinricpro-2.7.1/.dockerignore
+drwxrwxrwx   0        0        0        0 2023-06-10 16:09:20.312556 sinricpro-2.7.1/.github/
+drwxrwxrwx   0        0        0        0 2023-06-10 16:09:20.380544 sinricpro-2.7.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1096 2022-06-20 09:22:30.000000 sinricpro-2.7.1/.github/workflows/python-publish.yml
+-rw-rw-rw-   0        0        0      171 2021-11-21 15:17:10.000000 sinricpro-2.7.1/.gitignore
+-rw-rw-rw-   0        0        0      708 2023-06-10 16:09:20.464543 sinricpro-2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-06-08 09:49:54.000000 sinricpro-2.7.1/README.md
+-rw-rw-rw-   0        0        0      320 2022-06-20 09:22:30.000000 sinricpro-2.7.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-10 16:09:20.421546 sinricpro-2.7.1/examples/
+-rw-rw-rw-   0        0        0     1239 2023-06-10 15:59:29.000000 sinricpro-2.7.1/examples/blinds.py
+-rw-rw-rw-   0        0        0      937 2023-06-10 16:00:04.000000 sinricpro-2.7.1/examples/custom_device.py
+-rw-rw-rw-   0        0        0     1252 2023-06-10 16:00:17.000000 sinricpro-2.7.1/examples/dim_switch.py
+-rw-rw-rw-   0        0        0      808 2023-06-10 16:00:23.000000 sinricpro-2.7.1/examples/doorbell.py
+-rw-rw-rw-   0        0        0     1071 2023-06-10 16:00:34.000000 sinricpro-2.7.1/examples/garagedoor.py
+-rw-rw-rw-   0        0        0     2542 2023-06-10 16:00:45.000000 sinricpro-2.7.1/examples/light.py
+-rw-rw-rw-   0        0        0      688 2023-06-10 16:01:01.000000 sinricpro-2.7.1/examples/push_notification.py
+-rw-rw-rw-   0        0        0     1000 2023-06-10 16:01:14.000000 sinricpro-2.7.1/examples/smart_lock.py
+-rw-rw-rw-   0        0        0     1964 2023-06-10 16:01:28.000000 sinricpro-2.7.1/examples/speaker.py
+-rw-rw-rw-   0        0        0      926 2023-06-10 16:01:37.000000 sinricpro-2.7.1/examples/switch.py
+-rw-rw-rw-   0        0        0     1570 2023-06-10 16:01:54.000000 sinricpro-2.7.1/examples/temperature_sensor.py
+-rw-rw-rw-   0        0        0     1943 2023-06-10 16:01:58.000000 sinricpro-2.7.1/examples/tv.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 16:09:20.465545 sinricpro-2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-06-09 16:40:19.000000 sinricpro-2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:09:20.450544 sinricpro-2.7.1/sinric/
+-rw-rw-rw-   0        0        0      400 2023-06-10 09:50:12.000000 sinricpro-2.7.1/sinric/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-06-10 15:34:37.000000 sinricpro-2.7.1/sinric/_brightness_controller.py
+-rw-rw-rw-   0        0        0    31791 2023-06-10 15:53:38.000000 sinricpro-2.7.1/sinric/_callback_handler.py
+-rw-rw-rw-   0        0        0      645 2023-06-09 16:41:44.000000 sinricpro-2.7.1/sinric/_color_controller.py
+-rw-rw-rw-   0        0        0     1001 2023-06-09 16:40:20.000000 sinricpro-2.7.1/sinric/_color_temperature.py
+-rw-rw-rw-   0        0        0     8388 2023-06-10 15:58:53.000000 sinricpro-2.7.1/sinric/_events.py
+-rw-rw-rw-   0        0        0     1210 2023-06-09 16:19:15.000000 sinricpro-2.7.1/sinric/_leaky_bucket.py
+-rw-rw-rw-   0        0        0      575 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_lock_controller.py
+-rw-rw-rw-   0        0        0      652 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_mode_controller.py
+-rw-rw-rw-   0        0        0      520 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_power_controller.py
+-rw-rw-rw-   0        0        0     1169 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_power_level_controller.py
+-rw-rw-rw-   0        0        0      281 2023-06-09 16:40:27.000000 sinricpro-2.7.1/sinric/_queues.py
+-rw-rw-rw-   0        0        0     1248 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_range_value_controller.py
+-rw-rw-rw-   0        0        0      869 2023-06-09 16:36:00.000000 sinricpro-2.7.1/sinric/_signature.py
+-rw-rw-rw-   0        0        0     3841 2023-06-10 10:35:39.000000 sinricpro-2.7.1/sinric/_sinricpro.py
+-rw-rw-rw-   0        0        0     2387 2023-06-10 15:58:14.000000 sinricpro-2.7.1/sinric/_sinricpro_constants.py
+-rw-rw-rw-   0        0        0     2270 2023-06-09 16:40:28.000000 sinricpro-2.7.1/sinric/_sinricpro_udp.py
+-rw-rw-rw-   0        0        0     3258 2023-06-10 05:45:06.000000 sinricpro-2.7.1/sinric/_sinricpro_websocket.py
+-rw-rw-rw-   0        0        0     1612 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_speaker_controller.py
+-rw-rw-rw-   0        0        0      983 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_temperature_controller.py
+-rw-rw-rw-   0        0        0      547 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_thermostat_controller.py
+-rw-rw-rw-   0        0        0     1965 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_tv_contorller.py
+-rw-rw-rw-   0        0        0      657 2023-06-10 09:33:30.000000 sinricpro-2.7.1/sinric/_webrtc_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:09:20.463544 sinricpro-2.7.1/sinricpro.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-06-10 16:09:20.000000 sinricpro-2.7.1/sinricpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2023-06-10 16:09:20.000000 sinricpro-2.7.1/sinricpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 16:09:20.000000 sinricpro-2.7.1/sinricpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-10 16:09:20.000000 sinricpro-2.7.1/sinricpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 16:09:20.000000 sinricpro-2.7.1/sinricpro.egg-info/top_level.txt
```

### Comparing `sinricpro-2.6.4/.github/workflows/python-publish.yml` & `sinricpro-2.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sinricpro-2.6.4/PKG-INFO` & `sinricpro-2.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sinricpro
-Version: 2.6.4
+Version: 2.7.1
 Summary: A python package for Sinric Pro
 Home-page: https://github.com/sinricpro/python-sdk
-Author: Dhanush
-Author-email: dhanushdazz@gmail.com
+Author: sinric
+Author-email: support@sinric.com
 Maintainer: sinric
 Maintainer-email: support@sinric.com
 Keywords: sinric,sinric-pro
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 
 SINRIC  PRO
```

### Comparing `sinricpro-2.6.4/README.md` & `sinricpro-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
        pip install sinricpro --user
 
 ### Upgarde
 
        pip install sinricpro --upgrade --user
 
-### Check the examples [here](https://github.com/sinricpro/python-sdk/examples) 
+### Check the examples [here](https://github.com/sinricpro/python-sdk/tree/master/examples)
```

### Comparing `sinricpro-2.6.4/examples/custom_device.py` & `sinricpro-2.7.1/examples/custom_device.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-from sinric import SinricPro 
+from sinric import SinricPro, SinricProConstants
 import asyncio
- 
+
 APP_KEY = ''
 APP_SECRET = ''
 DEVICE_ID = ''
-  
+
+
 def power_state(device_id, state):
     print(device_id, state)
     return True, state
 
+
 def range_value(device_id, range_value, instance_id):
     print(device_id, range_value, instance_id)
     return True, range_value, instance_id
 
+
 def mode_value(device_id, mode_value, instance_id):
     print(device_id, mode_value, instance_id)
     return True, mode_value, instance_id
- 
+
+
 callbacks = {
-    'powerState': power_state,
-    'setRangeValue': range_value,
-    'setMode': mode_value
+    SinricProConstants.SET_POWER_STATE: power_state,
+    SinricProConstants.SET_RANGE_VALUE: range_value,
+    SinricProConstants.SET_MODE: mode_value
 }
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
-    client = SinricPro(APP_KEY, [DEVICE_ID], callbacks, enable_log=False, restore_states=False, secretKey=APP_SECRET)
-    loop.run_until_complete(client.connect())
+    client = SinricPro(APP_KEY, [DEVICE_ID], callbacks,
+                       enable_log=False, restore_states=False, secret_key=APP_SECRET)
+    loop.run_until_complete(client.connect())
```

### Comparing `sinricpro-2.6.4/examples/push_notification.py` & `sinricpro-2.7.1/examples/push_notification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from sinric import SinricPro 
+from sinric import SinricPro, SinricProConstants
 import asyncio
 from asyncio import sleep
-from loguru import logger
 
 APP_KEY = ''
 APP_SECRET = ''
 DEVICE_ID = ''
- 
+
+
 async def events():
     while True:
-        client.event_handler.raiseEvent(DEVICE_ID, 'pushNotification', data={'alert': "Hello there"})
-        await sleep(60) # Server will trottle / block IPs sending events too often.
+        client.event_handler.raise_event(
+            DEVICE_ID, SinricProConstants.PUSH_NOTIFICATION, data={'alert': "Hello there"})
+        # Server will trottle / block IPs sending events too often.
+        await sleep(60)
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
-    client = SinricPro(APP_KEY, [DEVICE_ID], {}, event_callbacks=events, enable_log=True, restore_states=False, secretKey=APP_SECRET)
+    client = SinricPro(APP_KEY, [DEVICE_ID], {}, event_callbacks=events,
+                       enable_log=True, restore_states=False, secret_key=APP_SECRET)
     loop.run_until_complete(client.connect())
```

### Comparing `sinricpro-2.6.4/examples/tv.py` & `sinricpro-2.7.1/examples/dim_switch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,32 @@
-from sinric import SinricPro 
+from sinric import SinricPro, SinricProConstants
 import asyncio
- 
+
 APP_KEY = ''
 APP_SECRET = ''
-TV_ID = ''
+DIM_SWITCH_ID = ''
+
 
 def power_state(device_id, state):
-    print('state : ', state)
-    # Do Something
+    print('device_id: {} state: {}'.format(device_id, state))
     return True, state
 
 
-def set_volume(device_id, volume):
-    print('volume : ', volume)
-
-    # Do Somethign
-    return True, volume
-
-
-def adjust_volume(device_id, volume):
-    print('volume : ', volume)
-    # Do something with volume
-    return True, volume
-
-
-def media_control(device_id, control):
-    print('control : ', control)
-    # Do something with control
-    return True, control
-
-
-def select_input(device_id, input):
-    print('input : ', input)
-    # Do something with input
-    return True, input
-
-
-def change_channel(device_id, channel_name):
-    print('channel_name : ', channel_name)
-    # Change Channel
-    return True, channel_name
-
-
-def skip_channels(device_id, channel_count):
-    print('channel_count : ', channel_count)
-    # Skip them
-    return True, channel_count
+def power_level(device_id, power_level):
+    print('device_id: {} power level: {}'.format(device_id, power_level))
+    return True, power_level
 
 
 callbacks = {
-    'powerState': power_state,
-    'setVolume': set_volume,
-    'adjustVolume': adjust_volume,
-    'mediaControl': media_control,
-    'selectInput': select_input,
-    'changeChannel': change_channel,
-    'skipChannels': skip_channels
+    SinricProConstants.SET_POWER_STATE: power_state,
+    SinricProConstants.SET_POWER_LEVEL: power_level
 }
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
-    client = SinricPro(APP_KEY, [TV_ID], callbacks, enable_log=False, restore_states=False, secretKey=APP_SECRET)
+    client = SinricPro(APP_KEY, [DIM_SWITCH_ID], callbacks,
+                       enable_log=False, restore_states=False, secret_key=APP_SECRET)
     loop.run_until_complete(client.connect())
 
-# To update the TV state on server:
-# client.event_handler.raiseEvent(tvId, 'setVolume',data={'volume': 0})
-# client.event_handler.raiseEvent(tvId, 'mediaControl',data={'control': 'FastForward'})
-# client.event_handler.raiseEvent(tvId, 'changeChannel',data={'name': 'HBO'})
-# client.event_handler.raiseEvent(tvId, 'selectInput',data={"input":"HDMI"})
+    # client.event_handler.raise_event(DIM_SWITCH_ID, SinricProConstants.SET_POWER_LEVEL, data = {SinricProConstants.POWER_LEVEL: 50 })
+    # client.event_handler.raise_event(DIM_SWITCH_ID, SinricProConstants.SET_POWER_STATE, data = {SinricProConstants.STATE: SinricProConstants.POWER_STATE_ON })
+    # client.event_handler.raise_event(DIM_SWITCH_ID, SinricProConstants.SET_POWER_STATE, data = {SinricProConstants.STATE: SinricProConstants.POWER_STATE_OFF })
```

### Comparing `sinricpro-2.6.4/setup.py` & `sinricpro-2.7.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 from setuptools import setup
 import sys
 
 if sys.version_info < (3,6):
     sys.exit('Sorry, Python < 3.6 is not supported')
 
-VERSION = "2.6.4"
+VERSION = "2.7.1"
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 setup(
     name="sinricpro",
     version=VERSION,
-    author="Dhanush",
-    author_email="dhanushdazz@gmail.com",
+    author="sinric",
+    author_email="support@sinric.com",
     maintainer = 'sinric',
     maintainer_email = 'support@sinric.com',
     description="A python package for Sinric Pro",
     long_description=long_description,
     url="https://github.com/sinricpro/python-sdk",
     packages=['sinric'],
     install_requires=["websockets==10.1","loguru"],
```

### Comparing `sinricpro-2.6.4/sinric/_brightnessController.py` & `sinricpro-2.7.1/sinric/_brightness_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 
-from ._jsoncommands import JSON_COMMANDS
+from ._sinricpro_constants import SinricProConstants
 
 class BrightnessController:
-    def __init__(self, x):
-        self.brightness_level = x
+    def __init__(self, brightness_level) -> None:
+        self.brightness_level = brightness_level
 
-    async def setBrightness(self, jsn, brightness_callback):
-        self.brightness_level = jsn.get("payload").get("value").get("brightness")
-        return brightness_callback(jsn.get("payload").get("deviceId"),
-                                   self.brightness_level)
+    async def set_brightness(self, jsn, brightness_callback):
+        self.brightness_level = jsn.get("payload").get(SinricProConstants.VALUE).get(SinricProConstants.BRIGHTNESS)
+        return brightness_callback(jsn.get("payload").get(SinricProConstants.DEVICEID), self.brightness_level)
 
-    async def adjustBrightness(self, jsn, brightness_callback):
-        self.brightness_level += jsn.get("payload").get("value").get("brightnessDelta")
+    async def adjust_brightness(self, jsn, brightness_callback):
+        self.brightness_level += jsn.get("payload").get(SinricProConstants.VALUE).get(SinricProConstants.BRIGHTNESS_DELTA)
         if self.brightness_level > 100:
             self.brightness_level = 100
         elif self.brightness_level < 0:
             self.brightness_level = 0
 
-        return brightness_callback(jsn.get("payload").get("deviceId"),
-                                   self.brightness_level)
+        return brightness_callback(jsn.get("payload").get(SinricProConstants.DEVICEID), self.brightness_level)
```

### Comparing `sinricpro-2.6.4/sinric/_colorController.py` & `sinricpro-2.7.1/sinric/_color_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 
-from sinric._jsoncommands import JSON_COMMANDS
-
 
 class ColorController:
-    def __init__(self, x):
-        pass
 
-    async def setColor(self, jsn, set_color_callback):
+    async def set_color(self, jsn, set_color_callback):
         return set_color_callback(jsn.get("payload").get("deviceId"),
                                   jsn.get("payload").get("value").get("color").get("r"),
                                   jsn.get("payload").get("value").get("color").get("g"),
                                   jsn.get("payload").get("value").get("color").get("b"))
```

### Comparing `sinricpro-2.6.4/sinric/_colorTemperature.py` & `sinricpro-2.7.1/sinric/_color_temperature.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 
-from sinric._jsoncommands import JSON_COMMANDS
-
 
 class ColorTemperatureController:
-    def __init__(self, x, arr):
-        self.temperatures_index = x
-        self.temperatures_array = arr
-        pass
+    def __init__(self, temperatures_index, temperatures_array):
+        self.temperatures_index = temperatures_index
+        self.temperatures_array = temperatures_array
 
-    async def setColorTemperature(self, jsn, set_callback):
+    async def set_color_temperature(self, jsn, set_callback):
         return set_callback(jsn.get("payload").get("deviceId"),
                             jsn.get("payload").get("value").get("colorTemperature"))
 
-    async def increaseColorTemperature(self, jsn, increase_callback):
+    async def increase_color_temperature(self, jsn, increase_callback):
         return increase_callback(jsn.get("payload").get("deviceId"), jsn.get("payload").get("value"))
 
-    async def decreaseColorTemperature(self, jsn, decrease_callback):
+    async def decrease_color_temperature(self, jsn, decrease_callback):
         return decrease_callback(jsn.get("payload").get("deviceId"), jsn.get("payload").get("value"))
```

### Comparing `sinricpro-2.6.4/sinric/_leakyBucket.py` & `sinricpro-2.7.1/sinric/_leaky_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
         self.drop_out_time = drop_out_time
         self.drop_in_bucket = 0
         self.last_drop = 0
 
     def millis(self):
         return int(round(time.time() * 1000))
 
-    def leakDrops(self):
+    def leak_drops(self):
         actual_millis = self.millis()
         drops_to_leak = round((actual_millis - self.last_drop) / self.drop_out_time)
         if drops_to_leak > 0:
             if self.drop_in_bucket <= drops_to_leak:
                 self.drop_in_bucket = 0
             else:
                 self.drop_in_bucket = self.drop_in_bucket - drops_to_leak
 
-    def addDrop(self):
-        self.leakDrops()
+    def add_drop(self):
+        self.leak_drops()
         actual_millis = self.millis()
         if (self.drop_in_bucket < self.bucket_size) and (
                 (actual_millis - self.last_drop) > (self.drop_in_bucket + self.drop_in_time)):
             self.drop_in_bucket = self.drop_in_bucket + 1
             self.last_drop = actual_millis
             return True
         if self.drop_in_bucket >= self.bucket_size:
```

### Comparing `sinricpro-2.6.4/sinric/_signature.py` & `sinricpro-2.7.1/sinric/_signature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from json import dumps
 from base64 import b64encode
 import hmac as sinricHmac
 from hashlib import sha256
 
 
 class Signature:
-    def __init__(self, secretKey):
-        self.secretKey = secretKey
+    def __init__(self, secret_key):
+        self.secret_key = secret_key
 
-    def verifySignature(self, payload, signature) -> bool:
-        self.myHmac = sinricHmac.new(self.secretKey.encode('utf-8'),
-                                     dumps(payload, separators=(',', ':')).encode('utf-8'), sha256)
-        return b64encode(self.myHmac.digest()).decode('utf-8') == signature
-
-    def getSignature(self, payload) -> dict:
-        replyHmac = sinricHmac.new(self.secretKey.encode('utf-8'),
+    def verify_signature(self, payload, signature) -> bool:
+        self.hmac = sinricHmac.new(self.secret_key.encode('utf-8'),
                                    dumps(payload, separators=(',', ':')).encode('utf-8'), sha256)
+        return b64encode(self.hmac.digest()).decode('utf-8') == signature
+
+    def get_signature(self, payload) -> dict:
+        reply_hmac = sinricHmac.new(self.secret_key.encode('utf-8'),
+                                    dumps(payload, separators=(',', ':')).encode('utf-8'), sha256)
 
-        encodedHmac = b64encode(replyHmac.digest())
+        encoded_hmac = b64encode(reply_hmac.digest())
 
         return {
-            "HMAC": encodedHmac.decode('utf-8')
+            "HMAC": encoded_hmac.decode('utf-8')
         }
```

### Comparing `sinricpro-2.6.4/sinric/_sinricpro.py` & `sinricpro-2.7.1/sinric/_sinricpro.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,104 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 
 import asyncio
-from ._sinricprosocket import SinricProSocket
-from threading import Thread
-from ._events import Events
-from loguru import logger
 import re
 import sys
 
-logger.add("{}.log".format("sinricpro_logfile"), rotation="10 MB")
+from loguru import logger
+from ._sinricpro_websocket import SinricProSocket
+from ._events import Events
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Iterable as TypingIterable,
+    List,
+    Optional,
+    Set,
+    Type,
+    Union,
+    cast,
+)
+
+# logger.add("{}.log".format("sinricpro_logfile"), rotation="10 MB")
 
 
 class SinricPro:
-    def __init__(self, api, deviceid, request_callbacks, event_callbacks=None, enable_log=False, restore_states=False,
-                 secretKey="", loopDelay=0.5):
+    def __init__(self, api, device_id, request_callbacks, event_callbacks=None, enable_log=False, restore_states=False,
+                 secret_key="", loop_delay=0.5):
         try:
-            assert (self.verify_deviceId_arr(deviceid))
+            assert (self.verify_device_ids(device_id))
             self.restore_states = restore_states
-            self.apiKey = api
-            self.loopDelay = loopDelay if loopDelay > 0 else 0.5
-            self.secretKey = secretKey
-            self.deviceid = deviceid
+            self.app_key = api
+            self.loop_delay = loop_delay if loop_delay > 0 else 0.5
+            self.secret_key = secret_key
+            self.device_id = device_id
             self.logger = logger
             self.request_callbacks = request_callbacks
-            self.socket = SinricProSocket(self.apiKey, self.deviceid, self.request_callbacks, enable_log, self.logger,
-                                          self.restore_states, self.secretKey, loopDelay=loopDelay)
+            self.socket = SinricProSocket(self.app_key, self.device_id, self.request_callbacks, enable_log, self.logger,
+                                          self.restore_states, self.secret_key, loop_delay=loop_delay)
             self.connection = None
             self.event_callbacks = event_callbacks
-            self.event_handler = Events(self.connection, self.logger, self.secretKey)
+            self.event_handler = Events(
+                self.connection, self.logger, self.secret_key)
 
-            
         except AssertionError as e:
             logger.error("Device Id verification failed")
             sys.exit(0)
 
-    def verify_deviceId_arr(self, deviceid_arr):
-        arr = deviceid_arr
+    def verify_device_ids(self, device_id_arr):
+        arr = device_id_arr
         for i in arr:
             res = re.findall(r'^[a-fA-F0-9]{24}$', i)
             if len(res) == 0:
                 return False
         return True
- 
 
-    async def connect(self, udp_client=None, sleep=0):        
+    async def connect(self, udp_client=None, sleep=0):
         try:
             self.connection = await self.socket.connect()
-            receive_message_task = asyncio.create_task(self.socket.receiveMessage(connection=self.connection))
-            handle_queue_task = asyncio.create_task(self.socket.handleQueue())
-             
+            receive_message_task = asyncio.create_task(self.socket.receive_message(connection=self.connection))
+            handle_queue_task = asyncio.create_task(self.socket.handle_queue())
+
             if self.event_callbacks is not None:
-                handle_event_queue_task = asyncio.create_task(self.event_callbacks())
-                await handle_event_queue_task             
-            
+                handle_event_queue_task = asyncio.create_task(
+                    self.event_callbacks())
+                await handle_event_queue_task
+
             await handle_queue_task
             await receive_message_task
-            
+
         except KeyboardInterrupt:
             self.logger.error('Keyboard interrupt')
         except Exception as e:
             self.logger.error(e)
+
+    # async def run_app(self, loop: Optional[asyncio.AbstractEventLoop] = None) -> None:
+    #     """Run an app locally"""
+
+    #     if loop is None:
+    #         loop = asyncio.new_event_loop()
         
+    #     #loop.set_debug(debug)
+    #     self.connection = await self.socket.connect()
+
+    #     receive_message_task = loop.create_task(self.socket.receive_message(connection=self.connection))
+    #     handle_queue_task = loop.create_task(self.socket.handle_queue())
+    #     #handle_event_queue_task = asyncio.create_task(self.event_callbacks())
+                    
+    #     try:
+    #         asyncio.set_event_loop(loop)
+    #         loop.run_until_complete([receive_message_task, handle_queue_task])
+    #     except (KeyboardInterrupt):  # pragma: no cover GracefulExit
+    #         pass
+    #     finally:
+    #         #_cancel_tasks({main_task}, loop)
+    #         #_cancel_tasks(asyncio.all_tasks(loop), loop)
+    #         loop.run_until_complete(loop.shutdown_asyncgens())
+    #         loop.close()
+    #         asyncio.set_event_loop(None)
```

### Comparing `sinricpro-2.6.4/sinric/_sinricprosocket.py` & `sinricpro-2.7.1/sinric/_sinricpro_websocket.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 
 from websockets import client
 from websockets.exceptions import ConnectionClosed
 import json
-from ._mainqueue import queue
-from ._cbhandler import CallBackHandler
+from ._queues import queue
+from ._callback_handler import CallBackHandler
 from ._signature import Signature
 from time import time
 import asyncio
 import pkg_resources
+
+
 class SinricProSocket(Signature):
 
-    def __init__(self, appKey, deviceId, callbacks, enable_trace=False, logger=None, restore_states=False,
-                 secretKey="", loopDelay=0.5):
-        self.appKey = appKey
-        self.secretKey = secretKey
+    def __init__(self, app_key, device_id, callbacks, enable_trace=False, logger=None, restore_states=False,
+                 secret_key="", loop_delay=0.5):
+        self.app_key = app_key
+        self.secret_key = secret_key
         self.restore_states = restore_states
         self.logger = logger
-        self.deviceIds = deviceId
+        self.device_ids = device_id
         self.connection = None
         self.callbacks = callbacks
-        self.loopDelay = loopDelay
+        self.loop_delay = loop_delay
 
         self.callbackHandler = CallBackHandler(self.callbacks, enable_trace, self.logger, self.restore_states,
-                                               secretKey=self.secretKey)
+                                               secret_key=self.secret_key)
         self.enableTrace = enable_trace
-        Signature.__init__(self, self.secretKey)
+        Signature.__init__(self, self.secret_key)
 
     async def connect(self):  # Producer
         sdk_version = pkg_resources.require("sinricpro")[0].version
-        self.connection = await client.connect('ws://ws.sinric.pro',
-                                                          extra_headers={'appkey': self.appKey,
-                                                                         'deviceids': ';'.join(self.deviceIds),
-                                                                         'platform': 'python',
-                                                                         'sdkversion' : sdk_version,
-                                                                         'restoredevicestates': (
-                                                                             'true' if self.restore_states else 'false')},
-                                                          ping_interval=30000, ping_timeout=10000)
+        self.connection = await client.connect('wss://testws.sinric.pro',
+                                               extra_headers={'appkey': self.app_key,
+                                                              'deviceids': ';'.join(self.device_ids),
+                                                              'platform': 'python',
+                                                              'sdkversion': sdk_version,
+                                                              'restoredevicestates': (
+                                                                  'true' if self.restore_states else 'false')},
+                                               ping_interval=30000, ping_timeout=10000)
         if self.connection.open:
             self.logger.success(f"{'Connected :)'}")
-            timestamp  = await self.connection.recv()
-            if(int(time()) - json.loads(timestamp).get('timestamp') > 60000):
-                self.logger.warning(f'Timestamp is not in sync check your system time. 🙄🙄🙄🙄🙄:(')
+            timestamp = await self.connection.recv()
+            if (int(time()) - json.loads(timestamp).get('timestamp') > 60000):
+                self.logger.warning(f'Timestamp is not in sync. Please check your system time.')
             return self.connection
 
-    async def receiveMessage(self, connection):
+    async def receive_message(self, connection):
         while True:
             try:
                 message = await connection.recv()
                 if self.enableTrace:
                     self.logger.info(f"Request : {message}")
-                requestJson = json.loads(message)
-                queue.put([requestJson, 'socket_response'])
-                await asyncio.sleep(self.loopDelay)
+                request = json.loads(message)
+                queue.put([request, 'socket_response', 'request_response'])
+                await asyncio.sleep(self.loop_delay)
             except ConnectionClosed as e:
                 self.logger.info('Connection with server closed')
                 raise e
 
-    async def handleQueue(self):
+    async def handle_queue(self):
         while True:
-            await asyncio.sleep(self.loopDelay)
-            
+            await asyncio.sleep(self.loop_delay)
+
             while queue.qsize() > 0:
-                await self.callbackHandler.handleCallBacks(queue.get(), self.connection, None)
+                await self.callbackHandler.handle_callbacks(queue.get(), self.connection, None)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sinricpro-2.6.4/sinric/_sinricproudp.py` & `sinricpro-2.7.1/sinric/_sinricpro_udp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 
 import asyncio
-import socket 
+import socket
 from socket import AF_INET, SOCK_DGRAM
-from ._mainqueue import queue
+from ._queues import queue
 import json
 from asyncio import sleep
 import struct
 
 
 class EchoServerProtocol(asyncio.DatagramProtocol):
-    def __init__(self,enablePrint, deviceIdArr=[]) -> None:
+    def __init__(self, enablePrint, deviceIdArr=[]) -> None:
         super().__init__()
         self.enablePrint = enablePrint
         self.deviceIdArr = deviceIdArr
 
     def connection_made(self, transport):
         self.transport = transport
 
     def datagram_received(self, data, addr):
         jsonData = json.loads(data.decode('ascii'))
         if jsonData.get('payload', None).get('deviceId', None) in self.deviceIdArr:
-                queue.put([jsonData, 'udp_response', addr])
+            queue.put([jsonData, 'udp_response', addr])
         else:
-                print('Invalid Device id')
+            print('Invalid Device id')
         if self.enablePrint:
-                print(data)
-                print('UDP senderID : ', addr)
+            print(data)
+            print('UDP senderID : ', addr)
+
 
 class SinricProUdp:
-    def __init__(self, callbacks_udp, deviceIdArr,enable_trace=False, loopDelay=0.5, loopInstance=None):
+    def __init__(self, callbacks_udp, deviceIdArr, enable_trace=False, loop_delay=0.5, loopInstance=None):
         self.callbacks = callbacks_udp
         self.deviceIdArr = deviceIdArr
         self.enablePrint = enable_trace
         self.loopInstance = loopInstance
-        self.loopDelay = loopDelay if loopDelay > 0 else 0.5
+        self.loop_delay = loop_delay if loop_delay > 0 else 0.5
         self.udp_ip = '224.9.9.9'
         self.udp_port = 3333
         self.address = ('', self.udp_port)
         self.sockServ = socket.socket(AF_INET, SOCK_DGRAM)
         self.sockServ.bind(self.address)
         self.sockServ.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP,
                                  struct.pack("4sl", socket.inet_aton(self.udp_ip), socket.INADDR_ANY))
 
     def sendResponse(self, data, sender):
         self.sockServ.sendto(data, sender)
 
     async def listen(self):
         await self.loopInstance.create_datagram_endpoint(
-        lambda: EchoServerProtocol(enablePrint=self.enablePrint, deviceIdArr=self.deviceIdArr),
-        local_addr=None,remote_addr=None, sock=self.sockServ)
+            lambda: EchoServerProtocol(
+                enablePrint=self.enablePrint, deviceIdArr=self.deviceIdArr),
+            local_addr=None, remote_addr=None, sock=self.sockServ)
         while True:
-            await asyncio.sleep(self.loopDelay)            
+            await asyncio.sleep(self.loop_delay)
```

### Comparing `sinricpro-2.6.4/sinric/_tvcontorller.py` & `sinricpro-2.7.1/sinric/_tv_contorller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """
- *  Copyright (c) 2019 Sinric. All rights reserved.
+ *  Copyright (c) 2019-2023 Sinric. All rights reserved.
  *  Licensed under Creative Commons Attribution-Share Alike (CC BY-SA)
  *
  *  This file is part of the Sinric Pro (https://github.com/sinricpro/)
 """
 
-from ._jsoncommands import JSON_COMMANDS
+from ._sinricpro_constants import SinricProConstants
 
 
 class TvController:
     def __init__(self, x):
         self.volume = x
 
-
-    async def setVolume(self, jsn, callback):
-        self.volume = jsn.get("payload").get(JSON_COMMANDS.get('VALUE')).get('volume')
-        return callback(jsn.get("payload").get(JSON_COMMANDS.get('DEVICEID')), self.volume)
-
-    async def adjustVolume(self, jsn, callback):
-        self.volume += jsn.get("payload").get(JSON_COMMANDS.get('VALUE')).get('volume')
+    async def set_volume(self, jsn, callback):
+        self.volume = jsn.get("payload").get(
+            SinricProConstants.VALUE).get('volume')
+        return callback(jsn.get("payload").get(SinricProConstants.DEVICEID), self.volume)
+
+    async def adjust_volume(self, jsn, callback):
+        self.volume += jsn.get("payload").get(
+            SinricProConstants.VALUE).get('volume')
         if self.volume > 100:
             self.volume = 100
         elif self.volume < 0:
             self.volume = 0
-        return callback(jsn.get("payload").get(JSON_COMMANDS.get('DEVICEID')), self.volume)
+        return callback(jsn.get("payload").get(SinricProConstants.DEVICEID), self.volume)
 
-    async def setMute(self, jsn, callback):
-        return callback(jsn.get("payload").get(JSON_COMMANDS.get('DEVICEID')), jsn.get("payload").get('value').get('mute'))
+    async def set_mute(self, jsn, callback):
+        return callback(jsn.get("payload").get(SinricProConstants.DEVICEID), jsn.get("payload").get(SinricProConstants.VALUE).get('mute'))
 
-    async def mediaControl(self, jsn, callback):
-        return callback(jsn.get("payload").get(JSON_COMMANDS.get('DEVICEID')), jsn.get("payload").get(JSON_COMMANDS.get('VALUE')).get('control'))
+    async def media_control(self, jsn, callback):
+        return callback(jsn.get("payload").get(SinricProConstants.DEVICEID), jsn.get("payload").get(SinricProConstants.VALUE).get('control'))
 
-    async def selectInput(self, jsn, callback):
-        inp = jsn.get("payload").get(JSON_COMMANDS.get('VALUE')).get('input')
-        return callback(jsn.get("payload").get(JSON_COMMANDS.get('DEVICEID')), inp)
+    async def select_input(self, jsn, callback):
+        inp = jsn.get("payload").get(SinricProConstants.VALUE).get('input')
+        return callback(jsn.get("payload").get(SinricProConstants.DEVICEID), inp)
 
-    async def changeChannel(self, jsn, callback):
-        return callback(jsn.get("payload").get(JSON_COMMANDS.get('DEVICEID')), jsn.get("payload").get('value').get('channel').get('name'))
+    async def change_channel(self, jsn, callback):
+        return callback(jsn.get("payload").get(SinricProConstants.DEVICEID), jsn.get("payload").get(SinricProConstants.VALUE).get('channel').get('name'))
 
-    async def skipChannels(self, jsn, callback):
-        return callback(jsn.get("payload").get(JSON_COMMANDS.get('DEVICEID')), jsn.get("payload").get(JSON_COMMANDS.get('VALUE')).get('channelCount'))
+    async def skip_channels(self, jsn, callback):
+        return callback(jsn.get("payload").get(SinricProConstants.DEVICEID), jsn.get("payload").get(SinricProConstants.VALUE).get('channelCount'))
```

### Comparing `sinricpro-2.6.4/sinricpro.egg-info/PKG-INFO` & `sinricpro-2.7.1/sinricpro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sinricpro
-Version: 2.6.4
+Version: 2.7.1
 Summary: A python package for Sinric Pro
 Home-page: https://github.com/sinricpro/python-sdk
-Author: Dhanush
-Author-email: dhanushdazz@gmail.com
+Author: sinric
+Author-email: support@sinric.com
 Maintainer: sinric
 Maintainer-email: support@sinric.com
 Keywords: sinric,sinric-pro
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 
 SINRIC  PRO
```

### Comparing `sinricpro-2.6.4/sinricpro.egg-info/SOURCES.txt` & `sinricpro-2.7.1/sinricpro.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 examples/push_notification.py
 examples/smart_lock.py
 examples/speaker.py
 examples/switch.py
 examples/temperature_sensor.py
 examples/tv.py
 sinric/__init__.py
-sinric/_brightnessController.py
-sinric/_cbhandler.py
-sinric/_colorController.py
-sinric/_colorTemperature.py
+sinric/_brightness_controller.py
+sinric/_callback_handler.py
+sinric/_color_controller.py
+sinric/_color_temperature.py
 sinric/_events.py
-sinric/_jsoncommands.py
-sinric/_leakyBucket.py
-sinric/_lockController.py
-sinric/_mainqueue.py
-sinric/_modeController.py
-sinric/_powerController.py
-sinric/_powerLevelController.py
-sinric/_rangeValueController.py
+sinric/_leaky_bucket.py
+sinric/_lock_controller.py
+sinric/_mode_controller.py
+sinric/_power_controller.py
+sinric/_power_level_controller.py
+sinric/_queues.py
+sinric/_range_value_controller.py
 sinric/_signature.py
 sinric/_sinricpro.py
-sinric/_sinricprosocket.py
-sinric/_sinricproudp.py
-sinric/_speakerController.py
-sinric/_temperatureController.py
-sinric/_thermostatController.py
-sinric/_tvcontorller.py
+sinric/_sinricpro_constants.py
+sinric/_sinricpro_udp.py
+sinric/_sinricpro_websocket.py
+sinric/_speaker_controller.py
+sinric/_temperature_controller.py
+sinric/_thermostat_controller.py
+sinric/_tv_contorller.py
+sinric/_webrtc_controller.py
 sinricpro.egg-info/PKG-INFO
 sinricpro.egg-info/SOURCES.txt
 sinricpro.egg-info/dependency_links.txt
 sinricpro.egg-info/requires.txt
 sinricpro.egg-info/top_level.txt
```


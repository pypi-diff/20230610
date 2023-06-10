# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a6.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a6.tar", last modified: Tue Jun  6 23:07:20 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.3a1.tar", last modified: Sat Jun 10 02:06:04 2023, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6.tar` & `ovos-PHAL-plugin-homeassistant-0.0.3a1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.220246 ovos-PHAL-plugin-homeassistant-0.0.2a6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.204246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/code/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.212246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.212246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.212246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.208246 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:07:20.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.204246 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:07:20.216246 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/icon/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:07:20.220246 ovos-PHAL-plugin-homeassistant-0.0.2a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-06 23:07:19.000000 ovos-PHAL-plugin-homeassistant-0.0.2a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35653 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a6
+Version: 0.0.3a1
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,31 +31,34 @@
             "switch": HomeAssistantSwitch,
             "climate": HomeAssistantClimate,
             "camera": HomeAssistantCamera,
             "scene": HomeAssistantScene,
             "automation": HomeAssistantAutomation,
         }
 
+
 class HomeAssistantPlugin(PHALPlugin):
     def __init__(self, bus=None, config=None):
         """ Initialize the plugin
 
             Args:
                 bus (MycroftBusClient): The Mycroft bus client
                 config (dict): The plugin configuration
         """
-        super().__init__(bus=bus, name="ovos-PHAL-plugin-homeassistant", config=config)
+        super().__init__(bus=bus, name="ovos-PHAL-plugin-homeassistant",
+                         config=config)
         self.oauth_client_id = None
         self.munged_id = "ovos-PHAL-plugin-homeassistant_homeassistant-phal-plugin"
         self.temporary_instance = None
         self.connector = None
         self.registered_devices = []  # Device objects
         self.registered_device_names = []  # Device friendly/entity names
         self.bus = bus
-        self.gui = GUIInterface(bus=self.bus, skill_id=self.name)
+        self.gui = GUIInterface(bus=self.bus, skill_id=self.name,
+                                config=self.config_core.get('gui'))
         self.integrator = Integrator(self.bus, self.gui)
         self.instance_available = False
         self.use_ws = False
         self.device_types = SUPPORTED_DEVICES
 
         # BUS API FOR HOME ASSISTANT
         self.bus.on("ovos.phal.plugin.homeassistant.get.devices",
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/connector.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/connector.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/device.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/device.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/integration.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/integration.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/socketclient.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/socketclient.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/logic/utils.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/code/helper.js` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/code/helper.js`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a6
+Version: 0.0.3a1
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a6/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a1/setup.py`

 * *Files identical despite different names*


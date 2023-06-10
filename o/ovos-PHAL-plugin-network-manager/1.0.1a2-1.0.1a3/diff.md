# Comparing `tmp/ovos-PHAL-plugin-network-manager-1.0.1a2.tar.gz` & `tmp/ovos-PHAL-plugin-network-manager-1.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-network-manager-1.0.1a2.tar", last modified: Tue Apr  4 23:08:57 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-network-manager-1.0.1a3.tar", last modified: Sat Jun 10 03:34:22 2023, max compression
```

## Comparing `ovos-PHAL-plugin-network-manager-1.0.1a2.tar` & `ovos-PHAL-plugin-network-manager-1.0.1a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:08:57.853414 ovos-PHAL-plugin-network-manager-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 23:08:50.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-04 23:08:57.853414 ovos-PHAL-plugin-network-manager-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-04 23:08:50.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:08:57.849414 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-04-04 23:08:50.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 23:08:52.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:08:57.853414 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-04 23:08:57.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-04 23:08:57.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 23:08:57.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-04 23:08:57.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-04 23:08:57.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 23:08:57.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 23:08:57.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 23:08:57.853414 ovos-PHAL-plugin-network-manager-1.0.1a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-04-04 23:08:50.000000 ovos-PHAL-plugin-network-manager-1.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:34:22.532613 ovos-PHAL-plugin-network-manager-1.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 03:34:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-10 03:34:22.532613 ovos-PHAL-plugin-network-manager-1.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-10 03:34:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:34:22.532613 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-06-10 03:34:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 03:34:17.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:34:22.532613 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-10 03:34:22.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-10 03:34:22.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:34:22.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-10 03:34:22.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 03:34:22.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 03:34:22.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:34:22.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 03:34:22.532613 ovos-PHAL-plugin-network-manager-1.0.1a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-06-10 03:34:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a3/setup.py
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a2/LICENSE` & `ovos-PHAL-plugin-network-manager-1.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a2/PKG-INFO` & `ovos-PHAL-plugin-network-manager-1.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-network-manager
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: Network Manager plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-network-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a2/README.md` & `ovos-PHAL-plugin-network-manager-1.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager/__init__.py` & `ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import subprocess
 import threading
 from distutils.spawn import find_executable
 
 from dbus_next.aio import MessageBus
 from dbus_next.constants import BusType
-from mycroft_bus_client.message import Message
+from ovos_bus_client.message import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.log import LOG
 
 
 # Event Documentation
 # ===================
 # Backend:
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a2/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO` & `ovos-PHAL-plugin-network-manager-1.0.1a3/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-network-manager
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: Network Manager plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-network-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a2/setup.py` & `ovos-PHAL-plugin-network-manager-1.0.1a3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/ovos-phal-plugin-connectivity-events-0.0.2a2.tar.gz` & `tmp/ovos-phal-plugin-connectivity-events-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.2a2.tar", last modified: Sat Mar  4 18:03:31 2023, max compression
+gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.3a1.tar", last modified: Sat Jun 10 01:53:50 2023, max compression
```

## Comparing `ovos-phal-plugin-connectivity-events-0.0.2a2.tar` & `ovos-phal-plugin-connectivity-events-0.0.3a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 18:03:31.908717 ovos-phal-plugin-connectivity-events-0.0.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-04 18:03:31.908717 ovos-phal-plugin-connectivity-events-0.0.2a2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 18:03:31.908717 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events/
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-03-04 18:03:20.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-04 18:03:26.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 18:03:31.908717 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-04 18:03:31.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-04 18:03:31.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 18:03:31.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-04 18:03:31.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-04 18:03:31.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-04 18:03:31.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 18:03:31.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 18:03:31.908717 ovos-phal-plugin-connectivity-events-0.0.2a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-03-04 18:03:20.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 18:03:31.908717 ovos-phal-plugin-connectivity-events-0.0.2a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-03-04 18:03:20.000000 ovos-phal-plugin-connectivity-events-0.0.2a2/test/test_connectivity_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.711756 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-10 01:53:42.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 01:53:45.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-10 01:53:42.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-10 01:53:42.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/test/test_connectivity_events.py
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.2a2/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.2a2
+Version: 0.0.3a1
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: # ovos-PHAL-plugin - Connectivity Events
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events/__init__.py` & `ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import IntEnum
 from threading import Event
 
-from mycroft_bus_client import Message
+from ovos_bus_client.message import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.log import LOG
 from ovos_utils.network_utils import is_connected_dns, is_connected_http
 
 
 class ConnectivityState(IntEnum):
     """ State of network/internet connectivity.
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.2a2
+Version: 0.0.3a1
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: # ovos-PHAL-plugin - Connectivity Events
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.2a2/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt` & `ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.2a2/setup.py` & `ovos-phal-plugin-connectivity-events-0.0.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.2a2/test/test_connectivity_events.py` & `ovos-phal-plugin-connectivity-events-0.0.3a1/test/test_connectivity_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import unittest
 from unittest.mock import Mock
 
-from mycroft_bus_client import Message
+from ovos_bus_client.message import Message
 from ovos_utils.messagebus import FakeBus
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 from ovos_phal_plugin_connectivity_events import ConnectivityEvents, ConnectivityState
 
 
 class TestPlugin(unittest.TestCase):
```


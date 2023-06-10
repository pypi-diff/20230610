# Comparing `tmp/ovos-PHAL-plugin-system-0.0.4a2.tar.gz` & `tmp/ovos-PHAL-plugin-system-0.0.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a2.tar", last modified: Tue Apr 11 16:19:49 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a3.tar", last modified: Sat Jun 10 02:13:44 2023, max compression
```

## Comparing `ovos-PHAL-plugin-system-0.0.4a2.tar` & `ovos-PHAL-plugin-system-0.0.4a3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.866209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Reboot.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Restart.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Shutdown.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Status.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/loading.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-fail.json
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-success.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 16:19:43.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.866209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:13:44.357010 ovos-PHAL-plugin-system-0.0.4a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 02:13:44.357010 ovos-PHAL-plugin-system-0.0.4a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:13:44.353010 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:13:44.357010 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Reboot.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Restart.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Shutdown.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Status.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:13:44.357010 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/animations/loading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/animations/status-fail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/animations/status-success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 02:13:38.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:13:44.353010 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 02:13:44.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-10 02:13:44.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:13:44.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 02:13:44.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 02:13:44.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-10 02:13:44.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:13:44.000000 ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:13:44.357010 ovos-PHAL-plugin-system-0.0.4a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-06-10 02:13:35.000000 ovos-PHAL-plugin-system-0.0.4a3/setup.py
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a2
+Version: 0.0.4a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/__init__.py` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 
 class SystemEvents(PHALPlugin):
     validator = SystemEventsValidator
 
     def __init__(self, bus=None, config=None):
         super().__init__(bus=bus, name="ovos-PHAL-plugin-system", config=config)
-        self.gui = GUIInterface(bus=self.bus, skill_id=self.name)
+        self.gui = GUIInterface(bus=self.bus, skill_id=self.name,
+                                config=self.config_core.get('gui'))
 
         self.bus.on("system.ntp.sync", self.handle_ntp_sync_request)
         self.bus.on("system.ssh.status", self.handle_ssh_status)
         self.bus.on("system.ssh.enable", self.handle_ssh_enable_request)
         self.bus.on("system.ssh.disable", self.handle_ssh_disable_request)
         self.bus.on("system.reboot", self.handle_reboot_request)
         self.bus.on("system.shutdown", self.handle_shutdown_request)
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Reboot.qml` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Reboot.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Restart.qml` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Restart.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Shutdown.qml` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Shutdown.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Status.qml` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/loading.json` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/animations/loading.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-fail.json` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-success.json` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system/ui/animations/status-success.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a2
+Version: 0.0.4a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-system-0.0.4a3/ovos_PHAL_plugin_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a2/setup.py` & `ovos-PHAL-plugin-system-0.0.4a3/setup.py`

 * *Files identical despite different names*


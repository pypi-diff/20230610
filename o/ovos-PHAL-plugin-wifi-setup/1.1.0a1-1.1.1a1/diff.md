# Comparing `tmp/ovos-PHAL-plugin-wifi-setup-1.1.0a1.tar.gz` & `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.0a1.tar", last modified: Sat Mar 11 02:51:26 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a1.tar", last modified: Sat Jun 10 02:14:04 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wifi-setup-1.1.0a1.tar` & `ovos-PHAL-plugin-wifi-setup-1.1.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:51:26.690932 ovos-PHAL-plugin-wifi-setup-1.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-11 02:51:18.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-11 02:51:26.690932 ovos-PHAL-plugin-wifi-setup-1.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-03-11 02:51:18.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:51:26.690932 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup/
--rw-r--r--   0 runner    (1001) docker     (123)    22793 2023-03-11 02:51:18.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-11 02:51:20.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:51:26.690932 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-11 02:51:26.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-11 02:51:26.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 02:51:26.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-11 02:51:26.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-11 02:51:26.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-11 02:51:26.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 02:51:26.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 02:51:26.690932 ovos-PHAL-plugin-wifi-setup-1.1.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-03-11 02:51:18.000000 ovos-PHAL-plugin-wifi-setup-1.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 02:13:58.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:14:04.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:14:04.421290 ovos-PHAL-plugin-wifi-setup-1.1.1a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-10 02:13:55.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a1/setup.py
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.0a1/LICENSE` & `ovos-PHAL-plugin-wifi-setup-1.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.0a1/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.0a1
+Version: 1.1.1a1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.0a1/README.md` & `ovos-PHAL-plugin-wifi-setup-1.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup/__init__.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,45 +130,58 @@
         self.time_between_checks = 30
         self.mycroft_ready = False
         self.stop_on_internet = False
         self.timeout_after_internet = 90
         self.active_client = None
         self.active_client_id = None
         self.registered_clients = []
-        self.gui = GUIInterface(bus=self.bus, skill_id=self.name)
+        self.gui = GUIInterface(bus=self.bus, skill_id=self.name,
+                                config=self.config_core.get('gui'))
 
         # 0 = Normal Operation, 1 = Skipped (User selected to skip setup)
-        # if the user selected to skip setup, we will not start the setup process or check for internet, etc.
-        # until the user explicitly tells us to start the setup process again either through VUI or GUI interaction
+        # if the user selected to skip setup, we will not start the setup
+        # process or check for internet, etc. until the user explicitly tells us
+        # to start the setup process again either through VUI or GUI interaction
         self.plugin_setup_mode = 0
 
         # Manage client registration, activation and deactivation
         # Multiple clients can be registered, but only one can be active at a time
-        self.bus.on("ovos.phal.wifi.plugin.register.client", self.handle_register_client)
-        self.bus.on("ovos.phal.wifi.plugin.deregister.client", self.handle_deregister_client)
-        self.bus.on("ovos.phal.wifi.plugin.get.registered.clients", self.handle_get_registered_clients)
-        self.bus.on("ovos.phal.wifi.plugin.set.active.client", self.handle_set_active_client)
-        self.bus.on("ovos.phal.wifi.plugin.remove.active.client", self.handle_remove_active_client)
+        self.bus.on("ovos.phal.wifi.plugin.register.client",
+                    self.handle_register_client)
+        self.bus.on("ovos.phal.wifi.plugin.deregister.client",
+                    self.handle_deregister_client)
+        self.bus.on("ovos.phal.wifi.plugin.get.registered.clients",
+                    self.handle_get_registered_clients)
+        self.bus.on("ovos.phal.wifi.plugin.set.active.client",
+                    self.handle_set_active_client)
+        self.bus.on("ovos.phal.wifi.plugin.remove.active.client",
+                    self.handle_remove_active_client)
 
         # Manage when the client is in setup and out of setup
-        self.bus.on("ovos.phal.wifi.plugin.client.setup.failure", self.handle_client_setup_failure)
+        self.bus.on("ovos.phal.wifi.plugin.client.setup.failure",
+                    self.handle_client_setup_failure)
 
         # GUI event to handle client selection
         # Client selection is presented to the user in the GUI if GUI and touch/mouse are available
-        self.bus.on("ovos.phal.wifi.plugin.client.select", self.handle_client_select)
+        self.bus.on("ovos.phal.wifi.plugin.client.select",
+                    self.handle_client_select)
         self.bus.on("ovos.phal.wifi.plugin.skip.setup", self.handle_skip_setup)
-        self.bus.on("ovos.phal.wifi.plugin.fully.offline", self.handle_fully_offline)
-        self.bus.on("ovos.phal.wifi.plugin.client.select.page.removed", self.handle_setup_page_removed)
+        self.bus.on("ovos.phal.wifi.plugin.fully.offline",
+                    self.handle_fully_offline)
+        self.bus.on("ovos.phal.wifi.plugin.client.select.page.removed",
+                    self.handle_setup_page_removed)
 
         # GUI event to handle user activation of plugin (user selected the plugin in the GUI)
         # or via voice command (user activated the plugin via voice command)
-        self.bus.on("ovos.phal.wifi.plugin.user.activated", self.handle_user_activated)
+        self.bus.on("ovos.phal.wifi.plugin.user.activated",
+                    self.handle_user_activated)
 
         # Handle Internet Connected Event
-        self.bus.on("mycroft.internet.connected", self.handle_internet_connected)
+        self.bus.on("mycroft.internet.connected",
+                    self.handle_internet_connected)
 
         # When the plugin comes online, we need to emit a message so clients can register
         self.bus.emit(Message("ovos.phal.wifi.plugin.alive"))
         # Also let the clients ask if the plugin is alive
         self.bus.on("ovos.phal.wifi.plugin.status", self.handle_status_request)
 
         # Check if internet is ready for mycroft_ready
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.0a1/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a1/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.0a1
+Version: 1.1.1a1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.0a1/setup.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a1/setup.py`

 * *Files identical despite different names*


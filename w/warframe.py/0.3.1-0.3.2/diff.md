# Comparing `tmp/warframe.py-0.3.1.tar.gz` & `tmp/warframe.py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warframe.py-0.3.1.tar", last modified: Sat Jun 10 12:12:08 2023, max compression
+gzip compressed data, was "warframe.py-0.3.2.tar", last modified: Sat Jun 10 19:40:10 2023, max compression
```

## Comparing `warframe.py-0.3.1.tar` & `warframe.py-0.3.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.720237 warframe.py-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-10 12:11:25.000000 warframe.py-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 12:12:08.720237 warframe.py-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-10 12:11:25.000000 warframe.py-0.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 12:11:25.000000 warframe.py-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 12:12:08.720237 warframe.py-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-10 12:11:25.000000 warframe.py-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/worldstate/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/worldstate/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/common/base_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/common/types_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/worldstate/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/mission_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/syndicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.720237 warframe.py-0.3.1/warframe/worldstate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/archon_hunt.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/cambion_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/cetus.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/counted_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/daily_deal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/fissure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/flash_sale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/invasion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/orb_vallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/sortie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/void_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/worldstate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.144306 warframe.py-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-10 19:39:37.000000 warframe.py-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 19:40:10.144306 warframe.py-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-10 19:39:37.000000 warframe.py-0.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 19:39:37.000000 warframe.py-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 19:40:10.144306 warframe.py-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-10 19:39:37.000000 warframe.py-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/worldstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/worldstate/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/common/base_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/common/types_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe/worldstate/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/mission_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/enums/syndicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.144306 warframe.py-0.3.2/warframe/worldstate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/archon_hunt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/cambion_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/cetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/counted_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/daily_deal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/fissure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/flash_sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/invasion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/orb_vallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/sortie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/models/void_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:39:37.000000 warframe.py-0.3.2/warframe/worldstate/worldstate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:40:10.140306 warframe.py-0.3.2/warframe.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 19:40:10.000000 warframe.py-0.3.2/warframe.py.egg-info/top_level.txt
```

### Comparing `warframe.py-0.3.1/LICENSE` & `warframe.py-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/PKG-INFO` & `warframe.py-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.1
+Version: 0.3.2
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.1/README.rst` & `warframe.py-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/setup.py` & `warframe.py-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/client.py` & `warframe.py-0.3.2/warframe/worldstate/client.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/common/base_objects.py` & `warframe.py-0.3.2/warframe/worldstate/common/base_objects.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/common/types_.py` & `warframe.py-0.3.2/warframe/worldstate/common/types_.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/endpoints.py` & `warframe.py-0.3.2/warframe/worldstate/endpoints.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/enums/mission_type.py` & `warframe.py-0.3.2/warframe/worldstate/enums/mission_type.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/exceptions.py` & `warframe.py-0.3.2/warframe/worldstate/exceptions.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/alert.py` & `warframe.py-0.3.2/warframe/worldstate/models/alert.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,31 @@
 __all__ = ["Alert"]
 
 
 class Alert(MultiQueryModel):
     __endpoint__ = "/alerts"
 
     # required
+    activation: datetime
+    "The time the mission began"
+
+    expiry: datetime
+    "The time the mission ends"
+
     mission: Mission
     "The mission that corresponds to this Alert"
-    expired: bool
-    "Whether the mission is expired or not"
+
     reward_types: List[ItemRewardType]
     "A list of reward types"
 
     # optional
-    activation: Optional[datetime] = None
-    "The time the mission began"
-    expiry: Optional[datetime] = None
-    "The time the mission ends"
     start_string: Optional[str] = None
     "Short-time-formatted duration string representing the start of the alert"
+
     active: Optional[bool] = None
     "Whether the alert is still active or not"
+
     eta: Optional[str] = None
     "Short-formatted string estimating the time until the Alert is closed"
+
+    expired: Optional[bool] = None
+    "Whether the mission is expired or not"
```

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/arbitration.py` & `warframe.py-0.3.2/warframe/worldstate/models/arbitration.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/archon_hunt.py` & `warframe.py-0.3.2/warframe/worldstate/models/archon_hunt.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/cetus.py` & `warframe.py-0.3.2/warframe/worldstate/models/cetus.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/daily_deal.py` & `warframe.py-0.3.2/warframe/worldstate/models/daily_deal.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/event.py` & `warframe.py-0.3.2/warframe/worldstate/models/event.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/fissure.py` & `warframe.py-0.3.2/warframe/worldstate/models/fissure.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/flash_sale.py` & `warframe.py-0.3.2/warframe/worldstate/models/flash_sale.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/invasion.py` & `warframe.py-0.3.2/warframe/worldstate/models/invasion.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/mission.py` & `warframe.py-0.3.2/warframe/worldstate/models/mission.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,41 +6,58 @@
 
 __all__ = ["Mission"]
 
 
 class Mission(SingleQueryModel):
     # required
     reward: Reward
+
     "The mission's reward"
+
     node: str
     "The localized node string"
+
     faction: Faction
     "The faction that houses the node/mission"
-    max_enemy_level: int
-    min_enemy_level: int
-    max_wave_num: int
+
     type: MissionType
     "The MissionType of the given mission (Capture, Spy, etc.)"
+
     nightmare: bool
     "Whether the mission is a nightmare mission"
+
     archwing_required: bool
     "Whether an archwing is required in order to play the mission"
+
     description: str
     "The mission's description"
 
     # optional
+    max_enemy_level: Optional[int] = None
+
+    min_enemy_level: Optional[int] = None
+
+    max_wave_num: Optional[int] = None
+
     is_sharkwing: Optional[bool] = None
     "Whether the mission takes place in a submerssible mission"
+
     enemy_spec: Optional[str] = None
     "Enemy specification for the mission"
+
     level_override: Optional[str] = None
     "Override for the map on this mission"
+
     advanced_spawners: Optional[List[str]] = None
     "Array of strings denoting extra spawners for a mission"
+
     required_items: Optional[List[str]] = None
     "Items required to enter the mission"
+
     consume_required_items: Optional[bool] = None
     "Whether the required items are consumed"
+
     leaders_always_allowed: Optional[bool] = None
     "Whether leaders are always allowed"
+
     level_auras: Optional[List[str]] = None
     "Affectors for this mission"
```

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/orb_vallis.py` & `warframe.py-0.3.2/warframe/worldstate/models/orb_vallis.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/reward.py` & `warframe.py-0.3.2/warframe/worldstate/models/reward.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/sortie.py` & `warframe.py-0.3.2/warframe/worldstate/models/sortie.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe/worldstate/models/void_trader.py` & `warframe.py-0.3.2/warframe/worldstate/models/void_trader.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.1/warframe.py.egg-info/PKG-INFO` & `warframe.py-0.3.2/warframe.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.1
+Version: 0.3.2
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.1/warframe.py.egg-info/SOURCES.txt` & `warframe.py-0.3.2/warframe.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/warframe.py-0.3.0.tar.gz` & `tmp/warframe.py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warframe.py-0.3.0.tar", last modified: Sat Jun 10 03:52:11 2023, max compression
+gzip compressed data, was "warframe.py-0.3.1.tar", last modified: Sat Jun 10 12:12:08 2023, max compression
```

## Comparing `warframe.py-0.3.0.tar` & `warframe.py-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:52:11.046097 warframe.py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-10 03:51:37.000000 warframe.py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 03:52:11.046097 warframe.py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-10 03:51:37.000000 warframe.py-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 03:51:37.000000 warframe.py-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 03:52:11.046097 warframe.py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-10 03:51:37.000000 warframe.py-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:52:11.042097 warframe.py-0.3.0/warframe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:52:11.046097 warframe.py-0.3.0/warframe/worldstate/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:52:11.046097 warframe.py-0.3.0/warframe/worldstate/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/common/base_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/common/types_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:52:11.046097 warframe.py-0.3.0/warframe/worldstate/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/enums/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/enums/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/enums/mission_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/enums/syndicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:52:11.046097 warframe.py-0.3.0/warframe/worldstate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/archon_hunt.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/cambion_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/cetus.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/counted_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/daily_deal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/fissure.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/flash_sale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/invasion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/orb_vallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/sortie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/models/void_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 03:51:37.000000 warframe.py-0.3.0/warframe/worldstate/worldstate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:52:11.042097 warframe.py-0.3.0/warframe.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 03:52:10.000000 warframe.py-0.3.0/warframe.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-10 03:52:11.000000 warframe.py-0.3.0/warframe.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:52:10.000000 warframe.py-0.3.0/warframe.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 03:52:10.000000 warframe.py-0.3.0/warframe.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 03:52:10.000000 warframe.py-0.3.0/warframe.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.720237 warframe.py-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-10 12:11:25.000000 warframe.py-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 12:12:08.720237 warframe.py-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-10 12:11:25.000000 warframe.py-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-10 12:11:25.000000 warframe.py-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 12:12:08.720237 warframe.py-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-10 12:11:25.000000 warframe.py-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/worldstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/worldstate/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/common/base_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/common/types_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe/worldstate/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/mission_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/enums/syndicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.720237 warframe.py-0.3.1/warframe/worldstate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/archon_hunt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/cambion_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/cetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/counted_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/daily_deal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/fissure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/flash_sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/invasion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/orb_vallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/sortie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/models/void_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 12:11:25.000000 warframe.py-0.3.1/warframe/worldstate/worldstate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:08.716237 warframe.py-0.3.1/warframe.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 12:12:08.000000 warframe.py-0.3.1/warframe.py.egg-info/top_level.txt
```

### Comparing `warframe.py-0.3.0/LICENSE` & `warframe.py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/PKG-INFO` & `warframe.py-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.0
+Version: 0.3.1
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.0/README.rst` & `warframe.py-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/setup.py` & `warframe.py-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/client.py` & `warframe.py-0.3.1/warframe/worldstate/client.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/common/base_objects.py` & `warframe.py-0.3.1/warframe/worldstate/common/base_objects.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/common/types_.py` & `warframe.py-0.3.1/warframe/worldstate/common/types_.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/endpoints.py` & `warframe.py-0.3.1/warframe/worldstate/endpoints.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/enums/mission_type.py` & `warframe.py-0.3.1/warframe/worldstate/enums/mission_type.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/exceptions.py` & `warframe.py-0.3.1/warframe/worldstate/exceptions.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/alert.py` & `warframe.py-0.3.1/warframe/worldstate/models/alert.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/arbitration.py` & `warframe.py-0.3.1/warframe/worldstate/models/arbitration.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/archon_hunt.py` & `warframe.py-0.3.1/warframe/worldstate/models/archon_hunt.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/event.py` & `warframe.py-0.3.1/warframe/worldstate/models/event.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/fissure.py` & `warframe.py-0.3.1/warframe/worldstate/models/fissure.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/invasion.py` & `warframe.py-0.3.1/warframe/worldstate/models/invasion.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/mission.py` & `warframe.py-0.3.1/warframe/worldstate/models/mission.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/reward.py` & `warframe.py-0.3.1/warframe/worldstate/models/reward.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,25 @@
 __all__ = ["Reward"]
 
 
 class Reward(SingleQueryModel):
     # required
     counted_items: List[CountedItem]
     "Items that have a quantity attached"
+
     thumbnail: str
     "Thumbnail URL"
+
     color: int
     "RGB value as an int assigned to this reward"
+
     credits: int
     "Amount of credits awarded"
+
     as_string: str
     "String representation of the reward"
+
     items: List[str]
     "Items' names possible to be won"
+
     item_string: str
     "formatted string describing all included items"
```

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/sortie.py` & `warframe.py-0.3.1/warframe/worldstate/models/sortie.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,43 +8,50 @@
 
 __all__ = ["Sortie"]
 
 
 class SortieMission(SingleQueryModel):
     node: str
     "The node the mission is on"
+
     type: MissionType = field(name="missionType")
     "The Type of the mission"
+
     modifier: str
     "The modifier applied to the mission"
+
     modifier_description: str
     "The description of the modifier"
 
 
 class Sortie(SingleQueryModel):
     __endpoint__ = "/sortie"
 
     # required
-
     boss: str
     "The boss you're up against"
+
     activation: datetime
     "The time the Sortie started"
+
     expiry: datetime
     "The time the Sortie ends"
+
     missions: List[SortieMission] = field(name="variants")
     "The 3 missions you have to play in order to get the reward"
+
     faction: Faction
     "The Faction you're up against"
+
     expired: bool
     "Whether the Sortie is still active"
+
     eta: str
     "Short-formatted string estimating the time until the Sortie ends"
 
     # optional
-
     start_string: Optional[str] = None
     "Short-time-formatted duration string of the start of the Fissure"
 
     @property
     def active(self):
         return not self.expired
```

### Comparing `warframe.py-0.3.0/warframe/worldstate/models/void_trader.py` & `warframe.py-0.3.1/warframe/worldstate/models/void_trader.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,34 +7,40 @@
 
 __all__ = ["VoidTrader"]
 
 
 class InventoryItem(WorldstateObject):
     item: str
     "The item that is being sold"
+
     ducats: int
     "The cost of ducats"
+
     credits: int
     "The cost of credits"
 
 
 class VoidTrader(SingleQueryModel):
     __endpoint__ = "/voidTrader"
 
     # required
-
     start_string: str
     "Short-time-formatted duration string of the arrival of the Void Trader"
+
     active: bool
     "Whether the Void Trader is currently active"
+
     location: str
     "The Relay on which the Void Trader is on"
+
     inventory: List[InventoryItem]
     "The Void Trader's inventory"
+
     end_string: str
     "Short-time-formatted duration string of the department of the Void Trader"
 
     # optional
     arrival: Optional[datetime] = field(name="activation", default=None)
     "The time the Void Trader arrived"
+
     department: Optional[datetime] = field(name="expiry", default=None)
     "The time the Void Trader departs"
```

### Comparing `warframe.py-0.3.0/warframe.py.egg-info/PKG-INFO` & `warframe.py-0.3.1/warframe.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.0
+Version: 0.3.1
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.0/warframe.py.egg-info/SOURCES.txt` & `warframe.py-0.3.1/warframe.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*


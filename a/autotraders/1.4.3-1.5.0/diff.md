# Comparing `tmp/autotraders-1.4.3.tar.gz` & `tmp/autotraders-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.4.3.tar", last modified: Wed Jun  7 02:59:56 2023, max compression
+gzip compressed data, was "autotraders-1.5.0.tar", last modified: Sat Jun 10 20:06:40 2023, max compression
```

## Comparing `autotraders-1.4.3.tar` & `autotraders-1.5.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.004780 autotraders-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 02:59:41.000000 autotraders-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:59:56.004780 autotraders-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 02:59:41.000000 autotraders-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 02:59:41.000000 autotraders-1.4.3/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.000780 autotraders-1.4.3/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 02:59:55.000000 autotraders-1.4.3/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 02:59:41.000000 autotraders-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 02:59:56.004780 autotraders-1.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:59:56.004780 autotraders-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 02:59:41.000000 autotraders-1.4.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-10 20:06:28.000000 autotraders-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-10 20:06:40.950999 autotraders-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-10 20:06:28.000000 autotraders-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-10 20:06:28.000000 autotraders-1.5.0/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.946999 autotraders-1.5.0/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 20:06:40.000000 autotraders-1.5.0/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-10 20:06:28.000000 autotraders-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 20:06:40.950999 autotraders-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 20:06:40.950999 autotraders-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-10 20:06:28.000000 autotraders-1.5.0/tests/test_util.py
```

### Comparing `autotraders-1.4.3/LICENSE` & `autotraders-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/PKG-INFO` & `autotraders-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.4.3
+Version: 1.5.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.4.3/README.md` & `autotraders-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/agent.py` & `autotraders-1.5.0/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/faction/__init__.py` & `autotraders-1.5.0/autotraders/faction/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional
-
 from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.shared_models.trait import Trait
 
 
 class Faction(SpaceTradersEntity):
+    is_recruiting: bool
+    traits: list[Trait]
+    headquarters: MapSymbol
+    description: str
+    name: str
+    symbol: str
+
     def __init__(self, symbol, session: AutoTradersSession, data=None):
-        self.is_recruiting: Optional[bool] = None
-        self.traits: Optional[list[Trait]] = None
-        self.headquarters: Optional[MapSymbol] = None
-        self.description: Optional[str] = None
-        self.name: Optional[str] = None
         self.symbol: str = symbol
         super().__init__(session, "factions/" + self.symbol, data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.name = data["name"]
```

### Comparing `autotraders-1.4.3/autotraders/faction/contract.py` & `autotraders-1.5.0/autotraders/faction/contract.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from datetime import datetime
 from typing import Optional
 
 from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.util import parse_time
+from autotraders.time import parse_time
 
 
 class Deliver:
     def __init__(self, data):
         self.trade_symbol = MapSymbol(data["tradeSymbol"])
         self.destination_symbol = MapSymbol(data["destinationSymbol"])
         self.units_required = data["unitsRequired"]
         self.units_fulfilled = data["unitsFulfilled"]
 
 
 class Contract(SpaceTradersEntity):
+    accepted: bool
+    fulfilled: bool
+    deadline: datetime
+    accept_deadline: datetime
+    on_fulfilled: str
+    on_accepted: str
+    contract_id: str
+
     def __init__(self, contract_id: str, session: AutoTradersSession, data=None):
         self.contract_data = None
-        self.accepted: Optional[bool] = None
-        self.fulfilled: Optional[bool] = None
-        self.deadline: Optional[datetime] = None
-        self.accept_deadline: Optional[datetime] = None
         self.contract_type = None
-        self.on_fulfilled: Optional[str] = None
-        self.on_accepted: Optional[str] = None
         self.contract_id: str = contract_id
         super().__init__(session, "my/contracts/" + self.contract_id, data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.on_accepted = data["terms"]["payment"]["onAccepted"]
```

### Comparing `autotraders-1.4.3/autotraders/map/system.py` & `autotraders-1.5.0/autotraders/map/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,20 +37,20 @@
             r = session.get(
                 session.base_url
                 + "systems?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
-            j = r.json()["data"]
+            j = r.json()
             if "error" in j:
                 raise IOError(j["error"]["message"])
             systems = []
-            for system in j:
+            for system in j["data"]:
                 s = System(system["symbol"], session, system)
                 systems.append(s)
-            return systems, r.json()["meta"]["total"]
+            return systems, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
```

### Comparing `autotraders-1.4.3/autotraders/map/waypoint.py` & `autotraders-1.5.0/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.5.0/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.5.0/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.5.0/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.5.0/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/paginated_list.py` & `autotraders-1.5.0/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/session.py` & `autotraders-1.5.0/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/shared_models/map_symbol.py` & `autotraders-1.5.0/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/shared_models/transaction.py` & `autotraders-1.5.0/autotraders/shared_models/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from autotraders.shared_models.item import Item
 from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.util import parse_time
+from autotraders.time import parse_time
 
 
 class ShipyardTransaction:
     def __init__(self, data):
         self.credits = data["price"]
         self.waypoint_symbol = MapSymbol(data["waypointSymbol"])
         self.ship_symbol = data["shipSymbol"]
```

### Comparing `autotraders-1.4.3/autotraders/ship/__init__.py` & `autotraders-1.5.0/autotraders/ship/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from autotraders.ship.nav import Nav
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
 from autotraders.ship.survey import Survey
-from autotraders.util import parse_time
+from autotraders.time import parse_time
 from autotraders.map.waypoint import Waypoint
 
 
 class Fuel:
     def __init__(self, current, total):
         self.current = current
         self.total = total
@@ -38,27 +38,40 @@
 class Registration:
     def __init__(self, data):
         self.name = data["name"]
         self.faction_symbol = data["factionSymbol"]
         self.role = data["role"]
 
 
+class Capabilities:
+    def __init__(self, modules, mounts):
+        warp_drives = [module for module in modules if "warp" in module.symbol.lower()]
+        jump_drives = [module for module in modules if "jump" in module.symbol.lower()]
+        mine = [mount for mount in mounts if "mine" in mount.symbol.lower()]
+        self.warp = len(warp_drives) > 0
+        self.jump = len(jump_drives) > 0
+        self.mine = len(mine) > 0
+
+
 class Ship(SpaceTradersEntity):
+    cargo: Cargo
+    fuel: Fuel
+    nav: Nav
+    symbol: str
+    frame: Frame
+    reactor: Reactor
+    engine: Engine
+    modules: list[Module]
+    mounts: list[Mount]
+    crew: Crew
+    registration: Registration
+    capabilities: Optional[Capabilities]
+
     def __init__(self, symbol, session: AutoTradersSession, data=None):
-        self.cargo: Optional[Cargo] = None
-        self.fuel: Optional[Fuel] = None
-        self.nav: Optional[Nav] = None
-        self.symbol: str = symbol
-        self.frame: Optional[Frame] = None
-        self.reactor: Optional[Reactor] = None
-        self.engine: Optional[Engine] = None
-        self.modules: Optional[list[Module]] = None
-        self.mounts: Optional[list[Mount]] = None
-        self.crew: Optional[Crew] = None
-        self.registration: Optional[Registration] = None
+        self.symbol = symbol
         super().__init__(session, "my/ships/" + self.symbol, data)
 
     def update(self, data: dict = None) -> None:
         if data is None:
             data = self.get()["data"]
 
         if "crew" in data:
@@ -77,14 +90,18 @@
             self.nav = Nav(self.symbol, self.session, data["nav"])
         if "fuel" in data:
             self.fuel = Fuel(data["fuel"]["current"], data["fuel"]["capacity"])
         if "cargo" in data:
             self.cargo = Cargo(self.symbol, self.session, data["cargo"])
         if "registration" in data:
             self.registration = Registration(data["registration"])
+        try:
+            self.capabilities = Capabilities(self.modules, self.mounts)
+        except:
+            pass
 
     async def navigate_async(self, waypoint: Union[str, MapSymbol], interval=1):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function waits for the ship to arrive.
         :param interval: Frequency of updates in seconds (default: 1)
         """
         j = self.post("navigate", data={"waypointSymbol": str(waypoint)})
```

### Comparing `autotraders-1.4.3/autotraders/ship/cargo.py` & `autotraders-1.5.0/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/ship/nav.py` & `autotraders-1.5.0/autotraders/ship/nav.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, timezone
 from typing import Optional
 
 from autotraders import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
-from autotraders.util import parse_time
+from autotraders.time import parse_time
 
 
 class Route:
     def __init__(self, data):
         self.destination = MapSymbol(data["destination"]["symbol"])
         self.departure = MapSymbol(data["departure"]["symbol"])
         self.departure_time = parse_time(data["departureTime"])
```

### Comparing `autotraders-1.4.3/autotraders/ship/ship_components.py` & `autotraders-1.5.0/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/space_traders_entity.py` & `autotraders-1.5.0/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/autotraders/status.py` & `autotraders-1.5.0/autotraders/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 import requests
 
-from autotraders.util import parse_time
+from autotraders.time import parse_time
 
 
 class LeaderboardPlayer:
     symbol: str
     value: int
```

### Comparing `autotraders-1.4.3/autotraders.egg-info/PKG-INFO` & `autotraders-1.5.0/autotraders.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.4.3
+Version: 1.5.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.4.3/autotraders.egg-info/SOURCES.txt` & `autotraders-1.5.0/autotraders.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 autotraders/__init__.py
 autotraders/agent.py
 autotraders/paginated_list.py
 autotraders/session.py
 autotraders/space_traders_entity.py
 autotraders/status.py
+autotraders/time.py
 autotraders/util.py
 autotraders.egg-info/PKG-INFO
 autotraders.egg-info/SOURCES.txt
 autotraders.egg-info/dependency_links.txt
 autotraders.egg-info/requires.txt
 autotraders.egg-info/top_level.txt
 autotraders/faction/__init__.py
@@ -26,12 +27,13 @@
 autotraders/shared_models/map_symbol.py
 autotraders/shared_models/trait.py
 autotraders/shared_models/transaction.py
 autotraders/ship/__init__.py
 autotraders/ship/cargo.py
 autotraders/ship/nav.py
 autotraders/ship/ship_components.py
+autotraders/ship/states.py
 autotraders/ship/survey.py
 tests/test_contract.py
 tests/test_init.py
 tests/test_ship.py
 tests/test_util.py
```

### Comparing `autotraders-1.4.3/pyproject.toml` & `autotraders-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.4.3"
+version = "1.5.0"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.4.3/tests/test_init.py` & `autotraders-1.5.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/tests/test_ship.py` & `autotraders-1.5.0/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.4.3/tests/test_util.py` & `autotraders-1.5.0/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.util import parse_time
+from autotraders.time import parse_time
 
 
 def test_time_parser():
     assert parse_time("2023-05-21T00:07:07.475Z").year == 2023
     assert parse_time("2023-05-21T00:07:07.475Z").month == 5
     assert parse_time("2023-05-21T00:07:07.475Z").day == 21
     assert parse_time("2023-05-21T00:07:07.475Z").hour == 0
```


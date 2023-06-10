# Comparing `tmp/adsbcot-5.1.2.tar.gz` & `tmp/adsbcot-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsbcot-5.1.2.tar", last modified: Thu Jan 19 22:44:28 2023, max compression
+gzip compressed data, was "adsbcot-6.0.0.tar", last modified: Sat Jun 10 03:17:47 2023, max compression
```

## Comparing `adsbcot-5.1.2.tar` & `adsbcot-6.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:44:28.746707 adsbcot-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-19 22:44:18.000000 adsbcot-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-19 22:44:18.000000 adsbcot-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-01-19 22:44:28.746707 adsbcot-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-01-19 22:44:18.000000 adsbcot-5.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:44:28.746707 adsbcot-5.1.2/adsbcot/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-19 22:44:18.000000 adsbcot-5.1.2/adsbcot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-01-19 22:44:18.000000 adsbcot-5.1.2/adsbcot/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-01-19 22:44:18.000000 adsbcot-5.1.2/adsbcot/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-01-19 22:44:18.000000 adsbcot-5.1.2/adsbcot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-01-19 22:44:18.000000 adsbcot-5.1.2/adsbcot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:44:28.746707 adsbcot-5.1.2/adsbcot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-01-19 22:44:28.000000 adsbcot-5.1.2/adsbcot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-19 22:44:28.000000 adsbcot-5.1.2/adsbcot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:44:28.000000 adsbcot-5.1.2/adsbcot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-19 22:44:28.000000 adsbcot-5.1.2/adsbcot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:44:28.000000 adsbcot-5.1.2/adsbcot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-19 22:44:28.000000 adsbcot-5.1.2/adsbcot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-19 22:44:28.000000 adsbcot-5.1.2/adsbcot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-19 22:44:28.750707 adsbcot-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-19 22:44:18.000000 adsbcot-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:17:47.043357 adsbcot-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-10 03:17:36.000000 adsbcot-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 03:17:36.000000 adsbcot-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-10 03:17:47.043357 adsbcot-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-10 03:17:36.000000 adsbcot-6.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:17:47.039357 adsbcot-6.0.0/adsbcot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-10 03:17:36.000000 adsbcot-6.0.0/adsbcot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:17:47.043357 adsbcot-6.0.0/adsbcot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-10 03:17:47.000000 adsbcot-6.0.0/adsbcot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 03:17:46.000000 adsbcot-6.0.0/adsbcot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-10 03:17:47.043357 adsbcot-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-10 03:17:36.000000 adsbcot-6.0.0/setup.py
```

### Comparing `adsbcot-5.1.2/LICENSE` & `adsbcot-6.0.0/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 Greg Albrecht <oss@undef.net>
+Copyright 2023 Sensors & Signals LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
```

### Comparing `adsbcot-5.1.2/adsbcot/commands.py` & `adsbcot-6.0.0/adsbcot/commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
+# Author:: Greg Albrecht <gba@snstac.com>
 #
 
 """PyTAK Command Line."""
 
 import pytak
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
 def main() -> None:
     """Boilerplate main func."""
     # PyTAK CLI tool boilerplate:
     pytak.cli(__name__.split(".", maxsplit=1)[0])
```

### Comparing `adsbcot-5.1.2/adsbcot/constants.py` & `adsbcot-6.0.0/adsbcot/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """ADSBCOT Constants."""
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
-# Dump1090 URL to use out of the box, in this case the HTTP JSON feed URL.
-DEFAULT_DUMP1090_URL: str = "http://piaware.local:8080/data/aircraft.json"
+# Feed URL to use out of the box, in this case the JSON from the local filesystem.
+DEFAULT_FEED_URL: str = "file:///run/dump1090-fa/aircraft.json"
 
-# Default dump1090 HTTP JSON feed polling interval, in seconds.
+# Default HTTP JSON feed polling interval, in seconds.
 DEFAULT_POLL_INTERVAL: str = "3"
 
-# Default non-HTTP TCP ports for dump1090, raw & beast.
-DEFAULT_DUMP1090_TCP_RAW_PORT: int = 30002
-DEFAULT_DUMP1090_TCP_BEAST_PORT: int = 30005
+# Default non-HTTP TCP ports for raw & beast.
+DEFAULT_TCP_RAW_PORT: int = 30002
+DEFAULT_TCP_BEAST_PORT: int = 30005
```

### Comparing `adsbcot-5.1.2/adsbcot/functions.py` & `adsbcot-6.0.0/adsbcot/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """ADSBCOT Functions."""
 
 import asyncio
+import importlib.util
 import warnings
-import xml.etree.ElementTree as ET
+import xml.etree.ElementTree as etree
 
 from configparser import SectionProxy
-from typing import Union, Set
+from typing import Optional, Set, Union
 from urllib.parse import ParseResult, urlparse
 
 import aircot
 import pytak
 import adsbcot
 
-
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
 APP_NAME = "adsbcot"
 
 # We won't use pyModeS if it isn't installed:
-WITH_PYMODES = False
 try:
     import pyModeS  # NOQA pylint: disable=unused-import
-
-    WITH_PYMODES = True
 except ImportError:
     pass
 
 
 def create_tasks(
     config: SectionProxy, clitool: pytak.CLITool
 ) -> Set[pytak.Worker,]:
@@ -63,58 +58,58 @@
     Returns
     -------
     `set`
         Set of PyTAK Worker classes for this application.
     """
     tasks = set()
 
-    _dump1090_url: str = config.get("DUMP1090_URL", adsbcot.DEFAULT_DUMP1090_URL)
-    config.setdefault("DUMP1090_URL", _dump1090_url)
-    _dump1090_url = config.get("DUMP1090_URL", "")
-
-    if "://" not in _dump1090_url:
-        warnings.warn(f"Invalid DUMP1090_URL: '{_dump1090_url}'", SyntaxWarning)
-        raise Exception(
-            "Please specify DUMP1090_URL with full URL, including '://', for "
+    _feed_url: str = config.get("FEED_URL", adsbcot.DEFAULT_FEED_URL)
+    config.setdefault("FEED_URL", _feed_url)
+    _feed_url = config.get("FEED_URL", "")
+
+    if "://" not in _feed_url:
+        warnings.warn(f"Invalid FEED_URL: '{_feed_url}'", SyntaxWarning)
+        raise ValueError(
+            "Please specify FEED_URL with full URL, including '://', for "
             "example: tcp+beast://example.com:30005"
         )
 
     # Gateway code:
-    dump1090_url: ParseResult = urlparse(config.get("DUMP1090_URL"))
+    feed_url: ParseResult = urlparse(config.get("FEED_URL"))
 
     # ADS-B Workers (receivers):
-    if "http" in dump1090_url.scheme:
+    if feed_url.scheme in ["http", "file"]:
         tasks.add(adsbcot.ADSBWorker(clitool.tx_queue, config))
-    elif "tcp" in dump1090_url.scheme:
-        if not WITH_PYMODES:
+    elif "tcp" in feed_url.scheme:
+        if importlib.util.find_spec("pyModeS") is None:
             warnings.warn(
                 (f"Please reinstall {APP_NAME} with pyModeS support:"
                  f"$ python3 -m pip install {APP_NAME}[with_pymodes]"), 
                  ImportWarning)
-            raise Exception
+            raise ValueError
 
         net_queue: asyncio.Queue = asyncio.Queue()
 
-        if "+" in dump1090_url.scheme:
-            _, data_type = dump1090_url.scheme.split("+")
+        if "+" in feed_url.scheme:
+            _, data_type = feed_url.scheme.split("+")
         else:
             data_type = "raw"
 
         tasks.add(adsbcot.ADSBNetReceiver(net_queue, config, data_type))
 
         tasks.add(adsbcot.ADSBNetWorker(clitool.tx_queue, net_queue, config, data_type))
 
     return tasks
 
 
 def adsb_to_cot_xml(  # NOQA pylint: disable=too-many-locals,too-many-branches,too-many-statements
     craft: dict,
-    config: Union[SectionProxy, None] = None,
-    known_craft: Union[dict, None] = None,
-) -> Union[ET.Element, None]:
+    config: Union[SectionProxy, dict, None] = None,
+    known_craft: Optional[dict] = None,
+) -> Optional[etree.Element]:
     """Serialize a Dump1090 ADS-B aircraft object as Cursor on Target XML.
 
     Parameters
     ----------
     craft : `dict`
         Key/Value data struct of decoded ADS-B aircraft data.
     config : `configparser.SectionProxy`
@@ -128,56 +123,58 @@
     """
     lat = craft.get("lat")
     lon = craft.get("lon")
 
     if lat is None or lon is None:
         return None
 
-    known_craft: dict = known_craft or {}
-    config: dict = config or {}
-    remarks_fields = []
-
-    uid_key = config.get("UID_KEY", "ICAO")
-    cot_stale = int(config.get("COT_STALE", pytak.DEFAULT_COT_STALE))
-    cot_host_id = config.get("COT_HOST_ID", pytak.DEFAULT_HOST_ID)
+    known_craft = known_craft or {}
+    config = config or {}
 
-    aircotx = ET.Element("_aircot_")
+    remarks_fields: list = []
+
+    uid_key: str = config.get("UID_KEY", "ICAO")
+    cot_stale: int = int(config.get("COT_STALE", pytak.DEFAULT_COT_STALE))
+    cot_host_id: str = config.get("COT_HOST_ID", pytak.DEFAULT_HOST_ID)
+
+    aircotx = etree.Element("_aircot_")
     aircotx.set("cot_host_id", cot_host_id)
 
-    icao_hex = craft.get("hex", "")
-    reg = craft.get("reg", "")
-    flight = craft.get("flight", "")
-    cat = craft.get("category")
-    squawk = craft.get("squawk")
+    icao_hex: str = str(craft.get("hex", craft.get("icao", ""))).strip().upper()
+    reg: str = str(craft.get("reg", craft.get("r", ""))).strip().upper()
+    flight: str = str(craft.get("flight", "")).strip().upper()
+    cat: str = str(craft.get("category", "")).strip().upper()
+    squawk: str = str(craft.get("squawk", "")).strip().upper()
+    craft_type: str = str(craft.get("t", "")).strip().upper()
 
     if flight:
-        flight = flight.strip().upper()
         remarks_fields.append(flight)
         aircotx.set("flight", flight)
 
     if reg:
-        reg = reg.strip().upper()
         remarks_fields.append(reg)
         aircotx.set("reg", reg)
 
     if squawk:
-        squawk = squawk.strip().upper()
         remarks_fields.append(f"Squawk: {squawk}")
         aircotx.set("squawk", squawk)
 
     if icao_hex:
-        icao_hex = icao_hex.strip().upper()
         remarks_fields.append(icao_hex)
         aircotx.set("icao", icao_hex)
 
     if cat:
-        cat = cat.strip().upper()
         remarks_fields.append(f"Cat.: {cat}")
         aircotx.set("cat", cat)
 
+    if craft_type:
+        remarks_fields.append(f"Type:{craft_type}")
+        aircotx.set("type", craft_type)
+
+    cot_uid: str = ""
     if "REG" in uid_key and reg:
         cot_uid = f"REG-{reg}"
     elif "ICAO" in uid_key and icao_hex:
         cot_uid = f"ICAO-{icao_hex}"
     if "FLIGHT" in uid_key and flight:
         cot_uid = f"FLIGHT-{flight}"
     elif icao_hex:
@@ -190,82 +187,70 @@
     if flight:
         callsign = flight
     elif reg:
         callsign = reg
     else:
         callsign = icao_hex
 
-    _, callsign = aircot.set_name_callsign(icao_hex, reg, None, flight, known_craft)
+    _, callsign = aircot.set_name_callsign(icao_hex, reg, craft_type, flight, known_craft)
     cat = aircot.set_category(cat, known_craft)
     cot_type = aircot.set_cot_type(icao_hex, cat, flight, known_craft)
 
-    point: ET.Element = ET.Element("point")
+    point: etree.Element = etree.Element("point")
     point.set("lat", str(lat))
     point.set("lon", str(lon))
     point.set("ce", str(craft.get("nac_p", "9999999.0")))
     point.set("le", str(craft.get("nac_v", "9999999.0")))
+    point.set("hae", aircot.functions.get_hae(craft.get("alt_geom")))
 
-    # alt_geom: geometric (GNSS / INS) altitude in feet referenced to the
-    #           WGS84 ellipsoid
-    alt_geom = int(craft.get("alt_geom", 0))
-    if alt_geom:
-        point.set("hae", str(alt_geom * 0.3048))
-    else:
-        point.set("hae", "9999999.0")
-
-    uid: ET.Element = ET.Element("UID")
-    uid.set("Droid", cot_uid)
-
-    contact: ET.Element = ET.Element("contact")
+    contact: etree.Element = etree.Element("contact")
     contact.set("callsign", callsign)
 
-    track: ET.Element = ET.Element("track")
+    track: etree.Element = etree.Element("track")
     track.set("course", str(craft.get("trk", craft.get("track", "9999999.0"))))
+    track.set("speed", aircot.functions.get_speed(craft.get("gs")))
 
-    # gs: ground speed in knots
-    gnds = int(craft.get("gs", 0))
-    if gnds:
-        track.set("speed", str(gnds * 0.514444))
-    else:
-        track.set("speed", "9999999.0")
-
-    detail = ET.Element("detail")
-    detail.set("uid", cot_uid)
-    detail.append(uid)
+    detail = etree.Element("detail")
     detail.append(contact)
     detail.append(track)
 
-    remarks = ET.Element("remarks")
+    icon = known_craft.get("ICON")
+    if icon:
+        usericon = etree.Element("usericon")
+        usericon.set("iconsetpath", icon)
+        detail.append(usericon)
+
+    remarks = etree.Element("remarks")
 
     remarks_fields.append(f"{cot_host_id}")
 
     _remarks = " ".join(list(filter(None, remarks_fields)))
 
     remarks.text = _remarks
     detail.append(remarks)
+    detail.append(aircotx)
 
-    root = ET.Element("event")
+    root = etree.Element("event")
     root.set("version", "2.0")
     root.set("type", cot_type)
     root.set("uid", cot_uid)
     root.set("how", "m-g")
     root.set("time", pytak.cot_time())
     root.set("start", pytak.cot_time())
     root.set("stale", pytak.cot_time(cot_stale))
 
     root.append(point)
     root.append(detail)
-    root.append(aircotx)
 
     return root
 
 
 def adsb_to_cot(
     craft: dict,
-    config: Union[SectionProxy, None] = None,
-    known_craft: Union[dict, None] = None,
-) -> Union[bytes, None]:
+    config: Union[SectionProxy, dict, None] = None,
+    known_craft: Optional[dict] = None,
+) -> Optional[bytes]:
     """Return CoT XML object as an XML string."""
-    cot: Union[ET.Element, None] = adsb_to_cot_xml(craft, config, known_craft)
+    cot: Optional[etree.Element] = adsb_to_cot_xml(craft, config, known_craft)
     return (
-        b"\n".join([pytak.DEFAULT_XML_DECLARATION, ET.tostring(cot)]) if cot else None
+        b"\n".join([pytak.DEFAULT_XML_DECLARATION, etree.tostring(cot)]) if cot else None
     )
```


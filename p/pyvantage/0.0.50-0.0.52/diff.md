# Comparing `tmp/pyvantage-0.0.50.tar.gz` & `tmp/pyvantage-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvantage-0.0.50.tar", last modified: Sun May 14 06:46:09 2023, max compression
+gzip compressed data, was "pyvantage-0.0.52.tar", last modified: Sat Jun 10 21:07:00 2023, max compression
```

## Comparing `pyvantage-0.0.50.tar` & `pyvantage-0.0.52.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:46:09.270359 pyvantage-0.0.50/
--rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.50/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 06:46:09.270479 pyvantage-0.0.50/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.50/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:46:09.267681 pyvantage-0.0.50/pyvantage/
--rw-r--r--   0 greg       (501) staff       (20)   100189 2023-05-14 06:44:28.000000 pyvantage-0.0.50/pyvantage/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:46:09.269732 pyvantage-0.0.50/pyvantage.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      218 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.50/pyvantage.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2023-05-14 06:46:09.270937 pyvantage-0.0.50/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      769 2023-05-14 06:44:58.000000 pyvantage-0.0.50/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 21:07:00.890995 pyvantage-0.0.52/
+-rw-r--r--   0 greg       (501) staff       (20)     1179 2021-06-03 17:37:04.000000 pyvantage-0.0.52/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-06-10 21:07:00.891090 pyvantage-0.0.52/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     2164 2023-04-23 17:44:30.000000 pyvantage-0.0.52/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 21:07:00.887921 pyvantage-0.0.52/pyvantage/
+-rw-r--r--   0 greg       (501) staff       (20)   103182 2023-06-10 21:04:47.000000 pyvantage-0.0.52/pyvantage/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-06-10 21:07:00.890344 pyvantage-0.0.52/pyvantage.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      218 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       10 2023-06-10 21:07:00.000000 pyvantage-0.0.52/pyvantage.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-23 18:11:37.000000 pyvantage-0.0.52/pyvantage.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-06-10 21:07:00.891452 pyvantage-0.0.52/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      769 2023-06-10 20:46:11.000000 pyvantage-0.0.52/setup.py
```

### Comparing `pyvantage-0.0.50/LICENSE` & `pyvantage-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.50/PKG-INFO` & `pyvantage-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.50
+Version: 0.0.52
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.50/README.md` & `pyvantage-0.0.52/README.md`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.50/pyvantage/__init__.py` & `pyvantage-0.0.52/pyvantage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 import threading
 import time
 import base64
 import re
 import json
 import os
 import traceback
+import math
 
 from collections import deque
 from xml.sax.saxutils import escape
 
 from colorsys import hsv_to_rgb, rgb_to_hsv
 from xml.etree import ElementTree as ET
 
@@ -147,14 +148,73 @@
 
 def level_to_mireds(level):
     """Convert a level to mired color temperature."""
     kelvin = level_to_kelvin(level)
     mireds = 1000000/kelvin
     return mireds
 
+def kelvin_to_rgb(colour_temperature):
+    """
+    Converts from K to RGB, algorithm courtesy of
+    http://www.tannerhelland.com/4435/convert-temperature-rgb-algorithm-code/
+    """
+    #range check
+    if colour_temperature < 1000:
+        colour_temperature = 1000
+    elif colour_temperature > 40000:
+        colour_temperature = 40000
+
+    tmp_internal = colour_temperature / 100.0
+
+    # red
+    if tmp_internal <= 66:
+        red = 255
+    else:
+        tmp_red = 329.698727446 * math.pow(tmp_internal - 60, -0.1332047592)
+        if tmp_red < 0:
+            red = 0
+        elif tmp_red > 255:
+            red = 255
+        else:
+            red = tmp_red
+
+    # green
+    if tmp_internal <=66:
+        tmp_green = 99.4708025861 * math.log(tmp_internal) - 161.1195681661
+        if tmp_green < 0:
+            green = 0
+        elif tmp_green > 255:
+            green = 255
+        else:
+            green = tmp_green
+    else:
+        tmp_green = 288.1221695283 * math.pow(tmp_internal - 60, -0.0755148492)
+        if tmp_green < 0:
+            green = 0
+        elif tmp_green > 255:
+            green = 255
+        else:
+            green = tmp_green
+
+    # blue
+    if tmp_internal >=66:
+        blue = 255
+    elif tmp_internal <= 19:
+        blue = 0
+    else:
+        tmp_blue = 138.5177312231 * math.log(tmp_internal - 10) - 305.0447927307
+        if tmp_blue < 0:
+            blue = 0
+        elif tmp_blue > 255:
+            blue = 255
+        else:
+            blue = tmp_blue
+
+    return red, green, blue
+
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class VantageException(Exception):
     """Top level module exception."""
 
@@ -1336,14 +1396,22 @@
             ts = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             ts.connect((self._host, self._file_port))
 
             if self._use_ssl:
                 ts = self._ssl_context.wrap_socket(ts)
 
             if self._user:
+                # _LOGGER.info("trying introspection")
+                # ts.send(("<IIntrospection><GetSysInfo><call></call></GetSysInfo></IIntrospection>\n").encode("ascii"))
+                # response = ""
+                # while not response.endswith("</IIntrospection>\n"):
+                #     response += ts.recv(4096).decode('ascii')
+                # _LOGGER.debug("introspection response = " + response)
+
+                _LOGGER.debug("trying to login")
                 ts.send(("<ILogin><Login><call><User>%s</User>"
                          "<Password>%s</Password>"
                          "</call></Login></ILogin>\n"
                          % (escape(self._user),
                             escape(self._password))).encode("ascii"))
                 response = ""
                 while not response.endswith("</ILogin>\n"):
@@ -1377,21 +1445,26 @@
                               " check username and password")
                 exit(-1)
             except socket.timeout:
                 ts.close()
             _LOGGER.debug("done reading, size = %s", len(response))
 
             response = response.decode('ascii')
+            orig_response = response
 
-            # read XML preserving processing instructions
-            response = ET.fromstring(response, parser=ET.XMLParser(target=ET.TreeBuilder(insert_pis=True)))
-            response = response.find("GetFile/return")
-            response = next(response.iter(tag=ET.ProcessingInstruction))
-            response = response.text.split()[2][1:]
-            xml_db = base64.b64decode(response).decode('utf-8')
+            try:
+                # read XML preserving processing instructions
+                response = ET.fromstring(response, parser=ET.XMLParser(target=ET.TreeBuilder(insert_pis=True)))
+                response = response.find("GetFile/return")
+                response = next(response.iter(tag=ET.ProcessingInstruction))
+                response = response.text.split()[2][1:]
+                xml_db = base64.b64decode(response).decode('utf-8')
+            except Exception as e:
+                _LOGGER.warning("Could not parse XML response:\n\"\"\"\n%s\n\"\"\"", orig_response)
+                raise e
             if len(xml_db) < 1000:
                 _LOGGER.warning("Downloaded short .dc file; "
                                 " check saved cache file on disk")
             try:
                 f = open(filename, "w")
                 f.write(xml_db)
                 f.close()
@@ -1830,17 +1903,17 @@
             self._invoke_rgb()
 
         if self._is_dimmable:
             if new_level == 0:
                 ramp_sec = self._ramp_sec[1]
             else:
                 ramp_sec = self._ramp_sec[0]
-            self._vantage.send("RAMPLOAD", self._vid, new_level, ramp_sec)
+            self._vantage.send("RAMPLOAD", self._vid, round(new_level), ramp_sec)
         else:
-            self._vantage.send("LOAD", self._vid, new_level)
+            self._vantage.send("LOAD", self._vid, round(new_level))
 
     level = property(_get_level, _set_level)
 
     @property
     def rgb(self):
         """Returns current color of the light."""
         return self._rgb
@@ -1867,15 +1940,19 @@
 
     def _invoke_rgb(self):
         """Update the RGB of the light to self._rgb"""
         (r, g, b) = self._rgb
         ratio = self._level/100
         self._vantage.send("INVOKE", self._vid,
                            ("RGBLoad.SetRGBW %d %d %d %d" %
-                            (r*ratio, g*ratio, b*ratio, 0)))
+                            (round(r*ratio), round(g*ratio), round(b*ratio), 0)))
+        if self._dmx_color and self._level > 0:
+            _LOGGER.debug('_invoke_rgb calling rampload to ensure dmx change is triggered')
+            self._vantage.send("RAMPLOAD", self._vid, self._level, 0.1)
+
         if self._level > 0:
             self._rgb_is_dirty = False
 
     @property
     # hue is scaled 0-360, saturation is 0-100
     def hs(self):
         """Returns current HS of the light."""
@@ -1895,14 +1972,20 @@
     def _invoke_hs(self):
         """Update the HS of the light to self._hsv
         It's worth noting that HS still specifies a color even when the light is off."""
         (h, s) = self._hs
         self._vantage.send("INVOKE", self._vid,
                            ("RGBLoad.SetHSL %d %d %d" %
                             (h, s, self._level)))
+        if self._dmx_color and self._level > 0:
+            _LOGGER.debug('_invoke_hs calling rampload to ensure dmx change is triggered')
+            self._vantage.send("RAMPLOAD", self._vid, self._level, 0.1)
+
+        if self._level > 0:
+            self._rgb_is_dirty = False
 
     @property
     def color_temp(self):
         """Returns the current output level by querying the controller."""
         # TODO: query the color temp
 #    ev = self._query_waiters.request(self.__do_query_color)
 #    ev.wait(self._wait_seconds)
@@ -1910,20 +1993,21 @@
 
     @color_temp.setter
     def color_temp(self, new_color_temp):
         """Sets the new color temp level."""
         if self._color_temp == new_color_temp:
             return
         if self._dmx_color or self._load_type == "DW":
-            _LOGGER.debug("%s: Ignoring call to setter for color_temp "
-                          "of dmx_color light", self)
-        else:
-            self._vantage.send("RAMPLOAD", self._color_control_vid,
-                               kelvin_to_level(new_color_temp),
-                               self._ramp_sec[2])
+            rgb = kelvin_to_rgb(new_color_temp)
+            _LOGGER.debug("%s: Using rgb of %s for call to setter for color_temp "
+                          "%s of dmx_color light", self, rgb, new_color_temp)
+            self.rgb = rgb
+        self._vantage.send("RAMPLOAD", self._color_control_vid,
+                            kelvin_to_level(new_color_temp),
+                            self._ramp_sec[2])
         self._color_temp = new_color_temp
 
 # At some later date, we may want to also specify fade and delay times
 #  def set_level(self, new_level, fade_time, delay):
 #    self._vantage.send(Vantage.OP_EXECUTE, Output.CMD_TYPE,
 #        Output.ACTION_ZONE_LEVEL, new_level, fade_time, delay)
 
@@ -2279,26 +2363,28 @@
         ratio = self._level/100
         for vid in self._load_vids:
             load = self._vantage._vid_to_load.get(vid)
             if load and (load._dmx_color or load._load_type == "DW"):
                 self._vantage.send("INVOKE", vid,
                                    ("RGBLoad.SetRGBW %d %d %d %d" %
                                     (r*ratio, g*ratio, b*ratio, 0)))
+                self._vantage.send("RAMPLOAD", vid, self._level, 0.1)
         if self._level > 0:
             self._rgb_is_dirty = False
 
     def _invoke_hs(self):
         """Update the RGB of the load group to self._rgb"""
         (h, s) = self._hs
         for vid in self._load_vids:
             load = self._vantage._vid_to_load.get(vid)
             if load and (load._dmx_color or load._load_type == "DW"):
                 self._vantage.send("INVOKE", vid,
                                    ("RGBLoad.SetHSL %d %d %d" %
-                                    (h, s, self._level)))
+                                    (h, s, self._level-1)))
+                self._vantage.send("RAMPLOAD", vid, self._level, 0.1)
 
     def __do_query_level(self):
         """Helper to perform the actual query the current dimmer level of the
         output. For pure on/off loads the result is either 0.0 or 100.0."""
         if self.support_color and not self._addedstatus:
             _LOGGER.debug("Using first color_vid = %s to ADDSTATUS for %s",
                           self._color_vids[0], self._vid)
```

### Comparing `pyvantage-0.0.50/pyvantage.egg-info/PKG-INFO` & `pyvantage-0.0.52/pyvantage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.50
+Version: 0.0.52
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.50/setup.py` & `pyvantage-0.0.52/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyvantage',
-    version='0.0.50',
+    version='0.0.52',
     license='MIT',
     description='Python library for Vantage Controller (for Home Assistant)',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyvantage',
     packages=find_packages(),
     classifiers=[
```


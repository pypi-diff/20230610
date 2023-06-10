# Comparing `tmp/az-st7735-0.1.0.tar.gz` & `tmp/az-st7735-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "az-st7735-0.1.0.tar", last modified: Sat Jun 10 10:47:51 2023, max compression
+gzip compressed data, was "az-st7735-0.1.1.tar", last modified: Sat Jun 10 12:12:27 2023, max compression
```

## Comparing `az-st7735-0.1.0.tar` & `az-st7735-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:47:51.674923 az-st7735-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 10:47:21.000000 az-st7735-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 10:47:51.674923 az-st7735-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 10:47:21.000000 az-st7735-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-10 10:47:21.000000 az-st7735-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-10 10:47:51.674923 az-st7735-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:47:51.670922 az-st7735-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:47:51.674923 az-st7735-0.1.0/src/az_st7735.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 10:47:51.000000 az-st7735-0.1.0/src/az_st7735.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-10 10:47:51.000000 az-st7735-0.1.0/src/az_st7735.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 10:47:51.000000 az-st7735-0.1.0/src/az_st7735.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 10:47:51.000000 az-st7735-0.1.0/src/az_st7735.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:47:51.674923 az-st7735-0.1.0/src/azst7735/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:47:21.000000 az-st7735-0.1.0/src/azst7735/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-10 10:47:21.000000 az-st7735-0.1.0/src/azst7735/st7735.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:27.646959 az-st7735-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 12:11:47.000000 az-st7735-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 12:12:27.646959 az-st7735-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 12:11:47.000000 az-st7735-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-10 12:11:47.000000 az-st7735-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-10 12:12:27.646959 az-st7735-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:27.646959 az-st7735-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:27.646959 az-st7735-0.1.1/src/az_st7735.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-10 12:12:27.000000 az-st7735-0.1.1/src/az_st7735.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-10 12:12:27.000000 az-st7735-0.1.1/src/az_st7735.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:12:27.000000 az-st7735-0.1.1/src/az_st7735.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 12:12:27.000000 az-st7735-0.1.1/src/az_st7735.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:12:27.646959 az-st7735-0.1.1/src/azst7735/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 12:11:47.000000 az-st7735-0.1.1/src/azst7735/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-06-10 12:11:47.000000 az-st7735-0.1.1/src/azst7735/st7735.py
```

### Comparing `az-st7735-0.1.0/LICENSE` & `az-st7735-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `az-st7735-0.1.0/PKG-INFO` & `az-st7735-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: az-st7735
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for the ST7735 controlled 1.8inch display from AZ-Delivery
 Home-page: https://github.com/mrbluesky125/az-st7735
 Author: Timo Zimmermann
 Author-email: github@timozimmermann.de
 Project-URL: Bug Tracker, https://github.com/mrbluesky125/az-st7735/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `az-st7735-0.1.0/setup.cfg` & `az-st7735-0.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = az-st7735
-version = 0.1.0
+version = 0.1.1
 author = Timo Zimmermann
 author_email = github@timozimmermann.de
 description = Python library for the ST7735 controlled 1.8inch display from AZ-Delivery
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mrbluesky125/az-st7735
 project_urls =
```

### Comparing `az-st7735-0.1.0/src/az_st7735.egg-info/PKG-INFO` & `az-st7735-0.1.1/src/az_st7735.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: az-st7735
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for the ST7735 controlled 1.8inch display from AZ-Delivery
 Home-page: https://github.com/mrbluesky125/az-st7735
 Author: Timo Zimmermann
 Author-email: github@timozimmermann.de
 Project-URL: Bug Tracker, https://github.com/mrbluesky125/az-st7735/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `az-st7735-0.1.0/src/azst7735/st7735.py` & `az-st7735-0.1.1/src/azst7735/st7735.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numbers
 import time
 import numpy as np
 
 import spidev
 import RPi.GPIO as GPIO
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 SPI_CLOCK_HZ = 16000000
 
 # Constants for interacting with display registers.
 ST7735_TFTWIDTH = 128
 ST7735_TFTHEIGHT = 160
 
@@ -329,10 +329,10 @@
         :param image: Should be RGB format and the same dimensions as the display hardware.
 
         """
         # Convert image to array of 16bit 565 RGB data bytes.
         # Unfortunate that this copy has to occur, but the SPI byte writing
         # function needs to take an array of bytes and PIL doesn't natively
         # store images in 16-bit 565 RGB format.
-        pixelbytes = list(image_to_data(image, self._rotation))
+        pixelbytes = list(image_to_data(image))
         # Write data to hardware.
         self.data(pixelbytes)
```


# Comparing `tmp/dymoprint-1.4.0.tar.gz` & `tmp/dymoprint-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymoprint-1.4.0.tar", last modified: Sat May 27 16:20:17 2023, max compression
+gzip compressed data, was "dymoprint-1.4.1.tar", last modified: Sat Jun 10 18:48:10 2023, max compression
```

## Comparing `dymoprint-1.4.0.tar` & `dymoprint-1.4.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.943106 dymoprint-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.943106 dymoprint-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-27 16:20:01.000000 dymoprint-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-27 16:20:01.000000 dymoprint-1.4.0/91-dymo-labelmanager-pnp.rules
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-27 16:20:01.000000 dymoprint-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-27 16:20:17.951106 dymoprint-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-27 16:20:01.000000 dymoprint-1.4.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-05-27 16:20:01.000000 dymoprint-1.4.0/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.943106 dymoprint-1.4.0/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.947106 dymoprint-1.4.0/data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   690516 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   816716 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   623416 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   635996 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/Carlito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/barcode_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/gui_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/img_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/qr_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-27 16:20:01.000000 dymoprint-1.4.0/data/fonts/txt_icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.947106 dymoprint-1.4.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-27 16:20:01.000000 dymoprint-1.4.0/doc/DymoPrint_example_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-05-27 16:20:01.000000 dymoprint-1.4.0/doc/DymoPrint_example_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-05-27 16:20:01.000000 dymoprint-1.4.0/doc/DymoPrint_example_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-27 16:20:01.000000 dymoprint-1.4.0/dymo-labelmanager-pnp.conf
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-27 16:20:01.000000 dymoprint-1.4.0/dymoprint.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-27 16:20:01.000000 dymoprint-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-27 16:20:17.951106 dymoprint-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-27 16:20:01.000000 dymoprint-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/src/dymoprint/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/barcode_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5638 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1575 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/dymo_print_engines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/font_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7501 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/q_dymo_label_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/q_dymo_labels_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/unicode_blocks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-05-27 16:20:01.000000 dymoprint-1.4.0/src/dymoprint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:20:17.951106 dymoprint-1.4.0/src/dymoprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 16:20:17.000000 dymoprint-1.4.0/src/dymoprint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.494597 dymoprint-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.486597 dymoprint-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-10 18:47:55.000000 dymoprint-1.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.486597 dymoprint-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-10 18:47:55.000000 dymoprint-1.4.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-10 18:47:55.000000 dymoprint-1.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-10 18:47:55.000000 dymoprint-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-10 18:47:55.000000 dymoprint-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-10 18:47:55.000000 dymoprint-1.4.1/91-dymo-labelmanager-pnp.rules
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-10 18:47:55.000000 dymoprint-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-10 18:48:10.494597 dymoprint-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-10 18:47:55.000000 dymoprint-1.4.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-10 18:47:55.000000 dymoprint-1.4.1/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.486597 dymoprint-1.4.1/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.490597 dymoprint-1.4.1/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   690516 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   816716 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   623416 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   635996 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/barcode_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/gui_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/img_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/qr_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-10 18:47:55.000000 dymoprint-1.4.1/data/fonts/txt_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.490597 dymoprint-1.4.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-10 18:47:55.000000 dymoprint-1.4.1/doc/DymoPrint_example_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-06-10 18:47:55.000000 dymoprint-1.4.1/doc/DymoPrint_example_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-06-10 18:47:55.000000 dymoprint-1.4.1/doc/DymoPrint_example_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-10 18:47:55.000000 dymoprint-1.4.1/dymo-labelmanager-pnp.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-10 18:47:55.000000 dymoprint-1.4.1/dymoprint.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-10 18:47:55.000000 dymoprint-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-10 18:48:10.494597 dymoprint-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-10 18:47:55.000000 dymoprint-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.490597 dymoprint-1.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.494597 dymoprint-1.4.1/src/dymoprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/barcode_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5743 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/dymo_print_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/font_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7537 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/q_dymo_label_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/q_dymo_labels_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/unicode_blocks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3128 2023-06-10 18:47:55.000000 dymoprint-1.4.1/src/dymoprint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 18:48:10.494597 dymoprint-1.4.1/src/dymoprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-10 18:48:10.000000 dymoprint-1.4.1/src/dymoprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-10 18:48:10.000000 dymoprint-1.4.1/src/dymoprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 18:48:10.000000 dymoprint-1.4.1/src/dymoprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-10 18:48:10.000000 dymoprint-1.4.1/src/dymoprint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-10 18:48:10.000000 dymoprint-1.4.1/src/dymoprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-10 18:48:10.000000 dymoprint-1.4.1/src/dymoprint.egg-info/top_level.txt
```

### Comparing `dymoprint-1.4.0/.github/workflows/pypi-publish.yml` & `dymoprint-1.4.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/.github/workflows/tests.yml` & `dymoprint-1.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/.gitignore` & `dymoprint-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/LICENSE` & `dymoprint-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/PKG-INFO` & `dymoprint-1.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: dymoprint
-Version: 1.4.0
-Summary: Linux Software to print with LabelManager PnP from Dymo
-Home-page: https://github.com/computerlyrik/dymoprint
-Author: Sebastian J. Bronner
-Author-email: waschtl@sbronner.com
-Maintainer: Ben Mares
-Maintainer-email: services-dymoprint@tensorial.com
-License: Apache License 2.0
-Project-URL: Source, https://github.com/computerlyrik/dymoprint
-Project-URL: Tracker, https://github.com/computerlyrik/dymoprint/issues
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Printing
-Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
-
 # dymoprint
 
 [![GitHub Actions (Tests)](https://github.com/computerlyrik/dymoprint/workflows/Tests/badge.svg)](https://github.com/computerlyrik/dymoprint)
 [![PyPI version](https://img.shields.io/pypi/v/dymoprint.svg)](https://pypi.org/project/dymoprint/)
 
 Linux Software to print with LabelManager PnP from Dymo
 
@@ -37,14 +15,18 @@
 * Supports text printing
 * Supports qr code printing
 * Supports barcode printing
 * Supports image printing
 * Supports combined barcode / qrcode and text printing
 * GUI Application based on PyQt6 - expanded combinations
 
+## HELP WANTED
+
+Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
+
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
 ```
@@ -57,21 +39,45 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
+## Experimental features
 
-To install for development, fork and clone this repository, and from this directory, and run (ideally within a venv):
+To install a test branch, by user `ghuser` for the branch `branchname`, run
+
+```bash
+pipx install --force git+https://github.com/ghuser/dymoprint@branchname
+```
+
+To revert back to the release version, run
+
+```bash
+pipx install --force dymoprint
+```
+
+To install a particular release version, specify `dymoprint==x.y.z` instead of `dymoprint` in the above command.
+
+## Development
+
+To install for development, fork and clone this repository, and run (ideally within a venv):
 
 ```bash
 pip install --editable .
 ```
 
+This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
+After installing the `pre-commit` executable, please run
+
+```bash
+pre-commit install
+```
+
 ## Configuration
 
 ### For ubuntu based distributions
 
 Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
 **modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
```

### Comparing `dymoprint-1.4.0/README.md` & `dymoprint-1.4.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: dymoprint
+Version: 1.4.1
+Summary: Linux Software to print with LabelManager PnP from Dymo
+Home-page: https://github.com/computerlyrik/dymoprint
+Author: Sebastian J. Bronner
+Author-email: waschtl@sbronner.com
+Maintainer: Ben Mares
+Maintainer-email: services-dymoprint@tensorial.com
+License: Apache License 2.0
+Project-URL: Source, https://github.com/computerlyrik/dymoprint
+Project-URL: Tracker, https://github.com/computerlyrik/dymoprint/issues
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Printing
+Requires-Python: <4,>=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
 # dymoprint
 
 [![GitHub Actions (Tests)](https://github.com/computerlyrik/dymoprint/workflows/Tests/badge.svg)](https://github.com/computerlyrik/dymoprint)
 [![PyPI version](https://img.shields.io/pypi/v/dymoprint.svg)](https://pypi.org/project/dymoprint/)
 
 Linux Software to print with LabelManager PnP from Dymo
 
@@ -15,14 +37,18 @@
 * Supports text printing
 * Supports qr code printing
 * Supports barcode printing
 * Supports image printing
 * Supports combined barcode / qrcode and text printing
 * GUI Application based on PyQt6 - expanded combinations
 
+## HELP WANTED
+
+Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
+
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
 ```
@@ -35,21 +61,45 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
+## Experimental features
 
-To install for development, fork and clone this repository, and from this directory, and run (ideally within a venv):
+To install a test branch, by user `ghuser` for the branch `branchname`, run
+
+```bash
+pipx install --force git+https://github.com/ghuser/dymoprint@branchname
+```
+
+To revert back to the release version, run
+
+```bash
+pipx install --force dymoprint
+```
+
+To install a particular release version, specify `dymoprint==x.y.z` instead of `dymoprint` in the above command.
+
+## Development
+
+To install for development, fork and clone this repository, and run (ideally within a venv):
 
 ```bash
 pip install --editable .
 ```
 
+This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
+After installing the `pre-commit` executable, please run
+
+```bash
+pre-commit install
+```
+
 ## Configuration
 
 ### For ubuntu based distributions
 
 Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
 **modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
```

### Comparing `dymoprint-1.4.0/TODO.md` & `dymoprint-1.4.1/TODO.md`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/Carlito-Bold.ttf` & `dymoprint-1.4.1/data/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/Carlito-BoldItalic.ttf` & `dymoprint-1.4.1/data/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/Carlito-Italic.ttf` & `dymoprint-1.4.1/data/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/Carlito-Regular.ttf` & `dymoprint-1.4.1/data/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/LICENSE` & `dymoprint-1.4.1/data/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/barcode_icon.png` & `dymoprint-1.4.1/data/fonts/barcode_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/gui_icon.png` & `dymoprint-1.4.1/data/fonts/gui_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/img_icon.png` & `dymoprint-1.4.1/data/fonts/img_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/data/fonts/txt_icon.png` & `dymoprint-1.4.1/data/fonts/txt_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/doc/DymoPrint_example_1.png` & `dymoprint-1.4.1/doc/DymoPrint_example_1.png`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/doc/DymoPrint_example_2.png` & `dymoprint-1.4.1/doc/DymoPrint_example_2.png`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/doc/DymoPrint_example_3.png` & `dymoprint-1.4.1/doc/DymoPrint_example_3.png`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/pyproject.toml` & `dymoprint-1.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # See configuration details in https://github.com/pypa/setuptools_scm
 version_scheme = "no-guess-dev"
 
 [tool.isort]
+src_paths = ["src"]
 profile = "black"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
   py37
```

### Comparing `dymoprint-1.4.0/setup.cfg` & `dymoprint-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/setup.py` & `dymoprint-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/src/README.md` & `dymoprint-1.4.1/src/README.md`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/src/dymoprint/barcode_writer.py` & `dymoprint-1.4.1/src/dymoprint/barcode_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,26 +60,24 @@
                     if line[i] == "1":
                         mlist.append(c)
                     else:
                         mlist.append(-c)
                     c = 1
             # Left quiet zone is x startposition
             xpos = self.quiet_zone
-            bxs = xpos  # x start of barcode
             for mod in mlist:
                 if mod < 1:
                     color = self.background
                 else:
                     color = self.foreground
                 # remove painting for background colored tiles?
                 self._callbacks["paint_module"](
                     xpos, ypos, self.module_width * abs(mod), color
                 )
                 xpos += self.module_width * abs(mod)
-            bxe = xpos
             # Add right quiet zone to every line, except last line,
             # quiet zone already provided with background,
             # should it be removed complety?
             if (cc + 1) != len(code):
                 self._callbacks["paint_module"](
                     xpos, ypos, self.quiet_zone, self.background
                 )
@@ -101,10 +99,10 @@
         ]
         self._draw.rectangle(size, outline=color, fill=color)
 
     def _finish(self):
         return self._image
 
     def save(self, filename, output):
-        filename = "{0}.{1}".format(filename, self.format.lower())
+        filename = f"{filename}.{self.format.lower()}"
         output.save(filename, self.format.upper())
         return filename
```

### Comparing `dymoprint-1.4.0/src/dymoprint/command_line.py` & `dymoprint-1.4.1/src/dymoprint/command_line.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import argparse
 import os
 
 from PIL import Image, ImageOps
 
 from . import __version__
-from .constants import USE_QR, e_qrcode
+from .constants import DEFAULT_MARGIN, USE_QR, e_qrcode
 from .dymo_print_engines import DymoPrinterServer, DymoRenderEngine
 from .font_config import font_filename
 from .metadata import our_metadata
 from .unicode_blocks import image_to_unicode
 from .utils import die
 
 
@@ -60,15 +60,18 @@
         "-j",
         choices=[
             "left",
             "center",
             "right",
         ],
         default="center",
-        help="Justify content of label if minimum label length is specified (left,center,right)",
+        help=(
+            "Justify content of label if minimum label length "
+            "is specified (left,center,right)"
+        ),
     )
     parser.add_argument("-u", nargs="?", help='Set user font, overrides "-s" parameter')
     parser.add_argument(
         "-n",
         "--preview",
         action="store_true",
         help="Unicode preview of label, do not send to printer",
@@ -106,15 +109,18 @@
             "upca",
         ],
         default=False,
         help="Printing the first text parameter as barcode",
     )
     parser.add_argument("-p", "--picture", help="Print the specified picture")
     parser.add_argument(
-        "-m", type=int, default=56, help="Override margin (default is 56*2)"
+        "-m",
+        type=int,
+        default=DEFAULT_MARGIN,
+        help=f"Override margin (default is {DEFAULT_MARGIN})",
     )
     parser.add_argument(
         "--scale", type=int, default=90, help="Scaling font factor, [0,10] [%%]"
     )
     parser.add_argument(
         "-t",
         type=int,
```

### Comparing `dymoprint-1.4.0/src/dymoprint/constants.py` & `dymoprint-1.4.1/src/dymoprint/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,13 +45,15 @@
 # Synchronization character preceding uncompressed print data
 SYN = 0x16
 
 FONT_SIZERATIO = 7 / 8
 
 DEFAULT_FONT_STYLE = "regular"
 
+DEFAULT_MARGIN = 56
+
 FLAG_TO_STYLE = {
     "r": "regular",
     "b": "bold",
     "i": "italic",
     "n": "narrow",
 }
```

### Comparing `dymoprint-1.4.0/src/dymoprint/dymo_print_engines.py` & `dymoprint-1.4.1/src/dymoprint/dymo_print_engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import barcode as barcode_module
 import usb
 from PIL import Image, ImageFont, ImageOps
 
 from . import DymoLabeler
 from .barcode_writer import BarcodeImageWriter
 from .constants import (
+    DEFAULT_MARGIN,
     DEV_CLASS,
     DEV_LM280_CLASS,
     DEV_LM280_PRODUCT,
     DEV_NAME,
     DEV_NODE,
     DEV_PRODUCT,
     DEV_VENDOR,
@@ -64,15 +65,16 @@
         # create an empty label image
         qr_scale = label_height // len(qr_text)
         qr_offset = (label_height - len(qr_text) * qr_scale) // 2
         label_width = len(qr_text) * qr_scale
 
         if not qr_scale:
             die(
-                "Error: too much information to store in the QR code, points are smaller than the device resolution"
+                "Error: too much information to store in the QR code, points "
+                "are smaller than the device resolution"
             )
 
         code_bitmap = Image.new("1", (label_width, label_height))
 
         with draw_image(code_bitmap) as label_draw:
             # write the qr-code into the empty image
             for i, line in enumerate(qr_text):
@@ -120,21 +122,23 @@
         labeltext: list[str],
         font_file_name: str,
         frame_width,
         font_size_ratio=0.9,
         align="left",
     ):
         """
-        Renders a text image from the input text, font file name, frame width, and font size ratio.
+        Renders a text image from the input text, font file name, frame width, and
+        font size ratio.
 
         Args:
             labeltext (list[str]): The input text to be rendered.
             font_file_name (str): The name of the font file to be used.
             frame_width (int): The width of the frame around the text.
-            font_size_ratio (float): The ratio of font size to line height. Default is 1.
+            font_size_ratio (float): The ratio of font size to line height. Default
+                is 1.
 
         Returns:
             Image: A text image.
         """
         if type(labeltext) is str:
             labeltext = [labeltext]
 
@@ -154,15 +158,14 @@
 
         font = ImageFont.truetype(font_file_name, fontsize)
         label_width = max(font.getsize(line)[0] for line in labeltext) + (
             font_offset * 2
         )
         text_bitmap = Image.new("1", (label_width, label_height))
         with draw_image(text_bitmap) as label_draw:
-
             # draw frame into empty image
             if frame_width:
                 label_draw.rectangle(
                     ((0, 4), (label_width - 1, label_height - 4)), fill=255
                 )
                 label_draw.rectangle(
                     (
@@ -259,21 +262,21 @@
             return out_label_bitmap
 
         return label_bitmap
 
 
 class DymoPrinterServer:
     @staticmethod
-    def print_label(label_bitmap, margin=56 * 2, tape_size: int = 12):
+    def print_label(label_bitmap, margin=DEFAULT_MARGIN, tape_size: int = 12):
         """
         Prints a label using a Dymo labeler object.
 
         :param label_bitmap: The image to be printed as a label.
         :type label_bitmap: Image
-        :param margin: The margin size in dots. Default is 56.
+        :param margin: The margin size in dots.
         :type margin: int, optional
         :param tape_size: The size of the tape in millimeters. Default is 12.
         :type tape_size: int, optional
         :return: None
         :rtype: None
         """
         # convert the image to the proper matrix for the dymo labeler object
@@ -295,15 +298,18 @@
         # get device file name
         if not DEV_NODE:
             dev = getDeviceFile(DEV_CLASS, DEV_VENDOR, DEV_PRODUCT)
         else:
             dev = DEV_NODE
 
         if dev:
-            devout = open(dev, "rb+")
+            try:
+                devout = open(dev, "rb+")
+            except PermissionError:
+                access_error(dev)
             devin = devout
             # We are in the normal HID file mode, so no syn_wait is needed.
             syn_wait = None
             in_usb_mode = False
         else:
             # We are in the experimental PyUSB mode, if a device can be found.
             syn_wait = 64
@@ -353,18 +359,16 @@
 
         if not devout or not devin:
             die("The device '%s' could not be found on this system." % DEV_NAME)
 
         # create dymo labeler object
         try:
             lm = DymoLabeler(devout, devin, synwait=syn_wait, tape_size=tape_size)
-        except IOError:
-            die(access_error(dev))
+        except OSError:
+            access_error(dev)
 
         print("Printing label..")
-        if margin is not None:
-            lm.printLabel(label_matrix, margin=margin)
-        else:
-            lm.printLabel(label_matrix)
+        lm.printLabel(label_matrix, margin=margin)
+        print("Done printing.")
 
         if in_usb_mode:
             usb.util.dispose_resources(dev)
```

### Comparing `dymoprint-1.4.0/src/dymoprint/font_config.py` & `dymoprint-1.4.1/src/dymoprint/font_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         "narrow": os.path.join(DEFAULT_FONT_DIR, "Carlito-BoldItalic.ttf"),
     }
 
     conf = ConfigParser(style_to_file)
     CONFIG_FILE = os.path.join(user_config_dir(), "dymoprint.ini")
     if conf.read(CONFIG_FILE):
         # reading FONTS section
-        if not "FONTS" in conf.sections():
+        if "FONTS" not in conf.sections():
             die('! config file "%s" not valid. Please change or remove.' % CONFIG_FILE)
         for style in style_to_file.keys():
             style_to_file[style] = conf.get("FONTS", style)
 
     return style_to_file[FLAG_TO_STYLE.get(flag, DEFAULT_FONT_STYLE)]
```

### Comparing `dymoprint-1.4.0/src/dymoprint/gui.py` & `dymoprint-1.4.1/src/dymoprint/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     QVBoxLayout,
     QWidget,
 )
 from usb.core import USBError
 
 import dymoprint_fonts
 
+from .constants import DEFAULT_MARGIN
 from .dymo_print_engines import DymoPrinterServer, DymoRenderEngine
 from .q_dymo_labels_list import QDymoLabelList
 
 
 class DymoPrintWindow(QWidget):
     def __init__(self):
         super().__init__()
@@ -62,15 +63,15 @@
 
         shadow = QGraphicsDropShadowEffect()
         shadow.setBlurRadius(15)
         self.label_render.setGraphicsEffect(shadow)
 
         self.margin.setMinimum(20)
         self.margin.setMaximum(1000)
-        self.margin.setValue(56)
+        self.margin.setValue(DEFAULT_MARGIN)
         self.tape_size.addItem("12", 12)
         self.tape_size.addItem("9", 9)
         self.tape_size.addItem("6", 6)
         self.min_label_len.setMinimum(0)
         self.min_label_len.setMaximum(1000)
         self.justify.addItems(["center", "left", "right"])
 
@@ -154,15 +155,15 @@
         p.end()
 
         self.label_render.setPixmap(q_image)
         self.label_render.adjustSize()
 
     def print_label(self):
         try:
-            self.print_server.print_label(self.label_bitmap, self.margin.value() * 2)
+            self.print_server.print_label(self.label_bitmap, self.margin.value())
         except RuntimeError as err:
             QMessageBox.warning(self, "Printing Failed!", f"{err}")
         except USBError as err:
             QMessageBox.warning(self, "Printing Failed!", f"{err}")
 
 
 def main():
```

### Comparing `dymoprint-1.4.0/src/dymoprint/labeler.py` & `dymoprint-1.4.1/src/dymoprint/labeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copying and distribution of this file, with or without modification, are
 # permitted in any medium without royalty provided the copyright notice and
 # this notice are preserved.
 # === END LICENSE STATEMENT ===
 import array
 from typing import Optional
 
-from .constants import ESC, SYN
+from .constants import DEFAULT_MARGIN, ESC, SYN
 
 
 class DymoLabeler:
     """Create and work with a Dymo LabelManager PnP object.
 
     This class contains both mid-level and high-level functions. In general,
     the high-level functions should be used. However, special purpose usage
@@ -185,24 +185,24 @@
     def getStatus(self):
         """Ask for and return the device's status. (HLF)"""
 
         self.statusRequest()
         response = self.sendCommand()
         print(response)
 
-    def printLabel(self, lines, margin=56 * 2):
+    def printLabel(self, lines, margin=DEFAULT_MARGIN):
         """Print the label described by lines. (Automatically split label if
         larger than maxLines)"""
 
         while len(lines) > self.maxLines + 1:
             self.rawPrintLabel(lines[0 : self.maxLines], margin=0)
             del lines[0 : self.maxLines]
         self.rawPrintLabel(lines, margin=margin)
 
-    def rawPrintLabel(self, lines, margin=56 * 2):
+    def rawPrintLabel(self, lines, margin=DEFAULT_MARGIN):
         """Print the label described by lines. (HLF)"""
 
         # optimize the matrix for the dymo label printer
         dottab = 0
         while [] not in lines and max(line[0] for line in lines) == 0:
             lines = [line[1:] for line in lines]
             dottab += 1
@@ -212,11 +212,11 @@
 
         self.initLabel
         self.tapeColor(0)
         self.dotTab(dottab)
         for line in lines:
             self.line(line)
         if margin > 0:
-            self.skipLines(margin)
+            self.skipLines(margin * 2)
         self.statusRequest()
         response = self.sendCommand()
         print(f"Post-send response: {response}")
```

### Comparing `dymoprint-1.4.0/src/dymoprint/q_dymo_label_widgets.py` & `dymoprint-1.4.1/src/dymoprint/q_dymo_label_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMessageBox,
     QPlainTextEdit,
     QPushButton,
     QSpinBox,
-    QVBoxLayout,
     QWidget,
 )
 
 import dymoprint_fonts
 
 from .font_config import parse_fonts
 
@@ -64,15 +63,15 @@
         font_size (QSpinBox): The font size selection spinner.
         draw_frame (QSpinBox): The frame width selection spinner.
     Signals:
         itemRenderSignal: A signal emitted when the content of the label changes.
     """
 
     def __init__(self, render_engine, parent=None):
-        super(TextDymoLabelWidget, self).__init__(parent)
+        super().__init__(parent)
         self.render_engine = render_engine
 
         self.label = QPlainTextEdit("text")
         self.label.setFixedHeight(15 * (len(self.label.toPlainText().splitlines()) + 2))
         self.setFixedHeight(self.label.height() + 10)
         self.font_style = QComboBox()
         self.font_size = QSpinBox()
@@ -81,15 +80,15 @@
         self.font_size.setSingleStep(1)
         self.font_size.setValue(90)
         self.draw_frame = QSpinBox()
         self.align = QComboBox()
 
         self.align.addItems(["left", "center", "right"])
 
-        for (name, font_path) in parse_fonts():
+        for name, font_path in parse_fonts():
             self.font_style.addItem(name, font_path)
             if "Regular" in name:
                 self.font_style.setCurrentText(name)
 
         layout = QHBoxLayout()
         ICON_DIR = os.path.dirname(dymoprint_fonts.__file__)
         item_icon = QLabel()
@@ -112,15 +111,16 @@
         self.font_size.valueChanged.connect(self.content_changed)
         self.font_style.currentTextChanged.connect(self.content_changed)
         self.align.currentTextChanged.connect(self.content_changed)
         self.setLayout(layout)
 
     def content_changed(self):
         """
-        Updates the height of the label and emits the itemRenderSignal when the content of the label changes.
+        Updates the height of the label and emits the itemRenderSignal when the
+        content of the label changes.
         """
         self.label.setFixedHeight(15 * (len(self.label.toPlainText().splitlines()) + 2))
         self.setFixedHeight(self.label.height() + 10)
         self.itemRenderSignal.emit()
 
     def render_label(self):
         """
@@ -144,26 +144,28 @@
             return self.render_engine.render_empty()
 
 
 class QrDymoLabelWidget(BaseDymoLabelWidget):
     """
     A widget for rendering QR codes on Dymo labels.
     Args:
-        render_engine (RenderEngine): The render engine to use for rendering the QR code.
+        render_engine (RenderEngine): The render engine to use for rendering
+            the QR code.
         parent (QWidget, optional): The parent widget. Defaults to None.
     """
 
     def __init__(self, render_engine, parent=None):
         """
         Initializes the QrDymoLabelWidget.
         Args:
-            render_engine (RenderEngine): The render engine to use for rendering the QR code.
+            render_engine (RenderEngine): The render engine to use for rendering
+                the QR code.
             parent (QWidget, optional): The parent widget. Defaults to None.
         """
-        super(QrDymoLabelWidget, self).__init__(parent)
+        super().__init__(parent)
         self.render_engine = render_engine
 
         self.label = QLineEdit("")
         layout = QHBoxLayout()
         ICON_DIR = os.path.dirname(dymoprint_fonts.__file__)
         item_icon = QLabel()
         item_icon.setPixmap(QIcon(os.path.join(ICON_DIR, "qr_icon.png")).pixmap(32, 32))
@@ -194,25 +196,29 @@
     """
     A widget for rendering barcode labels using the Dymo label printer.
     Args:
         render_engine (DymoRenderEngine): An instance of the DymoRenderEngine class.
         parent (QWidget): The parent widget of this widget.
     Attributes:
         render_engine (DymoRenderEngine): An instance of the DymoRenderEngine class.
-        label (QLineEdit): A QLineEdit widget for entering the content of the barcode label.
-        codding (QComboBox): A QComboBox widget for selecting the type of barcode to render.
+        label (QLineEdit): A QLineEdit widget for entering the content of the
+            barcode label.
+        codding (QComboBox): A QComboBox widget for selecting the type of barcode
+            to render.
     Signals:
-        content_changed(): Emitted when the content of the label or the selected barcode type changes.
+        content_changed(): Emitted when the content of the label or the selected
+            barcode type changes.
     Methods:
         __init__(self, render_engine, parent=None): Initializes the widget.
-        render_label(self): Renders the barcode label using the current content and barcode type.
+        render_label(self): Renders the barcode label using the current content
+            and barcode type.
     """
 
     def __init__(self, render_engine, parent=None):
-        super(BarcodeDymoLabelWidget, self).__init__(parent)
+        super().__init__(parent)
         self.render_engine = render_engine
 
         self.label = QLineEdit("")
         layout = QHBoxLayout()
         ICON_DIR = os.path.dirname(dymoprint_fonts.__file__)
         item_icon = QLabel()
         item_icon.setPixmap(
@@ -274,18 +280,19 @@
         parent (QWidget, optional): The parent widget. Defaults to None.
     """
 
     def __init__(self, render_engine, parent=None):
         """
         Initializes the ImageDymoLabelWidget.
         Args:
-            render_engine (RenderEngine): The render engine to use for rendering the label.
+            render_engine (RenderEngine): The render engine to use for rendering
+                the label.
             parent (QWidget, optional): The parent widget. Defaults to None.
         """
-        super(ImageDymoLabelWidget, self).__init__(parent)
+        super().__init__(parent)
         self.render_engine = render_engine
 
         self.label = QLineEdit("")
         layout = QHBoxLayout()
         ICON_DIR = os.path.dirname(dymoprint_fonts.__file__)
         item_icon = QLabel()
         item_icon.setPixmap(
```

### Comparing `dymoprint-1.4.0/src/dymoprint/q_dymo_labels_list.py` & `dymoprint-1.4.1/src/dymoprint/q_dymo_labels_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,30 @@
     Args:
         render_engine (RenderEngine): The render engine to use for rendering the label.
         parent (QWidget): The parent widget of this QListWidget.
     Attributes:
         renderSignal (QtCore.pyqtSignal): A signal emitted when the label is rendered.
         render_engine (RenderEngine): The render engine used for rendering the label.
     Methods:
-        __init__(self, render_engine, parent=None): Initializes the QListWidget with the given render engine and parent.
-        dropEvent(self, e) -> None: Overrides the default drop event to update the label rendering.
-        update_render_engine(self, render_engine): Updates the render engine used for rendering the label.
-        render_label(self): Renders the label using the current render engine and emits the renderSignal.
-        contextMenuEvent(self, event): Overrides the default context menu event to add or delete label widgets.
+        __init__(self, render_engine, parent=None): Initializes the QListWidget
+            with the given render engine and parent.
+        dropEvent(self, e) -> None: Overrides the default drop event to update
+            the label rendering.
+        update_render_engine(self, render_engine): Updates the render engine used
+            for rendering the label.
+        render_label(self): Renders the label using the current render engine and
+            emits the renderSignal.
+        contextMenuEvent(self, event): Overrides the default context menu event to
+            add or delete label widgets.
     """
 
     renderSignal = QtCore.pyqtSignal(Image.Image, name="renderSignal")
 
     def __init__(self, render_engine, min_payload_len=0, justify="center", parent=None):
-        super(QDymoLabelList, self).__init__(parent)
+        super().__init__(parent)
         self.min_payload_len = min_payload_len
         self.justify = justify
         self.render_engine = render_engine
         self.setAlternatingRowColors(True)
         self.setDragDropMode(QAbstractItemView.DragDropMode.InternalMove)
         for item_widget in [TextDymoLabelWidget(self.render_engine)]:
             item = QListWidgetItem(self)
```

### Comparing `dymoprint-1.4.0/src/dymoprint/unicode_blocks.py` & `dymoprint-1.4.1/src/dymoprint/unicode_blocks.py`

 * *Files identical despite different names*

### Comparing `dymoprint-1.4.0/src/dymoprint/utils.py` & `dymoprint-1.4.1/src/dymoprint/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,41 +3,30 @@
 #
 # Copying and distribution of this file, with or without modification, are
 # permitted in any medium without royalty provided the copyright notice and
 # this notice are preserved.
 # === END LICENSE STATEMENT ===
 
 import contextlib
-import fcntl
 import os
 import re
-import struct
 import subprocess
 import sys
-import termios
-import textwrap
 from typing import NoReturn
 
 from PIL import ImageDraw
 
 
 def die(message=None) -> NoReturn:
     if message:
         print(message, file=sys.stderr)
         raise RuntimeError(message)
     sys.exit(1)
 
 
-def pprint(par, fd=sys.stdout):
-    rows, columns = struct.unpack(
-        "HH", fcntl.ioctl(sys.stderr, termios.TIOCGWINSZ, struct.pack("HH", 0, 0))
-    )
-    print(textwrap.fill(par, columns), file=fd)
-
-
 def getDeviceFile(classID, vendorID, productID):
     # find file containing the device's major and minor numbers
     searchdir = "/sys/bus/hid/devices"
     pattern = "^%04d:%04X:%04X.[0-9A-F]{4}$" % (classID, vendorID, productID)
     deviceCandidates = os.listdir(searchdir)
     foundpath = None
     for devname in deviceCandidates:
@@ -48,15 +37,15 @@
         return
     searchdir = os.path.join(foundpath, "hidraw")
     devname = os.listdir(searchdir)[0]
     foundpath = os.path.join(searchdir, devname)
     filepath = os.path.join(foundpath, "dev")
 
     # get the major and minor numbers
-    f = open(filepath, "r")
+    f = open(filepath)
     devnums = [int(n) for n in f.readline().strip().split(":")]
     f.close()
     devnum = os.makedev(devnums[0], devnums[1])
 
     # check if a symlink with the major and minor numbers is available
     filepath = "/dev/char/%d:%d" % (devnums[0], devnums[1])
     if os.path.exists(filepath):
@@ -72,27 +61,30 @@
     for dirpath, dirnames, filenames in os.walk("/dev"):
         for filename in filenames:
             filepath = os.path.join(dirpath, filename)
             if os.stat(filepath).st_rdev == devnum:
                 return filepath
 
 
-def access_error(dev):
-    die("You do not have sufficient access to the device file %s:" % dev, sys.stderr)
+def access_error(dev) -> NoReturn:
+    print(f"You do not have sufficient access to the device file {dev}")
     subprocess.call(["ls", "-l", dev], stdout=sys.stderr)
     print(file=sys.stderr)
     filename = "91-dymo-labelmanager-pnp.rules"
-    die(
-        f"You probably want to add a rule like one of the following in /etc/udev/rules.d/{filename}"
+    print(
+        f"You probably want to add a rule like "
+        f"one of the following in /etc/udev/rules.d/{filename}"
     )
-    with open(filename, "r") as fin:
+    with open(filename) as fin:
         print(fin.read(), file=sys.stderr)
-    die(
-        "Following that, restart udev and re-plug your device. See README.md for details",
+    print(
+        "Following that, restart udev and re-plug "
+        "your device. See README.md for details",
     )
+    sys.exit(1)
 
 
 """ scaling pixel up, input: (x,y),scale-factor """
 
 
 def scaling(pix, sc):
     return [(pix[0] + i, pix[1] + j) for i in range(sc) for j in range(sc)]
```

### Comparing `dymoprint-1.4.0/src/dymoprint.egg-info/PKG-INFO` & `dymoprint-1.4.1/src/dymoprint.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoprint
-Version: 1.4.0
+Version: 1.4.1
 Summary: Linux Software to print with LabelManager PnP from Dymo
 Home-page: https://github.com/computerlyrik/dymoprint
 Author: Sebastian J. Bronner
 Author-email: waschtl@sbronner.com
 Maintainer: Ben Mares
 Maintainer-email: services-dymoprint@tensorial.com
 License: Apache License 2.0
@@ -37,14 +37,18 @@
 * Supports text printing
 * Supports qr code printing
 * Supports barcode printing
 * Supports image printing
 * Supports combined barcode / qrcode and text printing
 * GUI Application based on PyQt6 - expanded combinations
 
+## HELP WANTED
+
+Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
+
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
 ```
@@ -57,21 +61,45 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
+## Experimental features
+
+To install a test branch, by user `ghuser` for the branch `branchname`, run
+
+```bash
+pipx install --force git+https://github.com/ghuser/dymoprint@branchname
+```
+
+To revert back to the release version, run
+
+```bash
+pipx install --force dymoprint
+```
+
+To install a particular release version, specify `dymoprint==x.y.z` instead of `dymoprint` in the above command.
+
+## Development
 
-To install for development, fork and clone this repository, and from this directory, and run (ideally within a venv):
+To install for development, fork and clone this repository, and run (ideally within a venv):
 
 ```bash
 pip install --editable .
 ```
 
+This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
+After installing the `pre-commit` executable, please run
+
+```bash
+pre-commit install
+```
+
 ## Configuration
 
 ### For ubuntu based distributions
 
 Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
 **modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
```

### Comparing `dymoprint-1.4.0/src/dymoprint.egg-info/SOURCES.txt` & `dymoprint-1.4.1/src/dymoprint.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.md
 TODO.md
 dymo-labelmanager-pnp.conf
 dymoprint.ini
 pyproject.toml
 setup.cfg
 setup.py
+.github/dependabot.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 data/fonts/Carlito-Bold.ttf
 data/fonts/Carlito-BoldItalic.ttf
 data/fonts/Carlito-Italic.ttf
 data/fonts/Carlito-Regular.ttf
 data/fonts/LICENSE
```


# Comparing `tmp/circuitpython-ps2controller-1.1.2.tar.gz` & `tmp/circuitpython-ps2controller-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ps2controller-1.1.2.tar", last modified: Mon Jun  5 00:22:20 2023, max compression
+gzip compressed data, was "circuitpython-ps2controller-1.2.0.tar", last modified: Fri Jun  9 22:34:30 2023, max compression
```

## Comparing `circuitpython-ps2controller-1.1.2.tar` & `circuitpython-ps2controller-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.703778 circuitpython-ps2controller-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.695778 circuitpython-ps2controller-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.695778 circuitpython-ps2controller-1.1.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.699778 circuitpython-ps2controller-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.699778 circuitpython-ps2controller-1.1.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-05 00:22:20.703778 circuitpython-ps2controller-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.699778 circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-05 00:22:20.000000 circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-05 00:22:20.000000 circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:22:20.000000 circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 00:22:20.000000 circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 00:22:20.000000 circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.699778 circuitpython-ps2controller-1.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.699778 circuitpython-ps2controller-1.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:22:20.699778 circuitpython-ps2controller-1.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-05 00:22:10.000000 circuitpython-ps2controller-1.1.2/examples/ps2controller_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-05 00:22:10.000000 circuitpython-ps2controller-1.1.2/examples/ps2controller_usbkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-06-05 00:22:10.000000 circuitpython-ps2controller-1.1.2/ps2controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-05 00:22:10.000000 circuitpython-ps2controller-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 00:22:01.000000 circuitpython-ps2controller-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 00:22:20.703778 circuitpython-ps2controller-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.291277 circuitpython-ps2controller-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.291277 circuitpython-ps2controller-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.291277 circuitpython-ps2controller-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58754 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/ps2controller_wiring.png
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/ps2controller_wiring.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_datadump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_digital_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_usbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/ps2controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/setup.cfg
```

### Comparing `circuitpython-ps2controller-1.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-ps2controller-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/.github/workflows/release_gh.yml` & `circuitpython-ps2controller-1.2.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/.gitignore` & `circuitpython-ps2controller-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/.pre-commit-config.yaml` & `circuitpython-ps2controller-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/.pylintrc` & `circuitpython-ps2controller-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/CODE_OF_CONDUCT.md` & `circuitpython-ps2controller-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/LICENSE` & `circuitpython-ps2controller-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/LICENSES/CC-BY-4.0.txt` & `circuitpython-ps2controller-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/LICENSES/MIT.txt` & `circuitpython-ps2controller-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/LICENSES/Unlicense.txt` & `circuitpython-ps2controller-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/PKG-INFO` & `circuitpython-ps2controller-1.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: circuitpython-ps2controller
-Version: 1.1.2
-Summary: CircuitPython library to read Sony PS2 game controllers
-Author-email: Tod Kurt <tod@todbot.com>
-License: MIT
-Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
-Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-Provides-Extra: optional
-License-File: LICENSE
-
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/circuitpython-ps2controller/badge/?version=latest
     :target: https://circuitpython-ps2controller.readthedocs.io/
     :alt: Documentation Status
@@ -32,15 +14,15 @@
     :target: https://github.com/todbot/CircuitPython_PS2Controller/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython library to read Sony PS2 game controllers
+CircuitPython library to read Sony PS2 or PS1 game controllers
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -107,26 +89,48 @@
 
     import board
     from ps2controller import PS2Controller
 
     # one way to wire this up, for example on a Pico
     ps2 = PS2Controller(dat=board.GP2, cmd=board.GP3, att=board.GP4, clk=board.GP5)
 
-    print("hi press buttons")
+    print("hi! Press buttons")
     while True:
         events = ps2.update()
         if events:
             print("events", events)
             print("sticks: L:", ps2.analog_left(), "R:", ps2.analog_right())
 
+Wiring
+======
+
+Wiring to the PSX controller needs four GPIO pins.These can be any pins.
+The wiring is:
+
+* CLK pin - clock OUT to controller (blue wire)
+* CMD pin - command data OUT to controller (orange wire)
+* ATT pin - attention / chip select OUT to controller (yellow wire)
+* DAT pin - data IN from controller (brown wire)
+* GND pin - signal ground (black wire)
+* VCC pin - +3.3V power (red wire)
+* VCC2 pin - +7.5V power to rumble motors (optional)
+
+Here's one way to wire that up on a Raspberry Pi Pico:
+
+.. image:: https://raw.githubusercontent.com/todbot/CircuitPython_PS2Controller/main/docs/ps2controller_wiring.png
+
+(Thanks to `Vanepp <https://forum.fritzing.org/u/vanepp/summary>`_ via `nandanhere/PiPyPS2 <https://github.com/nandanhere/PiPyPS2>`_ for Fritzing wiring diagram)
+
 
 References
 ==========
 
-This library is a fairly direct port of `madsci1016/Arduino-PS2X <https://github.com/madsci1016/Arduino-PS2X>`_.
+This library is highly inspired by the `SukkoPera/PsxNewLib <https://github.com/SukkoPera/PsxNewLib>`_ library.
+It currently has only been tested on a handful of PS1 and PS2 controllers,
+but it should be easy to add any specialized controller tuning.
 
 Other resources that have been helpful:
 
 * https://store.curiousinventor.com/guides/PS2/
 * https://gist.github.com/scanlime/5042071
 * https://gamesx.com/wiki/doku.php?id=controls:playstation_controller
 * https://github.com/SukkoPera/PsxNewLib
```

### Comparing `circuitpython-ps2controller-1.1.2/README.rst` & `circuitpython-ps2controller-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: circuitpython-ps2controller
+Version: 1.2.0
+Summary: CircuitPython library to read Sony PS2 game controllers
+Author-email: Tod Kurt <tod@todbot.com>
+License: MIT
+Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
+Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/x-rst
+Provides-Extra: optional
+License-File: LICENSE
+
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/circuitpython-ps2controller/badge/?version=latest
     :target: https://circuitpython-ps2controller.readthedocs.io/
     :alt: Documentation Status
@@ -14,15 +32,15 @@
     :target: https://github.com/todbot/CircuitPython_PS2Controller/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython library to read Sony PS2 game controllers
+CircuitPython library to read Sony PS2 or PS1 game controllers
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -89,26 +107,48 @@
 
     import board
     from ps2controller import PS2Controller
 
     # one way to wire this up, for example on a Pico
     ps2 = PS2Controller(dat=board.GP2, cmd=board.GP3, att=board.GP4, clk=board.GP5)
 
-    print("hi press buttons")
+    print("hi! Press buttons")
     while True:
         events = ps2.update()
         if events:
             print("events", events)
             print("sticks: L:", ps2.analog_left(), "R:", ps2.analog_right())
 
+Wiring
+======
+
+Wiring to the PSX controller needs four GPIO pins.These can be any pins.
+The wiring is:
+
+* CLK pin - clock OUT to controller (blue wire)
+* CMD pin - command data OUT to controller (orange wire)
+* ATT pin - attention / chip select OUT to controller (yellow wire)
+* DAT pin - data IN from controller (brown wire)
+* GND pin - signal ground (black wire)
+* VCC pin - +3.3V power (red wire)
+* VCC2 pin - +7.5V power to rumble motors (optional)
+
+Here's one way to wire that up on a Raspberry Pi Pico:
+
+.. image:: https://raw.githubusercontent.com/todbot/CircuitPython_PS2Controller/main/docs/ps2controller_wiring.png
+
+(Thanks to `Vanepp <https://forum.fritzing.org/u/vanepp/summary>`_ via `nandanhere/PiPyPS2 <https://github.com/nandanhere/PiPyPS2>`_ for Fritzing wiring diagram)
+
 
 References
 ==========
 
-This library is a fairly direct port of `madsci1016/Arduino-PS2X <https://github.com/madsci1016/Arduino-PS2X>`_.
+This library is highly inspired by the `SukkoPera/PsxNewLib <https://github.com/SukkoPera/PsxNewLib>`_ library.
+It currently has only been tested on a handful of PS1 and PS2 controllers,
+but it should be easy to add any specialized controller tuning.
 
 Other resources that have been helpful:
 
 * https://store.curiousinventor.com/guides/PS2/
 * https://gist.github.com/scanlime/5042071
 * https://gamesx.com/wiki/doku.php?id=controls:playstation_controller
 * https://github.com/SukkoPera/PsxNewLib
```

### Comparing `circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/PKG-INFO` & `circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ps2controller
-Version: 1.1.2
+Version: 1.2.0
 Summary: CircuitPython library to read Sony PS2 game controllers
 Author-email: Tod Kurt <tod@todbot.com>
 License: MIT
 Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
 Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -32,15 +32,15 @@
     :target: https://github.com/todbot/CircuitPython_PS2Controller/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython library to read Sony PS2 game controllers
+CircuitPython library to read Sony PS2 or PS1 game controllers
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -107,26 +107,48 @@
 
     import board
     from ps2controller import PS2Controller
 
     # one way to wire this up, for example on a Pico
     ps2 = PS2Controller(dat=board.GP2, cmd=board.GP3, att=board.GP4, clk=board.GP5)
 
-    print("hi press buttons")
+    print("hi! Press buttons")
     while True:
         events = ps2.update()
         if events:
             print("events", events)
             print("sticks: L:", ps2.analog_left(), "R:", ps2.analog_right())
 
+Wiring
+======
+
+Wiring to the PSX controller needs four GPIO pins.These can be any pins.
+The wiring is:
+
+* CLK pin - clock OUT to controller (blue wire)
+* CMD pin - command data OUT to controller (orange wire)
+* ATT pin - attention / chip select OUT to controller (yellow wire)
+* DAT pin - data IN from controller (brown wire)
+* GND pin - signal ground (black wire)
+* VCC pin - +3.3V power (red wire)
+* VCC2 pin - +7.5V power to rumble motors (optional)
+
+Here's one way to wire that up on a Raspberry Pi Pico:
+
+.. image:: https://raw.githubusercontent.com/todbot/CircuitPython_PS2Controller/main/docs/ps2controller_wiring.png
+
+(Thanks to `Vanepp <https://forum.fritzing.org/u/vanepp/summary>`_ via `nandanhere/PiPyPS2 <https://github.com/nandanhere/PiPyPS2>`_ for Fritzing wiring diagram)
+
 
 References
 ==========
 
-This library is a fairly direct port of `madsci1016/Arduino-PS2X <https://github.com/madsci1016/Arduino-PS2X>`_.
+This library is highly inspired by the `SukkoPera/PsxNewLib <https://github.com/SukkoPera/PsxNewLib>`_ library.
+It currently has only been tested on a handful of PS1 and PS2 controllers,
+but it should be easy to add any specialized controller tuning.
 
 Other resources that have been helpful:
 
 * https://store.curiousinventor.com/guides/PS2/
 * https://gist.github.com/scanlime/5042071
 * https://gamesx.com/wiki/doku.php?id=controls:playstation_controller
 * https://github.com/SukkoPera/PsxNewLib
```

### Comparing `circuitpython-ps2controller-1.1.2/circuitpython_ps2controller.egg-info/SOURCES.txt` & `circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -26,12 +26,16 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/ps2controller_wiring.png
+docs/ps2controller_wiring.png.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/ps2controller_datadump.py
+examples/ps2controller_digital_only.py
 examples/ps2controller_simpletest.py
 examples/ps2controller_usbkeys.py
```

### Comparing `circuitpython-ps2controller-1.1.2/docs/_static/favicon.ico` & `circuitpython-ps2controller-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/docs/conf.py` & `circuitpython-ps2controller-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/docs/index.rst` & `circuitpython-ps2controller-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/examples/ps2controller_usbkeys.py` & `circuitpython-ps2controller-1.2.0/examples/ps2controller_usbkeys.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.1.2/pyproject.toml` & `circuitpython-ps2controller-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-ps2controller"
 description = "CircuitPython library to read Sony PS2 game controllers"
-version = "1.1.2"
+version = "1.2.0"
 readme = "README.rst"
 authors = [
     {name = "Tod Kurt", email = "tod@todbot.com"}
 ]
 urls = {Homepage = "https://github.com/todbot/CircuitPython_PS2Controller"}
 keywords = [
     "adafruit",
```


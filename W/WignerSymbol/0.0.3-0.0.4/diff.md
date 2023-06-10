# Comparing `tmp/WignerSymbol-0.0.3.tar.gz` & `tmp/WignerSymbol-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WignerSymbol-0.0.3.tar", last modified: Sat Jun 10 12:59:46 2023, max compression
+gzip compressed data, was "WignerSymbol-0.0.4.tar", last modified: Sat Jun 10 13:11:30 2023, max compression
```

## Comparing `WignerSymbol-0.0.3.tar` & `WignerSymbol-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:59:46.731632 WignerSymbol-0.0.3/
--rw-rw-rw-   0        0        0     1080 2023-06-10 12:36:47.000000 WignerSymbol-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      232 2023-06-10 12:59:46.729627 WignerSymbol-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-06-10 10:16:15.000000 WignerSymbol-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:59:46.722628 WignerSymbol-0.0.3/WignerSymbol/
--rw-rw-rw-   0        0        0    36389 2023-06-10 08:59:57.000000 WignerSymbol-0.0.3/WignerSymbol/WignerSymbol.hpp
-drwxrwxrwx   0        0        0        0 2023-06-10 12:59:46.728629 WignerSymbol-0.0.3/WignerSymbol.egg-info/
--rw-rw-rw-   0        0        0      232 2023-06-10 12:59:46.000000 WignerSymbol-0.0.3/WignerSymbol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-10 12:59:46.000000 WignerSymbol-0.0.3/WignerSymbol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:59:46.000000 WignerSymbol-0.0.3/WignerSymbol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 10:06:42.000000 WignerSymbol-0.0.3/WignerSymbol.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-10 12:59:46.000000 WignerSymbol-0.0.3/WignerSymbol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3403 2023-06-10 12:52:17.000000 WignerSymbol-0.0.3/lib.cpp
--rw-rw-rw-   0        0        0       67 2023-06-10 10:06:32.000000 WignerSymbol-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 12:59:46.731632 WignerSymbol-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      635 2023-06-10 12:59:34.000000 WignerSymbol-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:11:30.265959 WignerSymbol-0.0.4/
+-rw-rw-rw-   0        0        0     1080 2023-06-10 12:36:47.000000 WignerSymbol-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      232 2023-06-10 13:11:30.265959 WignerSymbol-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-06-10 10:16:15.000000 WignerSymbol-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 13:11:30.255953 WignerSymbol-0.0.4/WignerSymbol/
+-rw-rw-rw-   0        0        0    36389 2023-06-10 08:59:57.000000 WignerSymbol-0.0.4/WignerSymbol/WignerSymbol.hpp
+drwxrwxrwx   0        0        0        0 2023-06-10 13:11:30.264957 WignerSymbol-0.0.4/WignerSymbol.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-06-10 13:11:30.000000 WignerSymbol-0.0.4/WignerSymbol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-10 13:11:30.000000 WignerSymbol-0.0.4/WignerSymbol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 13:11:30.000000 WignerSymbol-0.0.4/WignerSymbol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-10 10:06:42.000000 WignerSymbol-0.0.4/WignerSymbol.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-10 13:11:30.000000 WignerSymbol-0.0.4/WignerSymbol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3403 2023-06-10 12:52:17.000000 WignerSymbol-0.0.4/lib.cpp
+-rw-rw-rw-   0        0        0       67 2023-06-10 10:06:32.000000 WignerSymbol-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:11:30.265959 WignerSymbol-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      635 2023-06-10 13:09:55.000000 WignerSymbol-0.0.4/setup.py
```

### Comparing `WignerSymbol-0.0.3/LICENSE` & `WignerSymbol-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `WignerSymbol-0.0.3/WignerSymbol/WignerSymbol.hpp` & `WignerSymbol-0.0.4/WignerSymbol/WignerSymbol.hpp`

 * *Files identical despite different names*

### Comparing `WignerSymbol-0.0.3/lib.cpp` & `WignerSymbol-0.0.4/lib.cpp`

 * *Files identical despite different names*

### Comparing `WignerSymbol-0.0.3/setup.py` & `WignerSymbol-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 ext_modules = [
     Pybind11Extension("WignerSymbol",
                       ["lib.cpp"],
                       define_macros=[("VERSION", __version__)]
                       ),
 ]
```


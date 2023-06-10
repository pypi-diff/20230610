# Comparing `tmp/atckit-1.0.1.tar.gz` & `tmp/atckit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atckit-1.0.1.tar", last modified: Sat Jun  3 10:31:59 2023, max compression
+gzip compressed data, was "atckit-1.0.2.tar", last modified: Sat Jun 10 20:54:22 2023, max compression
```

## Comparing `atckit-1.0.1.tar` & `atckit-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.596177 atckit-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-03 09:08:12.000000 atckit-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.0.1/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-03 09:08:12.000000 atckit-1.0.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-03 09:48:35.000000 atckit-1.0.1/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.0.1/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.0.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     2151 2023-06-03 10:31:59.592177 atckit-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-06-03 09:08:12.000000 atckit-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.0.1/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.0.1/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.0.1/icon.png
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-03 10:31:52.000000 atckit-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 10:31:59.596177 atckit-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.548178 atckit-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.580178 atckit-1.0.1/src/atckit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 10:20:40.000000 atckit-1.0.1/src/atckit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-06-03 09:44:24.000000 atckit-1.0.1/src/atckit/subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2023-06-03 09:44:24.000000 atckit-1.0.1/src/atckit/utilfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 10:31:59.592177 atckit-1.0.1/src/atckit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2151 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-03 10:31:59.000000 atckit-1.0.1/src/atckit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.764107 atckit-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-03 09:08:12.000000 atckit-1.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-10 20:52:22.000000 atckit-1.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-03 09:08:12.000000 atckit-1.0.2/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-03 09:08:12.000000 atckit-1.0.2/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)   115208 2023-06-10 20:36:02.000000 atckit-1.0.2/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-03 09:08:12.000000 atckit-1.0.2/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-03 09:08:12.000000 atckit-1.0.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-06-10 20:54:22.764107 atckit-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-10 20:36:02.000000 atckit-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-03 09:08:12.000000 atckit-1.0.2/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-03 09:08:12.000000 atckit-1.0.2/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)    23443 2023-06-03 09:08:12.000000 atckit-1.0.2/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-10 20:54:16.000000 atckit-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 20:54:22.764107 atckit-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.760107 atckit-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.764107 atckit-1.0.2/src/atckit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-10 20:53:34.000000 atckit-1.0.2/src/atckit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-06-10 20:40:43.000000 atckit-1.0.2/src/atckit/subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)     4804 2023-06-03 09:44:24.000000 atckit-1.0.2/src/atckit/utilfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 20:54:22.764107 atckit-1.0.2/src/atckit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-10 20:54:22.000000 atckit-1.0.2/src/atckit.egg-info/top_level.txt
```

### Comparing `atckit-1.0.1/.gitlab-ci.yml` & `atckit-1.0.2/.gitlab-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-image: debian:bullseye-slim
+image: python:3.9-slim-bullseye
 
 default:
   tags:
     - atc-runner
     - docker
 
 before_script:
   - apt update
-  - DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true apt -y install make python3 python3-pip python3-venv git curl jq
+  - DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true apt -y install make git curl jq
   - make install_build_deps
 
 stages:
   - lint
   - build
   - dist
```

### Comparing `atckit-1.0.1/.pylintrc` & `atckit-1.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `atckit-1.0.1/Doxyfile` & `atckit-1.0.2/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "AccidentallyTheCable's Utility Kit"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.0.1"
+PROJECT_NUMBER = "1.0.2"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `atckit-1.0.1/LICENSE.md` & `atckit-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atckit-1.0.1/Makefile` & `atckit-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `atckit-1.0.1/PKG-INFO` & `atckit-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: atckit
-Version: 1.0.1
-Summary: AccidentallyTheCable's Utility Kit
-Author-email: AccidentallyTheCable <cableninja@cableninja.net>
-License: GPLv3
-Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
-Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # ATCKit
 
 AccidentallyTheCable's Utility Kit
 
 - [ATCKit](#atckit)
   - [About](#about)
     - [How does it work?](#how-does-it-work)
@@ -57,14 +41,38 @@
 for cb in subscriber.functions:
     cb()
 
 >> I am a teapot
 >> I am definitely totally not also a teapot, I swear
 ```
 
+This class uses the `typing.Callable` type for function storage. You can extend the `FunctionSubscriber` class to define the
+callback function parameters, etc.
+
+```
+class MySubscriber(FunctionSubscriber):
+    """My Function Subscriber
+    Callback: (bool) -> None
+    """
+
+    _functions:list[Callable[[bool],None]]
+
+    def __iadd__(self,fn:Callable[[bool],None]) -> Self:
+        """Inline Add. Subscribe Function
+        @param method \c fn Method to Subscribe
+        """
+        return super().__iadd__(fn)
+
+    def __isub__(self,fn:Callable[[bool],None]) -> Self:
+        """Inline Subtract. Unsubscribe Function
+        @param method \c fn Method to Unsubscribe
+        """
+        return super().__isub__(fn)
+```
+
 ## UtilFuncs
 
 A Class containing various static methods:
 
  - scan_dir: Search a specified Path, and execute a callback function on discovered files.
    - Allows exclusion of Files/Dirs via regex pattern matching
  - deep_sort: Sort a Dictionary recursively, including through lists of dicts
```

### Comparing `atckit-1.0.1/git-tags.sh` & `atckit-1.0.2/git-tags.sh`

 * *Files identical despite different names*

### Comparing `atckit-1.0.1/icon.png` & `atckit-1.0.2/icon.png`

 * *Files identical despite different names*

### Comparing `atckit-1.0.1/pyproject.toml` & `atckit-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atckit"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "AccidentallyTheCable's Utility Kit"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `atckit-1.0.1/src/atckit/subscriber.py` & `atckit-1.0.2/src/atckit/subscriber.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from types import MethodType
+from typing import Callable
 import typing_extensions
 
 class FunctionSubscriber:
     """ Function subscriber
 
 
     Provides a += / -= interface for adding callback functions
@@ -37,38 +37,38 @@
     \li Execute subscribed functions
         \code{.py}
         for method_def in f.functions:
             method_def()
         \endcode
     """
 
-    __functions:list[MethodType]
+    _functions:list[Callable]
 
     @property
-    def functions(self) -> list[MethodType]:
+    def functions(self) -> list[Callable]:
         """\b \e PROPERTY; Currently Subscribed Functions"""
-        return self.__functions
+        return self._functions
 
     def __init__(self) -> None:
         """Initializer
         """
-        self.__functions = []
+        self._functions = []
 
-    def __iadd__(self,fn:MethodType) -> typing_extensions.Self:
+    def __iadd__(self,fn:Callable) -> typing_extensions.Self:
         """Inline Add. Subscribe Function
         @param method \c fn Method to Subscribe
         """
-        if fn not in self.__functions:
+        if fn not in self._functions:
             logging.debug(f"Adding Function {fn.__qualname__}")
-            self.__functions.append(fn)
+            self._functions.append(fn)
         return self
 
-    def __isub__(self,fn:MethodType) -> typing_extensions.Self:
+    def __isub__(self,fn:Callable) -> typing_extensions.Self:
         """Inline Subtract. Unsubscribe Function
         @param method \c fn Method to Unsubscribe
         """
-        if fn not in self.__functions:
+        if fn not in self._functions:
             return self
-        i:int = self.__functions.index(fn)
-        self.__functions.pop(i)
+        i:int = self._functions.index(fn)
+        self._functions.pop(i)
         logging.debug(f"Removing Function {fn.__qualname__}")
         return self
```

### Comparing `atckit-1.0.1/src/atckit/utilfuncs.py` & `atckit-1.0.2/src/atckit/utilfuncs.py`

 * *Files identical despite different names*

### Comparing `atckit-1.0.1/src/atckit.egg-info/PKG-INFO` & `atckit-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atckit
-Version: 1.0.1
+Version: 1.0.2
 Summary: AccidentallyTheCable's Utility Kit
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-atckit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -57,14 +57,38 @@
 for cb in subscriber.functions:
     cb()
 
 >> I am a teapot
 >> I am definitely totally not also a teapot, I swear
 ```
 
+This class uses the `typing.Callable` type for function storage. You can extend the `FunctionSubscriber` class to define the
+callback function parameters, etc.
+
+```
+class MySubscriber(FunctionSubscriber):
+    """My Function Subscriber
+    Callback: (bool) -> None
+    """
+
+    _functions:list[Callable[[bool],None]]
+
+    def __iadd__(self,fn:Callable[[bool],None]) -> Self:
+        """Inline Add. Subscribe Function
+        @param method \c fn Method to Subscribe
+        """
+        return super().__iadd__(fn)
+
+    def __isub__(self,fn:Callable[[bool],None]) -> Self:
+        """Inline Subtract. Unsubscribe Function
+        @param method \c fn Method to Unsubscribe
+        """
+        return super().__isub__(fn)
+```
+
 ## UtilFuncs
 
 A Class containing various static methods:
 
  - scan_dir: Search a specified Path, and execute a callback function on discovered files.
    - Allows exclusion of Files/Dirs via regex pattern matching
  - deep_sort: Sort a Dictionary recursively, including through lists of dicts
```


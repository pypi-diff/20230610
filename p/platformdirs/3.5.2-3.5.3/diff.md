# Comparing `tmp/platformdirs-3.5.2.tar.gz` & `tmp/platformdirs-3.5.3.tar.gz`

## Comparing `platformdirs-3.5.2.tar` & `platformdirs-3.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tox.ini
--rw-r--r--   0        0        0    19758 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/android.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/api.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/py.typed
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/version.py
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 platformdirs-3.5.2/src/platformdirs/windows.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/conftest.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_android.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_api.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_main.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 platformdirs-3.5.2/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.2/LICENSE
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 platformdirs-3.5.2/README.rst
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 platformdirs-3.5.2/pyproject.toml
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 platformdirs-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tox.ini
+-rw-r--r--   0        0        0    19758 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/android.py
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/version.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_android.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_api.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_main.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.3/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.3/LICENSE
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 platformdirs-3.5.3/README.rst
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.5.3/pyproject.toml
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 platformdirs-3.5.3/PKG-INFO
```

### Comparing `platformdirs-3.5.2/tox.ini` & `platformdirs-3.5.3/tox.ini`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/src/platformdirs/__init__.py` & `platformdirs-3.5.3/src/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/src/platformdirs/__main__.py` & `platformdirs-3.5.3/src/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/src/platformdirs/android.py` & `platformdirs-3.5.3/src/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/src/platformdirs/api.py` & `platformdirs-3.5.3/src/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/src/platformdirs/macos.py` & `platformdirs-3.5.3/src/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/src/platformdirs/unix.py` & `platformdirs-3.5.3/src/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/src/platformdirs/windows.py` & `platformdirs-3.5.3/src/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/tests/conftest.py` & `platformdirs-3.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/tests/test_android.py` & `platformdirs-3.5.3/tests/test_android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/tests/test_api.py` & `platformdirs-3.5.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/tests/test_comp_with_appdirs.py` & `platformdirs-3.5.3/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/tests/test_macos.py` & `platformdirs-3.5.3/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/tests/test_unix.py` & `platformdirs-3.5.3/tests/test_unix.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/LICENSE` & `platformdirs-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/README.rst` & `platformdirs-3.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.2/pyproject.toml` & `platformdirs-3.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = [
   "version",
 ]
```

### Comparing `platformdirs-3.5.2/PKG-INFO` & `platformdirs-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.5.2
+Version: 3.5.3
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: typing-extensions>=4.6.3; python_version < '3.8'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.5.20; extra == 'docs'
```


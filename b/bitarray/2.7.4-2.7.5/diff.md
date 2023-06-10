# Comparing `tmp/bitarray-2.7.4.tar.gz` & `tmp/bitarray-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitarray-2.7.4.tar", last modified: Mon May 29 17:34:27 2023, max compression
+gzip compressed data, was "bitarray-2.7.5.tar", last modified: Sat Jun 10 19:58:06 2023, max compression
```

## Comparing `bitarray-2.7.4.tar` & `bitarray-2.7.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:34:27.727053 bitarray-2.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-29 17:34:18.000000 bitarray-2.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-29 17:34:27.727053 bitarray-2.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31369 2023-05-29 17:34:18.000000 bitarray-2.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:34:27.727053 bitarray-2.7.4/bitarray/
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   117036 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/_bitarray.c
--rw-r--r--   0 runner    (1001) docker     (123)    62981 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/_util.c
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/bitarray.h
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/pythoncapi_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)   164438 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/test_bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/test_data.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    87937 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-29 17:34:18.000000 bitarray-2.7.4/bitarray/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:34:27.727053 bitarray-2.7.4/bitarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-29 17:34:27.000000 bitarray-2.7.4/bitarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-29 17:34:27.000000 bitarray-2.7.4/bitarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:34:27.000000 bitarray-2.7.4/bitarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:34:27.000000 bitarray-2.7.4/bitarray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 17:34:27.000000 bitarray-2.7.4/bitarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:34:27.727053 bitarray-2.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-29 17:34:18.000000 bitarray-2.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:58:06.272013 bitarray-2.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-10 19:57:58.000000 bitarray-2.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-06-10 19:58:06.272013 bitarray-2.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31369 2023-06-10 19:57:58.000000 bitarray-2.7.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:58:06.268013 bitarray-2.7.5/bitarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   117036 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/_bitarray.c
+-rw-r--r--   0 runner    (1001) docker     (123)    62981 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/bitarray.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/pythoncapi_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)   164438 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/test_bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/test_data.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    87937 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-10 19:57:58.000000 bitarray-2.7.5/bitarray/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:58:06.272013 bitarray-2.7.5/bitarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-06-10 19:58:06.000000 bitarray-2.7.5/bitarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-10 19:58:06.000000 bitarray-2.7.5/bitarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:58:06.000000 bitarray-2.7.5/bitarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:58:06.000000 bitarray-2.7.5/bitarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 19:58:06.000000 bitarray-2.7.5/bitarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:58:06.272013 bitarray-2.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-10 19:57:58.000000 bitarray-2.7.5/setup.py
```

### Comparing `bitarray-2.7.4/LICENSE` & `bitarray-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/PKG-INFO` & `bitarray-2.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitarray
-Version: 2.7.4
+Version: 2.7.5
 Summary: efficient arrays of booleans -- C extension
 Home-page: https://github.com/ilanschnell/bitarray
 Author: Ilan Schnell
 Author-email: ilanschnell@gmail.com
 License: PSF
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Development Status :: 6 - Mature
@@ -86,15 +86,15 @@
 
 Once you have installed the package, you may want to test it:
 
 .. code-block:: shell-session
 
     $ python -c 'import bitarray; bitarray.test()'
     bitarray is installed in: /Users/ilan/bitarray/bitarray
-    bitarray version: 2.7.4
+    bitarray version: 2.7.5
     sys.version: 3.11.0 (main, Oct 25 2022) [Clang 14.0.4]
     sys.prefix: /Users/ilan/Mini3/envs/py311
     pointer size: 64 bit
     sizeof(size_t): 8
     sizeof(bitarrayobject): 80
     __clang__ or __GNUC__ defined: 1
     PY_LITTLE_ENDIAN (use word shift): 1
@@ -430,15 +430,15 @@
         ...
     TypeError: frozenbitarray is immutable
 
 
 Reference
 =========
 
-bitarray version: 2.7.4 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
+bitarray version: 2.7.5 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
 
 In the following, ``item`` and ``value`` are usually a single bit -
 an integer 0 or 1.
 
 
 The bitarray object:
 --------------------
```

### Comparing `bitarray-2.7.4/README.rst` & `bitarray-2.7.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 Once you have installed the package, you may want to test it:
 
 .. code-block:: shell-session
 
     $ python -c 'import bitarray; bitarray.test()'
     bitarray is installed in: /Users/ilan/bitarray/bitarray
-    bitarray version: 2.7.4
+    bitarray version: 2.7.5
     sys.version: 3.11.0 (main, Oct 25 2022) [Clang 14.0.4]
     sys.prefix: /Users/ilan/Mini3/envs/py311
     pointer size: 64 bit
     sizeof(size_t): 8
     sizeof(bitarrayobject): 80
     __clang__ or __GNUC__ defined: 1
     PY_LITTLE_ENDIAN (use word shift): 1
@@ -403,15 +403,15 @@
         ...
     TypeError: frozenbitarray is immutable
 
 
 Reference
 =========
 
-bitarray version: 2.7.4 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
+bitarray version: 2.7.5 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
 
 In the following, ``item`` and ``value`` are usually a single bit -
 an integer 0 or 1.
 
 
 The bitarray object:
 --------------------
```

### Comparing `bitarray-2.7.4/bitarray/__init__.py` & `bitarray-2.7.5/bitarray/__init__.py`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray/__init__.pyi` & `bitarray-2.7.5/bitarray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray/_bitarray.c` & `bitarray-2.7.5/bitarray/_bitarray.c`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray/_util.c` & `bitarray-2.7.5/bitarray/_util.c`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray/bitarray.h` & `bitarray-2.7.5/bitarray/bitarray.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
    Copyright (c) 2008 - 2023, Ilan Schnell; All Rights Reserved
    bitarray is published under the PSF license.
 
    Author: Ilan Schnell
 */
-#define BITARRAY_VERSION  "2.7.4"
+#define BITARRAY_VERSION  "2.7.5"
 
 #ifdef STDC_HEADERS
 #include <stddef.h>
 #else  /* !STDC_HEADERS */
 #ifdef HAVE_SYS_TYPES_H
 #include <sys/types.h>      /* For size_t */
 #endif /* HAVE_SYS_TYPES_H */
```

### Comparing `bitarray-2.7.4/bitarray/pythoncapi_compat.h` & `bitarray-2.7.5/bitarray/pythoncapi_compat.h`

 * *Files 1% similar despite different names*

```diff
@@ -386,26 +386,28 @@
     tstate->use_tracing = use_tracing;
 #endif
 }
 #endif
 
 
 // bpo-37194 added PyObject_CallNoArgs() to Python 3.9.0a1
-#if PY_VERSION_HEX < 0x030900A1 || defined(PYPY_VERSION)
+// PyObject_CallNoArgs() added to PyPy 3.9.16-v7.3.11
+#if !defined(PyObject_CallNoArgs) && PY_VERSION_HEX < 0x030900A1
 PYCAPI_COMPAT_STATIC_INLINE(PyObject*)
 PyObject_CallNoArgs(PyObject *func)
 {
     return PyObject_CallFunctionObjArgs(func, NULL);
 }
 #endif
 
 
 // bpo-39245 made PyObject_CallOneArg() public (previously called
 // _PyObject_CallOneArg) in Python 3.9.0a4
-#if PY_VERSION_HEX < 0x030900A4 || defined(PYPY_VERSION)
+// PyObject_CallOneArg() added to PyPy 3.9.16-v7.3.11
+#if !defined(PyObject_CallOneArg) && PY_VERSION_HEX < 0x030900A4
 PYCAPI_COMPAT_STATIC_INLINE(PyObject*)
 PyObject_CallOneArg(PyObject *func, PyObject *arg)
 {
     return PyObject_CallFunctionObjArgs(func, arg, NULL);
 }
 #endif
```

### Comparing `bitarray-2.7.4/bitarray/test_bitarray.py` & `bitarray-2.7.5/bitarray/test_bitarray.py`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray/test_util.py` & `bitarray-2.7.5/bitarray/test_util.py`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray/util.py` & `bitarray-2.7.5/bitarray/util.py`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray/util.pyi` & `bitarray-2.7.5/bitarray/util.pyi`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.4/bitarray.egg-info/PKG-INFO` & `bitarray-2.7.5/bitarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitarray
-Version: 2.7.4
+Version: 2.7.5
 Summary: efficient arrays of booleans -- C extension
 Home-page: https://github.com/ilanschnell/bitarray
 Author: Ilan Schnell
 Author-email: ilanschnell@gmail.com
 License: PSF
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Development Status :: 6 - Mature
@@ -86,15 +86,15 @@
 
 Once you have installed the package, you may want to test it:
 
 .. code-block:: shell-session
 
     $ python -c 'import bitarray; bitarray.test()'
     bitarray is installed in: /Users/ilan/bitarray/bitarray
-    bitarray version: 2.7.4
+    bitarray version: 2.7.5
     sys.version: 3.11.0 (main, Oct 25 2022) [Clang 14.0.4]
     sys.prefix: /Users/ilan/Mini3/envs/py311
     pointer size: 64 bit
     sizeof(size_t): 8
     sizeof(bitarrayobject): 80
     __clang__ or __GNUC__ defined: 1
     PY_LITTLE_ENDIAN (use word shift): 1
@@ -430,15 +430,15 @@
         ...
     TypeError: frozenbitarray is immutable
 
 
 Reference
 =========
 
-bitarray version: 2.7.4 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
+bitarray version: 2.7.5 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
 
 In the following, ``item`` and ``value`` are usually a single bit -
 an integer 0 or 1.
 
 
 The bitarray object:
 --------------------
```

### Comparing `bitarray-2.7.4/setup.py` & `bitarray-2.7.5/setup.py`

 * *Files identical despite different names*


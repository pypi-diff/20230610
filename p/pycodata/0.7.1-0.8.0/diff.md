# Comparing `tmp/pycodata-0.7.1.tar.gz` & `tmp/pycodata-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodata-0.7.1.tar", last modified: Tue May  2 16:46:51 2023, max compression
+gzip compressed data, was "pycodata-0.8.0.tar", last modified: Sat Jun 10 05:09:58 2023, max compression
```

## Comparing `pycodata-0.7.1.tar` & `pycodata-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.799064 pycodata-0.7.1/
--rw-r--r--   0 milan      (501) staff       (20)       20 2023-04-22 07:20:52.000000 pycodata-0.7.1/INSTALL.TXT
--rw-r--r--   0 milan      (501) staff       (20)    35823 2023-04-22 07:20:52.000000 pycodata-0.7.1/LICENSE.TXT
--rw-r--r--   0 milan      (501) staff       (20)      195 2023-04-22 07:20:52.000000 pycodata-0.7.1/MANIFEST.in
--rw-r--r--   0 milan      (501) staff       (20)      996 2023-05-02 16:46:51.798020 pycodata-0.7.1/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)      418 2023-04-26 19:43:03.000000 pycodata-0.7.1/README.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.792064 pycodata-0.7.1/pycodata/
--rw-r--r--   0 milan      (501) staff       (20)       97 2023-04-22 07:20:52.000000 pycodata-0.7.1/pycodata/__init__.py
--rw-r--r--   0 milan      (501) staff       (20)    49602 2023-05-02 16:27:41.000000 pycodata-0.7.1/pycodata/codata.h
--rw-r--r--   0 milan      (501) staff       (20)    94969 2023-04-27 23:24:15.000000 pycodata-0.7.1/pycodata/cpycodata.c
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.796475 pycodata-0.7.1/pycodata/tests/
--rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.1/pycodata/tests/__init__.py
--rw-r--r--   0 milan      (501) staff       (20)      365 2023-04-27 23:38:11.000000 pycodata-0.7.1/pycodata/tests/test.py
--rw-r--r--   0 milan      (501) staff       (20)      555 2023-05-02 16:31:16.000000 pycodata-0.7.1/pycodata/version.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-02 16:46:51.795218 pycodata-0.7.1/pycodata.egg-info/
--rw-r--r--   0 milan      (501) staff       (20)      996 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)      365 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/SOURCES.txt
--rw-r--r--   0 milan      (501) staff       (20)        1 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/dependency_links.txt
--rw-r--r--   0 milan      (501) staff       (20)        9 2023-05-02 16:46:51.000000 pycodata-0.7.1/pycodata.egg-info/top_level.txt
--rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.7.1/requirements.txt
--rw-r--r--   0 milan      (501) staff       (20)       38 2023-05-02 16:46:51.799263 pycodata-0.7.1/setup.cfg
--rw-r--r--   0 milan      (501) staff       (20)     1562 2023-04-28 05:03:25.000000 pycodata-0.7.1/setup.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-06-10 05:09:58.111010 pycodata-0.8.0/
+-rw-r--r--   0 milan      (501) staff       (20)       50 2023-06-10 04:50:24.000000 pycodata-0.8.0/INSTALL.rst
+-rw-r--r--   0 milan      (501) staff       (20)    35823 2023-04-22 07:20:52.000000 pycodata-0.8.0/LICENSE.TXT
+-rw-r--r--   0 milan      (501) staff       (20)      199 2023-06-10 04:50:24.000000 pycodata-0.8.0/MANIFEST.in
+-rw-r--r--   0 milan      (501) staff       (20)      887 2023-06-10 05:09:58.110223 pycodata-0.8.0/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)      309 2023-06-10 04:50:24.000000 pycodata-0.8.0/README.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-06-10 05:09:58.094015 pycodata-0.8.0/pycodata/
+-rw-r--r--   0 milan      (501) staff       (20)       97 2023-04-22 07:20:52.000000 pycodata-0.8.0/pycodata/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)    52316 2023-06-10 05:08:59.000000 pycodata-0.8.0/pycodata/codata.h
+-rw-r--r--   0 milan      (501) staff       (20)    94969 2023-06-10 05:08:58.000000 pycodata-0.8.0/pycodata/cpycodata.c
+-rw-r--r--   0 milan      (501) staff       (20)    57024 2023-06-10 05:08:59.000000 pycodata-0.8.0/pycodata/libcodata.a
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-06-10 05:09:58.108004 pycodata-0.8.0/pycodata/tests/
+-rw-r--r--   0 milan      (501) staff       (20)        0 2023-05-02 17:06:30.000000 pycodata-0.8.0/pycodata/tests/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)      365 2023-05-02 17:06:30.000000 pycodata-0.8.0/pycodata/tests/test.py
+-rw-r--r--   0 milan      (501) staff       (20)      555 2023-06-10 04:50:24.000000 pycodata-0.8.0/pycodata/version.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-06-10 05:09:58.105128 pycodata-0.8.0/pycodata.egg-info/
+-rw-r--r--   0 milan      (501) staff       (20)      887 2023-06-10 05:09:57.000000 pycodata-0.8.0/pycodata.egg-info/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)      386 2023-06-10 05:09:57.000000 pycodata-0.8.0/pycodata.egg-info/SOURCES.txt
+-rw-r--r--   0 milan      (501) staff       (20)        1 2023-06-10 05:09:57.000000 pycodata-0.8.0/pycodata.egg-info/dependency_links.txt
+-rw-r--r--   0 milan      (501) staff       (20)        9 2023-06-10 05:09:57.000000 pycodata-0.8.0/pycodata.egg-info/top_level.txt
+-rw-r--r--   0 milan      (501) staff       (20)        0 2023-04-22 07:20:52.000000 pycodata-0.8.0/requirements.txt
+-rw-r--r--   0 milan      (501) staff       (20)       38 2023-06-10 05:09:58.111144 pycodata-0.8.0/setup.cfg
+-rw-r--r--   0 milan      (501) staff       (20)     1658 2023-06-10 04:50:24.000000 pycodata-0.8.0/setup.py
```

### Comparing `pycodata-0.7.1/LICENSE.TXT` & `pycodata-0.8.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `pycodata-0.7.1/pycodata/cpycodata.c` & `pycodata-0.8.0/pycodata/cpycodata.c`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PyMODINIT_FUNC PyInit_codata(void){
 	PyObject *m;
 	PyObject *d;
 	PyObject *v;
 	m = PyModule_Create(&codata);
 	d = PyModule_GetDict(m);
 
-	v = PyLong_FromLong(2018);
+	v = PyLong_FromLong(YEAR);
 	PyDict_SetItemString(d, "YEAR", v);
 	Py_INCREF(v);
 
 	v = PyFloat_FromDouble(ALPHA_PARTICLE_ELECTRON_MASS_RATIO);
 	PyDict_SetItemString(d, "ALPHA_PARTICLE_ELECTRON_MASS_RATIO", v);
 	Py_INCREF(v);
 	v = PyFloat_FromDouble(U_ALPHA_PARTICLE_ELECTRON_MASS_RATIO);
```

### Comparing `pycodata-0.7.1/pycodata/version.py` & `pycodata-0.8.0/pycodata/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,14 @@
            '__author_email__',
            '__maintainer__',
            '__maintainer_email__',
            '__copyright__',
            '__license__']
 
 __package_name__ = "pycodata"
-__version__ = "0.7.1"
+__version__ = "0.8.0"
 __author__ = "Milan Skocic"
 __author_email__ = "milan.skocic@icloud.com"
 __maintainer__ = __author__
 __maintainer_email__ = __author_email__
 __copyright__ = 'Copyright (C) 2023 ' + __author__
 __license__ = 'GNU General Public License v3 (GPLv3)'
```

### Comparing `pycodata-0.7.1/setup.py` & `pycodata-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 # Import only version.py file for extracting the version
 spec = importlib.util.spec_from_file_location('version', './pycodata/version.py')
 mod = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(mod)
 
 if __name__ == "__main__":
 
-    mod_ext = Extension(name="pycodata.codata", sources=["./pycodata/cpycodata.c"])
+    mod_ext = Extension(name="pycodata.codata", 
+                        sources=["./pycodata/cpycodata.c"], 
+                        extra_objects=["./pycodata/libcodata.a"])
+    
     setup(name=mod.__package_name__,
         version=mod.__version__,
         maintainer=mod.__maintainer__,
         maintainer_email=mod.__maintainer_email__,
         author=mod.__author__,
         author_email=mod.__author_email__,
         description=mod.__package_name__,
         long_description=pathlib.Path("README.rst").read_text(encoding="utf-8"),
         long_description_content_type="text/x-rst",
         url='https://milanskocic.github.io/codata/index.html',
         download_url='https://github.com/MilanSkocic/codata',
         packages=find_packages(),
-        include_package_data=False,
-        python_requires='>=3.7',
+        include_package_data=True,
+        python_requires='>=3.8',
         install_requires=pathlib.Path("requirements.txt").read_text(encoding="utf-8").split('\n'),
         classifiers=["Development Status :: 5 - Production/Stable",
                     "Intended Audience :: Science/Research",
                     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"],
         ext_modules=[mod_ext]
         )
```


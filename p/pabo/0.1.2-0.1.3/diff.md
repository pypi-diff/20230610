# Comparing `tmp/pabo-0.1.2.tar.gz` & `tmp/pabo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pabo-0.1.2.tar", last modified: Sat Jun 10 13:48:17 2023, max compression
+gzip compressed data, was "pabo-0.1.3.tar", last modified: Sat Jun 10 14:19:06 2023, max compression
```

## Comparing `pabo-0.1.2.tar` & `pabo-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.890246 pabo-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-10 13:48:06.000000 pabo-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-10 13:48:06.000000 pabo-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 13:48:06.000000 pabo-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-10 13:48:06.000000 pabo-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-10 13:48:06.000000 pabo-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-10 13:48:17.890246 pabo-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-10 13:48:06.000000 pabo-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-10 13:48:06.000000 pabo-0.1.2/assets/doc_cov.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-10 13:48:06.000000 pabo-0.1.2/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-10 13:48:06.000000 pabo-0.1.2/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-10 13:48:06.000000 pabo-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-10 13:48:17.890246 pabo-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-10 13:48:06.000000 pabo-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.886246 pabo-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.890246 pabo-0.1.2/src/pabo/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/bits.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/core.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/specify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-10 13:48:06.000000 pabo-0.1.2/src/pabo/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:48:17.890246 pabo-0.1.2/src/pabo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 13:48:17.000000 pabo-0.1.2/src/pabo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.758644 pabo-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.754644 pabo-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.754644 pabo-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-10 14:18:57.000000 pabo-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-10 14:18:57.000000 pabo-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 14:18:57.000000 pabo-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-10 14:18:57.000000 pabo-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-10 14:18:57.000000 pabo-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-10 14:19:06.758644 pabo-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-10 14:18:57.000000 pabo-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.754644 pabo-0.1.3/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-10 14:18:57.000000 pabo-0.1.3/assets/doc_cov.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.754644 pabo-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-10 14:18:57.000000 pabo-0.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-10 14:18:57.000000 pabo-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.758644 pabo-0.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-10 14:18:57.000000 pabo-0.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-10 14:18:57.000000 pabo-0.1.3/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-10 14:18:57.000000 pabo-0.1.3/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-10 14:18:57.000000 pabo-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-10 14:19:06.758644 pabo-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-10 14:18:57.000000 pabo-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.754644 pabo-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.758644 pabo-0.1.3/src/pabo/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 14:19:06.000000 pabo-0.1.3/src/pabo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/core.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/specify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-10 14:18:57.000000 pabo-0.1.3/src/pabo/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:19:06.758644 pabo-0.1.3/src/pabo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-10 14:19:06.000000 pabo-0.1.3/src/pabo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-10 14:19:06.000000 pabo-0.1.3/src/pabo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:19:06.000000 pabo-0.1.3/src/pabo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:19:06.000000 pabo-0.1.3/src/pabo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-10 14:19:06.000000 pabo-0.1.3/src/pabo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 14:19:06.000000 pabo-0.1.3/src/pabo.egg-info/top_level.txt
```

### Comparing `pabo-0.1.2/.github/workflows/release.yml` & `pabo-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/LICENSE` & `pabo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/PKG-INFO` & `pabo-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pabo
-Version: 0.1.2
+Version: 0.1.3
 Summary: "Binary parsing for dummies!"
 Home-page: https://github.com/astrogewgaw/pabo
 Author: "Ujjwal Panda"
 Author-email: "ujjwalpanda97@gmail.com"
 License: MIT License
 Project-URL: Source Code, https://github.com/astrogewgaw/pabo
 Project-URL: Documentation, https://pabo.readthedocs.io/en/latest
@@ -12,14 +12,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <img
```

### Comparing `pabo-0.1.2/README.md` & `pabo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/assets/doc_cov.svg` & `pabo-0.1.3/assets/doc_cov.svg`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/justfile` & `pabo-0.1.3/justfile`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/pyproject.toml` & `pabo-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/setup.cfg` & `pabo-0.1.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 	Operating System :: Unix
 	Operating System :: MacOS :: MacOS X
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 
 [options]
 zip_safe = False
 packages = find:
 package_dir = =src
 use_scm_version = True
 python_requires = >=3.6
 include_package_data = True
 setup_requires = setuptools_scm
-install_requires = attrs>=20.1.0; numpy>=1.20.0
+install_requires = attrs>=20.1.0; numpy>=1.19.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pabo-0.1.2/src/pabo/__init__.py` & `pabo-0.1.3/src/pabo/__init__.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/base.py` & `pabo-0.1.3/src/pabo/base.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/bits.py` & `pabo-0.1.3/src/pabo/bits.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/bytes.py` & `pabo-0.1.3/src/pabo/bytes.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/core.cpp` & `pabo-0.1.3/src/pabo/core.cpp`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/numeric.py` & `pabo-0.1.3/src/pabo/numeric.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/specify.py` & `pabo-0.1.3/src/pabo/specify.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/strings.py` & `pabo-0.1.3/src/pabo/strings.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo/wrappers.py` & `pabo-0.1.3/src/pabo/wrappers.py`

 * *Files identical despite different names*

### Comparing `pabo-0.1.2/src/pabo.egg-info/PKG-INFO` & `pabo-0.1.3/src/pabo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pabo
-Version: 0.1.2
+Version: 0.1.3
 Summary: "Binary parsing for dummies!"
 Home-page: https://github.com/astrogewgaw/pabo
 Author: "Ujjwal Panda"
 Author-email: "ujjwalpanda97@gmail.com"
 License: MIT License
 Project-URL: Source Code, https://github.com/astrogewgaw/pabo
 Project-URL: Documentation, https://pabo.readthedocs.io/en/latest
@@ -12,14 +12,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <img
```

### Comparing `pabo-0.1.2/src/pabo.egg-info/SOURCES.txt` & `pabo-0.1.3/src/pabo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


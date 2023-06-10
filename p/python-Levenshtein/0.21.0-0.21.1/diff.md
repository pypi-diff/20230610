# Comparing `tmp/python-Levenshtein-0.21.0.tar.gz` & `tmp/python-Levenshtein-0.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-Levenshtein-0.21.0.tar", last modified: Wed Apr 19 23:02:01 2023, max compression
+gzip compressed data, was "python-Levenshtein-0.21.1.tar", last modified: Sat Jun 10 14:58:47 2023, max compression
```

## Comparing `python-Levenshtein-0.21.0.tar` & `python-Levenshtein-0.21.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 23:01:50.000000 python-Levenshtein-0.21.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:02:01.000000 python-Levenshtein-0.21.0/python_Levenshtein.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-19 23:02:01.624031 python-Levenshtein-0.21.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:58:47.531758 python-Levenshtein-0.21.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-06-10 14:58:37.000000 python-Levenshtein-0.21.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-10 14:58:37.000000 python-Levenshtein-0.21.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 14:58:37.000000 python-Levenshtein-0.21.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-10 14:58:47.531758 python-Levenshtein-0.21.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-10 14:58:37.000000 python-Levenshtein-0.21.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 14:58:37.000000 python-Levenshtein-0.21.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:58:47.531758 python-Levenshtein-0.21.1/python_Levenshtein.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-10 14:58:47.000000 python-Levenshtein-0.21.1/python_Levenshtein.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-10 14:58:47.000000 python-Levenshtein-0.21.1/python_Levenshtein.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:58:47.000000 python-Levenshtein-0.21.1/python_Levenshtein.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 14:58:47.000000 python-Levenshtein-0.21.1/python_Levenshtein.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:58:47.000000 python-Levenshtein-0.21.1/python_Levenshtein.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-10 14:58:47.531758 python-Levenshtein-0.21.1/setup.cfg
```

### Comparing `python-Levenshtein-0.21.0/COPYING` & `python-Levenshtein-0.21.1/COPYING`

 * *Files identical despite different names*

### Comparing `python-Levenshtein-0.21.0/HISTORY.md` & `python-Levenshtein-0.21.1/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## Changelog
 
+### v0.21.1
+#### Changed
+- upgrade ``rapidfuzz-cpp`` to ``v2.0.0``
+
 ### v0.21.0
 #### Changed
 - relax dependency requirement on ``rapidfuzz``
 
 ### v0.20.9
 #### Fixed
 - fix function signature of `get_requires_for_build_wheel`
@@ -89,15 +93,15 @@
 * Fixed out of bound reads due to uninitialized variable in median
   * e.g. quickmedian(["test", "teste"], [0, 0]) caused out of bound reads
 
 #### Changed
 * Use a faster editops implementation provided by RapidFuzz
 * Reduce code duplication
 * reuse implementations from rapidfuzz-cpp
-* Transition to scikit-build 
+* Transition to scikit-build
 
 ### v0.17.0
 * Removed support for Python 3.5
 
 ### v0.16.1
 * Add support for RapidFuzz v1.9.*
```

### Comparing `python-Levenshtein-0.21.0/PKG-INFO` & `python-Levenshtein-0.21.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-Levenshtein
-Version: 0.21.0
+Version: 0.21.1
 Summary: Python extension for computing string edit distances and similarities.
 Home-page: https://github.com/maxbachmann/python-Levenshtein
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: GPL-2.0-or-later
 Keywords: string,Levenshtein,comparison,edit-distance
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.21.0 Summary: Python
+Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.21.1 Summary: Python
 extension for computing string edit distances and similarities. Home-page:
 https://github.com/maxbachmann/python-Levenshtein Author: Max Bachmann Author-
 email: pypi@maxbachmann.de License: GPL-2.0-or-later Keywords:
 string,Levenshtein,comparison,edit-distance Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `python-Levenshtein-0.21.0/README.md` & `python-Levenshtein-0.21.1/README.md`

 * *Files identical despite different names*

### Comparing `python-Levenshtein-0.21.0/python_Levenshtein.egg-info/PKG-INFO` & `python-Levenshtein-0.21.1/python_Levenshtein.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-Levenshtein
-Version: 0.21.0
+Version: 0.21.1
 Summary: Python extension for computing string edit distances and similarities.
 Home-page: https://github.com/maxbachmann/python-Levenshtein
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: GPL-2.0-or-later
 Keywords: string,Levenshtein,comparison,edit-distance
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.21.0 Summary: Python
+Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.21.1 Summary: Python
 extension for computing string edit distances and similarities. Home-page:
 https://github.com/maxbachmann/python-Levenshtein Author: Max Bachmann Author-
 email: pypi@maxbachmann.de License: GPL-2.0-or-later Keywords:
 string,Levenshtein,comparison,edit-distance Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `python-Levenshtein-0.21.0/setup.cfg` & `python-Levenshtein-0.21.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-Levenshtein
-version = 0.21.0
+version = 0.21.1
 description = Python extension for computing string edit distances and similarities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Max Bachmann
 author_email = pypi@maxbachmann.de
 url = https://github.com/maxbachmann/python-Levenshtein
 license = GPL-2.0-or-later
@@ -18,13 +18,13 @@
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 keywords = string, Levenshtein, comparison, edit-distance
 
 [options]
 python_requires = >=3.6
 install_requires = 
-	Levenshtein==0.21.0
+	Levenshtein==0.21.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


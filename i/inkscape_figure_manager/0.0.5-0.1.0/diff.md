# Comparing `tmp/inkscape_figure_manager-0.0.5.tar.gz` & `tmp/inkscape_figure_manager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_figure_manager-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "inkscape_figure_manager-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `inkscape_figure_manager-0.0.5.tar` & `inkscape_figure_manager-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.5/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/LICENSE
--rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.0.5/MANIFEST.in
--rw-r--r--   0        0        0      241 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/Pipfile
--rw-r--r--   0        0        0    28498 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/Pipfile.lock
--rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.0.5/README.md
--rw-r--r--   0        0        0      709 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/__init__.py
--rw-r--r--   0        0        0     8802 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/__main__.py
--rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/daemon.py
--rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/picker.py
--rw-r--r--   0        0        0     1989 2023-04-19 20:08:36.387298 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/template.svg
--rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher.py
--rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher_daemon.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.1.0/LICENSE
+-rw-r--r--   0        0        0       55 2023-04-01 20:00:47.807876 inkscape_figure_manager-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0      241 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.1.0/Pipfile
+-rw-r--r--   0        0        0    28498 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.1.0/Pipfile.lock
+-rw-r--r--   0        0        0     1038 2023-04-15 21:12:40.220852 inkscape_figure_manager-0.1.0/README.md
+-rw-r--r--   0        0        0      709 2023-06-10 21:23:55.459957 inkscape_figure_manager-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/__init__.py
+-rw-r--r--   0        0        0     8802 2023-06-10 21:13:37.556648 inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/__main__.py
+-rw-r--r--   0        0        0     4022 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/daemon.py
+-rw-r--r--   0        0        0     1427 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/picker.py
+-rw-r--r--   0        0        0     1989 2023-04-19 20:08:36.387298 inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/template.svg
+-rw-r--r--   0        0        0     3354 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/watcher.py
+-rw-r--r--   0        0        0     2504 2023-04-17 19:01:50.566703 inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/watcher_daemon.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 inkscape_figure_manager-0.1.0/PKG-INFO
```

### Comparing `inkscape_figure_manager-0.0.5/LICENSE` & `inkscape_figure_manager-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/Pipfile.lock` & `inkscape_figure_manager-0.1.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/README.md` & `inkscape_figure_manager-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/pyproject.toml` & `inkscape_figure_manager-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = 'inkscape_figure_manager'
-version = '0.0.5'
+version = '0.1.0'
 authors = [
   { name="Silas Waxter" },
   { name="Gille Castel" },
 ]
 description = "An API for managing inkscape figures."
 readme = "README.md"
 classifiers = [
```

### Comparing `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/__main__.py` & `inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/daemon.py` & `inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/picker.py` & `inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/picker.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/template.svg` & `inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/template.svg`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher.py` & `inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/watcher.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/src/inkscape_figure_manager/watcher_daemon.py` & `inkscape_figure_manager-0.1.0/src/inkscape_figure_manager/watcher_daemon.py`

 * *Files identical despite different names*

### Comparing `inkscape_figure_manager-0.0.5/PKG-INFO` & `inkscape_figure_manager-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_figure_manager
-Version: 0.0.5
+Version: 0.1.0
 Summary: An API for managing inkscape figures.
 Author: Silas Waxter, Gille Castel
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Dist: click
 Requires-Dist: appdirs
```


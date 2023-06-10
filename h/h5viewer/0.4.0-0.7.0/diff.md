# Comparing `tmp/h5viewer-0.4.0.tar.gz` & `tmp/h5viewer-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5viewer-0.4.0.tar", last modified: Sun Feb 19 23:29:25 2023, max compression
+gzip compressed data, was "h5viewer-0.7.0.tar", last modified: Sat Jun 10 12:10:47 2023, max compression
```

## Comparing `h5viewer-0.4.0.tar` & `h5viewer-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 23:29:25.474820 h5viewer-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-02-19 23:29:08.000000 h5viewer-0.4.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-19 23:29:08.000000 h5viewer-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-02-19 23:29:25.474820 h5viewer-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-19 23:29:08.000000 h5viewer-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-19 23:29:08.000000 h5viewer-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 23:29:25.474820 h5viewer-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-19 23:29:08.000000 h5viewer-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 23:29:25.470820 h5viewer-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 23:29:25.470820 h5viewer-0.4.0/src/h5viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-19 23:29:08.000000 h5viewer-0.4.0/src/h5viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-19 23:29:08.000000 h5viewer-0.4.0/src/h5viewer/hdf5_viewer.bat
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-02-19 23:29:08.000000 h5viewer-0.4.0/src/h5viewer/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 23:29:25.470820 h5viewer-0.4.0/src/h5viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-02-19 23:29:25.000000 h5viewer-0.4.0/src/h5viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-19 23:29:25.000000 h5viewer-0.4.0/src/h5viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 23:29:25.000000 h5viewer-0.4.0/src/h5viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-19 23:29:25.000000 h5viewer-0.4.0/src/h5viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-19 23:29:25.000000 h5viewer-0.4.0/src/h5viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-19 23:29:25.000000 h5viewer-0.4.0/src/h5viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:10:47.112730 h5viewer-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-10 12:10:30.000000 h5viewer-0.7.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-10 12:10:30.000000 h5viewer-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-10 12:10:47.112730 h5viewer-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-10 12:10:30.000000 h5viewer-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:10:47.108730 h5viewer-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:10:47.108730 h5viewer-0.7.0/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-10 12:10:30.000000 h5viewer-0.7.0/docs/releases/0.7.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 12:10:30.000000 h5viewer-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 12:10:47.112730 h5viewer-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-10 12:10:30.000000 h5viewer-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:10:47.108730 h5viewer-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:10:47.112730 h5viewer-0.7.0/src/h5viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 12:10:30.000000 h5viewer-0.7.0/src/h5viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 12:10:30.000000 h5viewer-0.7.0/src/h5viewer/hdf5_viewer.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-06-10 12:10:30.000000 h5viewer-0.7.0/src/h5viewer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:10:47.112730 h5viewer-0.7.0/src/h5viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-10 12:10:47.000000 h5viewer-0.7.0/src/h5viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-10 12:10:47.000000 h5viewer-0.7.0/src/h5viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:10:47.000000 h5viewer-0.7.0/src/h5viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-10 12:10:47.000000 h5viewer-0.7.0/src/h5viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 12:10:47.000000 h5viewer-0.7.0/src/h5viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 12:10:47.000000 h5viewer-0.7.0/src/h5viewer.egg-info/top_level.txt
```

### Comparing `h5viewer-0.4.0/LICENCE` & `h5viewer-0.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `h5viewer-0.4.0/PKG-INFO` & `h5viewer-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5viewer
-Version: 0.4.0
+Version: 0.7.0
 Summary: Viewer for hdf5 files created by labmate
 Home-page: https://github.com/kyrylo-gr/h5viewer
 Author: LKB-OMQ
 Author-email: cryo.paris.su@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -38,40 +38,40 @@
 ```python
 # SOURCE: C:\ProgramData\Anaconda3\Scripts\activate.bat&&conda activate pyqt
 ```
 
 ### How to run code before your analyze cell. `init_analyse.py`
 If you want to set up any variables or imports before running the analysis_cell, you can do in by adding the `init_analyse.py` file in the same directory as the data file.
 
-Example:
+Use case:
 This is the classical file structure if you use `labmate` library:
 - sample_001
     - analysis_code
         - analysis_script.py
     - data
         - experiment_1
             - init_analyse.py
             - data_file.h5
-
-So you open `data_file.h5` and try to run the code inside it. But to do that you need `analysis_script.py`. So inside `init_analyse.py` you need to import it:
+Suppose you opened `data_file.h5` and try to run the code inside it, but it needs dependencies from `analysis_script.py`. So they could be imported inside `init_analyse.py` like this:
 ```python
 from labmate.acquisition_notebook import AcquisitionAnalysisManager
 
 SCRIPT_DIR = os.path.join(os.path.dirname(__file__), os.pardir)
 sys.path.append(os.path.join(os.path.abspath(SCRIPT_DIR), 'analyse'))
 
 meas_dir = os.path.split(os.path.split(SCRIPT_DIR)[0])[0]
 aqm = AcquisitionAnalysisManager(meas_dir)
 
-from init_analyse import *
+from analysis_script import *
 ```
 
 
 ### Error
 Any error can be seen in the console view at the bottom right. Output from executing analysis_cell is also available there.
+
 ![docs/img/logger.png](./docs/img/logger.png)
 
 
 ### Set up `AcquisitionAnalysisManager` to create `init_analyse.py` automatically
 There is no need for you to create an `init_analyse.py` file in each directory.
 
 You can set any file to be an `init_analyse.py` by providing it to `AcquisitionAnalysisManager`:
```

### Comparing `h5viewer-0.4.0/README.md` & `h5viewer-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,40 +25,40 @@
 ```python
 # SOURCE: C:\ProgramData\Anaconda3\Scripts\activate.bat&&conda activate pyqt
 ```
 
 ### How to run code before your analyze cell. `init_analyse.py`
 If you want to set up any variables or imports before running the analysis_cell, you can do in by adding the `init_analyse.py` file in the same directory as the data file.
 
-Example:
+Use case:
 This is the classical file structure if you use `labmate` library:
 - sample_001
     - analysis_code
         - analysis_script.py
     - data
         - experiment_1
             - init_analyse.py
             - data_file.h5
-
-So you open `data_file.h5` and try to run the code inside it. But to do that you need `analysis_script.py`. So inside `init_analyse.py` you need to import it:
+Suppose you opened `data_file.h5` and try to run the code inside it, but it needs dependencies from `analysis_script.py`. So they could be imported inside `init_analyse.py` like this:
 ```python
 from labmate.acquisition_notebook import AcquisitionAnalysisManager
 
 SCRIPT_DIR = os.path.join(os.path.dirname(__file__), os.pardir)
 sys.path.append(os.path.join(os.path.abspath(SCRIPT_DIR), 'analyse'))
 
 meas_dir = os.path.split(os.path.split(SCRIPT_DIR)[0])[0]
 aqm = AcquisitionAnalysisManager(meas_dir)
 
-from init_analyse import *
+from analysis_script import *
 ```
 
 
 ### Error
 Any error can be seen in the console view at the bottom right. Output from executing analysis_cell is also available there.
+
 ![docs/img/logger.png](./docs/img/logger.png)
 
 
 ### Set up `AcquisitionAnalysisManager` to create `init_analyse.py` automatically
 There is no need for you to create an `init_analyse.py` file in each directory.
 
 You can set any file to be an `init_analyse.py` by providing it to `AcquisitionAnalysisManager`:
```

### Comparing `h5viewer-0.4.0/setup.py` & `h5viewer-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='h5viewer',
-    version="0.4.0",
+    version="0.7.0",
     author="LKB-OMQ",
     author_email="cryo.paris.su@gmail.com",
     description="Viewer for hdf5 files created by labmate",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kyrylo-gr/h5viewer",
     # py_modules=['h5viewer'],
```

### Comparing `h5viewer-0.4.0/src/h5viewer.egg-info/PKG-INFO` & `h5viewer-0.7.0/src/h5viewer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5viewer
-Version: 0.4.0
+Version: 0.7.0
 Summary: Viewer for hdf5 files created by labmate
 Home-page: https://github.com/kyrylo-gr/h5viewer
 Author: LKB-OMQ
 Author-email: cryo.paris.su@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -38,40 +38,40 @@
 ```python
 # SOURCE: C:\ProgramData\Anaconda3\Scripts\activate.bat&&conda activate pyqt
 ```
 
 ### How to run code before your analyze cell. `init_analyse.py`
 If you want to set up any variables or imports before running the analysis_cell, you can do in by adding the `init_analyse.py` file in the same directory as the data file.
 
-Example:
+Use case:
 This is the classical file structure if you use `labmate` library:
 - sample_001
     - analysis_code
         - analysis_script.py
     - data
         - experiment_1
             - init_analyse.py
             - data_file.h5
-
-So you open `data_file.h5` and try to run the code inside it. But to do that you need `analysis_script.py`. So inside `init_analyse.py` you need to import it:
+Suppose you opened `data_file.h5` and try to run the code inside it, but it needs dependencies from `analysis_script.py`. So they could be imported inside `init_analyse.py` like this:
 ```python
 from labmate.acquisition_notebook import AcquisitionAnalysisManager
 
 SCRIPT_DIR = os.path.join(os.path.dirname(__file__), os.pardir)
 sys.path.append(os.path.join(os.path.abspath(SCRIPT_DIR), 'analyse'))
 
 meas_dir = os.path.split(os.path.split(SCRIPT_DIR)[0])[0]
 aqm = AcquisitionAnalysisManager(meas_dir)
 
-from init_analyse import *
+from analysis_script import *
 ```
 
 
 ### Error
 Any error can be seen in the console view at the bottom right. Output from executing analysis_cell is also available there.
+
 ![docs/img/logger.png](./docs/img/logger.png)
 
 
 ### Set up `AcquisitionAnalysisManager` to create `init_analyse.py` automatically
 There is no need for you to create an `init_analyse.py` file in each directory.
 
 You can set any file to be an `init_analyse.py` by providing it to `AcquisitionAnalysisManager`:
```


# Comparing `tmp/bnpm-0.1.0.tar.gz` & `tmp/bnpm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bnpm-0.1.0.tar", last modified: Fri Jun  9 23:04:16 2023, max compression
+gzip compressed data, was "dist/bnpm-0.2.0.tar", last modified: Fri Jun  9 23:44:12 2023, max compression
```

## Comparing `bnpm-0.1.0.tar` & `bnpm-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:04:16.194145 bnpm-0.1.0/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     3719 2023-06-09 23:04:16.194234 bnpm-0.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3385 2023-06-09 19:32:54.000000 bnpm-0.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:04:16.192626 bnpm-0.1.0/bnpm/
--rwxrwxrwx   0 root         (0) root         (0)      888 2023-05-18 04:39:58.000000 bnpm-0.1.0/bnpm/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.1.0/bnpm/ca2p_preprocessing.py
--rwxrwxrwx   0 root         (0) root         (0)     4444 2023-06-08 15:16:51.000000 bnpm-0.1.0/bnpm/classification.py
--rwxrwxrwx   0 root         (0) root         (0)    55191 2023-05-14 23:41:40.000000 bnpm-0.1.0/bnpm/clustering.py
--rwxrwxrwx   0 root         (0) root         (0)    10099 2023-04-24 20:00:51.000000 bnpm-0.1.0/bnpm/container_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.1.0/bnpm/cross_validation.py
--rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.1.0/bnpm/cupy_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.1.0/bnpm/decomposition.py
--rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.1.0/bnpm/dtw.py
--rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.1.0/bnpm/email_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.1.0/bnpm/featurization.py
--rwxrwxrwx   0 root         (0) root         (0)    21239 2023-06-05 05:36:55.000000 bnpm-0.1.0/bnpm/file_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    11693 2023-06-08 14:03:50.000000 bnpm-0.1.0/bnpm/h5_handling.py
--rwxrwxrwx   0 root         (0) root         (0)    52633 2023-05-31 04:24:13.000000 bnpm-0.1.0/bnpm/image_processing.py
--rwxrwxrwx   0 root         (0) root         (0)    22721 2023-06-09 18:03:17.000000 bnpm-0.1.0/bnpm/indexing.py
--rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.1.0/bnpm/linear_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.1.0/bnpm/math_functions.py
--rwxrwxrwx   0 root         (0) root         (0)     9514 2023-06-09 18:43:59.000000 bnpm-0.1.0/bnpm/misc.py
--rwxrwxrwx   0 root         (0) root         (0)     4623 2023-05-12 16:20:07.000000 bnpm-0.1.0/bnpm/optimization.py
--rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.1.0/bnpm/other_peoples_code.py
--rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.1.0/bnpm/parallel_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.1.0/bnpm/path_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    29499 2023-06-09 06:50:59.000000 bnpm-0.1.0/bnpm/plotting_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.1.0/bnpm/resource_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)    34626 2023-04-21 22:51:53.000000 bnpm-0.1.0/bnpm/server.py
--rwxrwxrwx   0 root         (0) root         (0)    30842 2023-04-27 15:12:19.000000 bnpm-0.1.0/bnpm/similarity.py
--rwxrwxrwx   0 root         (0) root         (0)    22842 2023-05-11 22:58:37.000000 bnpm-0.1.0/bnpm/spectral.py
--rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.1.0/bnpm/stats.py
--rwxrwxrwx   0 root         (0) root         (0)    36798 2023-05-27 21:27:26.000000 bnpm-0.1.0/bnpm/timeSeries.py
--rwxrwxrwx   0 root         (0) root         (0)    13395 2023-02-28 17:16:58.000000 bnpm-0.1.0/bnpm/torch_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    46578 2023-01-27 18:26:44.000000 bnpm-0.1.0/bnpm/video.py
--rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.1.0/bnpm/welford_moving.py
--rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.1.0/bnpm/welford_moving_2D.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:04:16.193735 bnpm-0.1.0/bnpm.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3719 2023-06-09 23:04:16.000000 bnpm-0.1.0/bnpm.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-06-09 23:04:16.000000 bnpm-0.1.0/bnpm.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-09 23:04:16.000000 bnpm-0.1.0/bnpm.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      125 2023-06-09 23:04:16.000000 bnpm-0.1.0/bnpm.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-06-09 23:04:16.000000 bnpm-0.1.0/bnpm.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:04:16.193958 bnpm-0.1.0/demos/
--rwxrwxrwx   0 root         (0) root         (0)     1902 2022-05-10 23:33:18.000000 bnpm-0.1.0/demos/slurmDispatcher.py
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-09 23:04:16.194555 bnpm-0.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      556 2023-06-09 23:03:48.000000 bnpm-0.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.776153 bnpm-0.2.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     3084 2023-06-09 23:44:12.776241 bnpm-0.2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2725 2023-06-09 23:20:45.000000 bnpm-0.2.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.774622 bnpm-0.2.0/bnpm/
+-rwxrwxrwx   0 root         (0) root         (0)      907 2023-06-09 23:26:05.000000 bnpm-0.2.0/bnpm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.0/bnpm/ca2p_preprocessing.py
+-rwxrwxrwx   0 root         (0) root         (0)     4444 2023-06-08 15:16:51.000000 bnpm-0.2.0/bnpm/classification.py
+-rwxrwxrwx   0 root         (0) root         (0)    55191 2023-05-14 23:41:40.000000 bnpm-0.2.0/bnpm/clustering.py
+-rwxrwxrwx   0 root         (0) root         (0)    10099 2023-04-24 20:00:51.000000 bnpm-0.2.0/bnpm/container_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.0/bnpm/cross_validation.py
+-rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.0/bnpm/cupy_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.0/bnpm/decomposition.py
+-rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.0/bnpm/dtw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.0/bnpm/email_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.0/bnpm/featurization.py
+-rwxrwxrwx   0 root         (0) root         (0)    21239 2023-06-05 05:36:55.000000 bnpm-0.2.0/bnpm/file_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    11693 2023-06-08 14:03:50.000000 bnpm-0.2.0/bnpm/h5_handling.py
+-rwxrwxrwx   0 root         (0) root         (0)    52633 2023-05-31 04:24:13.000000 bnpm-0.2.0/bnpm/image_processing.py
+-rwxrwxrwx   0 root         (0) root         (0)    22721 2023-06-09 18:03:17.000000 bnpm-0.2.0/bnpm/indexing.py
+-rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.0/bnpm/linear_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.0/bnpm/math_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)     9514 2023-06-09 18:43:59.000000 bnpm-0.2.0/bnpm/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)     4623 2023-05-12 16:20:07.000000 bnpm-0.2.0/bnpm/optimization.py
+-rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.0/bnpm/other_peoples_code.py
+-rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.0/bnpm/parallel_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.0/bnpm/path_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    29499 2023-06-09 06:50:59.000000 bnpm-0.2.0/bnpm/plotting_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.0/bnpm/resource_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)    34626 2023-04-21 22:51:53.000000 bnpm-0.2.0/bnpm/server.py
+-rwxrwxrwx   0 root         (0) root         (0)    30842 2023-04-27 15:12:19.000000 bnpm-0.2.0/bnpm/similarity.py
+-rwxrwxrwx   0 root         (0) root         (0)    22842 2023-05-11 22:58:37.000000 bnpm-0.2.0/bnpm/spectral.py
+-rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.0/bnpm/stats.py
+-rwxrwxrwx   0 root         (0) root         (0)    36813 2023-06-09 23:34:38.000000 bnpm-0.2.0/bnpm/timeSeries.py
+-rwxrwxrwx   0 root         (0) root         (0)    13395 2023-02-28 17:16:58.000000 bnpm-0.2.0/bnpm/torch_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    46632 2023-06-09 23:30:37.000000 bnpm-0.2.0/bnpm/video.py
+-rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.0/bnpm/welford_moving.py
+-rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.0/bnpm/welford_moving_2D.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.775745 bnpm-0.2.0/bnpm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3084 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      895 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.775964 bnpm-0.2.0/demos/
+-rwxrwxrwx   0 root         (0) root         (0)     1902 2022-05-10 23:33:18.000000 bnpm-0.2.0/demos/slurmDispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-09 23:44:12.776564 bnpm-0.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-09 23:42:29.000000 bnpm-0.2.0/setup.py
```

### Comparing `bnpm-0.1.0/LICENSE` & `bnpm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/README.md` & `bnpm-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 [![repo size](https://img.shields.io/github/repo-size/RichieHakim/basic_neural_processing_modules)](https://github.com/RichieHakim/basic_neural_processing_modules/)
 
 #  basic_neural_processing_modules 
 Personal library of functions used in analyzing neural data.
 If you find a bug or just want to reach out: RichHakim@gmail.com
 
 ## Installation 
-A note on requirements: There are a lot of different libraries that are used in this package. As such there is a basic requirements.txt file that will install all the absolutely required libraries. However, there are other libraries that
-are imported in specific functions. These are listed in requirements_advanced.txt. I recommend installing only the libraries that you need for your specific project, as some require specific versions of other libraries or operating systems or GPUs.
+Normal installation of `bnpm` does not install all possible dependencies; there are some specific functions that wrap libraries that may need to be installed separately on a case-by-case basis.
 
-1. Clone the repository
-    - `cd path/to/your/preferred/directory`
-    - `git clone https://github.com/RichieHakim/basic_neural_processing_modules`
-
-2. Install requirements:
-    - `cd basic_neural_processing_modules`
-    - `pip install -e .`
-    - Install any other libraries in `requirements_advanced.txt` that you need for your project.
-
-3. Install the package:
-    - `cd path/to/basic_neural_processing_modules`
-    - `pip install -e .`
+`pip install git+https://github.com/RichieHakim/basic_neural_processing_modules.git`
+
+import with: `import bnpm`
 
-you can now import with: `import bnpm`
 
 ## Usage 
 My favorites:
 - **`featurization.Toeplitz_convolution2d`**
     - 1D and 2D convolution. Uses sparse Toeplitz matrix multiplication to speed up computation.
     - **Allows for sparse convolution.**
     - Same options as scipy.signal.convolve2d, but orders of magnitude faster in most cases.
```

### Comparing `bnpm-0.1.0/bnpm/__init__.py` & `bnpm-0.2.0/bnpm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,9 +26,11 @@
             'spectral',
             'stats',
             'timeSeries',
             'torch_helpers',
             'video',
         ]
 
-# for pkg in __all__:
-#     exec('from . import ' + pkg)
+for pkg in __all__:
+    exec('from . import ' + pkg)
+
+__version__ = '0.2.0'
```

### Comparing `bnpm-0.1.0/bnpm/ca2p_preprocessing.py` & `bnpm-0.2.0/bnpm/ca2p_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/classification.py` & `bnpm-0.2.0/bnpm/classification.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/clustering.py` & `bnpm-0.2.0/bnpm/clustering.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/container_helpers.py` & `bnpm-0.2.0/bnpm/container_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/cross_validation.py` & `bnpm-0.2.0/bnpm/cross_validation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/cupy_helpers.py` & `bnpm-0.2.0/bnpm/cupy_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/decomposition.py` & `bnpm-0.2.0/bnpm/decomposition.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/dtw.py` & `bnpm-0.2.0/bnpm/dtw.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/email_helpers.py` & `bnpm-0.2.0/bnpm/email_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/featurization.py` & `bnpm-0.2.0/bnpm/featurization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/file_helpers.py` & `bnpm-0.2.0/bnpm/file_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/h5_handling.py` & `bnpm-0.2.0/bnpm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/image_processing.py` & `bnpm-0.2.0/bnpm/image_processing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/indexing.py` & `bnpm-0.2.0/bnpm/indexing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/linear_regression.py` & `bnpm-0.2.0/bnpm/linear_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/math_functions.py` & `bnpm-0.2.0/bnpm/math_functions.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/misc.py` & `bnpm-0.2.0/bnpm/misc.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/optimization.py` & `bnpm-0.2.0/bnpm/optimization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/other_peoples_code.py` & `bnpm-0.2.0/bnpm/other_peoples_code.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/parallel_helpers.py` & `bnpm-0.2.0/bnpm/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/path_helpers.py` & `bnpm-0.2.0/bnpm/path_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/plotting_helpers.py` & `bnpm-0.2.0/bnpm/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/resource_tracking.py` & `bnpm-0.2.0/bnpm/resource_tracking.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/server.py` & `bnpm-0.2.0/bnpm/server.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/similarity.py` & `bnpm-0.2.0/bnpm/similarity.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/spectral.py` & `bnpm-0.2.0/bnpm/spectral.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/stats.py` & `bnpm-0.2.0/bnpm/stats.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/timeSeries.py` & `bnpm-0.2.0/bnpm/timeSeries.py`

 * *Files 0% similar despite different names*

```diff
@@ -883,15 +883,15 @@
 
     X_ptile = np.zeros(X.shape[0])
     for ii in prange(X.shape[0]):
         X_ptile[ii] = np.percentile(X[ii,:] , ptile)
     return X_ptile
 
 
-@jit(parallel=True)
+@jit(parallel=True, nopython=True)
 def zscore_numba(array):
     '''
     Parallel (multicore) Z-Score. Uses numba.
     Computes along second dimension (axis=1) for speed
     Best to input a contiguous array.
     RH 2021
```

### Comparing `bnpm-0.1.0/bnpm/torch_helpers.py` & `bnpm-0.2.0/bnpm/torch_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/video.py` & `bnpm-0.2.0/bnpm/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 ## This block of code is used to initialize cv2.imshow
 ## This is necessary because importing av and decord 
 ##  will cause cv2.imshow to fail unless it is initialized.
 ## Obviously, this should be commented out when running on
 ##  systems that do not support cv2.imshow like servers.
 ## Also be sure to import BNPM before importing most other
 ##  modules.
-test = np.zeros((1,300,400,3))
-for frame in test:
-    cv2.putText(frame, "Prepping CV2", (10,50), cv2.FONT_HERSHEY_SIMPLEX, 1, (255,255,255), 2)
-    cv2.putText(frame, "Calling this figure allows cv2.imshow ", (10,100), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255,255,255), 1)
-    cv2.putText(frame, "to run after importing av and decord", (10,120), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255,255,255), 1)
-    cv2.imshow('startup', frame)
-    cv2.waitKey(100)
-cv2.destroyWindow('startup')
+try:
+    test = np.zeros((1,300,400,3))
+    for frame in test:
+        cv2.putText(frame, "Prepping CV2", (10,50), cv2.FONT_HERSHEY_SIMPLEX, 1, (255,255,255), 2)
+        cv2.putText(frame, "Calling this figure allows cv2.imshow ", (10,100), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255,255,255), 1)
+        cv2.putText(frame, "to run after importing av and decord", (10,120), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255,255,255), 1)
+        cv2.imshow('startup', frame)
+        cv2.waitKey(100)
+    cv2.destroyWindow('startup')
+except:
+    pass
 ###############################################################################
 
 
 # import av
 import decord
 # # import cv2
```

### Comparing `bnpm-0.1.0/bnpm/welford_moving.py` & `bnpm-0.2.0/bnpm/welford_moving.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm/welford_moving_2D.py` & `bnpm-0.2.0/bnpm/welford_moving_2D.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/bnpm.egg-info/SOURCES.txt` & `bnpm-0.2.0/bnpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnpm-0.1.0/demos/slurmDispatcher.py` & `bnpm-0.2.0/demos/slurmDispatcher.py`

 * *Files identical despite different names*


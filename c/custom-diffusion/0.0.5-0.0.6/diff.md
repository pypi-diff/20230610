# Comparing `tmp/custom_diffusion-0.0.5.tar.gz` & `tmp/custom_diffusion-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.0.5.tar", last modified: Fri Jun  9 22:02:27 2023, max compression
+gzip compressed data, was "custom_diffusion-0.0.6.tar", last modified: Fri Jun  9 22:05:30 2023, max compression
```

## Comparing `custom_diffusion-0.0.5.tar` & `custom_diffusion-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 22:02:27.081354 custom_diffusion-0.0.5/
--rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1354 2023-06-09 22:02:27.082356 custom_diffusion-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 22:02:27.061349 custom_diffusion-0.0.5/custom_diffusion/
--rw-rw-rw-   0        0        0       22 2023-06-09 22:02:02.000000 custom_diffusion-0.0.5/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0      921 2023-06-09 21:56:06.000000 custom_diffusion-0.0.5/custom_diffusion/demo.py
--rw-rw-rw-   0        0        0     8952 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:02:27.080354 custom_diffusion-0.0.5/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1338 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0     1273 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3517 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:02:27.072351 custom_diffusion-0.0.5/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     1354 2023-06-09 22:02:26.000000 custom_diffusion-0.0.5/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-06-09 22:02:27.000000 custom_diffusion-0.0.5/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 22:02:26.000000 custom_diffusion-0.0.5/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-06-09 22:02:26.000000 custom_diffusion-0.0.5/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 22:02:26.000000 custom_diffusion-0.0.5/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       97 2023-06-09 22:01:15.000000 custom_diffusion-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-09 22:02:27.083353 custom_diffusion-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.170365 custom_diffusion-0.0.6/
+-rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1354 2023-06-09 22:05:30.170365 custom_diffusion-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.130354 custom_diffusion-0.0.6/custom_diffusion/
+-rw-rw-rw-   0        0        0       22 2023-06-09 22:05:01.000000 custom_diffusion-0.0.6/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0      921 2023-06-09 21:56:06.000000 custom_diffusion-0.0.6/custom_diffusion/demo.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.161360 custom_diffusion-0.0.6/custom_diffusion/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-06-09 22:04:46.000000 custom_diffusion-0.0.6/custom_diffusion/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     6684 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
+-rw-rw-rw-   0        0        0     6594 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/pipelines/controlnet_pipeline.py
+-rw-rw-rw-   0        0        0     8952 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.168363 custom_diffusion-0.0.6/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1338 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0     1273 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3517 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.155358 custom_diffusion-0.0.6/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     1354 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-06-09 22:05:30.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      105 2023-06-09 22:05:09.000000 custom_diffusion-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-09 22:05:30.172364 custom_diffusion-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/setup.py
```

### Comparing `custom_diffusion-0.0.5/LICENSE` & `custom_diffusion-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.5/PKG-INFO` & `custom_diffusion-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_diffusion
-Version: 0.0.5
+Version: 0.0.6
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `custom_diffusion-0.0.5/custom_diffusion/demo.py` & `custom_diffusion-0.0.6/custom_diffusion/demo.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.5/custom_diffusion/preprocces.py` & `custom_diffusion-0.0.6/custom_diffusion/preprocces.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.5/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.0.6/custom_diffusion/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.5/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.0.6/custom_diffusion/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.5/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.0.6/custom_diffusion/utils/scheduler_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.5/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.0.6/custom_diffusion/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.5/custom_diffusion.egg-info/PKG-INFO` & `custom_diffusion-0.0.6/custom_diffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-diffusion
-Version: 0.0.5
+Version: 0.0.6
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `custom_diffusion-0.0.5/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.0.6/custom_diffusion.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 custom_diffusion/demo.py
 custom_diffusion/preprocces.py
 custom_diffusion.egg-info/PKG-INFO
 custom_diffusion.egg-info/SOURCES.txt
 custom_diffusion.egg-info/dependency_links.txt
 custom_diffusion.egg-info/requires.txt
 custom_diffusion.egg-info/top_level.txt
+custom_diffusion/pipelines/__init__.py
+custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
+custom_diffusion/pipelines/controlnet_pipeline.py
 custom_diffusion/utils/__init__.py
 custom_diffusion/utils/data_utils.py
 custom_diffusion/utils/downloads.py
 custom_diffusion/utils/scheduler_utils.py
 custom_diffusion/utils/video_utils.py
```

### Comparing `custom_diffusion-0.0.5/setup.py` & `custom_diffusion-0.0.6/setup.py`

 * *Files identical despite different names*


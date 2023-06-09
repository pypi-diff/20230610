# Comparing `tmp/custom_diffusion-0.0.3.tar.gz` & `tmp/custom_diffusion-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.0.3.tar", last modified: Fri Jun  9 11:24:02 2023, max compression
+gzip compressed data, was "custom_diffusion-0.0.4.tar", last modified: Fri Jun  9 11:26:12 2023, max compression
```

## Comparing `custom_diffusion-0.0.3.tar` & `custom_diffusion-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 11:24:02.381320 custom_diffusion-0.0.3/
--rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 11:12:22.000000 custom_diffusion-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1331 2023-06-09 11:24:02.381320 custom_diffusion-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-06-09 11:15:50.000000 custom_diffusion-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 11:24:02.348408 custom_diffusion-0.0.3/custom_diffusion/
--rw-rw-rw-   0        0        0       21 2023-06-09 11:23:54.000000 custom_diffusion-0.0.3/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0     6872 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/controlnet_inpaint_pipeline.py
--rw-rw-rw-   0        0        0     6462 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/controlnet_pipeline.py
--rw-rw-rw-   0        0        0        0 2023-06-09 11:02:40.000000 custom_diffusion-0.0.3/custom_diffusion/demo.py
--rw-rw-rw-   0        0        0     9308 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:24:02.380320 custom_diffusion-0.0.3/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1375 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0     1312 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3637 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 11:24:02.370347 custom_diffusion-0.0.3/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     1331 2023-06-09 11:24:02.000000 custom_diffusion-0.0.3/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2023-06-09 11:24:02.000000 custom_diffusion-0.0.3/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 11:24:02.000000 custom_diffusion-0.0.3/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2023-06-09 11:24:02.000000 custom_diffusion-0.0.3/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 11:24:02.000000 custom_diffusion-0.0.3/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      196 2023-06-09 11:19:17.000000 custom_diffusion-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-09 11:24:02.385309 custom_diffusion-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2218 2023-06-09 11:16:34.000000 custom_diffusion-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:26:12.220585 custom_diffusion-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 11:12:22.000000 custom_diffusion-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1331 2023-06-09 11:26:12.220585 custom_diffusion-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-06-09 11:15:50.000000 custom_diffusion-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 11:26:12.187676 custom_diffusion-0.0.4/custom_diffusion/
+-rw-rw-rw-   0        0        0       21 2023-06-09 11:25:37.000000 custom_diffusion-0.0.4/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0     6872 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/controlnet_inpaint_pipeline.py
+-rw-rw-rw-   0        0        0     6462 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/controlnet_pipeline.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:02:40.000000 custom_diffusion-0.0.4/custom_diffusion/demo.py
+-rw-rw-rw-   0        0        0     9308 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:26:12.218562 custom_diffusion-0.0.4/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1375 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0     1312 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3637 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:26:12.208624 custom_diffusion-0.0.4/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     1331 2023-06-09 11:26:11.000000 custom_diffusion-0.0.4/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2023-06-09 11:26:12.000000 custom_diffusion-0.0.4/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:26:11.000000 custom_diffusion-0.0.4/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      247 2023-06-09 11:26:11.000000 custom_diffusion-0.0.4/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 11:26:11.000000 custom_diffusion-0.0.4/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      196 2023-06-09 11:19:17.000000 custom_diffusion-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-09 11:26:12.222551 custom_diffusion-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2218 2023-06-09 11:16:34.000000 custom_diffusion-0.0.4/setup.py
```

### Comparing `custom_diffusion-0.0.3/LICENSE` & `custom_diffusion-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/PKG-INFO` & `custom_diffusion-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_diffusion
-Version: 0.0.3
+Version: 0.0.4
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `custom_diffusion-0.0.3/custom_diffusion/controlnet_inpaint_pipeline.py` & `custom_diffusion-0.0.4/custom_diffusion/controlnet_inpaint_pipeline.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/custom_diffusion/controlnet_pipeline.py` & `custom_diffusion-0.0.4/custom_diffusion/controlnet_pipeline.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/custom_diffusion/preprocces.py` & `custom_diffusion-0.0.4/custom_diffusion/preprocces.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.0.4/custom_diffusion/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.0.4/custom_diffusion/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.0.4/custom_diffusion/utils/scheduler_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.0.4/custom_diffusion/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/custom_diffusion.egg-info/PKG-INFO` & `custom_diffusion-0.0.4/custom_diffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-diffusion
-Version: 0.0.3
+Version: 0.0.4
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `custom_diffusion-0.0.3/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.0.4/custom_diffusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.3/setup.py` & `custom_diffusion-0.0.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/devbio-napari-0.8.1.tar.gz` & `tmp/devbio-napari-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devbio-napari-0.8.1.tar", last modified: Sun Dec 11 11:00:52 2022, max compression
+gzip compressed data, was "devbio-napari-0.9.0.tar", last modified: Mon May  1 13:34:36 2023, max compression
```

## Comparing `devbio-napari-0.8.1.tar` & `devbio-napari-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-12-11 11:00:52.000583 devbio-napari-0.8.1/
--rw-rw-rw-   0        0        0     1505 2022-12-11 10:48:59.000000 devbio-napari-0.8.1/LICENSE
--rw-rw-rw-   0        0        0      127 2022-12-11 10:48:59.000000 devbio-napari-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9398 2022-12-11 11:00:52.001566 devbio-napari-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     8243 2022-12-11 10:48:59.000000 devbio-napari-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-11 11:00:51.992541 devbio-napari-0.8.1/devbio_napari/
--rw-rw-rw-   0        0        0     2741 2022-12-11 10:58:45.000000 devbio-napari-0.8.1/devbio_napari/__init__.py
--rw-rw-rw-   0        0        0      496 2022-12-11 10:48:59.000000 devbio-napari-0.8.1/devbio_napari/__main__.py
--rw-rw-rw-   0        0        0      434 2022-12-11 10:48:59.000000 devbio-napari-0.8.1/devbio_napari/_viewer.py
-drwxrwxrwx   0        0        0        0 2022-12-11 11:00:51.999560 devbio-napari-0.8.1/devbio_napari.egg-info/
--rw-rw-rw-   0        0        0     9398 2022-12-11 11:00:51.000000 devbio-napari-0.8.1/devbio_napari.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2022-12-11 11:00:51.000000 devbio-napari-0.8.1/devbio_napari.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-11 11:00:51.000000 devbio-napari-0.8.1/devbio_napari.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2022-12-11 11:00:51.000000 devbio-napari-0.8.1/devbio_napari.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      695 2022-12-11 11:00:51.000000 devbio-napari-0.8.1/devbio_napari.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-12-11 11:00:51.000000 devbio-napari-0.8.1/devbio_napari.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1056 2022-12-11 10:58:45.000000 devbio-napari-0.8.1/requirements.txt
--rw-rw-rw-   0        0        0     2243 2022-12-11 11:00:52.007582 devbio-napari-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0       89 2022-12-11 10:48:59.000000 devbio-napari-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:34:36.150435 devbio-napari-0.9.0/
+-rw-rw-rw-   0        0        0     1505 2022-12-11 10:48:59.000000 devbio-napari-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      127 2022-12-11 10:48:59.000000 devbio-napari-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9983 2023-05-01 13:34:36.150435 devbio-napari-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8828 2023-05-01 13:31:06.000000 devbio-napari-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 13:34:36.119181 devbio-napari-0.9.0/devbio_napari/
+-rw-rw-rw-   0        0        0     2741 2023-05-01 13:31:06.000000 devbio-napari-0.9.0/devbio_napari/__init__.py
+-rw-rw-rw-   0        0        0      496 2022-12-11 10:48:59.000000 devbio-napari-0.9.0/devbio_napari/__main__.py
+-rw-rw-rw-   0        0        0      434 2022-12-11 10:48:59.000000 devbio-napari-0.9.0/devbio_napari/_viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:34:36.150435 devbio-napari-0.9.0/devbio_napari.egg-info/
+-rw-rw-rw-   0        0        0     9983 2023-05-01 13:34:35.000000 devbio-napari-0.9.0/devbio_napari.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-01 13:34:36.000000 devbio-napari-0.9.0/devbio_napari.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:34:35.000000 devbio-napari-0.9.0/devbio_napari.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-05-01 13:34:35.000000 devbio-napari-0.9.0/devbio_napari.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      726 2023-05-01 13:34:35.000000 devbio-napari-0.9.0/devbio_napari.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-01 13:34:35.000000 devbio-napari-0.9.0/devbio_napari.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-05-01 13:31:06.000000 devbio-napari-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0     2278 2023-05-01 13:34:36.150435 devbio-napari-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0       89 2022-12-11 10:48:59.000000 devbio-napari-0.9.0/setup.py
```

### Comparing `devbio-napari-0.8.1/LICENSE` & `devbio-napari-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devbio-napari-0.8.1/PKG-INFO` & `devbio-napari-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devbio-napari
-Version: 0.8.1
+Version: 0.9.0
 Summary: A bundle of napari plugins useful for 3D+t image processing and analysis for studying developmental biology.
 Home-page: https://github.com/haesleinhuepf/devbio-napari
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/devbio-napari/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/devbio-napari#README.md
@@ -29,28 +29,30 @@
 [![PyPI](https://img.shields.io/pypi/v/devbio-napari.svg?color=green)](https://pypi.org/project/devbio-napari)
 [![Python Version](https://img.shields.io/pypi/pyversions/devbio-napari.svg?color=green)](https://python.org)
 [![tests](https://github.com/haesleinhuepf/devbio-napari/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari-plot-profile/actions)
 [![codecov](https://codecov.io/gh/haesleinhuepf/devbio-napari/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/devbio-napari)
 [![Development Status](https://img.shields.io/pypi/status/devbio-napari.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/devbio-napari)](https://napari-hub.org/plugins/devbio-napari)
 
-
+ 
 A bundle of napari plugins useful for 3D+t image processing and analysis for studying developmental biology.
 
 * [accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification)
   * Instance segmentation
   * Semantic segmentation
   * Object classification
   * Random Forest Classifier training
 * [animation](https://www.napari-hub.org/plugins/napari-animation) 
   * Visualization
 * [blob-detection](https://www.napari-hub.org/plugins/napari-blob-detection)
   * Detection
 * [brightness-contrast](https://www.napari-hub.org/plugins/napari-brightness-contrast)
   * Visualization
+* [cellpose](https://www.napari-hub.org/plugins/cellpose-napari)
+  * Segmentation 
 * [clusters-plotter](https://www.napari-hub.org/plugins/napari-clusters-plotter)
   * Visualization
   * Plotting
   * Semantic object segmentation
   * Dimensionality reduction
   * Unsupervised machine learning
 * [crop](https://www.napari-hub.org/plugins/napari-crop)
@@ -105,34 +107,34 @@
   * Visualization
 * [workflow-optimizer](https://www.napari-hub.org/plugins/napari-workflow-optimizer)
   * Interaction
   * Optimization
 
 ----------------------------------
 
-This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
-
 ## Installation
 
 You can install `devbio-napari` via conda/mamba. If you have never used conda before, please [read this guide first](https://biapol.github.io/blog/johannes_mueller/anaconda_getting_started/).  
 Start by installing mamba in your base environment:
 
 ```
 conda install mamba -c conda-forge
 ```
 
 Afterwards, create an environment using mamba.
 
 ```
-mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge
+mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge -c pytorch
 ```
 
 Afterwards, activate the environment like this:
-    
-    conda activate devbio-napari-env
+
+```
+mamba activate devbio-napari-env
+```
 
 Afterwards, run this command from the command line
 
 ```
 naparia
 ```
 
@@ -143,14 +145,15 @@
 
 ## Troubleshooting: Graphics cards drivers
 
 In case error messages contains "ImportError: DLL load failed while importing cl: The specified procedure could not be found" [see also](https://github.com/clEsperanto/pyclesperanto_prototype/issues/55) or ""clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR", please install recent drivers for your graphics card and/or OpenCL device. Select the right driver source depending on your hardware from this list:
 
 * [AMD drivers](https://www.amd.com/en/support)
 * [NVidia drivers](https://www.nvidia.com/download/index.aspx)
+* [Intel GPU drivers](https://www.intel.com/content/www/us/en/download/726609/intel-arc-graphics-windows-dch-driver.html)
 * [Intel CPU OpenCL drivers](https://www.intel.com/content/www/us/en/developer/articles/tool/opencl-drivers.html#latest_CPU_runtime)
 * [Microsoft Windows OpenCL support](https://www.microsoft.com/en-us/p/opencl-and-opengl-compatibility-pack/9nqpsl29bfff)
 
 Sometimes, mac-users need to install this:
 
     conda install -c conda-forge ocl_icd_wrapper_apple
 
@@ -161,14 +164,27 @@
 
 In case installation didn't work in the first attempt, you may have to call this command line to reset the napari configuration:
 
 ```
 napari --reset
 ```
 
+## Troubleshooting: pytorch
+
+In case pytorch-related plugins fail, install pytorch as explained on [its website](https://pytorch.org/get-started/locally/). Consider replacing `conda` with `mamba` in given instructions.
+
+For example if you have an NVidia GPU at hand, install pytorch like this:
+```
+mamba install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
+```
+Or if not:
+```
+mamba install pytorch torchvision torchaudio cpuonly -c pytorch
+```
+
 ## Contributing
 
 Contributions are very welcome. 
 If you want to [suggest a new napari plugin](https://github.com/haesleinhuepf/devbio-napari/pulls) to become part of this distribution, please make sure it interoperates nicely with the other plugins. 
 For example, if the plugin you suggest provided cell segmentation algorithms, please check if the resulting segmented cells can be analysed using napari-skimage-regionprops.
 Furthermore, please make sure the README of the plugin you are proposing comes with user documentation, e.g. a step-by-step guide with screenshots explaining what users can do with the plugin and how to use it. 
 It is recommended to provide example data as well so that end-users can try out the plugin under conditions it was developed for.
```

### Comparing `devbio-napari-0.8.1/README.md` & `devbio-napari-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 [![PyPI](https://img.shields.io/pypi/v/devbio-napari.svg?color=green)](https://pypi.org/project/devbio-napari)
 [![Python Version](https://img.shields.io/pypi/pyversions/devbio-napari.svg?color=green)](https://python.org)
 [![tests](https://github.com/haesleinhuepf/devbio-napari/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari-plot-profile/actions)
 [![codecov](https://codecov.io/gh/haesleinhuepf/devbio-napari/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/devbio-napari)
 [![Development Status](https://img.shields.io/pypi/status/devbio-napari.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/devbio-napari)](https://napari-hub.org/plugins/devbio-napari)
 
-
+ 
 A bundle of napari plugins useful for 3D+t image processing and analysis for studying developmental biology.
 
 * [accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification)
   * Instance segmentation
   * Semantic segmentation
   * Object classification
   * Random Forest Classifier training
 * [animation](https://www.napari-hub.org/plugins/napari-animation) 
   * Visualization
 * [blob-detection](https://www.napari-hub.org/plugins/napari-blob-detection)
   * Detection
 * [brightness-contrast](https://www.napari-hub.org/plugins/napari-brightness-contrast)
   * Visualization
+* [cellpose](https://www.napari-hub.org/plugins/cellpose-napari)
+  * Segmentation 
 * [clusters-plotter](https://www.napari-hub.org/plugins/napari-clusters-plotter)
   * Visualization
   * Plotting
   * Semantic object segmentation
   * Dimensionality reduction
   * Unsupervised machine learning
 * [crop](https://www.napari-hub.org/plugins/napari-crop)
@@ -80,34 +82,34 @@
   * Visualization
 * [workflow-optimizer](https://www.napari-hub.org/plugins/napari-workflow-optimizer)
   * Interaction
   * Optimization
 
 ----------------------------------
 
-This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
-
 ## Installation
 
 You can install `devbio-napari` via conda/mamba. If you have never used conda before, please [read this guide first](https://biapol.github.io/blog/johannes_mueller/anaconda_getting_started/).  
 Start by installing mamba in your base environment:
 
 ```
 conda install mamba -c conda-forge
 ```
 
 Afterwards, create an environment using mamba.
 
 ```
-mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge
+mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge -c pytorch
 ```
 
 Afterwards, activate the environment like this:
-    
-    conda activate devbio-napari-env
+
+```
+mamba activate devbio-napari-env
+```
 
 Afterwards, run this command from the command line
 
 ```
 naparia
 ```
 
@@ -118,14 +120,15 @@
 
 ## Troubleshooting: Graphics cards drivers
 
 In case error messages contains "ImportError: DLL load failed while importing cl: The specified procedure could not be found" [see also](https://github.com/clEsperanto/pyclesperanto_prototype/issues/55) or ""clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR", please install recent drivers for your graphics card and/or OpenCL device. Select the right driver source depending on your hardware from this list:
 
 * [AMD drivers](https://www.amd.com/en/support)
 * [NVidia drivers](https://www.nvidia.com/download/index.aspx)
+* [Intel GPU drivers](https://www.intel.com/content/www/us/en/download/726609/intel-arc-graphics-windows-dch-driver.html)
 * [Intel CPU OpenCL drivers](https://www.intel.com/content/www/us/en/developer/articles/tool/opencl-drivers.html#latest_CPU_runtime)
 * [Microsoft Windows OpenCL support](https://www.microsoft.com/en-us/p/opencl-and-opengl-compatibility-pack/9nqpsl29bfff)
 
 Sometimes, mac-users need to install this:
 
     conda install -c conda-forge ocl_icd_wrapper_apple
 
@@ -136,14 +139,27 @@
 
 In case installation didn't work in the first attempt, you may have to call this command line to reset the napari configuration:
 
 ```
 napari --reset
 ```
 
+## Troubleshooting: pytorch
+
+In case pytorch-related plugins fail, install pytorch as explained on [its website](https://pytorch.org/get-started/locally/). Consider replacing `conda` with `mamba` in given instructions.
+
+For example if you have an NVidia GPU at hand, install pytorch like this:
+```
+mamba install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
+```
+Or if not:
+```
+mamba install pytorch torchvision torchaudio cpuonly -c pytorch
+```
+
 ## Contributing
 
 Contributions are very welcome. 
 If you want to [suggest a new napari plugin](https://github.com/haesleinhuepf/devbio-napari/pulls) to become part of this distribution, please make sure it interoperates nicely with the other plugins. 
 For example, if the plugin you suggest provided cell segmentation algorithms, please check if the resulting segmented cells can be analysed using napari-skimage-regionprops.
 Furthermore, please make sure the README of the plugin you are proposing comes with user documentation, e.g. a step-by-step guide with screenshots explaining what users can do with the plugin and how to use it. 
 It is recommended to provide example data as well so that end-users can try out the plugin under conditions it was developed for.
```

### Comparing `devbio-napari-0.8.1/devbio_napari/__init__.py` & `devbio-napari-0.9.0/devbio_napari/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 0d0a 5f5f 7665 7273 696f 6e5f 5f20 3d20  ..__version__ = 
-00000010: 2230 2e38 2e31 220d 0a0d 0a0d 0a69 6d70  "0.8.1"......imp
+00000010: 2230 2e39 2e30 220d 0a0d 0a0d 0a69 6d70  "0.9.0"......imp
 00000020: 6f72 7420 6e61 7061 7269 0d0a 6672 6f6d  ort napari..from
 00000030: 206e 6170 6172 695f 7469 6d65 5f73 6c69   napari_time_sli
 00000040: 6365 7220 696d 706f 7274 2074 696d 655f  cer import time_
 00000050: 736c 6963 6572 0d0a 6672 6f6d 206e 6170  slicer..from nap
 00000060: 6172 695f 746f 6f6c 735f 6d65 6e75 2069  ari_tools_menu i
 00000070: 6d70 6f72 7420 7265 6769 7374 6572 5f66  mport register_f
 00000080: 756e 6374 696f 6e0d 0a66 726f 6d20 6e61  unction..from na
```

### Comparing `devbio-napari-0.8.1/devbio_napari.egg-info/PKG-INFO` & `devbio-napari-0.9.0/devbio_napari.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devbio-napari
-Version: 0.8.1
+Version: 0.9.0
 Summary: A bundle of napari plugins useful for 3D+t image processing and analysis for studying developmental biology.
 Home-page: https://github.com/haesleinhuepf/devbio-napari
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/devbio-napari/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/devbio-napari#README.md
@@ -29,28 +29,30 @@
 [![PyPI](https://img.shields.io/pypi/v/devbio-napari.svg?color=green)](https://pypi.org/project/devbio-napari)
 [![Python Version](https://img.shields.io/pypi/pyversions/devbio-napari.svg?color=green)](https://python.org)
 [![tests](https://github.com/haesleinhuepf/devbio-napari/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari-plot-profile/actions)
 [![codecov](https://codecov.io/gh/haesleinhuepf/devbio-napari/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/devbio-napari)
 [![Development Status](https://img.shields.io/pypi/status/devbio-napari.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/devbio-napari)](https://napari-hub.org/plugins/devbio-napari)
 
-
+ 
 A bundle of napari plugins useful for 3D+t image processing and analysis for studying developmental biology.
 
 * [accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification)
   * Instance segmentation
   * Semantic segmentation
   * Object classification
   * Random Forest Classifier training
 * [animation](https://www.napari-hub.org/plugins/napari-animation) 
   * Visualization
 * [blob-detection](https://www.napari-hub.org/plugins/napari-blob-detection)
   * Detection
 * [brightness-contrast](https://www.napari-hub.org/plugins/napari-brightness-contrast)
   * Visualization
+* [cellpose](https://www.napari-hub.org/plugins/cellpose-napari)
+  * Segmentation 
 * [clusters-plotter](https://www.napari-hub.org/plugins/napari-clusters-plotter)
   * Visualization
   * Plotting
   * Semantic object segmentation
   * Dimensionality reduction
   * Unsupervised machine learning
 * [crop](https://www.napari-hub.org/plugins/napari-crop)
@@ -105,34 +107,34 @@
   * Visualization
 * [workflow-optimizer](https://www.napari-hub.org/plugins/napari-workflow-optimizer)
   * Interaction
   * Optimization
 
 ----------------------------------
 
-This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
-
 ## Installation
 
 You can install `devbio-napari` via conda/mamba. If you have never used conda before, please [read this guide first](https://biapol.github.io/blog/johannes_mueller/anaconda_getting_started/).  
 Start by installing mamba in your base environment:
 
 ```
 conda install mamba -c conda-forge
 ```
 
 Afterwards, create an environment using mamba.
 
 ```
-mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge
+mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge -c pytorch
 ```
 
 Afterwards, activate the environment like this:
-    
-    conda activate devbio-napari-env
+
+```
+mamba activate devbio-napari-env
+```
 
 Afterwards, run this command from the command line
 
 ```
 naparia
 ```
 
@@ -143,14 +145,15 @@
 
 ## Troubleshooting: Graphics cards drivers
 
 In case error messages contains "ImportError: DLL load failed while importing cl: The specified procedure could not be found" [see also](https://github.com/clEsperanto/pyclesperanto_prototype/issues/55) or ""clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR", please install recent drivers for your graphics card and/or OpenCL device. Select the right driver source depending on your hardware from this list:
 
 * [AMD drivers](https://www.amd.com/en/support)
 * [NVidia drivers](https://www.nvidia.com/download/index.aspx)
+* [Intel GPU drivers](https://www.intel.com/content/www/us/en/download/726609/intel-arc-graphics-windows-dch-driver.html)
 * [Intel CPU OpenCL drivers](https://www.intel.com/content/www/us/en/developer/articles/tool/opencl-drivers.html#latest_CPU_runtime)
 * [Microsoft Windows OpenCL support](https://www.microsoft.com/en-us/p/opencl-and-opengl-compatibility-pack/9nqpsl29bfff)
 
 Sometimes, mac-users need to install this:
 
     conda install -c conda-forge ocl_icd_wrapper_apple
 
@@ -161,14 +164,27 @@
 
 In case installation didn't work in the first attempt, you may have to call this command line to reset the napari configuration:
 
 ```
 napari --reset
 ```
 
+## Troubleshooting: pytorch
+
+In case pytorch-related plugins fail, install pytorch as explained on [its website](https://pytorch.org/get-started/locally/). Consider replacing `conda` with `mamba` in given instructions.
+
+For example if you have an NVidia GPU at hand, install pytorch like this:
+```
+mamba install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
+```
+Or if not:
+```
+mamba install pytorch torchvision torchaudio cpuonly -c pytorch
+```
+
 ## Contributing
 
 Contributions are very welcome. 
 If you want to [suggest a new napari plugin](https://github.com/haesleinhuepf/devbio-napari/pulls) to become part of this distribution, please make sure it interoperates nicely with the other plugins. 
 For example, if the plugin you suggest provided cell segmentation algorithms, please check if the resulting segmented cells can be analysed using napari-skimage-regionprops.
 Furthermore, please make sure the README of the plugin you are proposing comes with user documentation, e.g. a step-by-step guide with screenshots explaining what users can do with the plugin and how to use it. 
 It is recommended to provide example data as well so that end-users can try out the plugin under conditions it was developed for.
```

### Comparing `devbio-napari-0.8.1/devbio_napari.egg-info/requires.txt` & `devbio-napari-0.9.0/devbio_napari.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 napari-accelerated-pixel-and-object-classification
 napari-brightness-contrast
 napari-plugin-search
 napari-segment-blobs-and-things-with-membranes
 napari-simpleitk-image-processing
 napari-folder-browser
 napari-crop
-napari-clusters-plotter
+napari-clusters-plotter>=0.7.1
 napari-tabu
 napari-workflow-optimizer
 napari-workflow-inspector
 napari-curtain
 napari-layer-details-display
 napari
 vispy
@@ -27,7 +27,9 @@
 napari-czifile2
 napari-roi
 pydantic!=1.10.0
 napari-pystackreg
 imageio!=2.22.1
 redlionfish
 jupyter_server<2.0.0
+cellpose-napari
+seaborn
```

### Comparing `devbio-napari-0.8.1/requirements.txt` & `devbio-napari-0.9.0/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 napari-accelerated-pixel-and-object-classification
 napari-brightness-contrast
 napari-plugin-search
 napari-segment-blobs-and-things-with-membranes
 napari-simpleitk-image-processing
 napari-folder-browser
 napari-crop
-napari-clusters-plotter
+napari-clusters-plotter>=0.7.1
 napari-tabu
 napari-workflow-optimizer
 napari-workflow-inspector
 napari-curtain
 napari-layer-details-display
 # https://github.com/napari/napari/issues/4415
 # https://github.com/napari/napari/issues/4708
@@ -30,7 +30,9 @@
 napari-czifile2
 napari-roi
 pydantic!=1.10.0 # https://twitter.com/Czaki_PL/status/1564908046186434566?s=20&t=YEAgvsUTuYIDRYlKREQp3A
 napari-pystackreg
 imageio!=2.22.1 # https://github.com/napari/napari/pull/5168
 redlionfish
 jupyter_server<2.0.0 # https://github.com/jupyter-server/jupyter_server/issues/1127
+cellpose-napari
+seaborn
```

### Comparing `devbio-napari-0.8.1/setup.cfg` & `devbio-napari-0.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6576 6269 6f2d 6e61 7061 7269   = devbio-napari
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 382e  ..version = 0.8.
-00000030: 310d 0a61 7574 686f 7220 3d20 526f 6265  1..author = Robe
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 392e  ..version = 0.9.
+00000030: 300d 0a61 7574 686f 7220 3d20 526f 6265  0..author = Robe
 00000040: 7274 2048 6161 7365 0d0a 6175 7468 6f72  rt Haase..author
 00000050: 5f65 6d61 696c 203d 2072 6f62 6572 742e  _email = robert.
 00000060: 6861 6173 6540 7475 2d64 7265 7364 656e  haase@tu-dresden
 00000070: 2e64 650d 0a6c 6963 656e 7365 203d 2042  .de..license = B
 00000080: 5344 2d33 0d0a 7572 6c20 3d20 6874 7470  SD-3..url = http
 00000090: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
 000000a0: 6165 736c 6569 6e68 7565 7066 2f64 6576  aesleinhuepf/dev
@@ -89,53 +89,55 @@
 00000580: 2d77 6974 682d 6d65 6d62 7261 6e65 730d  -with-membranes.
 00000590: 0a09 6e61 7061 7269 2d73 696d 706c 6569  ..napari-simplei
 000005a0: 746b 2d69 6d61 6765 2d70 726f 6365 7373  tk-image-process
 000005b0: 696e 670d 0a09 6e61 7061 7269 2d66 6f6c  ing...napari-fol
 000005c0: 6465 722d 6272 6f77 7365 720d 0a09 6e61  der-browser...na
 000005d0: 7061 7269 2d63 726f 700d 0a09 6e61 7061  pari-crop...napa
 000005e0: 7269 2d63 6c75 7374 6572 732d 706c 6f74  ri-clusters-plot
-000005f0: 7465 720d 0a09 6e61 7061 7269 2d74 6162  ter...napari-tab
-00000600: 750d 0a09 6e61 7061 7269 2d77 6f72 6b66  u...napari-workf
-00000610: 6c6f 772d 6f70 7469 6d69 7a65 720d 0a09  low-optimizer...
-00000620: 6e61 7061 7269 2d77 6f72 6b66 6c6f 772d  napari-workflow-
-00000630: 696e 7370 6563 746f 720d 0a09 6e61 7061  inspector...napa
-00000640: 7269 2d63 7572 7461 696e 0d0a 096e 6170  ri-curtain...nap
-00000650: 6172 692d 6c61 7965 722d 6465 7461 696c  ari-layer-detail
-00000660: 732d 6469 7370 6c61 790d 0a09 6e61 7061  s-display...napa
-00000670: 7269 0d0a 0976 6973 7079 0d0a 096e 6170  ri...vispy...nap
-00000680: 6172 692d 6d6f 7573 652d 636f 6e74 726f  ari-mouse-contro
-00000690: 6c73 0d0a 0974 6865 2d73 6567 6d65 6e74  ls...the-segment
-000006a0: 6174 696f 6e2d 6761 6d65 0d0a 096e 6170  ation-game...nap
-000006b0: 6172 692d 626c 6f62 2d64 6574 6563 7469  ari-blob-detecti
-000006c0: 6f6e 0d0a 096a 7570 7974 6572 6c61 620d  on...jupyterlab.
-000006d0: 0a09 6e61 7061 7269 2d63 7a69 6669 6c65  ..napari-czifile
-000006e0: 320d 0a09 6e61 7061 7269 2d72 6f69 0d0a  2...napari-roi..
-000006f0: 0970 7964 616e 7469 6321 3d31 2e31 302e  .pydantic!=1.10.
-00000700: 3020 2320 6874 7470 733a 2f2f 7477 6974  0 # https://twit
-00000710: 7465 722e 636f 6d2f 437a 616b 695f 504c  ter.com/Czaki_PL
-00000720: 2f73 7461 7475 732f 3135 3634 3930 3830  /status/15649080
-00000730: 3436 3138 3634 3334 3536 363f 733d 3230  46186434566?s=20
-00000740: 2674 3d59 4541 6776 7355 5475 5949 4452  &t=YEAgvsUTuYIDR
-00000750: 596c 4b52 4551 7033 410d 0a09 6e61 7061  YlKREQp3A...napa
-00000760: 7269 2d70 7973 7461 636b 7265 670d 0a09  ri-pystackreg...
-00000770: 696d 6167 6569 6f21 3d32 2e32 322e 3120  imageio!=2.22.1 
-00000780: 2320 6874 7470 733a 2f2f 6769 7468 7562  # https://github
-00000790: 2e63 6f6d 2f6e 6170 6172 692f 6e61 7061  .com/napari/napa
-000007a0: 7269 2f70 756c 6c2f 3531 3638 0d0a 0972  ri/pull/5168...r
-000007b0: 6564 6c69 6f6e 6669 7368 0d0a 096a 7570  edlionfish...jup
-000007c0: 7974 6572 5f73 6572 7665 723c 322e 302e  yter_server<2.0.
-000007d0: 3020 2320 6874 7470 733a 2f2f 6769 7468  0 # https://gith
-000007e0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2d73  ub.com/jupyter-s
-000007f0: 6572 7665 722f 6a75 7079 7465 725f 7365  erver/jupyter_se
-00000800: 7276 6572 2f69 7373 7565 732f 3131 3237  rver/issues/1127
-00000810: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000820: 7279 5f70 6f69 6e74 735d 0d0a 6e61 7061  ry_points]..napa
-00000830: 7269 2e70 6c75 6769 6e20 3d20 0d0a 0964  ri.plugin = ...d
-00000840: 6576 6269 6f5f 6e61 7061 7269 203d 2064  evbio_napari = d
-00000850: 6576 6269 6f5f 6e61 7061 7269 0d0a 636f  evbio_napari..co
-00000860: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
-00000870: 0d0a 0964 6576 6269 6f2d 6e61 7061 7269  ...devbio-napari
-00000880: 203d 2064 6576 6269 6f5f 6e61 7061 7269   = devbio_napari
-00000890: 3a6d 6169 6e0d 0a0d 0a5b 6567 675f 696e  :main....[egg_in
-000008a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000008b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000008c0: 0a0d 0a                                  ...
+000005f0: 7465 723e 3d30 2e37 2e31 0d0a 096e 6170  ter>=0.7.1...nap
+00000600: 6172 692d 7461 6275 0d0a 096e 6170 6172  ari-tabu...napar
+00000610: 692d 776f 726b 666c 6f77 2d6f 7074 696d  i-workflow-optim
+00000620: 697a 6572 0d0a 096e 6170 6172 692d 776f  izer...napari-wo
+00000630: 726b 666c 6f77 2d69 6e73 7065 6374 6f72  rkflow-inspector
+00000640: 0d0a 096e 6170 6172 692d 6375 7274 6169  ...napari-curtai
+00000650: 6e0d 0a09 6e61 7061 7269 2d6c 6179 6572  n...napari-layer
+00000660: 2d64 6574 6169 6c73 2d64 6973 706c 6179  -details-display
+00000670: 0d0a 096e 6170 6172 690d 0a09 7669 7370  ...napari...visp
+00000680: 790d 0a09 6e61 7061 7269 2d6d 6f75 7365  y...napari-mouse
+00000690: 2d63 6f6e 7472 6f6c 730d 0a09 7468 652d  -controls...the-
+000006a0: 7365 676d 656e 7461 7469 6f6e 2d67 616d  segmentation-gam
+000006b0: 650d 0a09 6e61 7061 7269 2d62 6c6f 622d  e...napari-blob-
+000006c0: 6465 7465 6374 696f 6e0d 0a09 6a75 7079  detection...jupy
+000006d0: 7465 726c 6162 0d0a 096e 6170 6172 692d  terlab...napari-
+000006e0: 637a 6966 696c 6532 0d0a 096e 6170 6172  czifile2...napar
+000006f0: 692d 726f 690d 0a09 7079 6461 6e74 6963  i-roi...pydantic
+00000700: 213d 312e 3130 2e30 2023 2068 7474 7073  !=1.10.0 # https
+00000710: 3a2f 2f74 7769 7474 6572 2e63 6f6d 2f43  ://twitter.com/C
+00000720: 7a61 6b69 5f50 4c2f 7374 6174 7573 2f31  zaki_PL/status/1
+00000730: 3536 3439 3038 3034 3631 3836 3433 3435  5649080461864345
+00000740: 3636 3f73 3d32 3026 743d 5945 4167 7673  66?s=20&t=YEAgvs
+00000750: 5554 7559 4944 5259 6c4b 5245 5170 3341  UTuYIDRYlKREQp3A
+00000760: 0d0a 096e 6170 6172 692d 7079 7374 6163  ...napari-pystac
+00000770: 6b72 6567 0d0a 0969 6d61 6765 696f 213d  kreg...imageio!=
+00000780: 322e 3232 2e31 2023 2068 7474 7073 3a2f  2.22.1 # https:/
+00000790: 2f67 6974 6875 622e 636f 6d2f 6e61 7061  /github.com/napa
+000007a0: 7269 2f6e 6170 6172 692f 7075 6c6c 2f35  ri/napari/pull/5
+000007b0: 3136 380d 0a09 7265 646c 696f 6e66 6973  168...redlionfis
+000007c0: 680d 0a09 6a75 7079 7465 725f 7365 7276  h...jupyter_serv
+000007d0: 6572 3c32 2e30 2e30 2023 2068 7474 7073  er<2.0.0 # https
+000007e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+000007f0: 7079 7465 722d 7365 7276 6572 2f6a 7570  pyter-server/jup
+00000800: 7974 6572 5f73 6572 7665 722f 6973 7375  yter_server/issu
+00000810: 6573 2f31 3132 370d 0a09 6365 6c6c 706f  es/1127...cellpo
+00000820: 7365 2d6e 6170 6172 690d 0a09 7365 6162  se-napari...seab
+00000830: 6f72 6e0d 0a0d 0a5b 6f70 7469 6f6e 732e  orn....[options.
+00000840: 656e 7472 795f 706f 696e 7473 5d0d 0a6e  entry_points]..n
+00000850: 6170 6172 692e 706c 7567 696e 203d 200d  apari.plugin = .
+00000860: 0a09 6465 7662 696f 5f6e 6170 6172 6920  ..devbio_napari 
+00000870: 3d20 6465 7662 696f 5f6e 6170 6172 690d  = devbio_napari.
+00000880: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+00000890: 203d 200d 0a09 6465 7662 696f 2d6e 6170   = ...devbio-nap
+000008a0: 6172 6920 3d20 6465 7662 696f 5f6e 6170  ari = devbio_nap
+000008b0: 6172 693a 6d61 696e 0d0a 0d0a 5b65 6767  ari:main....[egg
+000008c0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000008d0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000008e0: 2030 0d0a 0d0a                            0....
```


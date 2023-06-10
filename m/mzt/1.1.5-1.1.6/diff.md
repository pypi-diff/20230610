# Comparing `tmp/mzt-1.1.5.tar.gz` & `tmp/mzt-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzt-1.1.5.tar", last modified: Tue Apr 25 17:43:56 2023, max compression
+gzip compressed data, was "mzt-1.1.6.tar", last modified: Sat Jun 10 08:11:00 2023, max compression
```

## Comparing `mzt-1.1.5.tar` & `mzt-1.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    34523 2022-08-18 14:03:37.000000 mzt-1.1.5/LICENSE
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1246 2023-04-25 17:43:56.749558 mzt-1.1.5/PKG-INFO
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      715 2022-11-15 07:23:34.000000 mzt-1.1.5/README.md
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.745558 mzt-1.1.5/modelZoo/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      812 2023-04-25 17:36:17.000000 mzt-1.1.5/modelZoo/__init__.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.745558 mzt-1.1.5/modelZoo/graphs/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       47 2023-04-25 17:36:17.000000 mzt-1.1.5/modelZoo/graphs/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1585 2022-08-18 14:03:37.000000 mzt-1.1.5/modelZoo/graphs/dgcnn.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4341 2022-08-18 14:03:37.000000 mzt-1.1.5/modelZoo/mbnetv2.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     2016 2022-08-18 14:03:37.000000 mzt-1.1.5/modelZoo/shufflenet.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.745558 mzt-1.1.5/moduleZoo/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      777 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/__init__.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/attention/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      680 2022-08-18 14:48:00.000000 mzt-1.1.5/moduleZoo/attention/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    10289 2022-09-07 14:47:25.000000 mzt-1.1.5/moduleZoo/attention/conv_multi_head_attention.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      708 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/attention/conv_self_attention.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4730 2022-09-07 11:36:52.000000 mzt-1.1.5/moduleZoo/attention/linear_multi_head_attention.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      379 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/attention/utils.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/convolution/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      958 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/convolution/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     8907 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/convolution/convblocks.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     7226 2023-04-25 17:36:17.000000 mzt-1.1.5/moduleZoo/convolution/invertedconvblocks.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/dense/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       88 2022-08-18 14:49:30.000000 mzt-1.1.5/moduleZoo/dense/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1454 2022-08-18 14:48:27.000000 mzt-1.1.5/moduleZoo/dense/denseblocks.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/graphs/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       63 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/graphs/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     2519 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/graphs/grah_conv.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      947 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/graphs/utils.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/resblocks/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1175 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/resblocks/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     7821 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/resblocks/bottleneckresidual.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     5485 2023-04-25 17:36:17.000000 mzt-1.1.5/moduleZoo/resblocks/invertedresidual.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     6098 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/resblocks/residual.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      487 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/utils.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/mzExtras/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4018 2022-08-18 14:03:37.000000 mzt-1.1.5/mzExtras/LARC.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       44 2022-08-18 14:03:37.000000 mzt-1.1.5/mzExtras/__init__.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/mzLosses/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1963 2022-08-18 14:03:37.000000 mzt-1.1.5/mzLosses/contrastive.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/mzt.egg-info/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1246 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/PKG-INFO
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      962 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/SOURCES.txt
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)        1 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/dependency_links.txt
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       37 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/top_level.txt
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       38 2023-04-25 17:43:56.749558 mzt-1.1.5/setup.cfg
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1317 2023-04-25 17:41:01.000000 mzt-1.1.5/setup.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.682174 mzt-1.1.6/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    34523 2022-08-18 14:03:37.000000 mzt-1.1.6/LICENSE
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1246 2023-06-10 08:11:00.682174 mzt-1.1.6/PKG-INFO
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      715 2022-11-15 07:23:34.000000 mzt-1.1.6/README.md
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/modelZoo/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      813 2023-06-08 03:25:24.000000 mzt-1.1.6/modelZoo/__init__.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/modelZoo/graphs/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       47 2023-04-25 17:36:17.000000 mzt-1.1.6/modelZoo/graphs/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1585 2022-08-18 14:03:37.000000 mzt-1.1.6/modelZoo/graphs/dgcnn.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4341 2022-08-18 14:03:37.000000 mzt-1.1.6/modelZoo/mbnetv2.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     2016 2022-08-18 14:03:37.000000 mzt-1.1.6/modelZoo/shufflenet.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/moduleZoo/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      777 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/__init__.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/moduleZoo/attention/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      680 2023-06-04 23:52:02.000000 mzt-1.1.6/moduleZoo/attention/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    14550 2023-06-10 07:50:40.000000 mzt-1.1.6/moduleZoo/attention/conv_multi_head_attention.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      823 2023-06-10 07:52:16.000000 mzt-1.1.6/moduleZoo/attention/conv_self_attention.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     5473 2023-06-09 15:27:57.000000 mzt-1.1.6/moduleZoo/attention/linear_multi_head_attention.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      379 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/attention/utils.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/moduleZoo/convolution/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      958 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/convolution/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     8907 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/convolution/convblocks.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     7226 2023-06-08 03:25:35.000000 mzt-1.1.6/moduleZoo/convolution/invertedconvblocks.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/moduleZoo/dense/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       88 2022-08-18 14:49:30.000000 mzt-1.1.6/moduleZoo/dense/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1454 2022-08-18 14:48:27.000000 mzt-1.1.6/moduleZoo/dense/denseblocks.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/moduleZoo/graphs/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      320 2023-06-08 00:04:03.000000 mzt-1.1.6/moduleZoo/graphs/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     5468 2023-06-09 07:48:58.000000 mzt-1.1.6/moduleZoo/graphs/grah_conv.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      950 2023-06-08 15:13:14.000000 mzt-1.1.6/moduleZoo/graphs/utils.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.678174 mzt-1.1.6/moduleZoo/resblocks/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1175 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/resblocks/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     7821 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/resblocks/bottleneckresidual.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     5485 2023-04-25 17:36:17.000000 mzt-1.1.6/moduleZoo/resblocks/invertedresidual.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     6098 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/resblocks/residual.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      487 2022-08-18 14:03:37.000000 mzt-1.1.6/moduleZoo/utils.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.682174 mzt-1.1.6/mzExtras/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4018 2022-08-18 14:03:37.000000 mzt-1.1.6/mzExtras/LARC.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       44 2022-08-18 14:03:37.000000 mzt-1.1.6/mzExtras/__init__.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.682174 mzt-1.1.6/mzLosses/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1963 2022-08-18 14:03:37.000000 mzt-1.1.6/mzLosses/contrastive.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-06-10 08:11:00.682174 mzt-1.1.6/mzt.egg-info/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1246 2023-06-10 08:11:00.000000 mzt-1.1.6/mzt.egg-info/PKG-INFO
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      962 2023-06-10 08:11:00.000000 mzt-1.1.6/mzt.egg-info/SOURCES.txt
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)        1 2023-06-10 08:11:00.000000 mzt-1.1.6/mzt.egg-info/dependency_links.txt
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       37 2023-06-10 08:11:00.000000 mzt-1.1.6/mzt.egg-info/top_level.txt
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       38 2023-06-10 08:11:00.682174 mzt-1.1.6/setup.cfg
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1317 2023-06-10 08:01:15.000000 mzt-1.1.6/setup.py
```

### Comparing `mzt-1.1.5/LICENSE` & `mzt-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/PKG-INFO` & `mzt-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Package to host DeepLearning modules for pytorch ecosystem, to ease out model implementations.
 Home-page: https://github.com/ShivamPR21/ModuleZooTorch.git
 Author: Shivam Pandey
 Author-email: pandeyshivam2017robotics@gmail.com
 License: AGPLv3+
 Keywords: DeepLearning Pytorch Modules
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mzt-1.1.5/README.md` & `mzt-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/modelZoo/__init__.py` & `mzt-1.1.6/modelZoo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-'''
-Copyright (C) 2021  Shivam Pandey
+""" Copyright (C) 2021  Shivam Pandey.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published
 by the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
-'''
+"""
 
 from .graphs import DGCNN
 
 # from .mbnetv2 import MobileNetV2
 # from .shufflenet import ShuffleInvertedResidual
 
 __all__ = ('DGCNN',)
```

### Comparing `mzt-1.1.5/modelZoo/graphs/dgcnn.py` & `mzt-1.1.6/modelZoo/graphs/dgcnn.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/modelZoo/mbnetv2.py` & `mzt-1.1.6/modelZoo/mbnetv2.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/modelZoo/shufflenet.py` & `mzt-1.1.6/modelZoo/shufflenet.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/__init__.py` & `mzt-1.1.6/moduleZoo/__init__.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/attention/__init__.py` & `mzt-1.1.6/moduleZoo/attention/__init__.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/attention/conv_self_attention.py` & `mzt-1.1.6/moduleZoo/attention/conv_self_attention.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from typing import Tuple, Union
+from typing import Tuple
 
 from . import MultiHeadSelfAttention1d, MultiHeadSelfAttention2d
 
 
 class SelfAttention2d(MultiHeadSelfAttention2d):
 
-    def __init__(self, in_channels: int, out_channels: int, reduction_factor: int = 8, residual: bool = True, kernel_size: Union[int, Tuple[int, int]] = 1):
-        super().__init__(in_channels, out_channels, 1, reduction_factor, residual, kernel_size)
+    def __init__(self, in_channels: int, out_channels: int | None = None,
+                 residual: bool = True, kernel_size: int | Tuple[int, int] = 1,
+                 channel_cross_attention: bool = False):
+        super().__init__(in_channels, out_channels, 1, residual, kernel_size, channel_cross_attention)
 
 
 class SelfAttention1d(MultiHeadSelfAttention1d):
 
-    def __init__(self, in_channels: int, out_channels: int, reduction_factor: int = 8, residual: bool = True, kernel_size: Union[int, Tuple[int, int]] = 1):
-        super().__init__(in_channels, out_channels, 1, reduction_factor, residual, kernel_size)
+    def __init__(self, in_channels: int, out_channels: int | None = None,
+                 residual: bool = True, kernel_size: int | Tuple[int, int] = 1,
+                 channel_cross_attention: bool = False):
+        super().__init__(in_channels, out_channels, 1, residual, kernel_size, channel_cross_attention)
```

### Comparing `mzt-1.1.5/moduleZoo/attention/linear_multi_head_attention.py` & `mzt-1.1.6/moduleZoo/attention/linear_multi_head_attention.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 import torch
 import torch.nn as nn
 from torch.nn.functional import interpolate
 
 from .utils import split_cat
 
 
 class MultiHeadAttentionLinear(nn.Module):
-    """ Multi HeadSelf attention Layer"""
+    """ Multi Head Self attention Layer."""
     def __init__(self,
                  in_dim: int,
                  out_dim: Optional[int] = None,
                  y_in_dim: Optional[int] = None,
                  y_out_dim: Optional[int] = None,
                  n_heads: int = 1,
                  residual: bool = True,
@@ -40,73 +40,94 @@
         self.gamma = nn.Parameter(torch.rand((n_heads, 1, 1) if n_heads == 1 else (n_heads, 1, 1, 1))+0.001) if self.residual else None
 
         self.proj = 'id' if self.y_out_dim//self.n_heads == self.y_in_dim and not self.residual else 'projection'
         self.projection = nn.Linear(self.y_in_dim, self.y_out_dim//self.n_heads, bias=False) if self.proj == 'projection' else None
 
         self.softmax = nn.Softmax(dim=-1)
 
-    def forward(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+    def extract_qkv(self, x:torch.Tensor, y:torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        q, k, v = self.query(x), self.key(x), self.value(y)
+        return q, k, v
+
+    def forward(self, x: torch.Tensor, y: torch.Tensor,
+                proj_query: torch.Tensor | None = None,
+                proj_key: torch.Tensor | None = None,
+                proj_value: torch.Tensor | None = None) -> torch.Tensor:
+        # trunk-ignore(ruff/D401)
         """
             inputs :
-                x : input feature maps( B X 1 X N)
-                y : feature map attention to be applied
+                x : input feature maps( B X k X N) or ( B X N)
+                y : feature map attention to be applied( B X k X ON) or ( B X ON)
             returns :
-                out : self attention value or + input feature
+                out : self attention value or + input feature..
         """
-        b, n = x.size()
-        B, N = y.size()
+        final_squeeze = False
 
-        assert(b == B)
+        if x.ndim == 2:
+            x = x.unsqueeze(dim=1)
+            final_squeeze = True
 
-        proj_query = self.query(x).unsqueeze(dim=1) # B X 1 X N * n_heads
-        proj_key = self.key(x).unsqueeze(dim=1) # B X 1 X N * n_heads
+        if y.ndim == 2:
+            y = y.unsqueeze(dim=1)
+            final_squeeze = True
 
-        proj_value = self.value(y).unsqueeze(dim=1) # B X 1 X ON * n_heads
+        assert(x.ndim == 3 and y.ndim == 3)
+
+        b, k, n = x.size()
+        B, K, N = y.size()
+
+        assert(b == B and k == K)
+
+        if (proj_query is None or proj_key is None or proj_value is None):
+            # B X k X N * n_heads # B X k X N * n_heads # B X k X ON * n_heads
+            proj_query, proj_key, proj_value = self.extract_qkv(x, y)
 
         if self.n_heads != 1:
             split_size = [self.out_dim//self.n_heads, self.out_dim//self.n_heads, self.y_out_dim//self.n_heads]
-            # n_heads*B X 1 X N, n_heads*B X 1 X N, n_heads*B X 1 X ON
+            # n_heads*B X k X N, n_heads*B X k X N, n_heads*B X k X ON
             proj_query, proj_key, proj_value = \
                 split_cat(proj_query, split_size[0], 2, 0), \
                     split_cat(proj_key, split_size[1], 2, 0), \
                         split_cat(proj_value, split_size[2], 2, 0)
 
-        proj_query = proj_query.transpose(2, 1) # n_heads*B X N X 1
+        proj_query = proj_query.transpose(2, 1) # n_heads*B X N X k
 
         energy = torch.bmm(proj_query,proj_key) # transpose check # n_heads*B X N X N
         attention = self.softmax(energy) # n_heads*B X N X N
 
         if self.out_dim != self.y_out_dim:
             assert(self.interpolation_mode is not None)
             attention = interpolate(attention,
                                     (self.y_out_dim, self.y_out_dim),
                                     mode=self.interpolation_mode) # B, ON, ON
 
-        out = torch.bmm(proj_value, attention.transpose(2, 1)) # n_heads*B X 1 X ON
+        out = torch.bmm(proj_value, attention.transpose(2, 1)) # n_heads*B X k X ON
+
+        out = split_cat(out, B, 0, -1) # n_heads X B X 1 X ON
 
         if self.residual:
             if self.projection is not None:
-                y = self.projection(y).unsqueeze(dim=1) # B X 1 X ON
+                y = self.projection(y) # B X k X ON
 
-            if self.n_heads != 1:
-                out = split_cat(out, B, 0, -1) # n_heads X B X 1 X ON
-                y = y.unsqueeze(dim=0).repeat(self.n_heads, 1, 1, 1) # n_head X B X 1 X ON
+            y = y.unsqueeze(dim=0).repeat(self.n_heads, 1, 1, 1) # n_head X B X k X ON
 
             out = (self.gamma*out + y)/(1 + self.gamma)
 
-            if self.n_heads != 1:
-                out = split_cat(out, 1, 0, 2).squeeze(dim=0) # B X n_heads X ON
+        out = out.permute(1, 0, 2, 3) # B X n_heads X k X ON
 
-            return out
+        # print(f'{out.shape = }')
 
-        out = split_cat(out, B, 0, 1) # B X n_heads X ON
+        if final_squeeze:
+            out = out.squeeze(dim=2) # B X n_heads X ON
+            if self.n_heads == 1:
+                out = out.squeeze(dim=1) # B X ON
 
         return out
 
-    def shape(self, in_shape: int, y_in_shape: int):
+    def shape(self, in_shape: int, y_in_shape: int) -> int | List[int]:
         return self.y_out_dim//self.n_heads
 
 class MultiHeadSelfAttentionLinear(MultiHeadAttentionLinear):
 
     def __init__(self, in_dim: int, out_dim: Optional[int] = None, n_heads: int = 1, residual: bool = True):
         super().__init__(in_dim, out_dim, in_dim, out_dim, n_heads, residual, None)
```

### Comparing `mzt-1.1.5/moduleZoo/convolution/__init__.py` & `mzt-1.1.6/moduleZoo/convolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/convolution/convblocks.py` & `mzt-1.1.6/moduleZoo/convolution/convblocks.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/convolution/invertedconvblocks.py` & `mzt-1.1.6/moduleZoo/convolution/invertedconvblocks.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/dense/denseblocks.py` & `mzt-1.1.6/moduleZoo/dense/denseblocks.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/graphs/utils.py` & `mzt-1.1.6/moduleZoo/graphs/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import torch
 
 
 def knn(x: torch.Tensor, k: int) -> torch.Tensor:
-    # Assumed shape of x [B, n, d]
+    # Assumed shape of x -> [B, n, d]
     x = x.unsqueeze(dim=1) # [B, 1, n, d]
     n_x = x.transpose(2, 1) # [B, n, 1, d]
 
     x = -torch.sum((x - n_x)**2, dim=-1) # [B, n, n]
     idx = x.topk(k, dim=-1, sorted=True)[1] # [B, n, k], sorted indexes
 
     return idx
```

### Comparing `mzt-1.1.5/moduleZoo/resblocks/__init__.py` & `mzt-1.1.6/moduleZoo/resblocks/__init__.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/resblocks/bottleneckresidual.py` & `mzt-1.1.6/moduleZoo/resblocks/bottleneckresidual.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/resblocks/invertedresidual.py` & `mzt-1.1.6/moduleZoo/resblocks/invertedresidual.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/moduleZoo/resblocks/residual.py` & `mzt-1.1.6/moduleZoo/resblocks/residual.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/mzExtras/LARC.py` & `mzt-1.1.6/mzExtras/LARC.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/mzLosses/contrastive.py` & `mzt-1.1.6/mzLosses/contrastive.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/mzt.egg-info/PKG-INFO` & `mzt-1.1.6/mzt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Package to host DeepLearning modules for pytorch ecosystem, to ease out model implementations.
 Home-page: https://github.com/ShivamPR21/ModuleZooTorch.git
 Author: Shivam Pandey
 Author-email: pandeyshivam2017robotics@gmail.com
 License: AGPLv3+
 Keywords: DeepLearning Pytorch Modules
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mzt-1.1.5/mzt.egg-info/SOURCES.txt` & `mzt-1.1.6/mzt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mzt-1.1.5/setup.py` & `mzt-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "mzt",
-    version = "1.1.5",
+    version = "1.1.6",
     author = "Shivam Pandey",
     author_email = "pandeyshivam2017robotics@gmail.com",
     description = ("Package to host DeepLearning modules for pytorch ecosystem,"
                    " to ease out model implementations."),
     license = "AGPLv3+",
     keywords = "DeepLearning Pytorch Modules",
     url = "https://github.com/ShivamPR21/ModuleZooTorch.git",
```


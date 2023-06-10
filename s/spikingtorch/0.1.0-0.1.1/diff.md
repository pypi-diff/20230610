# Comparing `tmp/spikingtorch-0.1.0.tar.gz` & `tmp/spikingtorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikingtorch-0.1.0.tar", last modified: Tue Apr  4 16:49:07 2023, max compression
+gzip compressed data, was "spikingtorch-0.1.1.tar", last modified: Sat Jun 10 01:44:13 2023, max compression
```

## Comparing `spikingtorch-0.1.0.tar` & `spikingtorch-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-04 16:49:07.077272 spikingtorch-0.1.0/
--rw-r--r--   0 anglyan    (502) staff       (20)     1765 2023-04-04 16:38:00.000000 spikingtorch-0.1.0/LICENSE.md
--rw-r--r--   0 anglyan    (502) staff       (20)     1668 2023-04-04 16:49:07.077105 spikingtorch-0.1.0/PKG-INFO
--rw-r--r--   0 anglyan    (502) staff       (20)     1117 2023-04-04 16:45:30.000000 spikingtorch-0.1.0/README.md
--rw-r--r--   0 anglyan    (502) staff       (20)      680 2023-04-04 05:00:53.000000 spikingtorch-0.1.0/pyproject.toml
--rw-r--r--   0 anglyan    (502) staff       (20)       38 2023-04-04 16:49:07.077314 spikingtorch-0.1.0/setup.cfg
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-04 16:49:07.074635 spikingtorch-0.1.0/src/
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-04 16:49:07.076013 spikingtorch-0.1.0/src/spikingtorch/
--rw-r--r--   0 anglyan    (502) staff       (20)       50 2023-04-04 05:10:07.000000 spikingtorch-0.1.0/src/spikingtorch/__init__.py
--rw-r--r--   0 anglyan    (502) staff       (20)     2287 2023-04-04 05:49:12.000000 spikingtorch-0.1.0/src/spikingtorch/spikeio.py
--rw-r--r--   0 anglyan    (502) staff       (20)     3940 2023-04-04 13:25:44.000000 spikingtorch-0.1.0/src/spikingtorch/spikingnet.py
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-04 16:49:07.076905 spikingtorch-0.1.0/src/spikingtorch.egg-info/
--rw-r--r--   0 anglyan    (502) staff       (20)     1668 2023-04-04 16:49:07.000000 spikingtorch-0.1.0/src/spikingtorch.egg-info/PKG-INFO
--rw-r--r--   0 anglyan    (502) staff       (20)      322 2023-04-04 16:49:07.000000 spikingtorch-0.1.0/src/spikingtorch.egg-info/SOURCES.txt
--rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-04 16:49:07.000000 spikingtorch-0.1.0/src/spikingtorch.egg-info/dependency_links.txt
--rw-r--r--   0 anglyan    (502) staff       (20)        6 2023-04-04 16:49:07.000000 spikingtorch-0.1.0/src/spikingtorch.egg-info/requires.txt
--rw-r--r--   0 anglyan    (502) staff       (20)       13 2023-04-04 16:49:07.000000 spikingtorch-0.1.0/src/spikingtorch.egg-info/top_level.txt
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-06-10 01:44:13.262377 spikingtorch-0.1.1/
+-rw-r--r--   0 anglyan    (502) staff       (20)     1766 2023-06-09 22:10:24.000000 spikingtorch-0.1.1/LICENSE.md
+-rw-r--r--   0 anglyan    (502) staff       (20)     1668 2023-06-10 01:44:13.262190 spikingtorch-0.1.1/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)     1117 2023-06-09 22:15:01.000000 spikingtorch-0.1.1/README.md
+-rw-r--r--   0 anglyan    (502) staff       (20)      680 2023-06-10 01:37:47.000000 spikingtorch-0.1.1/pyproject.toml
+-rw-r--r--   0 anglyan    (502) staff       (20)       38 2023-06-10 01:44:13.262421 spikingtorch-0.1.1/setup.cfg
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-06-10 01:44:13.259163 spikingtorch-0.1.1/src/
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-06-10 01:44:13.261073 spikingtorch-0.1.1/src/spikingtorch/
+-rw-r--r--   0 anglyan    (502) staff       (20)      170 2023-06-09 22:12:01.000000 spikingtorch-0.1.1/src/spikingtorch/__init__.py
+-rw-r--r--   0 anglyan    (502) staff       (20)     3852 2023-06-09 22:11:47.000000 spikingtorch-0.1.1/src/spikingtorch/layers.py
+-rw-r--r--   0 anglyan    (502) staff       (20)     2841 2023-06-09 23:09:52.000000 spikingtorch-0.1.1/src/spikingtorch/spikeio.py
+-rw-r--r--   0 anglyan    (502) staff       (20)      703 2023-06-09 22:40:45.000000 spikingtorch-0.1.1/src/spikingtorch/spikingnet.py
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-06-10 01:44:13.261967 spikingtorch-0.1.1/src/spikingtorch.egg-info/
+-rw-r--r--   0 anglyan    (502) staff       (20)     1668 2023-06-10 01:44:13.000000 spikingtorch-0.1.1/src/spikingtorch.egg-info/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)      349 2023-06-10 01:44:13.000000 spikingtorch-0.1.1/src/spikingtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-06-10 01:44:13.000000 spikingtorch-0.1.1/src/spikingtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        6 2023-06-10 01:44:13.000000 spikingtorch-0.1.1/src/spikingtorch.egg-info/requires.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)       13 2023-06-10 01:44:13.000000 spikingtorch-0.1.1/src/spikingtorch.egg-info/top_level.txt
```

### Comparing `spikingtorch-0.1.0/LICENSE.md` & `spikingtorch-0.1.1/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright © 2020-2023, UChicago Argonne, LLC
 All Rights Reserved
-Software Name: Spikingtorch
+Software Name: spikingtorch
 
 By: Argonne National Laboratory
 
 OPEN SOURCE LICENSE
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
@@ -18,7 +18,8 @@
 
 
 ********************************************************************************
 DISCLAIMER
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ********************************************************************************
+
```

### Comparing `spikingtorch-0.1.0/PKG-INFO` & `spikingtorch-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikingtorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Inference and backprop training of spiking neural networks in Pytorch
 Author: Angel Yanguas-Gil
 Project-URL: Homepage, https://github.com/spikingnn/spikingtorch
 Keywords: spiking neurons,neural networks,AI,Pytorch,neuromorphic computing,spiking neural networks,neuroscience
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -52,13 +52,13 @@
 hardware, arXiv:2007.06176](https://arxiv.org/abs/2007.06176)
 
 
 ## Copyright and license
 
 Copyright © 2020-2022, UChicago Argonne, LLC
 
-Spikelearn is distributed under the terms of BSD License. See 
+spikelearn is distributed under the terms of BSD License. See 
 [LICENSE](https://github.com/spikingnn/spikingtorch/blob/master/LICENSE.md)
```

### Comparing `spikingtorch-0.1.0/README.md` & `spikingtorch-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,13 +39,13 @@
 hardware, arXiv:2007.06176](https://arxiv.org/abs/2007.06176)
 
 
 ## Copyright and license
 
 Copyright © 2020-2022, UChicago Argonne, LLC
 
-Spikelearn is distributed under the terms of BSD License. See 
+spikelearn is distributed under the terms of BSD License. See 
 [LICENSE](https://github.com/spikingnn/spikingtorch/blob/master/LICENSE.md)
```

### Comparing `spikingtorch-0.1.0/pyproject.toml` & `spikingtorch-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spikingtorch"
 authors = [
 { name="Angel Yanguas-Gil"}]
-version = "0.1.0"
+version = "0.1.1"
 description = "Inference and backprop training of spiking neural networks in Pytorch"
 readme = "README.md"
 keywords = ["spiking neurons", "neural networks", "AI", "Pytorch",
     "neuromorphic computing", "spiking neural networks", "neuroscience"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
```

### Comparing `spikingtorch-0.1.0/src/spikingtorch/spikeio.py` & `spikingtorch-0.1.1/src/spikingtorch/spikeio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,56 @@
-import torch
-
+# Copyright © 2020-2023, UChicago Argonne, LLC
+# All Rights Reserved
+# Software Name: spikingtorch
 
+import torch
 
 class PoissonEncoder:
 
     def __init__(self, nsteps, scale=1.0):
         self.nsteps = nsteps
         self.scale = scale
 
     def __call__(self, x):
 
-        kernel = torch.unsqueeze(x, 1)
         slist = []
         for _ in range(self.nsteps):
-            base = torch.rand_like(kernel)
-            base[self.scale*kernel<base] = 0.0
+            base = torch.rand_like(x)
+            base[self.scale*x<base] = 0.0
             base[base>0] = 1.0
             slist.append(base)
 
-        return torch.concat(slist, dim=1)
+        return torch.concat(slist, dim=1).detach()
+
+
+class PeriodicEncoder:
+
+    def __init__(self, nsteps, scale=1.0):
+        self.nsteps = nsteps
+        self.scale = scale
+
+    def __call__(self, x):
+
+        slist = []
+        memory = torch.zeros_like(x)
+        for _ in range(self.nsteps):
+            memory += self.scale*x
+            out = torch.clone(memory)
+            out[out<1] = 0
+            out[out>0] = 1
+            memory[out > 0] = 0
+            slist.append(out)
+
+        return torch.concat(slist, dim=1).detach()
 
 
 class RateDecoder:
     
     def __call__(self, x):
-        return torch.mean(x)
+        return torch.mean(x, dim=1)
 
 
 class SumDecoder:
 
     def __init__(self, nsteps, scale, offset=True):
         self.scale = scale
         self.nsteps = nsteps
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spikingtorch-0.1.0/src/spikingtorch.egg-info/PKG-INFO` & `spikingtorch-0.1.1/src/spikingtorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikingtorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Inference and backprop training of spiking neural networks in Pytorch
 Author: Angel Yanguas-Gil
 Project-URL: Homepage, https://github.com/spikingnn/spikingtorch
 Keywords: spiking neurons,neural networks,AI,Pytorch,neuromorphic computing,spiking neural networks,neuroscience
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -52,13 +52,13 @@
 hardware, arXiv:2007.06176](https://arxiv.org/abs/2007.06176)
 
 
 ## Copyright and license
 
 Copyright © 2020-2022, UChicago Argonne, LLC
 
-Spikelearn is distributed under the terms of BSD License. See 
+spikelearn is distributed under the terms of BSD License. See 
 [LICENSE](https://github.com/spikingnn/spikingtorch/blob/master/LICENSE.md)
```


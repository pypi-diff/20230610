# Comparing `tmp/adv-ml-0.0.2.tar.gz` & `tmp/adv-ml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adv-ml-0.0.2.tar", last modified: Thu May 18 14:34:08 2023, max compression
+gzip compressed data, was "adv-ml-0.0.4.tar", last modified: Sat Jun 10 10:07:31 2023, max compression
```

## Comparing `adv-ml-0.0.2.tar` & `adv-ml-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 14:34:08.191524 adv-ml-0.0.2/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-05-17 06:04:26.000000 adv-ml-0.0.2/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-27 10:12:58.000000 adv-ml-0.0.2/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4291 2023-05-18 14:34:08.191524 adv-ml-0.0.2/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2327 2023-05-18 14:32:34.000000 adv-ml-0.0.2/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 14:34:08.187524 adv-ml-0.0.2/adv_ml/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       22 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     6601 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      162 2023-05-18 13:43:34.000000 adv-ml-0.0.2/adv_ml/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2902 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/evasion.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3396 2023-05-18 14:34:03.000000 adv-ml-0.0.2/adv_ml/input_optimization.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 14:34:08.191524 adv-ml-0.0.2/adv_ml.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4291 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      360 2023-05-18 14:34:08.000000 adv-ml-0.0.2/adv_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       55 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 08:49:32.000000 adv-ml-0.0.2/adv_ml.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       50 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        7 2023-05-18 14:34:07.000000 adv-ml-0.0.2/adv_ml.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1081 2023-05-18 14:33:18.000000 adv-ml-0.0.2/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-18 14:34:08.191524 adv-ml-0.0.2/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2596 2023-04-27 10:12:58.000000 adv-ml-0.0.2/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:07:31.346856 adv-ml-0.0.4/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-06-09 06:55:18.000000 adv-ml-0.0.4/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-06-09 06:55:18.000000 adv-ml-0.0.4/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5606 2023-06-10 10:07:31.346856 adv-ml-0.0.4/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3258 2023-06-09 06:55:18.000000 adv-ml-0.0.4/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:07:31.346856 adv-ml-0.0.4/adv_ml/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       22 2023-06-10 10:07:19.000000 adv-ml-0.0.4/adv_ml/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     9691 2023-06-10 10:07:19.000000 adv-ml-0.0.4/adv_ml/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      175 2023-06-09 06:55:18.000000 adv-ml-0.0.4/adv_ml/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2146 2023-06-10 10:07:19.000000 adv-ml-0.0.4/adv_ml/backdoor.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1097 2023-06-10 10:07:19.000000 adv-ml-0.0.4/adv_ml/badnets.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3059 2023-06-10 10:07:19.000000 adv-ml-0.0.4/adv_ml/evasion.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3406 2023-06-10 10:07:19.000000 adv-ml-0.0.4/adv_ml/input_optimization.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-06-10 10:07:31.346856 adv-ml-0.0.4/adv_ml.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5606 2023-06-10 10:07:31.000000 adv-ml-0.0.4/adv_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      397 2023-06-10 10:07:31.000000 adv-ml-0.0.4/adv_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-10 10:07:31.000000 adv-ml-0.0.4/adv_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       55 2023-06-10 10:07:31.000000 adv-ml-0.0.4/adv_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-06-09 06:56:55.000000 adv-ml-0.0.4/adv_ml.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       56 2023-06-10 10:07:31.000000 adv-ml-0.0.4/adv_ml.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        7 2023-06-10 10:07:31.000000 adv-ml-0.0.4/adv_ml.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1084 2023-06-10 10:07:13.000000 adv-ml-0.0.4/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-06-10 10:07:31.346856 adv-ml-0.0.4/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2596 2023-06-09 06:55:18.000000 adv-ml-0.0.4/setup.py
```

### Comparing `adv-ml-0.0.2/LICENSE` & `adv-ml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adv-ml-0.0.2/README.md` & `adv-ml-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -42,94 +42,142 @@
       <th>accuracy</th>
       <th>time</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>0</td>
-      <td>0.160490</td>
-      <td>0.165644</td>
-      <td>0.954900</td>
-      <td>00:17</td>
+      <td>0.154410</td>
+      <td>0.177410</td>
+      <td>0.953900</td>
+      <td>00:32</td>
     </tr>
   </tbody>
 </table>
 
 ``` python
 sub_dsets = mnist.valid.random_sub_dsets(64)
 learn.show_results(shuffle=False, dl=sub_dsets.dl())
 ```
 
 ![](index_files/figure-commonmark/cell-4-output-2.png)
 
 ``` python
-attack = InputOptimizer(classifier, LinfPGD(epsilon=.15), n_epochs=10)
+attack = InputOptimizer(classifier, LinfPGD(epsilon=.15), n_epochs=10, epoch_size=20)
 perturbed_dsets = attack.perturb(sub_dsets)
 ```
 
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: left;">
       <th>epoch</th>
       <th>train_loss</th>
       <th>time</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>0</td>
-      <td>-3.627444</td>
+      <td>-4.302573</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>1</td>
-      <td>-6.452563</td>
+      <td>-7.585707</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>2</td>
-      <td>-7.652328</td>
+      <td>-9.014968</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>3</td>
-      <td>-8.258670</td>
+      <td>-9.700548</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>4</td>
-      <td>-8.617092</td>
+      <td>-10.075110</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>5</td>
-      <td>-8.851709</td>
+      <td>-10.296636</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>6</td>
-      <td>-9.014016</td>
+      <td>-10.433834</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>7</td>
-      <td>-9.130360</td>
+      <td>-10.521141</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>8</td>
-      <td>-9.216579</td>
+      <td>-10.577673</td>
       <td>00:00</td>
     </tr>
     <tr>
       <td>9</td>
-      <td>-9.281565</td>
+      <td>-10.614740</td>
       <td>00:00</td>
     </tr>
   </tbody>
 </table>
 
 ``` python
 learn.show_results(shuffle=False, dl=TfmdDL(perturbed_dsets))
 ```
 
 ![](index_files/figure-commonmark/cell-6-output-2.png)
+
+### Data Poisoning
+
+``` python
+patch = torch.tensor([[1, 0, 1],
+                      [0, 1, 0],
+                      [1, 0, 1]]).int()*255
+trigger = F.pad(patch, (25, 0, 25, 0)).numpy()
+learn = Learner(mnist.dls(), MLP(10), metrics=accuracy, cbs=BadNetsAttack(trigger, '0'))
+learn.fit_one_cycle(1)
+```
+
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: left;">
+      <th>epoch</th>
+      <th>train_loss</th>
+      <th>valid_loss</th>
+      <th>accuracy</th>
+      <th>time</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <td>0</td>
+      <td>0.103652</td>
+      <td>0.097075</td>
+      <td>0.971400</td>
+      <td>00:23</td>
+    </tr>
+  </tbody>
+</table>
+
+Benign performance:
+
+``` python
+learn.show_results()
+```
+
+![](index_files/figure-commonmark/cell-8-output-2.png)
+
+Attack success:
+
+``` python
+learn.show_results(2)
+```
+
+![](index_files/figure-commonmark/cell-9-output-2.png)
```

### Comparing `adv-ml-0.0.2/adv_ml/evasion.py` & `adv-ml-0.0.4/adv_ml/evasion.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,52 +31,53 @@
             self.p.data = (x + self.p).clamp(0., 1.) - x 
 
     def suggest_lr(self, input_opt: InputOptimizer):
         return self.epsilon / input_opt.epoch_size
 
     def before_step(self):
         with torch.no_grad():
-            self.normalize(self.p.grad)
+            self.steepest_descent()
 
     def after_batch(self):
         with torch.no_grad():
-            self.project(self.p)
+            self.project_pert()
             self.clamp_pixel_values(self.x)
 
 # %% ../nbs/evasion.ipynb 6
 @patch()
 @abstractmethod
 def rand_init(self: PGDCallback, shape) -> Tensor:
     "Initialize a random perturbation in the $\epsilon$-ball"
     ...
 
 # %% ../nbs/evasion.ipynb 7
 @patch
 @abstractmethod
-def normalize(self: PGDCallback, t) -> None:
+def steepest_descent(self: PGDCallback) -> None:
+    "Edit the perturbation's gradient to implement steepest descent"
     ...
 
 # %% ../nbs/evasion.ipynb 8
 @patch
 @abstractmethod
-def project(self: PGDCallback, t) -> None:
-    "Project to the $\epsilon$-ball"
+def project_pert(self: PGDCallback) -> None:
+    "Project the perturbation to the $\epsilon$-ball"
     ...
 
 # %% ../nbs/evasion.ipynb 20
 class LinfPGD(PGDCallback):
     "Implements PGD by bounding the $l_\infty$ norm"
     def rand_init(self, shape):
         return torch.rand(shape) * self.epsilon
 
-    def normalize(self, t):
-        t.sign_()
+    def steepest_descent(self):
+        self.p.grad.sign_()
 
-    def project(self, t):
-        t.clamp_(-self.epsilon, self.epsilon)
+    def project_pert(self):
+        self.p.clamp_(-self.epsilon, self.epsilon)
 
 # %% ../nbs/evasion.ipynb 30
 import torch.nn.functional as F
 from torch.linalg import vector_norm
 
 
 @delegates(F.normalize)
@@ -96,12 +97,13 @@
 class L2PGD(PGDCallback):
     "Implements PGD by bounding the $l_2$ norm"
     def rand_init(self, shape):
         rand_dir = _random_unit_vector(shape)
         rand_len = torch.rand(1) * self.epsilon
         return rand_dir * rand_len
 
-    def normalize(self, t):
-        t.data = _batch_normalize(self.p.grad)
+    def steepest_descent(self):
+        self.p.grad.data = _batch_normalize(self.p.grad)
 
-    def project(self, t):
-        t.mul_(torch.min(self.epsilon/_batch_norm(t), torch.ones_like(t)))
+    def project_pert(self):
+        norm = _batch_norm(self.p)
+        self.p.mul_(torch.min(self.epsilon/norm, torch.ones_like(norm)))
```

### Comparing `adv-ml-0.0.2/adv_ml/input_optimization.py` & `adv-ml-0.0.4/adv_ml/input_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/input_optimization.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/Core/input_optimization.ipynb.
 
 # %% auto 0
 __all__ = ['PerturbationCallback', 'InputOptimizer']
 
-# %% ../nbs/input_optimization.ipynb 4
+# %% ../nbs/Core/input_optimization.ipynb 4
 from typing import Type
 from abc import ABC, abstractmethod
 
 from torch import nn
 from fastai.vision.all import *
```

### Comparing `adv-ml-0.0.2/settings.ini` & `adv-ml-0.0.4/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = adv-ml
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = adv_ml
@@ -35,9 +35,9 @@
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Irad-Zehavi
 
 ### Optional ###
 requirements = fastai fastai_datasets similarity_learning
-# dev_requirements = 
+dev_requirements = nbdev
 # console_scripts =
```

### Comparing `adv-ml-0.0.2/setup.py` & `adv-ml-0.0.4/setup.py`

 * *Files identical despite different names*


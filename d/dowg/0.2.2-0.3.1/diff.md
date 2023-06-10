# Comparing `tmp/dowg-0.2.2.tar.gz` & `tmp/dowg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dowg-0.2.2.tar", last modified: Fri Jun  9 15:46:06 2023, max compression
+gzip compressed data, was "dowg-0.3.1.tar", last modified: Sat Jun 10 02:37:12 2023, max compression
```

## Comparing `dowg-0.2.2.tar` & `dowg-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.458937 dowg-0.2.2/
--rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-09 15:46:06.457936 dowg-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.2.2/README.md
--rw-rw-rw-   0        0        0      552 2023-06-09 15:45:46.000000 dowg-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 15:46:06.458937 dowg-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.431882 dowg-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.446417 dowg-0.2.2/src/dowg/
--rw-rw-rw-   0        0        0     1988 2023-06-09 15:43:56.000000 dowg-0.2.2/src/dowg/CoordinateDoWG.py
--rw-rw-rw-   0        0        0     2005 2023-06-09 15:45:29.000000 dowg-0.2.2/src/dowg/ScalarDoWG.py
--rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.2.2/src/dowg/__init__.py
--rw-rw-rw-   0        0        0      660 2023-06-09 15:41:00.000000 dowg-0.2.2/src/dowg/clip.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.456938 dowg-0.2.2/src/dowg.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:12.494187 dowg-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-10 02:37:12.493187 dowg-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.3.1/README.md
+-rw-rw-rw-   0        0        0      552 2023-06-10 02:36:58.000000 dowg-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 02:37:12.495189 dowg-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:12.452982 dowg-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:12.478279 dowg-0.3.1/src/dowg/
+-rw-rw-rw-   0        0        0     2122 2023-06-10 02:36:21.000000 dowg-0.3.1/src/dowg/CoordinateDoWG.py
+-rw-rw-rw-   0        0        0     2009 2023-06-10 02:36:29.000000 dowg-0.3.1/src/dowg/ScalarDoWG.py
+-rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.3.1/src/dowg/__init__.py
+-rw-rw-rw-   0        0        0     1243 2023-06-10 02:36:37.000000 dowg-0.3.1/src/dowg/clip.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:12.491179 dowg-0.3.1/src/dowg.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-10 02:37:12.000000 dowg-0.3.1/src/dowg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-06-10 02:37:12.000000 dowg-0.3.1/src/dowg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 02:37:12.000000 dowg-0.3.1/src/dowg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-10 02:37:12.000000 dowg-0.3.1/src/dowg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 02:37:12.492180 dowg-0.3.1/tests/
+-rw-rw-rw-   0        0        0      660 2023-06-09 15:52:18.000000 dowg-0.3.1/tests/test_CoordinateDoWG.py
```

### Comparing `dowg-0.2.2/LICENSE` & `dowg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dowg-0.2.2/PKG-INFO` & `dowg-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.2.2
+Version: 0.3.1
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dowg-0.2.2/pyproject.toml` & `dowg-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dowg"
-version = "0.2.2"
+version = "0.3.1"
 authors = [
   { name="Patrick Shanahan", email="patrick.e.shanahan@gmail.com" },
 ]
 description = "DoWG parameter-free adaptive optimizer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dowg-0.2.2/src/dowg/CoordinateDoWG.py` & `dowg-0.3.1/src/dowg/CoordinateDoWG.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,48 +9,46 @@
         Args:
             params (iterable): iterable of parameters to optimize or dicts defining
                 parameter groups
             eps (float, optional): term added to the denominator to improve
                 numerical stability (default: 1e-8)
         """
 
-    def __init__(self, params, eps=1e-8, clip=0.5, *args, **kwargs):
-        defaults = dict(epsilon=1-eps, lr=1, clip=clip)
+    def __init__(self, params, eps=1e-4, clip=0.5, *args, **kwargs):
+        defaults = dict(epsilon=eps, lr=1, clip=clip)
         super(CoordinateDoWG, self).__init__(params, defaults)
 
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
         """
         loss = None
         if closure is not None:
             loss = closure()
 
         for group in self.param_groups:
-            for p in group['params']:
-                if p.grad is None:
-                    continue
-                grad = p.grad.data
-                state = self.state[p]
-
-                # Initialize state variables
-                if 'x0' not in state:
-                    state['x0'] = torch.clone(p).detach()
-                if 'rt2' not in state:
-                    state['rt2'] = torch.zeros_like(p.data).add_(group['epsilon'])
-                if 'vt' not in state:
-                    state['vt'] = torch.zeros_like(p.data)
+            with torch.no_grad():
+                for p in group['params']:
+                    if p.grad is None:
+                        continue
+                    grad = p.grad.data.to(dtype=torch.float32)
+                    state = self.state[p]
+
+                    # Initialize state variables
+                    if 'x0' not in state:
+                        state['x0'] = p.detach().to(dtype=torch.float32)
+                    if 'rt2' not in state:
+                        state['rt2'] = torch.zeros_like(p.data).add_(group['epsilon']).to(dtype=torch.float32)
+                    if 'vt' not in state:
+                        state['vt'] = torch.zeros_like(p.data).to(dtype=torch.float32)
 
-                with torch.no_grad():
                     state['rt2'] = torch.max(state['rt2'], (p - state['x0']) ** 2)
                     rt2, vt = state['rt2'], state['vt']
                     vt.add_(rt2 * grad ** 2)
-                    gt_hat = rt2 * clip_gradient(p, group['clip'])
-                    denom = vt.sqrt().add_(group['epsilon'])
-                p.addcdiv_(gt_hat, denom, value=-1.0)
-        return loss
-    
-
+                    gt_hat = rt2 * grad.clamp(-group['clip'], group['clip'])
 
+                    denom = vt.sqrt().add_(group['epsilon'])
+                    p.data.addcdiv_(gt_hat, denom, value=-1.0)
+        return loss
```

### Comparing `dowg-0.2.2/src/dowg/ScalarDoWG.py` & `dowg-0.3.1/src/dowg/ScalarDoWG.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 
 from .clip import clip_gradient
 
 
 class ScalarDoWG(torch.optim.Optimizer):
-    def __init__(self, params, eps=1e-4, clip=0.01, *args, **kwargs):
+    def __init__(self, params, eps=1e-4, clip=0.5, *args, **kwargs):
         defaults = dict(epsilon=1-eps, lr=1, clip=clip)
         self.epsilon = 1-eps
         super(ScalarDoWG, self).__init__(params, defaults)
 
     def step(self, closure=None):
         
         state = self.state
@@ -44,9 +44,9 @@
                 state["vt"] += state["rt2"] * grad_sq_norm
                 rt2, vt = state["rt2"], state["vt"]
     
             for group in self.param_groups:
                 for p in group["params"]:
                     gt_hat = rt2 * clip_gradient(p.grad.data.clone(), group["clip"])
                     denom = torch.sqrt(vt).add_(group["epsilon"])
-                    p.addcdiv_(gt_hat, denom, value=-1.0)
+                    p.data.addcdiv_(gt_hat, denom, value=-1.0)
         return loss
```

### Comparing `dowg-0.2.2/src/dowg.egg-info/PKG-INFO` & `dowg-0.3.1/src/dowg.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.2.2
+Version: 0.3.1
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```


# Comparing `tmp/quik-ai-1.0.0.tar.gz` & `tmp/quik-ai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik-ai-1.0.0.tar", last modified: Sat Jun 10 03:33:07 2023, max compression
+gzip compressed data, was "quik-ai-1.0.1.tar", last modified: Sat Jun 10 17:43:42 2023, max compression
```

## Comparing `quik-ai-1.0.0.tar` & `quik-ai-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 03:33:07.017194 quik-ai-1.0.0/
--rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2262 2023-06-10 03:33:07.017194 quik-ai-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2023-06-10 03:32:27.000000 quik-ai-1.0.0/README.md
--rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      768 2023-06-10 03:33:07.020341 quik-ai-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 03:33:06.957850 quik-ai-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 03:33:06.990761 quik-ai-1.0.0/src/quik_ai/
--rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.0.0/src/quik_ai/__init__.py
--rw-rw-rw-   0        0        0     2158 2023-06-05 20:31:06.000000 quik-ai-1.0.0/src/quik_ai/backend.py
--rw-rw-rw-   0        0        0    11609 2023-06-08 23:02:28.000000 quik-ai-1.0.0/src/quik_ai/engine.py
--rw-rw-rw-   0        0        0     4917 2023-06-07 22:39:50.000000 quik-ai-1.0.0/src/quik_ai/heads.py
--rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.0.0/src/quik_ai/layers.py
--rw-rw-rw-   0        0        0      940 2023-06-07 22:39:39.000000 quik-ai-1.0.0/src/quik_ai/losses.py
--rw-rw-rw-   0        0        0     1291 2023-06-10 01:46:43.000000 quik-ai-1.0.0/src/quik_ai/metrics.py
--rw-rw-rw-   0        0        0    29827 2023-06-10 01:44:03.000000 quik-ai-1.0.0/src/quik_ai/models.py
--rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.0.0/src/quik_ai/optimizers.py
--rw-rw-rw-   0        0        0     8285 2023-06-09 01:51:02.000000 quik-ai-1.0.0/src/quik_ai/predictors.py
--rw-rw-rw-   0        0        0     9621 2023-06-08 21:13:03.000000 quik-ai-1.0.0/src/quik_ai/tuners.py
--rw-rw-rw-   0        0        0     3330 2023-06-07 18:32:31.000000 quik-ai-1.0.0/src/quik_ai/tuning.py
-drwxrwxrwx   0        0        0        0 2023-06-10 03:33:07.015236 quik-ai-1.0.0/src/quik_ai.egg-info/
--rw-rw-rw-   0        0        0     2262 2023-06-10 03:33:06.000000 quik-ai-1.0.0/src/quik_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-10 03:33:06.000000 quik-ai-1.0.0/src/quik_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 03:33:06.000000 quik-ai-1.0.0/src/quik_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-06-10 03:33:06.000000 quik-ai-1.0.0/src/quik_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 03:33:06.000000 quik-ai-1.0.0/src/quik_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.283012 quik-ai-1.0.1/
+-rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2262 2023-06-10 17:43:42.284011 quik-ai-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1724 2023-06-10 03:32:27.000000 quik-ai-1.0.1/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      768 2023-06-10 17:43:42.294007 quik-ai-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.216522 quik-ai-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.254092 quik-ai-1.0.1/src/quik_ai/
+-rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.0.1/src/quik_ai/__init__.py
+-rw-rw-rw-   0        0        0     2158 2023-06-05 20:31:06.000000 quik-ai-1.0.1/src/quik_ai/backend.py
+-rw-rw-rw-   0        0        0    11609 2023-06-08 23:02:28.000000 quik-ai-1.0.1/src/quik_ai/engine.py
+-rw-rw-rw-   0        0        0     4917 2023-06-07 22:39:50.000000 quik-ai-1.0.1/src/quik_ai/heads.py
+-rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.0.1/src/quik_ai/layers.py
+-rw-rw-rw-   0        0        0      940 2023-06-07 22:39:39.000000 quik-ai-1.0.1/src/quik_ai/losses.py
+-rw-rw-rw-   0        0        0     1291 2023-06-10 01:46:43.000000 quik-ai-1.0.1/src/quik_ai/metrics.py
+-rw-rw-rw-   0        0        0    29903 2023-06-10 15:57:06.000000 quik-ai-1.0.1/src/quik_ai/models.py
+-rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.0.1/src/quik_ai/optimizers.py
+-rw-rw-rw-   0        0        0     8285 2023-06-10 16:20:00.000000 quik-ai-1.0.1/src/quik_ai/predictors.py
+-rw-rw-rw-   0        0        0     9621 2023-06-08 21:13:03.000000 quik-ai-1.0.1/src/quik_ai/tuners.py
+-rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.0.1/src/quik_ai/tuning.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:43:42.282049 quik-ai-1.0.1/src/quik_ai.egg-info/
+-rw-rw-rw-   0        0        0     2262 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 17:43:42.000000 quik-ai-1.0.1/src/quik_ai.egg-info/top_level.txt
```

### Comparing `quik-ai-1.0.0/LICENSE` & `quik-ai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/PKG-INFO` & `quik-ai-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.1.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quik-ai-1.0.0/README.md` & `quik-ai-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/setup.cfg` & `quik-ai-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7569 6b2d 6169 0d0a 7665 7273   = quik-ai..vers
-00000020: 696f 6e20 3d20 312e 302e 300d 0a61 7574  ion = 1.0.0..aut
+00000020: 696f 6e20 3d20 312e 302e 310d 0a61 7574  ion = 1.0.1..aut
 00000030: 686f 7220 3d20 416c 656b 7361 6e64 7220  hor = Aleksandr 
 00000040: 546f 757a 6f76 0d0a 6465 7363 7269 7074  Touzov..descript
 00000050: 696f 6e20 3d20 5175 6963 6b20 556e 6966  ion = Quick Unif
 00000060: 7969 6e67 2049 6e66 7261 7374 7275 6374  ying Infrastruct
 00000070: 7572 6520 4b69 7420 666f 7220 4d61 6368  ure Kit for Mach
 00000080: 696e 6520 4c65 6172 6e69 6e67 2061 6e64  ine Learning and
 00000090: 2041 490d 0a6c 6f6e 675f 6465 7363 7269   AI..long_descri
@@ -16,15 +16,15 @@
 000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000100: 2f74 6f75 7a6f 7631 3031 322f 7175 696b  /touzov1012/quik
 00000110: 2d61 690d 0a64 6f77 6e6c 6f61 645f 7572  -ai..download_ur
 00000120: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000130: 7562 2e63 6f6d 2f74 6f75 7a6f 7631 3031  ub.com/touzov101
 00000140: 322f 7175 696b 2d61 692f 6172 6368 6976  2/quik-ai/archiv
 00000150: 652f 7265 6673 2f74 6167 732f 7631 2e30  e/refs/tags/v1.0
-00000160: 2e30 2e74 6172 2e67 7a0d 0a63 6c61 7373  .0.tar.gz..class
+00000160: 2e31 2e74 6172 2e67 7a0d 0a63 6c61 7373  .1.tar.gz..class
 00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
 00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
 000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001b0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
 000001c0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
 000001d0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
```

### Comparing `quik-ai-1.0.0/src/quik_ai/backend.py` & `quik-ai-1.0.1/src/quik_ai/backend.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/engine.py` & `quik-ai-1.0.1/src/quik_ai/engine.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/heads.py` & `quik-ai-1.0.1/src/quik_ai/heads.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/layers.py` & `quik-ai-1.0.1/src/quik_ai/layers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/losses.py` & `quik-ai-1.0.1/src/quik_ai/losses.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/metrics.py` & `quik-ai-1.0.1/src/quik_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/models.py` & `quik-ai-1.0.1/src/quik_ai/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 try:
     import mlflow
 except ImportError:  # pragma: no cover
     mlflow = None  # pragma: no cover
 
 import os
-import pickle
+import cloudpickle
 import tensorflow as tf
 import tensorflow_probability as tfp
 import keras_tuner as kt
 import numpy as np
 import pandas as pd
 
 class HyperModel(kt.HyperModel, tuning.Tunable):
@@ -52,15 +52,15 @@
         model = None
         tf_model_path = backend.join_path(filepath, 'tf_model')
         if os.path.exists(tf_model_path):
             model = tf.keras.models.load_model(tf_model_path)
 
         # load other attributes
         with open(backend.join_path(filepath, 'model.pkl'), 'rb') as f:
-            data = pickle.load(f)
+            data = cloudpickle.load(f)
 
         attrs = data['attrs']
         class_name = data['class_name']
         attrs['instance'] = model
 
         # get the class
         actual_class = globals()[class_name]
@@ -74,23 +74,23 @@
         # make sure the directory exists
         os.makedirs(filepath, exist_ok=True)
 
         # save model in a subfolder, if it exists
         if self.instance is not None:
             self.instance.save(backend.join_path(filepath, 'tf_model'))
 
-        # save other attributes with pickle
+        # save other attributes with cloudpickle
         attrs = {name: attr for name, attr in self.__dict__.items() if name != 'instance' and not callable(attr) and not name.startswith('_')}
         data = {
             'class_name': self.__class__.__name__,
             'attrs': attrs,
         }
         
         with open(backend.join_path(filepath, 'model.pkl'), 'wb') as f:
-            pickle.dump(data, f)
+            cloudpickle.dump(data, f)
     
     def get_parameters(self, hp):
         config = super().get_parameters(hp)
         config.update({
             'time_window' : self._get_hp(None, 'time_window', hp),
             'time_dropout' : self._get_hp(None, 'time_dropout', hp),
             'seed' : self._get_hp(None, 'seed', hp),
@@ -463,15 +463,15 @@
             for output in outputs:
                 batch.append(tf.exp(output.log_prob(value)))
             results.append(tf.concat(batch, 0))
 
         # concat results along the second axis
         return tf.stack(results, axis=-1)
     
-    def evaluate(self, data=None):
+    def evaluate(self, data=None, verbose=1):
         
         if self.instance is None:
             backend.error('Cannot evaluate for a NULL instance. Make sure you train the model before invoking.')
             return None
         
         # default to the test set
         if data is None:
@@ -485,24 +485,24 @@
             run_forever=False, 
             time_window=self.time_window, 
             hp=None, 
             shuffle=False
         )
         
         # evalute the results
-        evals = self.instance.evaluate(tdf)
+        evals = self.instance.evaluate(tdf, verbose=verbose)
         
         # pair each result with the metric name
         res = {}
         for i in range(len(evals)):
             res[self.instance.metrics[i].name.strip('_')] = evals[i]
         
         return res
     
-    def report(self, filepath='./model'):
+    def report(self, filepath='./model', verbose=0):
         
         if self.instance is None:
             backend.error('Cannot report for a NULL instance. Make sure you train the model before invoking.')
             return
         
         # make sure the directory exists
         os.makedirs(filepath, exist_ok=True)
@@ -530,15 +530,15 @@
             parameters = {k: v for k, v in parameters.items() if not isinstance(v, tuning.HyperVariable)}
             parameters = pd.DataFrame(list(parameters.items()), columns=['Parameter', 'Value'])
             lines.append('#### Model parameters:\n\n')
             lines.append('%s\n\n' % parameters.to_markdown(index=False))
 
         # save full model scores
         if self.driver is not None and self.driver.testing_data is not None:
-            scores = self.evaluate(self.driver.testing_data)
+            scores = self.evaluate(self.driver.testing_data, verbose=verbose)
             scores = pd.DataFrame(list(scores.items()), columns=['Metric', 'Value'])
             lines.append('#### Test performance:\n\n')
             lines.append('%s\n\n' % scores.to_markdown(index=False))
 
         if active_run is not None:
             mlflow.log_text(''.join(lines), fname)
         else:
```

### Comparing `quik-ai-1.0.0/src/quik_ai/optimizers.py` & `quik-ai-1.0.1/src/quik_ai/optimizers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/predictors.py` & `quik-ai-1.0.1/src/quik_ai/predictors.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/tuners.py` & `quik-ai-1.0.1/src/quik_ai/tuners.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.0/src/quik_ai/tuning.py` & `quik-ai-1.0.1/src/quik_ai/tuning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 class NullScope():
     def __init__(self):
         pass
     def __enter__(self):
-        pass
+        return self
     def __exit__(self, type, value, traceback):
         pass
 
 class FixedScope():
     def __init__(self):
         pass
     def __enter__(self):
-        pass
+        return self
     def __exit__(self, type, value, traceback):
         pass
 
 class HyperVariable:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
```

### Comparing `quik-ai-1.0.0/src/quik_ai.egg-info/PKG-INFO` & `quik-ai-1.0.1/src/quik_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.1.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


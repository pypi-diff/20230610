# Comparing `tmp/libmultilabel-0.2.1.tar.gz` & `tmp/libmultilabel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/LibMultiLabel/LibMultiLabel/dist/.tmp-uzg9r_cd/libmultilabel-0.2.1.tar", last modified: Wed May  3 09:22:23 2023, max compression
+gzip compressed data, was "libmultilabel-0.3.0.tar", last modified: Fri Jun  9 23:22:52 2023, max compression
```

## Comparing `libmultilabel-0.2.1.tar` & `libmultilabel-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23621 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/bert_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/caml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/kim_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/labelwise_attention_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/xml_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/nn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/libmultilabel/nn/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/bert_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/caml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/kim_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/labelwise_attention_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/xml_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/nn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libmultilabel-0.2.1/LICENSE` & `libmultilabel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.1/PKG-INFO` & `libmultilabel-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.2.1
+Version: 0.3.0
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.6
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: linear
 License-File: LICENSE
 
 See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
```

### Comparing `libmultilabel-0.2.1/README.md` & `libmultilabel-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 - end-to-end services from raw texts to final evaluation/analysis
 - support for common neural network architectures and linear classifiers
 - easy hyper-parameter selection
 
 This is an on-going development so many improvements are still being made. Comments are very welcome.
 
 ## Environments
-- Python: 3.7+
+- Python: 3.8+
 - CUDA: 11.6 (if training neural networks by GPU)
 - Pytorch 1.13.1+
 
 If you have a different version of CUDA, follow the installation instructions for PyTorch LTS at their [website](https://pytorch.org/).
 
 ## Documentation
 See the documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
```

### Comparing `libmultilabel-0.2.1/libmultilabel/common_utils.py` & `libmultilabel-0.3.0/libmultilabel/common_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,48 +70,46 @@
         with open(log_path) as fp:
             result = json.load(fp)
     else:
         result = dict()
 
     if config:
         config_to_save = copy.deepcopy(dict(config))
-        config_to_save.pop('device', None)  # delete if device exists
-        result['config'] = config_to_save
+        config_to_save.pop("device", None)  # delete if device exists
+        result["config"] = config_to_save
     if split and metrics:
         if split in result:
             result[split].append(metrics)
         else:
             result[split] = [metrics]
 
-    with open(log_path, 'w') as fp:
+    with open(log_path, "w") as fp:
         json.dump(result, fp)
 
-    logging.info(f'Finish writing log to {log_path}.')
+    logging.info(f"Finish writing log to {log_path}.")
 
 
 def argsort_top_k(vals, k, axis=-1):
     """Get the indices of the top-k elements in a 2D array.
 
     Args:
         vals: Array to sort.
         k: Consider only the top k elements for each query
         axis: Axis along which to sort. The default is -1 (the last axis).
 
     Returns: Array of indices that sort vals along the specified axis.
     """
     unsorted_top_k_idx = np.argpartition(vals, -k, axis=axis)[:, -k:]
-    unsorted_top_k_scores = np.take_along_axis(
-        vals, unsorted_top_k_idx, axis=axis)
+    unsorted_top_k_scores = np.take_along_axis(vals, unsorted_top_k_idx, axis=axis)
     sorted_order = np.argsort(-unsorted_top_k_scores, axis=axis)
-    sorted_top_k_idx = np.take_along_axis(
-        unsorted_top_k_idx, sorted_order, axis=axis)
+    sorted_top_k_idx = np.take_along_axis(unsorted_top_k_idx, sorted_order, axis=axis)
     return sorted_top_k_idx
 
 
-def is_multiclass_dataset(dataset, label='label'):
+def is_multiclass_dataset(dataset, label="label"):
     """Determine whether the dataset is multi-class.
 
     Args:
         dataset (Union[list, scipy.sparse.csr_matrix]): The training dataset
             in `nn` or `linear` format.
         label (str, optional): Label key. Defaults to 'label'.
 
@@ -124,9 +122,10 @@
         label_sizes = dataset[label].sum(axis=1)
 
     ratio = float((label_sizes == 1).sum()) / len(label_sizes)
     if ratio > 0.999 and ratio != 1.0:
         logging.info(
             f"""Only {(1-ratio)*100:.4f}% of training instances are multi-label.
             You may double check if your application should be a multi-label or
-            a multi-class problem.""")
+            a multi-class problem."""
+        )
     return ratio == 1.0
```

### Comparing `libmultilabel-0.2.1/libmultilabel/linear/linear.py` & `libmultilabel-0.3.0/libmultilabel/linear/linear.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 import os
 
 import numpy as np
 import scipy.sparse as sparse
 from liblinear.liblinearutil import train
 from tqdm import tqdm
 
-__all__ = ['train_1vsrest',
-           'train_thresholding',
-           'train_cost_sensitive',
-           'train_cost_sensitive_micro',
-           'train_binary_and_multiclass',
-           'predict_values',
-           'get_topk_labels',
-           'get_positive_labels']
+__all__ = [
+    "train_1vsrest",
+    "train_thresholding",
+    "train_cost_sensitive",
+    "train_cost_sensitive_micro",
+    "train_binary_and_multiclass",
+    "predict_values",
+    "get_topk_labels",
+    "get_positive_labels",
+]
 
 
 class FlatModel:
-    def __init__(self, name: str,
-                 weights: np.matrix,
-                 bias: float,
-                 thresholds: float | np.ndarray,
-                 ):
+    def __init__(
+        self,
+        name: str,
+        weights: np.matrix,
+        bias: float,
+        thresholds: float | np.ndarray,
+    ):
         self.name = name
         self.weights = weights
         self.bias = bias
         self.thresholds = thresholds
 
     def predict_values(self, x: sparse.csr_matrix) -> np.ndarray:
         """Calculates the decision values associated with x.
@@ -39,33 +43,35 @@
             np.ndarray: A matrix with dimension number of instances * number of classes.
         """
         bias = self.bias
         bias_col = np.full((x.shape[0], 1 if bias > 0 else 0), bias)
         num_feature = self.weights.shape[0]
         num_feature -= 1 if bias > 0 else 0
         if x.shape[1] < num_feature:
-            x = sparse.hstack([
-                x,
-                np.zeros((x.shape[0], num_feature - x.shape[1])),
-                bias_col,
-            ], 'csr')
+            x = sparse.hstack(
+                [
+                    x,
+                    np.zeros((x.shape[0], num_feature - x.shape[1])),
+                    bias_col,
+                ],
+                "csr",
+            )
         else:
-            x = sparse.hstack([
-                x[:, :num_feature],
-                bias_col,
-            ], 'csr')
+            x = sparse.hstack(
+                [
+                    x[:, :num_feature],
+                    bias_col,
+                ],
+                "csr",
+            )
 
         return (x * self.weights).A + self.thresholds
 
 
-def train_1vsrest(y: sparse.csr_matrix,
-                  x: sparse.csr_matrix,
-                  options: str = '',
-                  verbose: bool = True
-                  ) -> FlatModel:
+def train_1vsrest(y: sparse.csr_matrix, x: sparse.csr_matrix, options: str = "", verbose: bool = True) -> FlatModel:
     """Trains a linear model for multiabel data using a one-vs-rest strategy.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str, optional): The option string passed to liblinear. Defaults to ''.
         verbose (bool, optional): Output extra progress information. Defaults to True.
@@ -75,26 +81,23 @@
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
     x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
-    weights = np.zeros((num_feature, num_class), order='F')
+    weights = np.zeros((num_feature, num_class), order="F")
 
     if verbose:
-        logging.info(f'Training one-vs-rest model on {num_class} labels')
+        logging.info(f"Training one-vs-rest model on {num_class} labels")
     for i in tqdm(range(num_class), disable=not verbose):
         yi = y[:, i].toarray().reshape(-1)
-        weights[:, i] = _do_train(2*yi - 1, x, options).ravel()
+        weights[:, i] = _do_train(2 * yi - 1, x, options).ravel()
 
-    return FlatModel(name='1vsrest',
-                     weights=np.asmatrix(weights),
-                     bias=bias,
-                     thresholds=0)
+    return FlatModel(name="1vsrest", weights=np.asmatrix(weights), bias=bias, thresholds=0)
 
 
 def _prepare_options(x: sparse.csr_matrix, options: str) -> tuple[sparse.csr_matrix, str, float]:
     """Prepare options and x for multi-label training. Called in the first line of
     any training function.
 
     Args:
@@ -102,52 +105,52 @@
         options (str): The option string passed to liblinear.
 
     Returns:
         tuple[sparse.csr_matrix, str, float]: Transformed x, transformed options and
         bias parsed from options.
     """
     if options is None:
-        options = ''
-    if any(o in options for o in ['-R', '-C', '-v']):
-        raise ValueError('-R, -C and -v are not supported')
+        options = ""
+    if any(o in options for o in ["-R", "-C", "-v"]):
+        raise ValueError("-R, -C and -v are not supported")
 
     options_split = options.split()
-    if '-s' in options_split:
-        i = options_split.index('-s')
-        solver_type = int(options_split[i+1])
+    if "-s" in options_split:
+        i = options_split.index("-s")
+        solver_type = int(options_split[i + 1])
         if solver_type < 0 or solver_type > 7:
-            raise ValueError(
-                "Invalid LIBLINEAR solver type. Only classification solvers are allowed.")
+            raise ValueError("Invalid LIBLINEAR solver type. Only classification solvers are allowed.")
     else:
         # workaround for liblinear warning about unspecified solver
-        options_split.extend(['-s', '2'])
+        options_split.extend(["-s", "2"])
 
-    bias = -1.
-    if '-B' in options_split:
-        i = options_split.index('-B')
-        bias = float(options_split[i+1])
-        options_split = options_split[:i] + options_split[i+2:]
-        x = sparse.hstack([
-            x,
-            np.full((x.shape[0], 1), bias),
-        ], 'csr')
-    if not '-q' in options_split:
-        options_split.append('-q')
-    if not '-m' in options:
-        options_split.append(f'-m {int(os.cpu_count() / 2)}')
+    bias = -1.0
+    if "-B" in options_split:
+        i = options_split.index("-B")
+        bias = float(options_split[i + 1])
+        options_split = options_split[:i] + options_split[i + 2 :]
+        x = sparse.hstack(
+            [
+                x,
+                np.full((x.shape[0], 1), bias),
+            ],
+            "csr",
+        )
+    if not "-q" in options_split:
+        options_split.append("-q")
+    if not "-m" in options:
+        options_split.append(f"-m {int(os.cpu_count() / 2)}")
 
-    options = ' '.join(options_split)
+    options = " ".join(options_split)
     return x, options, bias
 
 
-def train_thresholding(y: sparse.csr_matrix,
-                       x: sparse.csr_matrix,
-                       options: str = '',
-                       verbose: bool = True
-                       ) -> FlatModel:
+def train_thresholding(
+    y: sparse.csr_matrix, x: sparse.csr_matrix, options: str = "", verbose: bool = True
+) -> FlatModel:
     """Trains a linear model for multilabel data using a one-vs-rest strategy
     and cross-validation to pick optimal decision thresholds for Macro-F1.
     Outperforms train_1vsrest in most aspects at the cost of higher
     time complexity.
     See user guide for more details.
 
     Args:
@@ -161,35 +164,29 @@
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
     x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
-    weights = np.zeros((num_feature, num_class), order='F')
+    weights = np.zeros((num_feature, num_class), order="F")
     thresholds = np.zeros(num_class)
 
     if verbose:
-        logging.info(f'Training thresholding model on {num_class} labels')
+        logging.info(f"Training thresholding model on {num_class} labels")
     for i in tqdm(range(num_class), disable=not verbose):
         yi = y[:, i].toarray().reshape(-1)
-        w, t = _thresholding_one_label(2*yi - 1, x, options)
+        w, t = _thresholding_one_label(2 * yi - 1, x, options)
         weights[:, i] = w.ravel()
         thresholds[i] = t
 
-    return FlatModel(name='thresholding',
-                     weights=np.asmatrix(weights),
-                     bias=bias,
-                     thresholds=thresholds)
+    return FlatModel(name="thresholding", weights=np.asmatrix(weights), bias=bias, thresholds=thresholds)
 
 
-def _thresholding_one_label(y: np.ndarray,
-                            x: sparse.csr_matrix,
-                            options: str
-                            ) -> tuple[np.ndarray, float]:
+def _thresholding_one_label(y: np.ndarray, x: sparse.csr_matrix, options: str) -> tuple[np.ndarray, float]:
     """Outer cross-validation for thresholding on a single label.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
@@ -203,42 +200,37 @@
     l = y.shape[0]
 
     perm = np.random.permutation(l)
 
     f_list = np.zeros_like(fbr_list)
 
     for fold in range(nr_fold):
-        mask = np.zeros_like(perm, dtype='?')
-        mask[np.arange(int(fold*l/nr_fold), int((fold+1)*l/nr_fold))] = 1
+        mask = np.zeros_like(perm, dtype="?")
+        mask[np.arange(int(fold * l / nr_fold), int((fold + 1) * l / nr_fold))] = 1
         val_idx = perm[mask]
         train_idx = perm[mask != True]
 
-        scutfbr_w, scutfbr_b_list = _scutfbr(
-            y[train_idx], x[train_idx], fbr_list, options)
+        scutfbr_w, scutfbr_b_list = _scutfbr(y[train_idx], x[train_idx], fbr_list, options)
         wTx = (x[val_idx] * scutfbr_w).A1
 
         for i in range(fbr_list.size):
-            F = _fmeasure(y[val_idx], 2*(wTx > -scutfbr_b_list[i]) - 1)
+            F = _fmeasure(y[val_idx], 2 * (wTx > -scutfbr_b_list[i]) - 1)
             f_list[i] += F
 
     best_fbr = fbr_list[::-1][np.argmax(f_list[::-1])]  # last largest
     if np.max(f_list) == 0:
         best_fbr = np.min(fbr_list)
 
     # final model
     w, b_list = _scutfbr(y, x, np.array([best_fbr]), options)
 
     return w, b_list[0]
 
 
-def _scutfbr(y: np.ndarray,
-             x: sparse.csr_matrix,
-             fbr_list: list[float],
-             options: str
-             ) -> tuple[np.matrix, np.ndarray]:
+def _scutfbr(y: np.ndarray, x: sparse.csr_matrix, fbr_list: list[float], options: str) -> tuple[np.matrix, np.ndarray]:
     """Inner cross-validation for SCutfbr heuristic.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         fbr_list (list[float]): list of fbr values.
         options (str): The option string passed to liblinear.
@@ -252,76 +244,73 @@
     nr_fold = 3
 
     l = y.shape[0]
 
     perm = np.random.permutation(l)
 
     for fold in range(nr_fold):
-        mask = np.zeros_like(perm, dtype='?')
-        mask[np.arange(int(fold*l/nr_fold), int((fold+1)*l/nr_fold))] = 1
+        mask = np.zeros_like(perm, dtype="?")
+        mask[np.arange(int(fold * l / nr_fold), int((fold + 1) * l / nr_fold))] = 1
         val_idx = perm[mask]
         train_idx = perm[mask != True]
 
         w = _do_train(y[train_idx], x[train_idx], options)
         wTx = (x[val_idx] * w).A1
-        scut_b = 0.
-        start_F = _fmeasure(y[val_idx], 2*(wTx > -scut_b) - 1)
+        scut_b = 0.0
+        start_F = _fmeasure(y[val_idx], 2 * (wTx > -scut_b) - 1)
 
         # stableness to match the MATLAB implementation
-        sorted_wTx_index = np.argsort(wTx, kind='stable')
+        sorted_wTx_index = np.argsort(wTx, kind="stable")
         sorted_wTx = wTx[sorted_wTx_index]
 
         tp = np.sum(y[val_idx] == 1)
         fp = val_idx.size - tp
         fn = 0
         cut = -1
-        best_F = 2*tp / (2*tp + fp + fn)
+        best_F = 2 * tp / (2 * tp + fp + fn)
         y_val = y[val_idx]
 
         # following MATLAB implementation to suppress NaNs
-        prev_settings = np.seterr('ignore')
+        prev_settings = np.seterr("ignore")
         for i in range(val_idx.size):
             if y_val[sorted_wTx_index[i]] == -1:
                 fp -= 1
             else:
                 tp -= 1
                 fn += 1
 
             # There will be NaNs, but the behaviour is correct
-            F = 2*tp / (2*tp + fp + fn)
+            F = 2 * tp / (2 * tp + fp + fn)
 
             if F >= best_F:
                 best_F = F
                 cut = i
         np.seterr(**prev_settings)
 
         if best_F > start_F:
             if cut == -1:  # i.e. all 1 in scut
                 scut_b = np.nextafter(-sorted_wTx[0], np.inf)  # predict all 1
             elif cut == val_idx.size - 1:
                 scut_b = np.nextafter(-sorted_wTx[-1], np.inf)
             else:
                 scut_b = -(sorted_wTx[cut] + sorted_wTx[cut + 1]) / 2
 
-        F = _fmeasure(y_val, 2*(wTx > -scut_b) - 1)
+        F = _fmeasure(y_val, 2 * (wTx > -scut_b) - 1)
 
         for i in range(fbr_list.size):
             if F > fbr_list[i]:
                 b_list[i] += scut_b
             else:
                 b_list[i] -= np.max(wTx)
 
     b_list = b_list / nr_fold
     return _do_train(y, x, options), b_list
 
 
-def _do_train(y: np.ndarray,
-              x: sparse.csr_matrix,
-              options: str
-              ) -> np.matrix:
+def _do_train(y: np.ndarray, x: sparse.csr_matrix, options: str) -> np.matrix:
     """Wrapper around liblinear.liblinearutil.train.
     Forcibly suppresses all IO regardless of options.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
@@ -380,23 +369,21 @@
     """
     tp = np.sum(np.logical_and(y_true == 1, y_pred == 1))
     fn = np.sum(np.logical_and(y_true == 1, y_pred == -1))
     fp = np.sum(np.logical_and(y_true == -1, y_pred == 1))
 
     F = 0
     if tp != 0 or fp != 0 or fn != 0:
-        F = 2*tp / (2*tp + fp + fn)
+        F = 2 * tp / (2 * tp + fp + fn)
     return F
 
 
-def train_cost_sensitive(y: sparse.csr_matrix,
-                         x: sparse.csr_matrix,
-                         options: str = '',
-                         verbose: bool = True
-                         ) -> FlatModel:
+def train_cost_sensitive(
+    y: sparse.csr_matrix, x: sparse.csr_matrix, options: str = "", verbose: bool = True
+) -> FlatModel:
     """Trains a linear model for multilabel data using a one-vs-rest strategy
     and cross-validation to pick an optimal asymmetric misclassification cost
     for Macro-F1.
     Outperforms train_1vsrest in most aspects at the cost of higher
     time complexity.
     See user guide for more details.
 
@@ -411,34 +398,27 @@
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
     x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
-    weights = np.zeros((num_feature, num_class), order='F')
+    weights = np.zeros((num_feature, num_class), order="F")
 
     if verbose:
-        logging.info(
-            f'Training cost-sensitive model for Macro-F1 on {num_class} labels')
+        logging.info(f"Training cost-sensitive model for Macro-F1 on {num_class} labels")
     for i in tqdm(range(num_class), disable=not verbose):
         yi = y[:, i].toarray().reshape(-1)
-        w = _cost_sensitive_one_label(2*yi - 1, x, options)
+        w = _cost_sensitive_one_label(2 * yi - 1, x, options)
         weights[:, i] = w.ravel()
 
-    return FlatModel(name='cost_sensitive',
-                     weights=np.asmatrix(weights),
-                     bias=bias,
-                     thresholds=0)
+    return FlatModel(name="cost_sensitive", weights=np.asmatrix(weights), bias=bias, thresholds=0)
 
 
-def _cost_sensitive_one_label(y: np.ndarray,
-                              x: sparse.csr_matrix,
-                              options: str
-                              ) -> np.ndarray:
+def _cost_sensitive_one_label(y: np.ndarray, x: sparse.csr_matrix, options: str) -> np.ndarray:
     """Loop over parameter space for cost-sensitive on a single label.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
@@ -449,60 +429,54 @@
     l = y.shape[0]
     perm = np.random.permutation(l)
 
     param_space = [1, 1.33, 1.8, 2.5, 3.67, 6, 13]
 
     bestScore = -np.Inf
     for a in param_space:
-        cv_options = f'{options} -w1 {a}'
+        cv_options = f"{options} -w1 {a}"
         pred = _cross_validate(y, x, cv_options, perm)
         score = _fmeasure(y, pred)
         if bestScore < score:
             bestScore = score
             bestA = a
 
-    final_options = f'{options} -w1 {bestA}'
+    final_options = f"{options} -w1 {bestA}"
     return _do_train(y, x, final_options)
 
 
-def _cross_validate(y: np.ndarray,
-                    x: sparse.csr_matrix,
-                    options: str,
-                    perm: np.ndarray
-                    ) -> np.ndarray:
+def _cross_validate(y: np.ndarray, x: sparse.csr_matrix, options: str, perm: np.ndarray) -> np.ndarray:
     """Cross-validation for cost-sensitive.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
     Returns:
         np.ndarray: Cross-validation result as a +1/-1 array.
     """
     l = y.shape[0]
     nr_fold = 3
     pred = np.zeros_like(y)
     for fold in range(nr_fold):
-        mask = np.zeros_like(perm, dtype='?')
-        mask[np.arange(int(fold*l/nr_fold), int((fold+1)*l/nr_fold))] = 1
+        mask = np.zeros_like(perm, dtype="?")
+        mask[np.arange(int(fold * l / nr_fold), int((fold + 1) * l / nr_fold))] = 1
         val_idx = perm[mask]
         train_idx = perm[mask != True]
 
         w = _do_train(y[train_idx], x[train_idx], options)
         pred[val_idx] = (x[val_idx] * w).A1 > 0
 
-    return 2*pred - 1
+    return 2 * pred - 1
 
 
-def train_cost_sensitive_micro(y: sparse.csr_matrix,
-                               x: sparse.csr_matrix,
-                               options: str = '',
-                               verbose: bool = True
-                               ) -> FlatModel:
+def train_cost_sensitive_micro(
+    y: sparse.csr_matrix, x: sparse.csr_matrix, options: str = "", verbose: bool = True
+) -> FlatModel:
     """Trains a linear model for multilabel data using a one-vs-rest strategy
     and cross-validation to pick an optimal asymmetric misclassification cost
     for Micro-F1.
     Outperforms train_1vsrest in most aspects at the cost of higher
     time complexity.
     See user guide for more details.
 
@@ -517,100 +491,93 @@
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
     x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
-    weights = np.zeros((num_feature, num_class), order='F')
+    weights = np.zeros((num_feature, num_class), order="F")
 
     l = y.shape[0]
     perm = np.random.permutation(l)
     param_space = [1, 1.33, 1.8, 2.5, 3.67, 6, 13]
     bestScore = -np.Inf
 
     if verbose:
-        logging.info(
-            f'Training cost-sensitive model for Micro-F1 on {num_class} labels')
+        logging.info(f"Training cost-sensitive model for Micro-F1 on {num_class} labels")
     for a in param_space:
         tp = fn = fp = 0
         for i in tqdm(range(num_class), disable=not verbose):
             yi = y[:, i].toarray().reshape(-1)
-            yi = 2*yi - 1
+            yi = 2 * yi - 1
 
-            cv_options = f'{options} -w1 {a}'
+            cv_options = f"{options} -w1 {a}"
             pred = _cross_validate(yi, x, cv_options, perm)
             tp = tp + np.sum(np.logical_and(yi == 1, pred == 1))
             fn = fn + np.sum(np.logical_and(yi == 1, pred == -1))
             fp = fp + np.sum(np.logical_and(yi == -1, pred == 1))
 
-        score = 2*tp / (2*tp + fn + fp)
+        score = 2 * tp / (2 * tp + fn + fp)
         if bestScore < score:
             bestScore = score
             bestA = a
 
-    final_options = f'{options} -w1 {bestA}'
+    final_options = f"{options} -w1 {bestA}"
     for i in range(num_class):
         yi = y[:, i].toarray().reshape(-1)
-        w = _do_train(2*yi - 1, x, final_options)
+        w = _do_train(2 * yi - 1, x, final_options)
         weights[:, i] = w.ravel()
 
-    return FlatModel(name='cost_sensitive_micro',
-                     weights=np.asmatrix(weights),
-                     bias=bias,
-                     thresholds=0)
+    return FlatModel(name="cost_sensitive_micro", weights=np.asmatrix(weights), bias=bias, thresholds=0)
 
 
-def train_binary_and_multiclass(y: sparse.csr_matrix,
-                                x: sparse.csr_matrix,
-                                options: str = '',
-                                verbose: bool = True
-                                ) -> FlatModel:
+def train_binary_and_multiclass(
+    y: sparse.csr_matrix, x: sparse.csr_matrix, options: str = "", verbose: bool = True
+) -> FlatModel:
     """Trains a linear model for binary and multi-class data.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str, optional): The option string passed to liblinear. Defaults to ''.
         verbose (bool, optional): Output extra progress information. Defaults to True.
 
     Returns:
         A model which can be used in predict_values.
     """
     x, options, bias = _prepare_options(x, options)
     num_instances, num_labels = y.shape
     nonzero_instance_ids, nonzero_label_ids = y.nonzero()
-    assert len(set(nonzero_instance_ids)) == num_instances, """
+    assert (
+        len(set(nonzero_instance_ids)) == num_instances
+    ), """
         Invalid dataset. Only multi-class dataset is allowed."""
     y = np.squeeze(nonzero_label_ids)
 
     with silent_stderr():
         model = train(y, x, options)
 
     # Labels appeared in training set; length may be smaller than num_labels
-    train_labels = np.array(model.get_labels(), dtype='int')
+    train_labels = np.array(model.get_labels(), dtype="int")
     weights = np.zeros((x.shape[1], num_labels))
-    if num_labels == 2 and '-s 4' not in options:
+    if num_labels == 2 and "-s 4" not in options:
         # For binary classification, liblinear returns weights
         # with shape (number of features * 1) except '-s 4'.
         w = np.ctypeslib.as_array(model.w, (x.shape[1], 1))
         weights[:, train_labels[0]] = w[:, 0]
         weights[:, train_labels[1]] = -w[:, 0]
     else:
         # Map label to the original index
         w = np.ctypeslib.as_array(model.w, (x.shape[1], len(train_labels)))
         weights[:, train_labels] = w
 
     # For labels not appeared in training, assign thresholds to -inf so they won't be predicted.
     thresholds = np.full(num_labels, -np.inf)
     thresholds[train_labels] = 0
-    return FlatModel(name='binary_and_multiclass',
-                     weights=np.asmatrix(weights),
-                     bias=bias,
-                     thresholds=thresholds)
+    return FlatModel(name="binary_and_multiclass", weights=np.asmatrix(weights), bias=bias, thresholds=thresholds)
 
 
 def predict_values(model, x: sparse.csr_matrix) -> np.ndarray:
     """Calculates the decision values associated with x.
 
     Args:
         model: A model returned from a training function.
@@ -618,30 +585,27 @@
 
     Returns:
         np.ndarray: A matrix with dimension number of instances * number of classes.
     """
     return model.predict_values(x)
 
 
-def get_topk_labels(preds: np.ndarray,
-                    label_mapping: np.ndarray,
-                    top_k: int = 5
-                    ) -> tuple[np.ndarray, np.ndarray]:
+def get_topk_labels(preds: np.ndarray, label_mapping: np.ndarray, top_k: int = 5) -> tuple[np.ndarray, np.ndarray]:
     """Get labels and scores of top k predictions from decision values.
 
     Args:
         preds (np.ndarray): A matrix of decision values with dimension (number of instances * number of classes).
         label_mapping (np.ndarray): A ndarray of class labels that maps each index (from 0 to ``num_class-1``) to its label.
         top_k (int): Determine how many classes per instance should be predicted.
 
     Returns:
         Two 2d ndarray with first one containing predicted labels and the other containing corresponding scores.
-        Both have dimension (num_instances * top_k). 
+        Both have dimension (num_instances * top_k).
     """
-    idx = np.argpartition(preds, -top_k)[:, :-top_k-1:-1]
+    idx = np.argpartition(preds, -top_k)[:, : -top_k - 1 : -1]
     row_idx = np.arange(preds.shape[0])[:, None]
     sorted_idx = idx[row_idx, np.argsort(-preds[row_idx, idx])]
     scores = preds[row_idx, sorted_idx]
     return label_mapping[sorted_idx], scores
 
 
 def get_positive_labels(preds: np.ndarray, label_mapping: np.ndarray) -> tuple[list[list[str]], list[list[float]]]:
```

### Comparing `libmultilabel-0.2.1/libmultilabel/linear/metrics.py` & `libmultilabel-0.3.0/libmultilabel/linear/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from __future__ import annotations
 
 import re
 
 import numpy as np
 
-__all__ = ['get_metrics',
-           'compute_metrics',
-           'tabulate_metrics',
-           'MetricCollection']
+__all__ = ["get_metrics", "compute_metrics", "tabulate_metrics", "MetricCollection"]
 
 
 def _DCG(preds: np.ndarray, target: np.ndarray, k: int = 5) -> np.ndarray:
-    """Compute the discounted cumulative gains (DCG).
-    """
+    """Compute the discounted cumulative gains (DCG)."""
     # Self-implemented dcg is used here. scikit-learn's implementation has
     # an average time complexity O(NlogN) as it directly applies quicksort
     # to preds regardless of k. Here the average time complexity is reduced to
     # O(N + klogk) by first partitioning off the k largest elements and then
     # applying quicksort to the subarray.
     row_idx = np.arange(preds.shape[0])[:, np.newaxis]
     preds_unsorted_idx = np.argpartition(preds, -k)[:, -k:]
@@ -80,21 +76,17 @@
 
         self.top_k = top_k
         self.score = 0
         self.num_sample = 0
 
     def update(self, preds: np.ndarray, target: np.ndarray):
         assert preds.shape == target.shape  # (batch_size, num_classes)
-        top_k_idx = np.argpartition(preds, -self.top_k)[:, -self.top_k:]
-        num_relevant = np.take_along_axis(
-            target, top_k_idx, axis=-1).sum(axis=-1)  # (batch_size, top_k)
-        self.score += np.nan_to_num(
-            num_relevant / np.minimum(self.top_k, target.sum(axis=-1)),
-            nan=0.0
-        ).sum()
+        top_k_idx = np.argpartition(preds, -self.top_k)[:, -self.top_k :]
+        num_relevant = np.take_along_axis(target, top_k_idx, axis=-1).sum(axis=-1)  # (batch_size, top_k)
+        self.score += np.nan_to_num(num_relevant / np.minimum(self.top_k, target.sum(axis=-1)), nan=0.0).sum()
         self.num_sample += preds.shape[0]
 
     def compute(self) -> float:
         return self.score / self.num_sample
 
     def reset(self):
         self.score = 0
@@ -106,26 +98,26 @@
         """Compute the Precision@K.
 
         Args:
             num_classes: The number of classes.
             average: Define the reduction that is applied over labels. Currently only "samples" is supported.
             top_k: Consider only the top k elements for each query.
         """
-        if average != 'samples':
-            raise ValueError('unsupported average')
+        if average != "samples":
+            raise ValueError("unsupported average")
 
         _check_top_k(top_k)
 
         self.top_k = top_k
         self.score = 0
         self.num_sample = 0
 
     def update(self, preds: np.ndarray, target: np.ndarray):
         assert preds.shape == target.shape  # (batch_size, num_classes)
-        top_k_idx = np.argpartition(preds, -self.top_k)[:, -self.top_k:]
+        top_k_idx = np.argpartition(preds, -self.top_k)[:, -self.top_k :]
         num_relevant = np.take_along_axis(target, top_k_idx, -1).sum()
         self.score += num_relevant / self.top_k
         self.num_sample += preds.shape[0]
 
     def compute(self) -> float:
         return self.score / self.num_sample
 
@@ -141,16 +133,16 @@
         Args:
             num_classes: The number of labels.
             average: Define the reduction that is applied over labels. Should be one of "macro", "micro",
             "another-macro".
             multiclass: Whether the task is a multiclass task.
         """
         self.num_classes = num_classes
-        if average not in {'macro', 'micro', 'another-macro'}:
-            raise ValueError('unsupported average')
+        if average not in {"macro", "micro", "another-macro"}:
+            raise ValueError("unsupported average")
         self.average = average
         self.multiclass = multiclass
         self.tp = self.fp = self.fn = 0
 
     def update(self, preds: np.ndarray, target: np.ndarray):
         assert preds.shape == target.shape  # (batch_size, num_classes)
         if self.multiclass:
@@ -160,29 +152,24 @@
         else:
             preds = preds > 0
         self.tp += np.logical_and(target == 1, preds == 1).sum(axis=0)
         self.fn += np.logical_and(target == 1, preds == 0).sum(axis=0)
         self.fp += np.logical_and(target == 0, preds == 1).sum(axis=0)
 
     def compute(self) -> float:
-        prev_settings = np.seterr('ignore')
+        prev_settings = np.seterr("ignore")
 
-        if self.average == 'macro':
-            score = np.nansum(
-                2*self.tp / (2*self.tp + self.fp + self.fn)) / self.num_classes
-        elif self.average == 'micro':
-            score = np.nan_to_num(2*np.sum(self.tp) /
-                                  np.sum(2*self.tp + self.fp + self.fn))
-        elif self.average == 'another-macro':
-            macro_prec = np.nansum(
-                self.tp / (self.tp + self.fp)) / self.num_classes
-            macro_recall = np.nansum(
-                self.tp / (self.tp + self.fn)) / self.num_classes
-            score = np.nan_to_num(
-                2 * macro_prec * macro_recall / (macro_prec + macro_recall))
+        if self.average == "macro":
+            score = np.nansum(2 * self.tp / (2 * self.tp + self.fp + self.fn)) / self.num_classes
+        elif self.average == "micro":
+            score = np.nan_to_num(2 * np.sum(self.tp) / np.sum(2 * self.tp + self.fp + self.fn))
+        elif self.average == "another-macro":
+            macro_prec = np.nansum(self.tp / (self.tp + self.fp)) / self.num_classes
+            macro_recall = np.nansum(self.tp / (self.tp + self.fn)) / self.num_classes
+            score = np.nan_to_num(2 * macro_prec * macro_recall / (macro_prec + macro_recall))
 
         np.seterr(**prev_settings)
         return score
 
     def reset(self):
         self.tp = self.fp = self.fn = 0
 
@@ -216,24 +203,20 @@
         """
         ret = {}
         for name, metric in self.metrics.items():
             ret[name] = metric.compute()
         return ret
 
     def reset(self):
-        """Clears the accumulated batches of decision values and labels.
-        """
+        """Clears the accumulated batches of decision values and labels."""
         for metric in self.metrics.values():
             metric.reset()
 
 
-def get_metrics(monitor_metrics: list[str],
-                num_classes: int,
-                multiclass: bool = False
-                ) -> MetricCollection:
+def get_metrics(monitor_metrics: list[str], num_classes: int, multiclass: bool = False) -> MetricCollection:
     """Get a collection of metrics by their names.
     See MetricCollection for more details.
 
     Args:
         monitor_metrics (list[str]): A list of metric names.
         num_classes (int): The number of classes.
         multiclass (bool, optional): Enable multiclass mode. Defaults to False.
@@ -241,36 +224,31 @@
     Returns:
         MetricCollection: A metric collection of the list of metrics.
     """
     if monitor_metrics is None:
         monitor_metrics = []
     metrics = {}
     for metric in monitor_metrics:
-        if re.match('P@\d+', metric):
-            metrics[metric] = Precision(
-                num_classes, average='samples', top_k=int(metric[2:]))
-        elif re.match('RP@\d+', metric):
+        if re.match("P@\d+", metric):
+            metrics[metric] = Precision(num_classes, average="samples", top_k=int(metric[2:]))
+        elif re.match("RP@\d+", metric):
             metrics[metric] = RPrecision(top_k=int(metric[3:]))
-        elif re.match('NDCG@\d+', metric):
+        elif re.match("NDCG@\d+", metric):
             metrics[metric] = NDCG(top_k=int(metric[5:]))
-        elif metric in {'Another-Macro-F1', 'Macro-F1', 'Micro-F1'}:
-            metrics[metric] = F1(num_classes,
-                                 average=metric[:-3].lower(),
-                                 multiclass=multiclass)
+        elif metric in {"Another-Macro-F1", "Macro-F1", "Micro-F1"}:
+            metrics[metric] = F1(num_classes, average=metric[:-3].lower(), multiclass=multiclass)
         else:
-            raise ValueError(f'invalid metric: {metric}')
+            raise ValueError(f"invalid metric: {metric}")
 
     return MetricCollection(metrics)
 
 
-def compute_metrics(preds: np.ndarray,
-                    target: np.ndarray,
-                    monitor_metrics: list[str],
-                    multiclass: bool = False
-                    ) -> dict[str, float]:
+def compute_metrics(
+    preds: np.ndarray, target: np.ndarray, monitor_metrics: list[str], multiclass: bool = False
+) -> dict[str, float]:
     """Compute metrics with decision values and labels.
     See get_metrics and MetricCollection if decision values and labels are too
     large to hold in memory.
 
 
     Args:
         preds (np.ndarray): A matrix of decision values with dimensions number of instances * number of classes.
@@ -294,18 +272,19 @@
     Args:
         metric_dict (dict[str, float]): A dictionary of metric values.
         split (str): Name of the data split.
 
     Returns:
         str: Pretty formatted string.
     """
-    msg = f'====== {split} dataset evaluation result =======\n'
-    header = '|'.join([f'{k:^18}' for k in metric_dict.keys()])
-    values = '|'.join([f'{x:^18.4f}' if isinstance(x, (np.floating,
-                      float)) else f'{x:^18}' for x in metric_dict.values()])
+    msg = f"====== {split} dataset evaluation result =======\n"
+    header = "|".join([f"{k:^18}" for k in metric_dict.keys()])
+    values = "|".join(
+        [f"{x:^18.4f}" if isinstance(x, (np.floating, float)) else f"{x:^18}" for x in metric_dict.values()]
+    )
     msg += f"|{header}|\n|{'-----------------:|' * len(metric_dict)}\n|{values}|\n"
     return msg
 
 
 def _check_top_k(k):
     if not (isinstance(k, int) and k > 0):
         raise ValueError('"k" has to be a positive integer')
```

### Comparing `libmultilabel-0.2.1/libmultilabel/linear/tree.py` & `libmultilabel-0.3.0/libmultilabel/linear/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 import scipy.sparse as sparse
 import sklearn.cluster
 import sklearn.preprocessing
 from tqdm import tqdm
 
 from . import linear
 
-__all__ = ['train_tree']
+__all__ = ["train_tree"]
 
 
 class Node:
-    def __init__(self,
-                 label_map: np.ndarray,
-                 children: list[Node],
-                 ):
+    def __init__(
+        self,
+        label_map: np.ndarray,
+        children: list[Node],
+    ):
         """
         Args:
             label_map (np.ndarray): The labels under this node.
             children (list[Node]): Children of this node. Must be an empty list if this is a leaf node.
         """
         self.label_map = label_map
         self.children = children
@@ -33,89 +34,89 @@
         visit(self)
         # Stops if self.children is empty, i.e. self is a leaf node
         for child in self.children:
             child.dfs(visit)
 
 
 class TreeModel:
-    def __init__(self,
-                 root: Node,
-                 flat_model: linear.FlatModel,
-                 weight_map: np.ndarray,
-                 ):
-        self.name = 'tree'
+    def __init__(
+        self,
+        root: Node,
+        flat_model: linear.FlatModel,
+        weight_map: np.ndarray,
+    ):
+        self.name = "tree"
         self.root = root
         self.flat_model = flat_model
         self.weight_map = weight_map
 
-    def predict_values(self, x: sparse.csr_matrix,
-                       beam_width: int = 10,
-                       ) -> np.ndarray:
+    def predict_values(
+        self,
+        x: sparse.csr_matrix,
+        beam_width: int = 10,
+    ) -> np.ndarray:
         """Calculates the decision values associated with x.
 
         Args:
             x (sparse.csr_matrix): A matrix with dimension number of instances * number of features.
             beam_width (int, optional): Number of candidates considered during beam search. Defaults to 10.
 
         Returns:
             np.ndarray: A matrix with dimension number of instances * number of classes.
         """
         # number of instances * number of labels + total number of metalabels
         all_preds = linear.predict_values(self.flat_model, x)
-        return np.vstack([self._beam_search(all_preds[i], beam_width)
-                          for i in range(all_preds.shape[0])])
+        return np.vstack([self._beam_search(all_preds[i], beam_width) for i in range(all_preds.shape[0])])
 
     def _beam_search(self, instance_preds: np.ndarray, beam_width: int) -> np.ndarray:
         """Predict with beam search using cached decision values for a single instance.
 
         Args:
             instance_preds (np.ndarray): A vector of cached decision values of each node, has dimension number of labels + total number of metalabels.
             beam_width (int): Number of candidates considered.
 
         Returns:
             np.ndarray: A vector with dimension number of classes.
         """
-        cur_level = [(self.root, 0.)]   # pairs of (node, score)
+        cur_level = [(self.root, 0.0)]  # pairs of (node, score)
         next_level = []
         while True:
-            num_internal = sum(
-                map(lambda pair: not pair[0].isLeaf(), cur_level))
+            num_internal = sum(map(lambda pair: not pair[0].isLeaf(), cur_level))
             if num_internal == 0:
                 break
 
             for node, score in cur_level:
                 if node.isLeaf():
                     next_level.append((node, score))
                     continue
-                slice = np.s_[self.weight_map[node.index]:
-                              self.weight_map[node.index+1]]
+                slice = np.s_[self.weight_map[node.index] : self.weight_map[node.index + 1]]
                 pred = instance_preds[slice]
-                children_score = score - np.maximum(0, 1 - pred)**2
+                children_score = score - np.maximum(0, 1 - pred) ** 2
                 next_level.extend(zip(node.children, children_score.tolist()))
 
-            cur_level = sorted(next_level, key=lambda pair: -
-                               pair[1])[:beam_width]
+            cur_level = sorted(next_level, key=lambda pair: -pair[1])[:beam_width]
             next_level = []
 
         num_labels = len(self.root.label_map)
         scores = np.full(num_labels, -np.inf)
         for node, score in cur_level:
-            slice = np.s_[self.weight_map[node.index]:
-                          self.weight_map[node.index+1]]
+            slice = np.s_[self.weight_map[node.index] : self.weight_map[node.index + 1]]
             pred = instance_preds[slice]
-            scores[node.label_map] = np.exp(score - np.maximum(0, 1 - pred)**2)
+            scores[node.label_map] = np.exp(score - np.maximum(0, 1 - pred) ** 2)
         return scores
 
 
-def train_tree(y: sparse.csr_matrix,
-               x: sparse.csr_matrix,
-               options: str = '',
-               K=100, dmax=10,
-               verbose: bool = True,
-               ) -> TreeModel:
+def train_tree(
+    y: sparse.csr_matrix,
+    x: sparse.csr_matrix,
+    options: str = "",
+    K=100,
+    dmax=10,
+    verbose: bool = True,
+) -> TreeModel:
     """Trains a linear model for multiabel data using a divide-and-conquer strategy.
     The algorithm used is based on https://github.com/xmc-aalto/bonsai.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
@@ -123,110 +124,97 @@
         dmax (int, optional): Maximum depth of the tree. Defaults to 10.
         verbose (bool, optional): Output extra progress information. Defaults to True.
 
     Returns:
         A model which can be used in predict_values.
     """
     label_representation = (y.T * x).tocsr()
-    label_representation = sklearn.preprocessing.normalize(
-        label_representation, norm='l2', axis=1)
+    label_representation = sklearn.preprocessing.normalize(label_representation, norm="l2", axis=1)
     root = _build_tree(label_representation, np.arange(y.shape[1]), 0, K, dmax)
 
     num_nodes = 0
 
     def count(node):
         nonlocal num_nodes
         num_nodes += 1
+
     root.dfs(count)
 
     pbar = tqdm(total=num_nodes, disable=not verbose)
 
     def visit(node):
         relevant_instances = y[:, node.label_map].getnnz(axis=1) > 0
-        _train_node(y[relevant_instances],
-                    x[relevant_instances], options, node)
+        _train_node(y[relevant_instances], x[relevant_instances], options, node)
         pbar.update()
 
     root.dfs(visit)
     pbar.close()
 
     flat_model, weight_map = _flatten_model(root)
     return TreeModel(root, flat_model, weight_map)
 
 
-def _build_tree(label_representation: sparse.csr_matrix,
-                label_map: np.ndarray,
-                d: int, K: int, dmax: int
-                ) -> Node:
+def _build_tree(label_representation: sparse.csr_matrix, label_map: np.ndarray, d: int, K: int, dmax: int) -> Node:
     """Builds the tree recursively by kmeans clustering.
 
     Args:
         label_representation (sparse.csr_matrix): A matrix with dimensions number of classes under this node * number of features.
         label_map (np.ndarray): Maps 0..label_representation.shape[0] to the original label indices.
         d (int): Current depth.
         K (int): Maximum degree of nodes in the tree.
         dmax (int): Maximum depth of the tree.
 
     Returns:
         Node: root of the (sub)tree built from label_representation.
     """
     if d >= dmax or label_representation.shape[0] <= K:
-        return Node(label_map=label_map,
-                    children=[])
+        return Node(label_map=label_map, children=[])
 
-    metalabels = sklearn.cluster.KMeans(
-        K,
-        random_state=np.random.randint(2**31 - 1),
-        n_init=1,
-        max_iter=300,
-        tol=0.0001,
-        algorithm='elkan',
-    ).fit(label_representation).labels_
+    metalabels = (
+        sklearn.cluster.KMeans(
+            K,
+            random_state=np.random.randint(2**31 - 1),
+            n_init=1,
+            max_iter=300,
+            tol=0.0001,
+            algorithm="elkan",
+        )
+        .fit(label_representation)
+        .labels_
+    )
 
     children = []
     for i in range(K):
         child_representation = label_representation[metalabels == i]
         child_map = label_map[metalabels == i]
-        child = _build_tree(child_representation,
-                            child_map,
-                            d + 1, K, dmax)
+        child = _build_tree(child_representation, child_map, d + 1, K, dmax)
         children.append(child)
 
-    return Node(label_map=label_map,
-                children=children)
+    return Node(label_map=label_map, children=children)
 
 
-def _train_node(y: sparse.csr_matrix,
-                x: sparse.csr_matrix,
-                options: str,
-                node: Node
-                ):
+def _train_node(y: sparse.csr_matrix, x: sparse.csr_matrix, options: str, node: Node):
     """If node is internal, computes the metalabels representing each child and trains
     on the metalabels. Otherwise, train on y.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
         node (Node): Node to be trained.
     """
     if node.isLeaf():
-        node.model = linear.train_1vsrest(
-            y[:, node.label_map], x, options, False
-        )
+        node.model = linear.train_1vsrest(y[:, node.label_map], x, options, False)
     else:
         # meta_y[i, j] is 1 if the ith instance is relevant to the jth child.
         # getnnz returns an ndarray of shape number of instances.
         # This must be reshaped into number of instances * 1 to be interpreted as a column.
-        meta_y = [y[:, child.label_map].getnnz(axis=1)[:, np.newaxis] > 0
-                  for child in node.children]
+        meta_y = [y[:, child.label_map].getnnz(axis=1)[:, np.newaxis] > 0 for child in node.children]
         meta_y = sparse.csr_matrix(np.hstack(meta_y))
-        node.model = linear.train_1vsrest(
-            meta_y, x, options, False
-        )
+        node.model = linear.train_1vsrest(meta_y, x, options, False)
 
     node.model.weights = sparse.csr_matrix(node.model.weights)
 
 
 def _flatten_model(root: Node) -> tuple[linear.FlatModel, np.ndarray]:
     """Flattens tree weight matrices into a single weight matrix. The flattened weight
     matrix is used to predict all possible values, which is cached for beam search.
@@ -249,23 +237,22 @@
     bias = root.model.bias
 
     def visit(node):
         assert bias == node.model.bias
         nonlocal index
         node.index = index
         index += 1
-        weights.append(node.model.__dict__.pop('weights'))
+        weights.append(node.model.__dict__.pop("weights"))
 
     root.dfs(visit)
 
     model = linear.FlatModel(
-        name='flattened-tree',
-        weights=sparse.hstack(weights, 'csr'),
+        name="flattened-tree",
+        weights=sparse.hstack(weights, "csr"),
         bias=bias,
         thresholds=0,
     )
 
     # w.shape[1] is the number of labels/metalabels of each node
-    weight_map = np.cumsum(
-        [0] + list(map(lambda w: w.shape[1], weights)))
+    weight_map = np.cumsum([0] + list(map(lambda w: w.shape[1], weights)))
 
     return model, weight_map
```

### Comparing `libmultilabel-0.2.1/libmultilabel/linear/utils.py` & `libmultilabel-0.3.0/libmultilabel/linear/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,91 +13,87 @@
 import sklearn.pipeline
 import sklearn.utils
 
 import libmultilabel.linear as linear
 
 from .preprocessor import Preprocessor
 
-__all__ = ['save_pipeline', 'load_pipeline',
-           'MultiLabelEstimator', 'GridSearchCV']
+__all__ = ["save_pipeline", "load_pipeline", "MultiLabelEstimator", "GridSearchCV"]
 
 
 LINEAR_TECHNIQUES = {
-    '1vsrest': linear.train_1vsrest,
-    'thresholding': linear.train_thresholding,
-    'cost_sensitive': linear.train_cost_sensitive,
-    'cost_sensitive_micro': linear.train_cost_sensitive_micro,
-    'binary_and_multiclass': linear.train_binary_and_multiclass,
-    'tree': linear.train_tree,
+    "1vsrest": linear.train_1vsrest,
+    "thresholding": linear.train_thresholding,
+    "cost_sensitive": linear.train_cost_sensitive,
+    "cost_sensitive_micro": linear.train_cost_sensitive_micro,
+    "binary_and_multiclass": linear.train_binary_and_multiclass,
+    "tree": linear.train_tree,
 }
 
 
 def save_pipeline(checkpoint_dir: str, preprocessor: Preprocessor, model):
     """Saves preprocessor and model to checkpoint_dir/linear_pipline.pickle.
 
     Args:
         checkpoint_dir (str): The directory to save to.
         preprocessor (Preprocessor): A Preprocessor.
         model: A model returned from one of the training functions.
     """
     pathlib.Path(checkpoint_dir).mkdir(parents=True, exist_ok=True)
-    checkpoint_path = os.path.join(checkpoint_dir, 'linear_pipeline.pickle')
+    checkpoint_path = os.path.join(checkpoint_dir, "linear_pipeline.pickle")
 
-    with open(checkpoint_path, 'wb') as f:
-        pickle.dump({
-            'preprocessor': preprocessor,
-            'model': model,
-        }, f)
+    with open(checkpoint_path, "wb") as f:
+        pickle.dump(
+            {
+                "preprocessor": preprocessor,
+                "model": model,
+            },
+            f,
+        )
 
 
 def load_pipeline(checkpoint_path: str) -> tuple[Preprocessor, Any]:
     """Loads preprocessor and model from checkpoint_path.
 
     Args:
         checkpoint_path (str): The path to a previously saved pipeline.
 
     Returns:
         tuple[Preprocessor, Any]: A tuple of the preprocessor and model.
     """
-    with open(checkpoint_path, 'rb') as f:
+    with open(checkpoint_path, "rb") as f:
         pipeline = pickle.load(f)
-    return (pipeline['preprocessor'], pipeline['model'])
+    return (pipeline["preprocessor"], pipeline["model"])
 
 
 class MultiLabelEstimator(sklearn.base.BaseEstimator):
     """Customized sklearn estimator for the multi-label classifier.
 
     Args:
         options (str, optional): The option string passed to liblinear. Defaults to ''.
         linear_technique (str, optional): Multi-label technique defined in `utils.LINEAR_TECHNIQUES`.
             Defaults to '1vsrest'.
         scoring_metric (str, optional): The scoring metric. Defaults to 'P@1'.
     """
 
-    def __init__(self, options: str = '',
-                 linear_technique: str = '1vsrest',
-                 scoring_metric: str = 'P@1'
-                 ):
+    def __init__(self, options: str = "", linear_technique: str = "1vsrest", scoring_metric: str = "P@1"):
         super().__init__()
         self.options = options
         self.linear_technique = linear_technique
         self.scoring_metric = scoring_metric
         self._is_fitted = False
 
     def fit(self, X: sparse.csr_matrix, y: sparse.csr_matrix):
-        X, y = sklearn.utils.validation.check_X_y(
-            X, y, accept_sparse=True, multi_output=True)
+        X, y = sklearn.utils.validation.check_X_y(X, y, accept_sparse=True, multi_output=True)
         self._is_fitted = True
-        self.model = LINEAR_TECHNIQUES[self.linear_technique](
-            y, X, self.options)
+        self.model = LINEAR_TECHNIQUES[self.linear_technique](y, X, self.options)
         return self
 
     def predict(self, X: sparse.csr_matrix) -> np.ndarray:
-        sklearn.utils.validation.check_is_fitted(
-            self, attributes=['_is_fitted'])
+        sklearn.utils.validation.check_is_fitted(self, attributes=["_is_fitted"])
         preds = linear.predict_values(self.model, X)
         return preds
 
     def score(self, X: sparse.csr_matrix, y: sparse.csr_matrix) -> float:
         metrics = linear.get_metrics(
             [self.scoring_metric],
             y.shape[1],
@@ -114,38 +110,34 @@
 
     Args:
         pipeline (sklearn.pipeline.Pipeline): A sklearn Pipeline for grid search.
         param_grid (dict): Search space for a grid search containing a dictionary of
             parameters and their corresponding list of candidate values.
         n_jobs (int, optional): Number of CPU cores run in parallel. Defaults to None.
     """
-    _required_parameters = ['pipeline', 'param_grid']
+
+    _required_parameters = ["pipeline", "param_grid"]
 
     def __init__(self, pipeline: sklearn.pipeline.Pipeline, param_grid: dict, n_jobs=None, **kwargs):
         assert isinstance(pipeline, sklearn.pipeline.Pipeline)
         if n_jobs is not None and n_jobs > 1:
             param_grid = self._set_singlecore_options(pipeline, param_grid)
-        if 'scoring' in kwargs.keys():
+        if "scoring" in kwargs.keys():
             raise ValueError(
-                'Please specify the validation metric with `MultiLabelEstimator.scoring_metric` in the Pipeline instead of using the parameter `scoring`.')
+                "Please specify the validation metric with `MultiLabelEstimator.scoring_metric` in the Pipeline instead of using the parameter `scoring`."
+            )
 
-        super().__init__(
-            estimator=pipeline,
-            n_jobs=n_jobs,
-            param_grid=param_grid,
-            **kwargs
-        )
+        super().__init__(estimator=pipeline, n_jobs=n_jobs, param_grid=param_grid, **kwargs)
 
     def _set_singlecore_options(self, pipeline: sklearn.pipeline.Pipeline, param_grid: dict):
         """Set liblinear options to `-m 1`. The grid search option `n_jobs`
         runs multiple processes in parallel. Using multithreaded liblinear
         in conjunction with grid search oversubscribes the CPU and deteriorates
         the performance significantly.
         """
         params = pipeline.get_params()
         for name, transform in params.items():
             if isinstance(transform, MultiLabelEstimator):
-                regex = r'-m \d+'
-                key = f'{name}__options'
-                param_grid[key] = [
-                    f"{re.sub(regex, '', v)} -m 1" for v in param_grid[key]]
+                regex = r"-m \d+"
+                key = f"{name}__options"
+                param_grid[key] = [f"{re.sub(regex, '', v)} -m 1" for v in param_grid[key]]
         return param_grid
```

### Comparing `libmultilabel-0.2.1/libmultilabel/logging.py` & `libmultilabel-0.3.0/libmultilabel/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-LOG_FORMAT = '%(asctime)s %(levelname)s:%(message)s'
+LOG_FORMAT = "%(asctime)s %(levelname)s:%(message)s"
 
 
 class ListHandler(logging.Handler):
     """Collect logged messages to a list of strings that can be obtained later.
     The `logging` module does not provide this function, so we implement one.
     """
 
@@ -22,16 +22,18 @@
         Returns:
             list[str]: A list of formatted logs.
         """
         logs = self.logs
         self.logs = []
         return logs
 
+
 stream_handler = None
 
+
 def add_stream_handler(level=logging.INFO):
     """Create and return a stream handler so that logging messages are
     sent to the terminal. The stream handler is attached to the root logger.
     The logging messages from the `transformer` and `pytorch_lighting`
     modules are propagated to the root logger so they can be managed by
     us (e.g., silence them in silent mode).
     If the handler had been created, this function returns the handler
@@ -41,36 +43,39 @@
         logging.StreamHandler: The created stream handler.
     """
     global stream_handler
 
     if stream_handler:
         return stream_handler
     else:
-        logging.getLogger().setLevel(logging.NOTSET) # use handlers to control levels
+        logging.getLogger().setLevel(logging.NOTSET)  # use handlers to control levels
 
         try:
             import transformers.utils.logging as transformer_logging
+
             transformer_logging.disable_default_handler()
             transformer_logging.enable_propagation()
         except ImportError:
             pass
 
-        lightning_logger = logging.getLogger('pytorch_lightning')
+        lightning_logger = logging.getLogger("pytorch_lightning")
         lightning_logger.handlers.clear()
         lightning_logger.propagate = True
 
         stream_handler = logging.StreamHandler()
         stream_handler.setLevel(level)
         stream_handler.setFormatter(logging.Formatter(LOG_FORMAT))
         logging.getLogger().addHandler(stream_handler)
 
     return stream_handler
 
+
 collect_handler = None
 
+
 def add_collect_handler(level=logging.NOTSET):
     """Create and return a ListHandler so that logging records with the attribute
     `collect=True` is collected. The ListHandler is attached to the root logger.
     If the handler had been created, this function returns the handler created
     earlier instead.
 
     To collect a log, set the key 'collect' with the value `True` in the `extra`
@@ -82,15 +87,15 @@
         ListHandler: The created ListHandler.
     """
     global collect_handler
 
     if collect_handler:
         return collect_handler
     else:
-        logging.getLogger().setLevel(logging.NOTSET) # use handlers to control levels
+        logging.getLogger().setLevel(logging.NOTSET)  # use handlers to control levels
 
         collect_handler = ListHandler(level=level)
         collect_handler.setFormatter(logging.Formatter(LOG_FORMAT))
-        collect_handler.addFilter(lambda record: record.__dict__.get('collect', False))
+        collect_handler.addFilter(lambda record: record.__dict__.get("collect", False))
         logging.getLogger().addHandler(collect_handler)
 
     return collect_handler
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/data_utils.py` & `libmultilabel-0.3.0/libmultilabel/nn/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from sklearn.preprocessing import MultiLabelBinarizer
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset
 from torchtext.vocab import build_vocab_from_iterator, pretrained_aliases, Vocab
 from tqdm import tqdm
 
 transformers.logging.set_verbosity_error()
-warnings.simplefilter(action='ignore', category=FutureWarning)
+warnings.simplefilter(action="ignore", category=FutureWarning)
 
-UNK = '<unk>'
-PAD = '<pad>'
+UNK = "<unk>"
+PAD = "<pad>"
 
 
 class TextDataset(Dataset):
     """Class for text dataset.
 
     Args:
         data (list[dict]): List of instances with index, label, and text.
@@ -30,14 +30,15 @@
         max_seq_length (int, optional): The maximum number of tokens of a sample.
         add_special_tokens (bool, optional): Whether to add the special tokens. Defaults to True.
         tokenizer (transformers.PreTrainedTokenizerBase, optional): HuggingFace's tokenizer of
             the transformer-based pretrained language model. Defaults to None.
         word_dict (torchtext.vocab.Vocab, optional): A vocab object for word tokenizer to
             map tokens to indices. Defaults to None.
     """
+
     def __init__(
         self,
         data,
         classes,
         max_seq_length,
         add_special_tokens=True,
         *,
@@ -50,62 +51,58 @@
         self.word_dict = word_dict
         self.tokenizer = tokenizer
         self.add_special_tokens = add_special_tokens
 
         self.num_classes = len(self.classes)
         self.label_binarizer = MultiLabelBinarizer().fit([classes])
 
-        if not isinstance(self.word_dict, Vocab) ^ isinstance(
-            self.tokenizer, transformers.PreTrainedTokenizerBase):
-            raise ValueError(
-                'Please specify exactly one of word_dict or tokenizer')
+        if not isinstance(self.word_dict, Vocab) ^ isinstance(self.tokenizer, transformers.PreTrainedTokenizerBase):
+            raise ValueError("Please specify exactly one of word_dict or tokenizer")
 
     def __len__(self):
         return len(self.data)
 
     def __getitem__(self, index):
         data = self.data[index]
         if self.tokenizer is not None:  # transformers tokenizer
             if self.add_special_tokens:  # tentatively hard code
-                input_ids = self.tokenizer.encode(data['text'],
-                                                  padding='max_length',
-                                                  max_length=self.max_seq_length,
-                                                  truncation=True)
-            else:
                 input_ids = self.tokenizer.encode(
-                    data['text'], add_special_tokens=False)
+                    data["text"], padding="max_length", max_length=self.max_seq_length, truncation=True
+                )
+            else:
+                input_ids = self.tokenizer.encode(data["text"], add_special_tokens=False)
         else:
-            input_ids = [self.word_dict[word] for word in data['text']]
+            input_ids = [self.word_dict[word] for word in data["text"]]
         return {
-            'text': torch.LongTensor(input_ids[:self.max_seq_length]),
-            'label': torch.IntTensor(self.label_binarizer.transform([data['label']])[0])
+            "text": torch.LongTensor(input_ids[: self.max_seq_length]),
+            "label": torch.IntTensor(self.label_binarizer.transform([data["label"]])[0]),
         }
 
 
 def tokenize(text):
     """Tokenize text.
 
     Args:
         text (str): Text to tokenize.
 
     Returns:
         list: A list of tokens.
     """
-    tokenizer = RegexpTokenizer(r'\w+')
+    tokenizer = RegexpTokenizer(r"\w+")
     return [t.lower() for t in tokenizer.tokenize(text) if not t.isnumeric()]
 
 
 def generate_batch(data_batch):
-    text_list = [data['text'] for data in data_batch]
-    label_list = [data['label'] for data in data_batch]
-    length_list = [len(data['text']) for data in data_batch]
+    text_list = [data["text"] for data in data_batch]
+    label_list = [data["label"] for data in data_batch]
+    length_list = [len(data["text"]) for data in data_batch]
     return {
-        'text': pad_sequence(text_list, batch_first=True),
-        'label': torch.stack(label_list),
-        'length': torch.IntTensor(length_list)
+        "text": pad_sequence(text_list, batch_first=True),
+        "label": torch.stack(label_list),
+        "length": torch.IntTensor(length_list),
     }
 
 
 def get_dataset_loader(
     data,
     classes,
     device,
@@ -134,28 +131,23 @@
         word_dict (torchtext.vocab.Vocab, optional): A vocab object for word tokenizer to
             map tokens to indices. Defaults to None.
 
     Returns:
         torch.utils.data.DataLoader: A pytorch DataLoader.
     """
     dataset = TextDataset(
-        data,
-        classes,
-        max_seq_length,
-        word_dict=word_dict,
-        tokenizer=tokenizer,
-        add_special_tokens=add_special_tokens
+        data, classes, max_seq_length, word_dict=word_dict, tokenizer=tokenizer, add_special_tokens=add_special_tokens
     )
     dataset_loader = torch.utils.data.DataLoader(
         dataset,
         batch_size=batch_size,
         shuffle=shuffle,
         num_workers=data_workers,
         collate_fn=generate_batch,
-        pin_memory='cuda' in device.type,
+        pin_memory="cuda" in device.type,
     )
     return dataset_loader
 
 
 def _load_raw_data(data, is_test=False, tokenize_text=True, remove_no_label_data=False):
     """Load and tokenize raw data in file or dataframe.
 
@@ -166,53 +158,52 @@
             This is effective only when is_test=False. Defaults to False.
 
     Returns:
         pandas.DataFrame: Data composed of index, label, and tokenized text.
     """
     assert isinstance(data, str) or isinstance(data, pd.DataFrame), "Data must be from a file or pandas dataframe."
     if isinstance(data, str):
-        logging.info(f'Load data from {data}.')
-        data = pd.read_csv(data, sep='\t', header=None,
-                           on_bad_lines='warn', quoting=csv.QUOTE_NONE).fillna('')
+        logging.info(f"Load data from {data}.")
+        data = pd.read_csv(data, sep="\t", header=None, on_bad_lines="warn", quoting=csv.QUOTE_NONE).fillna("")
     data = data.astype(str)
     if data.shape[1] == 2:
-        data.columns = ['label', 'text']
+        data.columns = ["label", "text"]
         data = data.reset_index()
     elif data.shape[1] == 3:
-        data.columns = ['index', 'label', 'text']
+        data.columns = ["index", "label", "text"]
     else:
-        raise ValueError(f'Expected 2 or 3 columns, got {data.shape[1]}.')
+        raise ValueError(f"Expected 2 or 3 columns, got {data.shape[1]}.")
 
-    data['label'] = data['label'].astype(str).map(lambda s: s.split())
+    data["label"] = data["label"].astype(str).map(lambda s: s.split())
     if tokenize_text:
-        data['text'] = data['text'].map(tokenize)
-    data = data.to_dict('records')
+        data["text"] = data["text"].map(tokenize)
+    data = data.to_dict("records")
     if not is_test:
-        num_no_label_data = sum(1 for d in data if len(d['label']) == 0)
+        num_no_label_data = sum(1 for d in data if len(d["label"]) == 0)
         if num_no_label_data > 0:
             if remove_no_label_data:
                 logging.info(
-                    f'Remove {num_no_label_data} instances that have no labels from data.',
-                    extra={'collect': True})
-                data = [d for d in data if len(d['label']) > 0]
+                    f"Remove {num_no_label_data} instances that have no labels from data.", extra={"collect": True}
+                )
+                data = [d for d in data if len(d["label"]) > 0]
             else:
                 logging.info(
-                    f'Keep {num_no_label_data} instances that have no labels from data.',
-                    extra={'collect': True})
+                    f"Keep {num_no_label_data} instances that have no labels from data.", extra={"collect": True}
+                )
     return data
 
 
 def load_datasets(
     training_data=None,
     test_data=None,
     val_data=None,
     val_size=0.2,
     merge_train_val=False,
     tokenize_text=True,
-    remove_no_label_data=False
+    remove_no_label_data=False,
 ):
     """Load data from the specified data paths or the given dataframe.
     If `val_data` does not exist but `val_size` > 0, the validation set will be split from the training dataset.
 
     Args:
         training_data (Union[str, pandas,.Dataframe], optional): Path to training data or a dataframe.
         test_data (Union[str, pandas,.Dataframe], optional): Path to test data or a dataframe.
@@ -227,52 +218,56 @@
 
     Returns:
         dict: A dictionary of datasets.
     """
     if isinstance(training_data, str) or isinstance(test_data, str):
         assert training_data or test_data, "At least one of `training_data` and `test_data` must be specified."
     elif isinstance(training_data, pd.DataFrame) or isinstance(test_data, pd.DataFrame):
-        assert not training_data.empty or not test_data.empty, "At least one of `training_data` and `test_data` must be specified."
+        assert (
+            not training_data.empty or not test_data.empty
+        ), "At least one of `training_data` and `test_data` must be specified."
 
     datasets = {}
     if training_data is not None:
-        datasets['train'] = _load_raw_data(
-            training_data, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data)
+        datasets["train"] = _load_raw_data(
+            training_data, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data
+        )
 
     if val_data is not None:
-        datasets['val'] = _load_raw_data(
-            val_data, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data)
+        datasets["val"] = _load_raw_data(
+            val_data, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data
+        )
     elif val_size > 0:
-        datasets['train'], datasets['val'] = train_test_split(
-            datasets['train'], test_size=val_size, random_state=42)
+        datasets["train"], datasets["val"] = train_test_split(datasets["train"], test_size=val_size, random_state=42)
 
     if test_data is not None:
-        datasets['test'] = _load_raw_data(
-            test_data, is_test=True, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data)
+        datasets["test"] = _load_raw_data(
+            test_data, is_test=True, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data
+        )
 
     if merge_train_val:
-        datasets['train'] = datasets['train'] + datasets['val']
-        for i in range(len(datasets['train'])):
-            datasets['train'][i]['index'] = i
-        del datasets['val']
+        datasets["train"] = datasets["train"] + datasets["val"]
+        for i in range(len(datasets["train"])):
+            datasets["train"][i]["index"] = i
+        del datasets["val"]
         gc.collect()
 
-    msg = ' / '.join(f'{k}: {len(v)}' for k, v in datasets.items())
-    logging.info(f'Finish loading dataset ({msg})')
+    msg = " / ".join(f"{k}: {len(v)}" for k, v in datasets.items())
+    logging.info(f"Finish loading dataset ({msg})")
     return datasets
 
 
 def load_or_build_text_dict(
     dataset,
     vocab_file=None,
     min_vocab_freq=1,
     embed_file=None,
     embed_cache_dir=None,
     silent=False,
-    normalize_embed=False
+    normalize_embed=False,
 ):
     """Build or load the vocabulary from the training dataset or the predefined `vocab_file`.
     The pretrained embedding can be either from a self-defined `embed_file` or from one of
     the vectors defined in torchtext.vocab.pretrained_aliases
     (https://github.com/pytorch/text/blob/main/torchtext/vocab/vectors.py).
 
     Args:
@@ -284,41 +279,37 @@
         silent (bool, optional): Enable silent mode. Defaults to False.
         normalize_embed (bool, optional): Whether the embeddings of each word is normalized to a unit vector. Defaults to False.
 
     Returns:
         tuple[torchtext.vocab.Vocab, torch.Tensor]: A vocab object which maps tokens to indices and the pre-trained word vectors of shape (vocab_size, embed_dim).
     """
     if vocab_file:
-        logging.info(f'Load vocab from {vocab_file}')
-        with open(vocab_file, 'r') as fp:
+        logging.info(f"Load vocab from {vocab_file}")
+        with open(vocab_file, "r") as fp:
             vocab_list = [[vocab.strip() for vocab in fp.readlines()]]
         # Keep PAD index 0 to align `padding_idx` of
         # class Embedding in libmultilabel.nn.networks.modules.
-        vocabs = build_vocab_from_iterator(vocab_list, min_freq=1,
-                                           specials=[PAD, UNK])
+        vocabs = build_vocab_from_iterator(vocab_list, min_freq=1, specials=[PAD, UNK])
     else:
-        vocab_list = [set(data['text']) for data in dataset]
-        vocabs = build_vocab_from_iterator(vocab_list, min_freq=min_vocab_freq,
-                                           specials=[PAD, UNK])
+        vocab_list = [set(data["text"]) for data in dataset]
+        vocabs = build_vocab_from_iterator(vocab_list, min_freq=min_vocab_freq, specials=[PAD, UNK])
     vocabs.set_default_index(vocabs[UNK])
-    logging.info(f'Read {len(vocabs)} vocabularies.')
+    logging.info(f"Read {len(vocabs)} vocabularies.")
 
-    embedding_weights = get_embedding_weights_from_file(
-        vocabs, embed_file, silent, embed_cache_dir)
+    embedding_weights = get_embedding_weights_from_file(vocabs, embed_file, silent, embed_cache_dir)
 
     if normalize_embed:
         # To have better precision for calculating the normalization, we convert the original
         # embedding_weights from a torch.FloatTensor to a torch.DoubleTensor.
         # After the normalization, we will convert the embedding_weights back to a torch.FloatTensor.
         embedding_weights = embedding_weights.double()
         for i, vector in enumerate(embedding_weights):
             # We use the constant 1e-6 by following https://github.com/jamesmullenbach/caml-mimic/blob/44a47455070d3d5c6ee69fb5305e32caec104960/dataproc/extract_wvs.py#L60
             # for an internal experiment of reproducing their results.
-            embedding_weights[i] = vector / \
-                float(torch.linalg.norm(vector) + 1e-6)
+            embedding_weights[i] = vector / float(torch.linalg.norm(vector) + 1e-6)
         embedding_weights = embedding_weights.float()
 
     return vocabs, embedding_weights
 
 
 def load_or_build_label(datasets, label_file=None, include_test_labels=False):
     """Obtain the label set from loading a label file or from the given data sets. The label set contains
@@ -332,31 +323,30 @@
         include_test_labels (bool, optional): Whether to include labels in the test dataset.
             Defaults to False.
 
     Returns:
         list: A list of labels sorted in alphabetical order.
     """
     if label_file is not None:
-        logging.info(f'Load labels from {label_file}.')
-        with open(label_file, 'r') as fp:
+        logging.info(f"Load labels from {label_file}.")
+        with open(label_file, "r") as fp:
             classes = sorted([s.strip() for s in fp.readlines()])
     else:
-        if 'test' not in datasets and include_test_labels:
-            raise ValueError(
-                f'Specified the inclusion of test labels but test file does not exist')
+        if "test" not in datasets and include_test_labels:
+            raise ValueError(f"Specified the inclusion of test labels but test file does not exist")
 
         classes = set()
 
         for split, data in datasets.items():
-            if split == 'test' and not include_test_labels:
+            if split == "test" and not include_test_labels:
                 continue
             for instance in data:
-                classes.update(instance['label'])
+                classes.update(instance["label"])
         classes = sorted(classes)
-    logging.info(f'Read {len(classes)} labels.')
+    logging.info(f"Read {len(classes)} labels.")
     return classes
 
 
 def get_embedding_weights_from_file(word_dict, embed_file, silent=False, cache=None):
     """If the word exists in the embedding file, load the pretrained word embedding.
     Otherwise, assign a zero vector to that word.
 
@@ -368,31 +358,31 @@
 
     Returns:
         torch.Tensor: Embedding weights (vocab_size, embed_size)
     """
     # Load pretrained word embedding
     load_embedding_from_file = embed_file not in pretrained_aliases
     if load_embedding_from_file:
-        logging.info(f'Load pretrained embedding from file: {embed_file}.')
+        logging.info(f"Load pretrained embedding from file: {embed_file}.")
         with open(embed_file) as f:
             word_vectors = f.readlines()
-        embed_size = len(word_vectors[0].split())-1
+        embed_size = len(word_vectors[0].split()) - 1
         vector_dict = {}
         for word_vector in tqdm(word_vectors, disable=silent):
-            word, vector = word_vector.rstrip().split(' ', 1)
+            word, vector = word_vector.rstrip().split(" ", 1)
             vector = torch.Tensor(list(map(float, vector.split())))
             vector_dict[word] = vector
     else:
-        logging.info(f'Load pretrained embedding from torchtext.')
+        logging.info(f"Load pretrained embedding from torchtext.")
         # Adapted from https://pytorch.org/text/0.9.0/_modules/torchtext/vocab.html#Vocab.load_vectors.
         if embed_file not in pretrained_aliases:
             raise ValueError(
                 "Got embed_file {}, but allowed pretrained "
-                "vectors are {}".format(
-                    embed_file, list(pretrained_aliases.keys())))
+                "vectors are {}".format(embed_file, list(pretrained_aliases.keys()))
+            )
         vector_dict = pretrained_aliases[embed_file](cache=cache)
         embed_size = vector_dict.dim
 
     embedding_weights = torch.zeros(len(word_dict), embed_size)
 
     if load_embedding_from_file:
         # Add UNK embedding
@@ -407,10 +397,10 @@
         # The condition can be used to process the word that does not in the embedding file.
         # Note that torchtext vector object has already dealt with this,
         # so we can directly make a query without addtional handling.
         if (load_embedding_from_file and word in vector_dict) or not load_embedding_from_file:
             embedding_weights[word_dict[word]] = vector_dict[word]
             vec_counts += 1
 
-    logging.info(f'loaded {vec_counts}/{len(word_dict)} word embeddings')
+    logging.info(f"loaded {vec_counts}/{len(word_dict)} word embeddings")
 
     return embedding_weights
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/metrics.py` & `libmultilabel-0.3.0/libmultilabel/nn/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 from torchmetrics.utilities.data import select_topk
 
 
 class Loss(Metric):
     """Loss records the batch-wise losses
     and then obtains a mean loss from the recorded losses.
     """
+
     # If the metric state of one batch is independent of the state of other batches,
     # full_state_update can be set to False,
     # which leads to more efficient computation with calling update() only once.
     # Please find the detailed explanation here:
     # https://torchmetrics.readthedocs.io/en/stable/pages/implement.html
     full_state_update = False
 
     def __init__(self):
         super().__init__()
-        self.add_state("loss", default=torch.tensor(
-            0., dtype=torch.double), dist_reduce_fx="sum")
-        self.add_state("num_sample", default=torch.tensor(0),
-                       dist_reduce_fx="sum")
+        self.add_state("loss", default=torch.tensor(0.0, dtype=torch.double), dist_reduce_fx="sum")
+        self.add_state("num_sample", default=torch.tensor(0), dist_reduce_fx="sum")
 
     def update(self, preds, target, loss):
         assert preds.shape == target.shape
         self.loss += loss * len(preds)
         self.num_sample += len(preds)
 
     def compute(self):
@@ -46,25 +45,23 @@
     https://scikit-learn.org/stable/modules/generated/sklearn.metrics.ndcg_score.html
     Please find the formal definition here:
     https://nlp.stanford.edu/IR-book/html/htmledition/evaluation-of-ranked-retrieval-results-1.html
 
     Args:
         top_k (int): the top k relevant labels to evaluate.
     """
+
     # If the metric state of one batch is independent of the state of other batches,
     # full_state_update can be set to False,
     # which leads to more efficient computation with calling update() only once.
     # Please find the detailed explanation here:
     # https://torchmetrics.readthedocs.io/en/stable/pages/implement.html
     full_state_update = False
 
-    def __init__(
-        self,
-        top_k
-    ):
+    def __init__(self, top_k):
         super().__init__()
         self.top_k = top_k
         self.add_state("ndcg", default=[], dist_reduce_fx="cat")
 
     def update(self, preds, target):
         assert preds.shape == target.shape
         # implement batch-wise calculations instead of storing results of all batches
@@ -81,42 +78,35 @@
     """R-precision calculates precision at k by adjusting k to the minimum value of the number of
     relevant labels and k. The definition is given at Appendix C equation (3) of
     https://aclanthology.org/P19-1636.pdf
 
     Args:
         top_k (int): the top k relevant labels to evaluate.
     """
+
     # If the metric state of one batch is independent of the state of other batches,
     # full_state_update can be set to False,
     # which leads to more efficient computation with calling update() only once.
     # Please find the detailed explanation here:
     # https://torchmetrics.readthedocs.io/en/stable/pages/implement.html
     full_state_update = False
 
-    def __init__(
-        self,
-        top_k
-    ):
+    def __init__(self, top_k):
         super().__init__()
         self.top_k = top_k
-        self.add_state("score", default=torch.tensor(
-            0., dtype=torch.double), dist_reduce_fx="sum")
-        self.add_state("num_sample", default=torch.tensor(0),
-                       dist_reduce_fx="sum")
+        self.add_state("score", default=torch.tensor(0.0, dtype=torch.double), dist_reduce_fx="sum")
+        self.add_state("num_sample", default=torch.tensor(0), dist_reduce_fx="sum")
 
     def update(self, preds, target):
         assert preds.shape == target.shape
         binary_topk_preds = select_topk(preds, self.top_k)
         target = target.to(dtype=torch.int)
         num_relevant = torch.sum(binary_topk_preds & target, dim=-1)
-        top_ks = torch.tensor([self.top_k]*preds.shape[0]).to(preds.device)
-        self.score += torch.nan_to_num(
-            num_relevant / torch.min(top_ks, target.sum(dim=-1)),
-            posinf=0.
-        ).sum()
+        top_ks = torch.tensor([self.top_k] * preds.shape[0]).to(preds.device)
+        self.score += torch.nan_to_num(num_relevant / torch.min(top_ks, target.sum(dim=-1)), posinf=0.0).sum()
         self.num_sample += len(preds)
 
     def compute(self):
         return self.score / self.num_sample
 
 
 class MacroF1(Metric):
@@ -127,60 +117,49 @@
         metric_threshold (float): The decision value threshold over which a label is predicted as positive.
         another_macro_f1 (bool, optional): Whether to compute the 'Another-Macro-F1' score.
             The 'Another-Macro-F1' is the f1 value of macro-precision and macro-recall.
             This variant of macro-f1 is less preferred but is used in some works.
             Please refer to Opitz et al. 2019 [https://arxiv.org/pdf/1911.03347.pdf].
             Defaults to False.
     """
+
     # If the metric state of one batch is independent of the state of other batches,
     # full_state_update can be set to False,
     # which leads to more efficient computation with calling update() only once.
     # Please find the detailed explanation here:
     # https://torchmetrics.readthedocs.io/en/stable/pages/implement.html
     full_state_update = False
 
-    def __init__(
-        self,
-        num_classes,
-        metric_threshold,
-        another_macro_f1=False,
-        top_k=None
-    ):
+    def __init__(self, num_classes, metric_threshold, another_macro_f1=False, top_k=None):
         super().__init__()
         self.metric_threshold = metric_threshold
         self.another_macro_f1 = another_macro_f1
         self.top_k = top_k
-        self.add_state("preds_sum", default=torch.zeros(
-            num_classes, dtype=torch.double))
-        self.add_state("target_sum", default=torch.zeros(
-            num_classes, dtype=torch.double))
-        self.add_state("tp_sum", default=torch.zeros(
-            num_classes, dtype=torch.double))
+        self.add_state("preds_sum", default=torch.zeros(num_classes, dtype=torch.double))
+        self.add_state("target_sum", default=torch.zeros(num_classes, dtype=torch.double))
+        self.add_state("tp_sum", default=torch.zeros(num_classes, dtype=torch.double))
 
     def update(self, preds, target):
         assert preds.shape == target.shape
         if self.top_k:
             preds = select_topk(preds, self.top_k)
         else:
             preds = torch.where(preds > self.metric_threshold, 1, 0)
 
         self.preds_sum = torch.add(self.preds_sum, preds.sum(dim=0))
         self.target_sum = torch.add(self.target_sum, target.sum(dim=0))
         self.tp_sum = torch.add(self.tp_sum, (preds & target).sum(dim=0))
 
     def compute(self):
         if self.another_macro_f1:
-            macro_prec = torch.mean(torch.nan_to_num(
-                self.tp_sum / self.preds_sum, posinf=0.))
-            macro_recall = torch.mean(torch.nan_to_num(
-                self.tp_sum / self.target_sum, posinf=0.))
+            macro_prec = torch.mean(torch.nan_to_num(self.tp_sum / self.preds_sum, posinf=0.0))
+            macro_recall = torch.mean(torch.nan_to_num(self.tp_sum / self.target_sum, posinf=0.0))
             return 2 * (macro_prec * macro_recall) / (macro_prec + macro_recall + 1e-10)
         else:
-            label_f1 = 2 * self.tp_sum / \
-                (self.preds_sum + self.target_sum + 1e-10)
+            label_f1 = 2 * self.tp_sum / (self.preds_sum + self.target_sum + 1e-10)
             return torch.mean(label_f1)
 
 
 def get_metrics(metric_threshold, monitor_metrics, num_classes, top_k=None):
     """Map monitor metrics to the corresponding classes defined in `torchmetrics.Metric`
     (https://torchmetrics.readthedocs.io/en/latest/references/modules.html).
 
@@ -204,55 +183,52 @@
 
     metrics = dict()
     for metric in monitor_metrics:
         if isinstance(metric, Metric):  # customized metric
             metrics[type(metric).__name__] = metric
             continue
 
-        match_top_k = re.match(r'\b(P|R|RP|nDCG)\b@(\d+)', metric)
-        match_metric = re.match(
-            r'\b(Micro|Macro)\b-\b(Precision|Recall|F1)\b', metric)
+        match_top_k = re.match(r"\b(P|R|RP|nDCG)\b@(\d+)", metric)
+        match_metric = re.match(r"\b(Micro|Macro)\b-\b(Precision|Recall|F1)\b", metric)
 
         if match_top_k:
             metric_abbr = match_top_k.group(1)  # P, R, PR, or nDCG
             top_k = int(match_top_k.group(2))
             if top_k >= num_classes:
                 raise ValueError(
-                    f'Invalid metric: {metric}. top_k ({top_k}) is greater than num_classes({num_classes}).')
-            if metric_abbr == 'P':
-                metrics[metric] = Precision(
-                    num_classes, average='samples', top_k=top_k)
-            elif metric_abbr == 'R':
-                metrics[metric] = Recall(
-                    num_classes, average='samples', top_k=top_k)
-            elif metric_abbr == 'RP':
+                    f"Invalid metric: {metric}. top_k ({top_k}) is greater than num_classes({num_classes})."
+                )
+            if metric_abbr == "P":
+                metrics[metric] = Precision(num_classes, average="samples", top_k=top_k)
+            elif metric_abbr == "R":
+                metrics[metric] = Recall(num_classes, average="samples", top_k=top_k)
+            elif metric_abbr == "RP":
                 metrics[metric] = RPrecision(top_k=top_k)
-            elif metric_abbr == 'nDCG':
+            elif metric_abbr == "nDCG":
                 metrics[metric] = NDCG(top_k=top_k)
                 # The implementation in torchmetrics stores the prediction/target of all batches,
                 # which can lead to CUDA out of memory.
                 # metrics[metric] = RetrievalNormalizedDCG(k=top_k)
-        elif metric == 'Another-Macro-F1':
-            metrics[metric] = MacroF1(
-                num_classes, metric_threshold, another_macro_f1=True, top_k=top_k)
-        elif metric == 'Macro-F1':
-            metrics[metric] = MacroF1(
-                num_classes, metric_threshold, top_k=top_k)
-        elif metric == 'Loss':
+        elif metric == "Another-Macro-F1":
+            metrics[metric] = MacroF1(num_classes, metric_threshold, another_macro_f1=True, top_k=top_k)
+        elif metric == "Macro-F1":
+            metrics[metric] = MacroF1(num_classes, metric_threshold, top_k=top_k)
+        elif metric == "Loss":
             metrics[metric] = Loss()
         elif match_metric:
             average_type = match_metric.group(1).lower()  # Micro
             metric_type = match_metric.group(2)  # Precision, Recall, or F1
-            metric_type = metric_type.replace(
-                'F1', 'F1Score')  # to be determined
+            metric_type = metric_type.replace("F1", "F1Score")  # to be determined
             metrics[metric] = getattr(torchmetrics.classification, metric_type)(
-                num_classes, metric_threshold, average=average_type, top_k=top_k)
+                num_classes, metric_threshold, average=average_type, top_k=top_k
+            )
         else:
             raise ValueError(
-                f'Invalid metric: {metric}. Make sure the metric is in the right format: Macro/Micro-Precision/Recall/F1 (ex. Micro-F1)')
+                f"Invalid metric: {metric}. Make sure the metric is in the right format: Macro/Micro-Precision/Recall/F1 (ex. Micro-F1)"
+            )
 
     # If compute_groups is set to True (default), incorrect results may be calculated.
     # Please refer to https://github.com/Lightning-AI/metrics/issues/746 for more details.
     return MetricCollection(metrics, compute_groups=False)
 
 
 def tabulate_metrics(metric_dict: dict[str, float], split: str) -> str:
@@ -261,13 +237,14 @@
     Args:
         metric_dict (dict[str, float]): A dictionary of metric values.
         split (str): Name of the data split.
 
     Returns:
         str: Pretty formatted string.
     """
-    msg = f'====== {split} dataset evaluation result =======\n'
-    header = '|'.join([f'{k:^18}' for k in metric_dict.keys()])
-    values = '|'.join([f'{x:^18.4f}' if isinstance(x, (np.floating,
-                      float)) else f'{x:^18}' for x in metric_dict.values()])
+    msg = f"====== {split} dataset evaluation result =======\n"
+    header = "|".join([f"{k:^18}" for k in metric_dict.keys()])
+    values = "|".join(
+        [f"{x:^18.4f}" if isinstance(x, (np.floating, float)) else f"{x:^18}" for x in metric_dict.values()]
+    )
     msg += f"|{header}|\n|{'-----------------:|' * len(metric_dict)}\n|{values}|\n"
     return msg
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/model.py` & `libmultilabel-0.3.0/libmultilabel/nn/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         save_k_predictions (int, optional): Save top k predictions on test set. Defaults to 0.
     """
 
     def __init__(
         self,
         num_classes,
         learning_rate=0.0001,
-        optimizer='adam',
+        optimizer="adam",
         momentum=0.9,
         weight_decay=0,
         metric_threshold=0.5,
         monitor_metrics=None,
         log_path=None,
         multiclass=False,
         silent=False,
@@ -54,46 +54,37 @@
         self.log_path = log_path
         self.silent = silent
         self.save_k_predictions = save_k_predictions
 
         # metrics for evaluation
         self.multiclass = multiclass
         top_k = 1 if self.multiclass else None
-        self.eval_metric = get_metrics(
-            metric_threshold, monitor_metrics, num_classes, top_k=top_k)
+        self.eval_metric = get_metrics(metric_threshold, monitor_metrics, num_classes, top_k=top_k)
 
     @abstractmethod
     def shared_step(self, batch):
         """Return loss and predicted logits"""
         return NotImplemented
 
     def configure_optimizers(self):
-        """Initialize an optimizer for the free parameters of the network.
-        """
+        """Initialize an optimizer for the free parameters of the network."""
         parameters = [p for p in self.parameters() if p.requires_grad]
         optimizer_name = self.optimizer
-        if optimizer_name == 'sgd':
-            optimizer = optim.SGD(parameters, self.learning_rate,
-                                  momentum=self.momentum,
-                                  weight_decay=self.weight_decay)
-        elif optimizer_name == 'adam':
-            optimizer = optim.Adam(parameters,
-                                   weight_decay=self.weight_decay,
-                                   lr=self.learning_rate)
-        elif optimizer_name == 'adamw':
-            optimizer = optim.AdamW(parameters,
-                                    weight_decay=self.weight_decay,
-                                    lr=self.learning_rate)
-        elif optimizer_name == 'adamax':
-            optimizer = optim.Adamax(parameters,
-                                     weight_decay=self.weight_decay,
-                                     lr=self.learning_rate)
+        if optimizer_name == "sgd":
+            optimizer = optim.SGD(
+                parameters, self.learning_rate, momentum=self.momentum, weight_decay=self.weight_decay
+            )
+        elif optimizer_name == "adam":
+            optimizer = optim.Adam(parameters, weight_decay=self.weight_decay, lr=self.learning_rate)
+        elif optimizer_name == "adamw":
+            optimizer = optim.AdamW(parameters, weight_decay=self.weight_decay, lr=self.learning_rate)
+        elif optimizer_name == "adamax":
+            optimizer = optim.Adamax(parameters, weight_decay=self.weight_decay, lr=self.learning_rate)
         else:
-            raise RuntimeError(
-                'Unsupported optimizer: {self.optimizer}')
+            raise RuntimeError("Unsupported optimizer: {self.optimizer}")
 
         torch.nn.utils.clip_grad_value_(parameters, 0.5)
 
         return optimizer
 
     def training_step(self, batch, batch_idx):
         loss, _ = self.shared_step(batch)
@@ -102,37 +93,37 @@
     def validation_step(self, batch, batch_idx):
         return self._shared_eval_step(batch, batch_idx)
 
     def validation_step_end(self, batch_parts):
         return self._shared_eval_step_end(batch_parts)
 
     def validation_epoch_end(self, step_outputs):
-        return self._shared_eval_epoch_end(step_outputs, 'val')
+        return self._shared_eval_epoch_end(step_outputs, "val")
 
     def test_step(self, batch, batch_idx):
         return self._shared_eval_step(batch, batch_idx)
 
     def test_step_end(self, batch_parts):
         return self._shared_eval_step_end(batch_parts)
 
     def test_epoch_end(self, step_outputs):
-        return self._shared_eval_epoch_end(step_outputs, 'test')
+        return self._shared_eval_epoch_end(step_outputs, "test")
 
     def _shared_eval_step(self, batch, batch_idx):
         loss, pred_logits = self.shared_step(batch)
-        return {'batch_idx': batch_idx,
-                'loss': loss,
-                'pred_scores': torch.sigmoid(pred_logits),
-                'target': batch['label']}
+        return {
+            "batch_idx": batch_idx,
+            "loss": loss,
+            "pred_scores": torch.sigmoid(pred_logits),
+            "target": batch["label"],
+        }
 
     def _shared_eval_step_end(self, batch_parts):
         return self.eval_metric.update(
-            preds=batch_parts['pred_scores'],
-            target=batch_parts['target'],
-            loss=batch_parts['loss']
+            preds=batch_parts["pred_scores"], target=batch_parts["target"], loss=batch_parts["loss"]
         )
 
     def _shared_eval_epoch_end(self, step_outputs, split):
         """Get scores such as `Micro-F1`, `Macro-F1`, and monitor metrics defined
         in the configuration file in the end of an epoch.
 
         Args:
@@ -165,16 +156,15 @@
         """
         _, pred_logits = self.shared_step(batch)
         pred_scores = pred_logits.detach().cpu().numpy()
         k = self.save_k_predictions
         top_k_idx = argsort_top_k(pred_scores, k, axis=1)
         top_k_scores = np.take_along_axis(pred_scores, top_k_idx, axis=1)
 
-        return {'top_k_pred': top_k_idx,
-                'top_k_pred_scores': top_k_scores}
+        return {"top_k_pred": top_k_idx, "top_k_pred_scores": top_k_scores}
 
     def print(self, *args, **kwargs):
         """Prints only from process 0 and not in silent mode. Use this in any
         distributed mode to log only once."""
 
         if not self.silent:
             # print() in LightningModule to print only from process 0
@@ -196,41 +186,43 @@
 
     def __init__(
         self,
         classes,
         word_dict,
         embed_vecs,
         network,
-        loss_function='binary_cross_entropy_with_logits',
+        loss_function="binary_cross_entropy_with_logits",
         log_path=None,
         **kwargs
     ):
         super().__init__(num_classes=len(classes), log_path=log_path, **kwargs)
         self.save_hyperparameters()
         self.word_dict = word_dict
         self.embed_vecs = embed_vecs
         self.classes = classes
         self.network = network
         self.configure_loss_function(loss_function)
 
     def configure_loss_function(self, loss_function):
-        assert hasattr(F, loss_function), """
+        assert hasattr(
+            F, loss_function
+        ), """
             Invalid `loss_function`. Make sure the loss function is defined here:
             https://pytorch.org/docs/stable/nn.functional.html#loss-functions"""
         self.loss_function = getattr(F, loss_function)
 
     def shared_step(self, batch):
         """Return loss and predicted logits of the network.
 
         Args:
             batch (dict): A batch of text and label.
 
         Returns:
             loss (torch.Tensor): Loss between target and predict logits.
             pred_logits (torch.Tensor): The predict logits (batch_size, num_classes).
         """
-        target_labels = batch['label']
+        target_labels = batch["label"]
         outputs = self.network(batch)
-        pred_logits = outputs['logits']
+        pred_logits = outputs["logits"]
         loss = self.loss_function(pred_logits, target_labels.float())
 
         return loss, pred_logits
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/__init__.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 from .labelwise_attention_networks import BiLSTMLWMHAN
 from .labelwise_attention_networks import CNNLWAN
 
 
 def get_init_weight_func(init_weight):
     def init_weight_func(m):
         if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.Conv2d):
-            getattr(nn.init, init_weight + '_')(m.weight)
+            getattr(nn.init, init_weight + "_")(m.weight)
+
     return init_weight_func
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/bert.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/bert.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,35 +9,26 @@
         num_classes (int): Total number of classes.
         dropout (float): The dropout rate of the word embedding. Defaults to 0.2.
         lm_weight (str): Pretrained model name or path. Defaults to 'bert-base-cased'.
         lm_window (int): Length of the subsequences to be split before feeding them to
             the language model. Defaults to 512.
     """
 
-    def __init__(
-        self,
-        num_classes,
-        dropout=0.2,
-        lm_weight='bert-base-cased',
-        lm_window=512,
-        **kwargs
-    ):
+    def __init__(self, num_classes, dropout=0.2, lm_weight="bert-base-cased", lm_window=512, **kwargs):
         super().__init__()
         self.lm_window = lm_window
 
-        self.lm = AutoModelForSequenceClassification.from_pretrained(lm_weight,
-                                                                     num_labels=num_classes,
-                                                                     hidden_dropout_prob=dropout,
-                                                                     torchscript=True)
+        self.lm = AutoModelForSequenceClassification.from_pretrained(
+            lm_weight, num_labels=num_classes, hidden_dropout_prob=dropout, torchscript=True
+        )
 
     def forward(self, input):
-        input_ids = input['text']  # (batch_size, sequence_length)
+        input_ids = input["text"]  # (batch_size, sequence_length)
         if input_ids.size(-1) > self.lm.config.max_position_embeddings:
             # Support for sequence length greater than 512 is not available yet
             raise ValueError(
                 f"Got maximum sequence length {input_ids.size(-1)}, "
                 f"please set max_seq_length to a value less than or equal to "
                 f"{self.lm.config.max_position_embeddings}"
             )
-        x = self.lm(
-            input_ids, attention_mask=input_ids != self.lm.config.pad_token_id)[0]  # (batch_size, num_classes)
-        return {'logits': x}
+        x = self.lm(input_ids, attention_mask=input_ids != self.lm.config.pad_token_id)[0]  # (batch_size, num_classes)
+        return {"logits": x}
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/bert_attention.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/bert_attention.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,41 +19,39 @@
         attention_dropout (float): The dropout rate for the attention. Defaults to 0.0.
     """
 
     def __init__(
         self,
         num_classes,
         dropout=0.2,
-        lm_weight='bert-base-cased',
+        lm_weight="bert-base-cased",
         lm_window=512,
         num_heads=8,
-        attention_type='multihead',
+        attention_type="multihead",
         attention_dropout=0.0,
         **kwargs
     ):
         super().__init__()
         self.lm_window = lm_window
         self.attention_type = attention_type
 
         self.lm = AutoModel.from_pretrained(lm_weight, torchscript=True)
         self.embed_drop = nn.Dropout(p=dropout)
 
         self.attention_type = attention_type
-        assert attention_type in [
-            'singlehead', 'multihead'], "attention_type must be 'singlehead' or 'multihead'"
-        if attention_type == 'singlehead':
-            self.attention = LabelwiseAttention(
-                self.lm.config.hidden_size, num_classes)
+        assert attention_type in ["singlehead", "multihead"], "attention_type must be 'singlehead' or 'multihead'"
+        if attention_type == "singlehead":
+            self.attention = LabelwiseAttention(self.lm.config.hidden_size, num_classes)
         else:
             self.attention = LabelwiseMultiHeadAttention(
-                self.lm.config.hidden_size, num_classes, num_heads, attention_dropout)
+                self.lm.config.hidden_size, num_classes, num_heads, attention_dropout
+            )
 
         # Final layer: create a matrix to use for the #labels binary classifiers
-        self.output = LabelwiseLinearOutput(
-            self.lm.config.hidden_size, num_classes)
+        self.output = LabelwiseLinearOutput(self.lm.config.hidden_size, num_classes)
 
     def lm_feature(self, input_ids):
         """BERT takes an input of a sequence of no more than 512 tokens.
         Therefore, long sequence are split into subsequences of size `lm_window`, which is a number no greater than 512.
         If the split subsequence is shorter than `lm_window`, pad it with the pad token.
 
         Args:
@@ -70,37 +68,35 @@
             seq_lengths = []
             for token_id in input_ids:
                 indexes = []
                 seq_length = (token_id != self.lm.config.pad_token_id).sum()
                 seq_lengths.append(seq_length)
                 for i in range(0, seq_length, self.lm_window):
                     indexes.append(len(inputs))
-                    inputs.append(token_id[i: i + self.lm_window])
+                    inputs.append(token_id[i : i + self.lm_window])
                 batch_indexes.append(indexes)
 
             padded_inputs = pad_sequence(inputs, batch_first=True)
-            last_hidden_states = self.lm(
-                padded_inputs, attention_mask=padded_inputs != self.lm.config.pad_token_id)[0]
+            last_hidden_states = self.lm(padded_inputs, attention_mask=padded_inputs != self.lm.config.pad_token_id)[0]
 
             x = []
             for seq_l, mapping in zip(seq_lengths, batch_indexes):
-                last_hidden_state = last_hidden_states[mapping].view(
-                    -1, last_hidden_states.size(-1))[:seq_l, :]
+                last_hidden_state = last_hidden_states[mapping].view(-1, last_hidden_states.size(-1))[:seq_l, :]
                 x.append(last_hidden_state)
             return pad_sequence(x, batch_first=True)
 
     def forward(self, input):
-        input_ids = input['text']  # (batch_size, sequence_length)
+        input_ids = input["text"]  # (batch_size, sequence_length)
         attention_mask = input_ids == self.lm.config.pad_token_id
         # (batch_size, sequence_length, lm_hidden_size)
         x = self.lm_feature(input_ids)
         x = self.embed_drop(x)
 
         # Apply per-label attention.
-        if self.attention_type == 'singlehead':
+        if self.attention_type == "singlehead":
             logits, attention = self.attention(x)
         else:
             logits, attention = self.attention(x, attention_mask)
 
         # Compute a probability for each label
         x = self.output(logits)
-        return {'logits': x, 'attention': attention}
+        return {"logits": x, "attention": attention}
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/caml.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/caml.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,41 +25,40 @@
         num_classes,
         filter_sizes=None,
         num_filter_per_size=50,
         dropout=0.2,
     ):
         super(CAML, self).__init__()
         if not filter_sizes and len(filter_sizes) != 1:
-            raise ValueError(
-                f'CAML expect 1 filter size. Got filter_sizes={filter_sizes}')
+            raise ValueError(f"CAML expect 1 filter size. Got filter_sizes={filter_sizes}")
         filter_size = filter_sizes[0]
 
-        self.embedding = nn.Embedding(
-            len(embed_vecs), embed_vecs.shape[1], padding_idx=0)
+        self.embedding = nn.Embedding(len(embed_vecs), embed_vecs.shape[1], padding_idx=0)
         self.embedding.weight.data = embed_vecs.clone()
         self.embed_drop = nn.Dropout(p=dropout)
 
         # Initialize conv layer
-        self.conv = nn.Conv1d(embed_vecs.shape[1], num_filter_per_size,
-                              kernel_size=filter_size, padding=int(floor(filter_size/2)))
+        self.conv = nn.Conv1d(
+            embed_vecs.shape[1], num_filter_per_size, kernel_size=filter_size, padding=int(floor(filter_size / 2))
+        )
         xavier_uniform_(self.conv.weight)
 
         """Context vectors for computing attention with
         (in_features, out_features) = (num_filter_per_size, num_classes)
         """
         self.Q = nn.Linear(num_filter_per_size, num_classes)
         xavier_uniform_(self.Q.weight)
 
         # Final layer: create a matrix to use for the #labels binary classifiers
         self.output = nn.Linear(num_filter_per_size, num_classes)
         xavier_uniform_(self.output.weight)
 
     def forward(self, input):
         # Get embeddings and apply dropout
-        x = self.embedding(input['text'])  # (batch_size, length, embed_dim)
+        x = self.embedding(input["text"])  # (batch_size, length, embed_dim)
         x = self.embed_drop(x)
         x = x.transpose(1, 2)  # (batch_size, embed_dim, length)
 
         """ Apply convolution and nonlinearity (tanh). The shapes are:
             - self.conv(x): (batch_size, num_filte_per_size, length)
             - x after transposing the first and the second dimension and applying
               the activation function: (batch_size, length, num_filte_per_size)
@@ -73,11 +72,10 @@
         """
         alpha = torch.softmax(self.Q.weight.matmul(Z.transpose(1, 2)), dim=2)
 
         # Document representations are weighted sums using the attention
         E = alpha.matmul(Z)  # (batch_size, num_classes, num_filter_per_size)
 
         # Compute a probability for each label
-        logits = self.output.weight.mul(E).sum(dim=2).add(
-            self.output.bias)  # (batch_size, num_classes)
+        logits = self.output.weight.mul(E).sum(dim=2).add(self.output.bias)  # (batch_size, num_classes)
 
-        return {'logits': logits, 'attention': alpha}
+        return {"logits": logits, "attention": alpha}
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/kim_cnn.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/kim_cnn.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,23 +21,23 @@
         self,
         embed_vecs,
         num_classes,
         filter_sizes=None,
         num_filter_per_size=128,
         embed_dropout=0.2,
         encoder_dropout=0,
-        activation='relu'
+        activation="relu",
     ):
         super(KimCNN, self).__init__()
         self.embedding = Embedding(embed_vecs, embed_dropout)
-        self.encoder = CNNEncoder(embed_vecs.shape[1], filter_sizes,
-                                  num_filter_per_size, activation,
-                                  encoder_dropout, num_pool=1)
+        self.encoder = CNNEncoder(
+            embed_vecs.shape[1], filter_sizes, num_filter_per_size, activation, encoder_dropout, num_pool=1
+        )
         conv_output_size = num_filter_per_size * len(filter_sizes)
         self.linear = nn.Linear(conv_output_size, num_classes)
 
     def forward(self, input):
-        x = self.embedding(input['text'])  # (batch_size, length, embed_dim)
+        x = self.embedding(input["text"])  # (batch_size, length, embed_dim)
         x = self.encoder(x)  # (batch_size, num_filter, 1)
         x = torch.squeeze(x, 2)  # (batch_size, num_filter)
         x = self.linear(x)  # (batch_size, num_classes)
-        return {'logits': x}
+        return {"logits": x}
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/labelwise_attention_networks.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/labelwise_attention_networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from abc import ABC, abstractmethod
 
 import torch.nn as nn
 
-from .modules import Embedding, GRUEncoder, LSTMEncoder, CNNEncoder, LabelwiseAttention, LabelwiseMultiHeadAttention, LabelwiseLinearOutput
+from .modules import (
+    Embedding,
+    GRUEncoder,
+    LSTMEncoder,
+    CNNEncoder,
+    LabelwiseAttention,
+    LabelwiseMultiHeadAttention,
+    LabelwiseLinearOutput,
+)
 
 
 class LabelwiseAttentionNetwork(ABC, nn.Module):
     """Base class for Labelwise Attention Network
 
     Args:
         embed_vecs (torch.Tensor): The pre-trained word vectors of shape (vocab_size, embed_dim).
@@ -33,25 +41,24 @@
 
     @abstractmethod
     def _get_attention(self):
         raise NotImplementedError
 
 
 class RNNLWAN(LabelwiseAttentionNetwork):
-    """Base class for RNN Labelwise Attention Network
-    """
+    """Base class for RNN Labelwise Attention Network"""
 
     def forward(self, input):
         # (batch_size, sequence_length, embed_dim)
-        x = self.embedding(input['text'])
+        x = self.embedding(input["text"])
         # (batch_size, sequence_length, hidden_dim)
-        x = self.encoder(x, input['length'])
+        x = self.encoder(x, input["length"])
         x, _ = self.attention(x)  # (batch_size, num_classes, hidden_dim)
         x = self.output(x)  # (batch_size, num_classes)
-        return {'logits': x}
+        return {"logits": x}
 
 
 class BiGRULWAN(RNNLWAN):
     """BiGRU Labelwise Attention Network
 
     Args:
         embed_vecs (torch.Tensor): The pre-trained word vectors of shape (vocab_size, embed_dim).
@@ -59,28 +66,19 @@
         rnn_dim (int): The size of bidirectional hidden layers. The hidden size of the GRU network
             is set to rnn_dim//2. Defaults to 512.
         rnn_layers (int): The number of recurrent layers. Defaults to 1.
         embed_dropout (float): The dropout rate of the word embedding. Defaults to 0.2.
         encoder_dropout (float): The dropout rate of the encoder output. Defaults to 0.
     """
 
-    def __init__(
-        self,
-        embed_vecs,
-        num_classes,
-        rnn_dim=512,
-        rnn_layers=1,
-        embed_dropout=0.2,
-        encoder_dropout=0
-    ):
+    def __init__(self, embed_vecs, num_classes, rnn_dim=512, rnn_layers=1, embed_dropout=0.2, encoder_dropout=0):
         self.num_classes = num_classes
         self.rnn_dim = rnn_dim
         self.rnn_layers = rnn_layers
-        super(BiGRULWAN, self).__init__(embed_vecs, num_classes, embed_dropout,
-                                        encoder_dropout, rnn_dim)
+        super(BiGRULWAN, self).__init__(embed_vecs, num_classes, embed_dropout, encoder_dropout, rnn_dim)
 
     def _get_encoder(self, input_size, dropout):
         assert self.rnn_dim % 2 == 0, """`rnn_dim` should be even."""
         return GRUEncoder(input_size, self.rnn_dim // 2, self.rnn_layers, dropout)
 
     def _get_attention(self):
         return LabelwiseAttention(self.rnn_dim, self.num_classes)
@@ -95,28 +93,19 @@
         rnn_dim (int): The size of bidirectional hidden layers. The hidden size of the LSTM network
             is set to rnn_dim//2. Defaults to 512.
         rnn_layers (int): The number of recurrent layers. Defaults to 1.
         embed_dropout (float): The dropout rate of the word embedding. Defaults to 0.2.
         encoder_dropout (float): The dropout rate of the encoder output. Defaults to 0.
     """
 
-    def __init__(
-        self,
-        embed_vecs,
-        num_classes,
-        rnn_dim=512,
-        rnn_layers=1,
-        embed_dropout=0.2,
-        encoder_dropout=0
-    ):
+    def __init__(self, embed_vecs, num_classes, rnn_dim=512, rnn_layers=1, embed_dropout=0.2, encoder_dropout=0):
         self.num_classes = num_classes
         self.rnn_dim = rnn_dim
         self.rnn_layers = rnn_layers
-        super(BiLSTMLWAN, self).__init__(embed_vecs, num_classes, embed_dropout,
-                                         encoder_dropout, rnn_dim)
+        super(BiLSTMLWAN, self).__init__(embed_vecs, num_classes, embed_dropout, encoder_dropout, rnn_dim)
 
     def _get_encoder(self, input_size, dropout):
         assert self.rnn_dim % 2 == 0, """`rnn_dim` should be even."""
         return LSTMEncoder(input_size, self.rnn_dim // 2, self.rnn_layers, dropout)
 
     def _get_attention(self):
         return LabelwiseAttention(self.rnn_dim, self.num_classes)
@@ -142,41 +131,39 @@
         embed_vecs,
         num_classes,
         rnn_dim=512,
         rnn_layers=1,
         embed_dropout=0.2,
         encoder_dropout=0,
         num_heads=8,
-        attention_dropout=0.0
+        attention_dropout=0.0,
     ):
         self.num_classes = num_classes
         self.rnn_dim = rnn_dim
         self.rnn_layers = rnn_layers
         self.num_heads = num_heads
         self.attention_dropout = attention_dropout
-        super(BiLSTMLWMHAN, self).__init__(embed_vecs, num_classes, embed_dropout,
-                                           encoder_dropout, rnn_dim)
+        super(BiLSTMLWMHAN, self).__init__(embed_vecs, num_classes, embed_dropout, encoder_dropout, rnn_dim)
 
     def _get_encoder(self, input_size, dropout):
         assert self.rnn_dim % 2 == 0, """`rnn_dim` should be even."""
-        return LSTMEncoder(input_size, self.rnn_dim // 2,
-                           self.rnn_layers, dropout)
+        return LSTMEncoder(input_size, self.rnn_dim // 2, self.rnn_layers, dropout)
 
     def _get_attention(self):
         return LabelwiseMultiHeadAttention(self.rnn_dim, self.num_classes, self.num_heads, self.attention_dropout)
 
     def forward(self, input):
         # (batch_size, sequence_length, embed_dim)
-        x = self.embedding(input['text'])
+        x = self.embedding(input["text"])
         # (batch_size, sequence_length, hidden_dim)
-        x = self.encoder(x, input['length'])
+        x = self.encoder(x, input["length"])
         # (batch_size, num_classes, hidden_dim)
-        x, _ = self.attention(x, attention_mask=input['text'] == 0)
+        x, _ = self.attention(x, attention_mask=input["text"] == 0)
         x = self.output(x)  # (batch_size, num_classes)
-        return {'logits': x}
+        return {"logits": x}
 
 
 class CNNLWAN(LabelwiseAttentionNetwork):
     """CNN Labelwise Attention Network
 
     Args:
         embed_vecs (torch.Tensor): The pre-trained word vectors of shape (vocab_size, embed_dim).
@@ -192,32 +179,31 @@
         self,
         embed_vecs,
         num_classes,
         filter_sizes=None,
         num_filter_per_size=50,
         embed_dropout=0.2,
         encoder_dropout=0,
-        activation='tanh'
+        activation="tanh",
     ):
         self.num_classes = num_classes
         self.filter_sizes = filter_sizes
         self.num_filter_per_size = num_filter_per_size
         self.activation = activation
         self.hidden_dim = num_filter_per_size * len(filter_sizes)
-        super(CNNLWAN, self).__init__(embed_vecs, num_classes, embed_dropout,
-                                      encoder_dropout, self.hidden_dim)
+        super(CNNLWAN, self).__init__(embed_vecs, num_classes, embed_dropout, encoder_dropout, self.hidden_dim)
 
     def _get_encoder(self, input_size, dropout):
-        return CNNEncoder(input_size, self.filter_sizes,
-                          self.num_filter_per_size, self.activation, dropout,
-                          channel_last=True)
+        return CNNEncoder(
+            input_size, self.filter_sizes, self.num_filter_per_size, self.activation, dropout, channel_last=True
+        )
 
     def _get_attention(self):
         return LabelwiseAttention(self.hidden_dim, self.num_classes)
 
     def forward(self, input):
         # (batch_size, sequence_length, embed_dim)
-        x = self.embedding(input['text'])
+        x = self.embedding(input["text"])
         x = self.encoder(x)  # (batch_size, sequence_length, hidden_dim)
         x, _ = self.attention(x)  # (batch_size, num_classes, hidden_dim)
         x = self.output(x)  # (batch_size, num_classes)
-        return {'logits': x}
+        return {"logits": x}
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/modules.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     Args:
         embed_vecs (torch.Tensor): The pre-trained word vectors of shape (vocab_size, embed_dim).
         dropout (float): The dropout rate of the word embedding. Defaults to 0.2.
     """
 
     def __init__(self, embed_vecs, dropout=0.2):
         super(Embedding, self).__init__()
-        self.embedding = nn.Embedding.from_pretrained(
-            embed_vecs, freeze=False, padding_idx=0)
+        self.embedding = nn.Embedding.from_pretrained(embed_vecs, freeze=False, padding_idx=0)
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, input):
         return self.dropout(self.embedding(input))
 
 
 class RNNEncoder(ABC, nn.Module):
@@ -38,20 +37,17 @@
         super(RNNEncoder, self).__init__()
         self.rnn = self._get_rnn(input_size, hidden_size, num_layers)
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, input, length, **kwargs):
         self.rnn.flatten_parameters()
         idx = torch.argsort(length, descending=True)
-        length_clamped = length[idx].cpu().clamp(
-            min=1)  # avoid the empty text with length 0
-        packed_input = pack_padded_sequence(
-            input[idx], length_clamped, batch_first=True)
-        outputs, _ = pad_packed_sequence(
-            self.rnn(packed_input)[0], batch_first=True)
+        length_clamped = length[idx].cpu().clamp(min=1)  # avoid the empty text with length 0
+        packed_input = pack_padded_sequence(input[idx], length_clamped, batch_first=True)
+        outputs, _ = pad_packed_sequence(self.rnn(packed_input)[0], batch_first=True)
         return self.dropout(outputs[torch.argsort(idx)])
 
     @abstractmethod
     def _get_rnn(self, input_size, hidden_size, num_layers):
         raise NotImplementedError
 
 
@@ -62,39 +58,35 @@
         input_size (int): The number of expected features in the input.
         hidden_size (int): The number of features in the hidden state.
         num_layers (int): The number of recurrent layers.
         dropout (float): The dropout rate of the encoder. Defaults to 0.
     """
 
     def __init__(self, input_size, hidden_size, num_layers, dropout=0):
-        super(GRUEncoder, self).__init__(input_size, hidden_size, num_layers,
-                                         dropout)
+        super(GRUEncoder, self).__init__(input_size, hidden_size, num_layers, dropout)
 
     def _get_rnn(self, input_size, hidden_size, num_layers):
-        return nn.GRU(input_size, hidden_size, num_layers,
-                      batch_first=True, bidirectional=True)
+        return nn.GRU(input_size, hidden_size, num_layers, batch_first=True, bidirectional=True)
 
 
 class LSTMEncoder(RNNEncoder):
     """Bi-directional LSTM encoder with dropout
 
     Args:
         input_size (int): The number of expected features in the input.
         hidden_size (int): The number of features in the hidden state.
         num_layers (int): The number of recurrent layers.
         dropout (float): The dropout rate of the encoder. Defaults to 0.
     """
 
     def __init__(self, input_size, hidden_size, num_layers, dropout=0):
-        super(LSTMEncoder, self).__init__(input_size, hidden_size, num_layers,
-                                          dropout)
+        super(LSTMEncoder, self).__init__(input_size, hidden_size, num_layers, dropout)
 
     def _get_rnn(self, input_size, hidden_size, num_layers):
-        return nn.LSTM(input_size, hidden_size, num_layers,
-                       batch_first=True, bidirectional=True)
+        return nn.LSTM(input_size, hidden_size, num_layers, batch_first=True, bidirectional=True)
 
 
 class CNNEncoder(nn.Module):
     """Multi-filter-size CNN encoder for text classification with max-pooling
 
     Args:
         input_size (int): The number of expected features in the input.
@@ -105,27 +97,24 @@
         num_pool (int): The number of pools for max-pooling.
                         If num_pool = 0, do nothing.
                         If num_pool = 1, do typical max-pooling.
                         If num_pool > 1, do adaptive max-pooling.
         channel_last (bool): Whether to transpose the dimension from (batch_size, num_channel, length) to (batch_size, length, num_channel)
     """
 
-    def __init__(self, input_size, filter_sizes, num_filter_per_size,
-                 activation, dropout=0, num_pool=0, channel_last=False):
+    def __init__(
+        self, input_size, filter_sizes, num_filter_per_size, activation, dropout=0, num_pool=0, channel_last=False
+    ):
         super(CNNEncoder, self).__init__()
         if not filter_sizes:
-            raise ValueError(f'CNNEncoder expect non-empty filter_sizes. '
-                             f'Got: {filter_sizes}')
+            raise ValueError(f"CNNEncoder expect non-empty filter_sizes. " f"Got: {filter_sizes}")
         self.channel_last = channel_last
         self.convs = nn.ModuleList()
         for filter_size in filter_sizes:
-            conv = nn.Conv1d(
-                in_channels=input_size,
-                out_channels=num_filter_per_size,
-                kernel_size=filter_size)
+            conv = nn.Conv1d(in_channels=input_size, out_channels=num_filter_per_size, kernel_size=filter_size)
             self.convs.append(conv)
         self.num_pool = num_pool
         if num_pool > 1:
             self.pool = nn.AdaptiveMaxPool1d(num_pool)
         self.activation = getattr(torch, activation, getattr(F, activation))
         self.dropout = nn.Dropout(dropout)
 
@@ -177,26 +166,23 @@
         num_classes (int): Total number of classes.
         num_heads (int): The number of parallel attention heads.
         attention_dropout (float): The dropout rate for the attention. Defaults to 0.0.
     """
 
     def __init__(self, input_size, num_classes, num_heads, attention_dropout=0.0):
         super(LabelwiseMultiHeadAttention, self).__init__()
-        self.attention = nn.MultiheadAttention(
-            embed_dim=input_size, num_heads=num_heads, dropout=attention_dropout)
+        self.attention = nn.MultiheadAttention(embed_dim=input_size, num_heads=num_heads, dropout=attention_dropout)
         self.Q = nn.Linear(input_size, num_classes)
 
     def forward(self, input, attention_mask=None):
         # (sequence_length, batch_size, hidden_dim)
         key = value = input.permute(1, 0, 2)
-        query = self.Q.weight.repeat(input.size(0), 1, 1).transpose(
-            0, 1)  # (num_classes, batch_size, hidden_dim)
+        query = self.Q.weight.repeat(input.size(0), 1, 1).transpose(0, 1)  # (num_classes, batch_size, hidden_dim)
 
-        logits, attention = self.attention(
-            query, key, value, key_padding_mask=attention_mask)
+        logits, attention = self.attention(query, key, value, key_padding_mask=attention_mask)
         # (batch_size, num_classes, hidden_dim)
         logits = logits.permute(1, 0, 2)
         return logits, attention
 
 
 class LabelwiseLinearOutput(nn.Module):
     """Applies a linear transformation to the incoming data for each label
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/networks/xml_cnn.py` & `libmultilabel-0.3.0/libmultilabel/nn/networks/xml_cnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,28 +26,26 @@
         num_classes,
         embed_dropout=0.2,
         encoder_dropout=0,
         filter_sizes=None,
         hidden_dim=512,
         num_filter_per_size=256,
         num_pool=2,
-        activation='relu'
+        activation="relu",
     ):
         super(XMLCNN, self).__init__()
         self.embedding = Embedding(embed_vecs, embed_dropout)
-        self.encoder = CNNEncoder(embed_vecs.shape[1], filter_sizes,
-                                  num_filter_per_size, activation,
-                                  num_pool=num_pool)
+        self.encoder = CNNEncoder(embed_vecs.shape[1], filter_sizes, num_filter_per_size, activation, num_pool=num_pool)
         total_output_size = len(filter_sizes) * num_filter_per_size * num_pool
         self.dropout = nn.Dropout(encoder_dropout)
         self.linear1 = nn.Linear(total_output_size, hidden_dim)
         self.linear2 = nn.Linear(hidden_dim, num_classes)
         self.activation = getattr(torch, activation, getattr(F, activation))
 
     def forward(self, input):
-        x = self.embedding(input['text'])  # (batch_size, length, embed_dim)
+        x = self.embedding(input["text"])  # (batch_size, length, embed_dim)
         x = self.encoder(x)  # (batch_size, num_filter, num_pool)
         x = x.view(x.shape[0], -1)  # (batch_size, num_filter * num_pool)
         x = self.activation(self.linear1(x))
         x = self.dropout(x)
         x = self.linear2(x)
-        return {'logits': x}
+        return {"logits": x}
```

### Comparing `libmultilabel-0.2.1/libmultilabel/nn/nn_utils.py` & `libmultilabel-0.3.0/libmultilabel/nn/nn_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,41 +20,43 @@
     Returns:
         torch.device: One of cuda or cpu.
     """
 
     if not use_cpu and torch.cuda.is_available():
         # Set a debug environment variable CUBLAS_WORKSPACE_CONFIG to ":16:8" (may limit overall performance) or ":4096:8" (will increase library footprint in GPU memory by approximately 24MiB).
         # https://docs.nvidia.com/cuda/cublas/index.html
-        os.environ['CUBLAS_WORKSPACE_CONFIG'] = ":4096:8"
-        device = torch.device('cuda')
+        os.environ["CUBLAS_WORKSPACE_CONFIG"] = ":4096:8"
+        device = torch.device("cuda")
     else:
-        device = torch.device('cpu')
+        device = torch.device("cpu")
         # https://github.com/pytorch/pytorch/issues/11201
-        torch.multiprocessing.set_sharing_strategy('file_system')
-    logging.info(f'Using device: {device}')
+        torch.multiprocessing.set_sharing_strategy("file_system")
+    logging.info(f"Using device: {device}")
     return device
 
 
-def init_model(model_name,
-               network_config,
-               classes,
-               word_dict=None,
-               embed_vecs=None,
-               init_weight=None,
-               log_path=None,
-               learning_rate=0.0001,
-               optimizer='adam',
-               momentum=0.9,
-               weight_decay=0,
-               metric_threshold=0.5,
-               monitor_metrics=None,
-               multiclass=False,
-               loss_function='binary_cross_entropy_with_logits',
-               silent=False,
-               save_k_predictions=0):
+def init_model(
+    model_name,
+    network_config,
+    classes,
+    word_dict=None,
+    embed_vecs=None,
+    init_weight=None,
+    log_path=None,
+    learning_rate=0.0001,
+    optimizer="adam",
+    momentum=0.9,
+    weight_decay=0,
+    metric_threshold=0.5,
+    monitor_metrics=None,
+    multiclass=False,
+    loss_function="binary_cross_entropy_with_logits",
+    silent=False,
+    save_k_predictions=0,
+):
     """Initialize a `Model` class for initializing and training a neural network.
 
     Args:
         model_name (str): Model to be used such as KimCNN.
         network_config (dict): Configuration for defining the network.
         classes (list): List of class names.
         word_dict (torchtext.vocab.Vocab, optional): A vocab object for word tokenizer to
@@ -78,25 +80,20 @@
         save_k_predictions (int, optional): Save top k predictions on test set. Defaults to 0.
 
     Returns:
         Model: A class that implements `MultiLabelModel` for initializing and training a neural network.
     """
 
     try:
-        network = getattr(networks, model_name)(
-            embed_vecs=embed_vecs,
-            num_classes=len(classes),
-            **dict(network_config)
-        )
+        network = getattr(networks, model_name)(embed_vecs=embed_vecs, num_classes=len(classes), **dict(network_config))
     except:
-        raise AttributeError(f'Failed to initialize {model_name}.')
+        raise AttributeError(f"Failed to initialize {model_name}.")
 
     if init_weight is not None:
-        init_weight = networks.get_init_weight_func(
-            init_weight=init_weight)
+        init_weight = networks.get_init_weight_func(init_weight=init_weight)
         network.apply(init_weight)
 
     model = Model(
         classes=classes,
         word_dict=word_dict,
         embed_vecs=embed_vecs,
         network=network,
@@ -106,31 +103,33 @@
         momentum=momentum,
         weight_decay=weight_decay,
         metric_threshold=metric_threshold,
         monitor_metrics=monitor_metrics,
         multiclass=multiclass,
         loss_function=loss_function,
         silent=silent,
-        save_k_predictions=save_k_predictions
+        save_k_predictions=save_k_predictions,
     )
     return model
 
 
-def init_trainer(checkpoint_dir,
-                 epochs=10000,
-                 patience=5,
-                 early_stopping_metric='P@1',
-                 val_metric='P@1',
-                 silent=False,
-                 use_cpu=False,
-                 limit_train_batches=1.0,
-                 limit_val_batches=1.0,
-                 limit_test_batches=1.0,
-                 search_params=False,
-                 save_checkpoints=True):
+def init_trainer(
+    checkpoint_dir,
+    epochs=10000,
+    patience=5,
+    early_stopping_metric="P@1",
+    val_metric="P@1",
+    silent=False,
+    use_cpu=False,
+    limit_train_batches=1.0,
+    limit_val_batches=1.0,
+    limit_test_batches=1.0,
+    search_params=False,
+    save_checkpoints=True,
+):
     """Initialize a torch lightning trainer.
 
     Args:
         checkpoint_dir (str): Directory for saving models and log.
         epochs (int): Number of epochs to train. Defaults to 10000.
         patience (int): Number of epochs to wait for improvement before early stopping. Defaults to 5.
         early_stopping_metric (str): The metric to monitor for early stopping. Defaults to 'P@1'.
@@ -149,47 +148,58 @@
     """
 
     # The value of `mode` equals to 'min' only when the metric is 'Loss'
     # because now for other supported metrics such as F1 or Precision, we maximize them in the training process.
     # But if in the future, we further support other metrics that need to be minimized,
     # we may need a dictionary that records a metric-mode mapping for a better practice.
     # Set strict to False to prevent EarlyStopping from crashing the training if no validation data are provided
-    early_stopping_callback = EarlyStopping(patience=patience,
-                                            monitor=early_stopping_metric,
-                                            mode='min' if early_stopping_metric == 'Loss' else 'max',
-                                            strict=False)
+    early_stopping_callback = EarlyStopping(
+        patience=patience,
+        monitor=early_stopping_metric,
+        mode="min" if early_stopping_metric == "Loss" else "max",
+        strict=False,
+    )
     callbacks = [early_stopping_callback]
     if save_checkpoints:
-        callbacks += [ModelCheckpoint(dirpath=checkpoint_dir, filename='best_model',
-                                      save_last=True, save_top_k=1,
-                                      monitor=val_metric,
-                                      mode='min' if val_metric == 'Loss' else 'max')]
+        callbacks += [
+            ModelCheckpoint(
+                dirpath=checkpoint_dir,
+                filename="best_model",
+                save_last=True,
+                save_top_k=1,
+                monitor=val_metric,
+                mode="min" if val_metric == "Loss" else "max",
+            )
+        ]
     if search_params:
         from ray.tune.integration.pytorch_lightning import TuneReportCallback
-        callbacks += [TuneReportCallback(
-            {f'val_{val_metric}': val_metric}, on="validation_end")]
 
-    trainer = pl.Trainer(logger=False, num_sanity_val_steps=0,
-                         accelerator='cpu' if use_cpu else 'gpu',
-                         devices=None if use_cpu else 1,
-                         enable_progress_bar=False if silent else True,
-                         max_epochs=epochs,
-                         callbacks=callbacks,
-                         limit_train_batches=limit_train_batches,
-                         limit_val_batches=limit_val_batches,
-                         limit_test_batches=limit_test_batches,
-                         deterministic='warn')
+        callbacks += [TuneReportCallback({f"val_{val_metric}": val_metric}, on="validation_end")]
+
+    trainer = pl.Trainer(
+        logger=False,
+        num_sanity_val_steps=0,
+        accelerator="cpu" if use_cpu else "gpu",
+        devices=None if use_cpu else 1,
+        enable_progress_bar=False if silent else True,
+        max_epochs=epochs,
+        callbacks=callbacks,
+        limit_train_batches=limit_train_batches,
+        limit_val_batches=limit_val_batches,
+        limit_test_batches=limit_test_batches,
+        deterministic="warn",
+    )
     return trainer
 
 
 def set_seed(seed):
     """Set seeds for numpy and pytorch.
 
     Args:
         seed (int): Random seed.
     """
 
     if seed is not None:
         if seed >= 0:
             seed_everything(seed=seed, workers=True)
         else:
-            logging.warning('the random seed should be a non-negative integer')
+            logging.warning("the random seed should be a non-negative integer")
```

### Comparing `libmultilabel-0.2.1/libmultilabel.egg-info/PKG-INFO` & `libmultilabel-0.3.0/libmultilabel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.2.1
+Version: 0.3.0
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.6
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: linear
 License-File: LICENSE
 
 See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
```

### Comparing `libmultilabel-0.2.1/libmultilabel.egg-info/SOURCES.txt` & `libmultilabel-0.3.0/libmultilabel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 libmultilabel/logging.py
 libmultilabel.egg-info/PKG-INFO
 libmultilabel.egg-info/SOURCES.txt
 libmultilabel.egg-info/dependency_links.txt
 libmultilabel.egg-info/requires.txt
 libmultilabel.egg-info/top_level.txt
 libmultilabel/linear/__init__.py
+libmultilabel/linear/data_utils.py
 libmultilabel/linear/linear.py
 libmultilabel/linear/metrics.py
 libmultilabel/linear/preprocessor.py
 libmultilabel/linear/tree.py
 libmultilabel/linear/utils.py
 libmultilabel/nn/__init__.py
 libmultilabel/nn/data_utils.py
```

### Comparing `libmultilabel-0.2.1/setup.cfg` & `libmultilabel-0.3.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libmultilabel
-version = 0.2.1
+version = 0.3.0
 author = LibMultiLabel Team
 license = MIT License
 license_file = LICENSE
 description = A library for multi-label text classification
 long_description = See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 url = https://github.com/ASUS-AICS/LibMultiLabel
 project_urls = 
@@ -15,15 +15,14 @@
 	Environment :: GPU :: NVIDIA CUDA :: 11.6
 	Intended Audience :: Developers
 	Intended Audience :: Education
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 
 [options]
 packages = find:
 install_requires = 
 	nltk
 	pandas>1.3.0
@@ -34,15 +33,15 @@
 	torchtext>=0.13.0
 	pytorch-lightning==1.7.7
 	tqdm
 	liblinear-multicore
 	numba
 	scipy
 	transformers
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.extras_require]
 linear = 
 	liblinear-multicore
 	numba
 	pandas
 	scikit-learn
```


# Comparing `tmp/label_noise_correction-0.0.1.tar.gz` & `tmp/label_noise_correction-0.0.2.tar.gz`

## Comparing `label_noise_correction-0.0.1.tar` & `label_noise_correction-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/__init__.py
--rwxr-xr-x   0        0        0     2856 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/be.py
--rwxr-xr-x   0        0        0     2654 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/cc.py
--rwxr-xr-x   0        0        0     5798 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/fair_obnc.py
--rwxr-xr-x   0        0        0     3923 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/hlnc.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/labelcorrection.py
--rwxr-xr-x   0        0        0     1793 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/obnc.py
--rwxr-xr-x   0        0        0     1676 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/pl.py
--rwxr-xr-x   0        0        0     4060 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/src/label_noise_correction/stc.py
--rwxr-xr-x   0        0        0     3238 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/.gitignore
--rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     3501 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/README.md
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 label_noise_correction-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/__init__.py
+-rwxr-xr-x   0        0        0     2893 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/be.py
+-rwxr-xr-x   0        0        0     2669 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/cc.py
+-rwxr-xr-x   0        0        0     5831 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/fair_obnc.py
+-rwxr-xr-x   0        0        0     3935 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/hlnc.py
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/labelcorrection.py
+-rwxr-xr-x   0        0        0     1809 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/obnc.py
+-rwxr-xr-x   0        0        0     1699 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/pl.py
+-rwxr-xr-x   0        0        0     4076 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/src/label_noise_correction/stc.py
+-rwxr-xr-x   0        0        0     3238 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     3501 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/README.md
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 label_noise_correction-0.0.2/PKG-INFO
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/be.py` & `label_noise_correction-0.0.2/src/label_noise_correction/be.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ----------
     alpha : float
         Noise rate
     n_folds : int
         Number of folds to use
     """
     def __init__(self, alpha, n_folds):
+        super().__init__('BE')
         self.alpha = alpha
         self.n_folds = n_folds
 
     def evaluate(self, X:pd.DataFrame, y:pd.Series):
         kf = StratifiedKFold(n_splits=self.n_folds, random_state=42, shuffle=True)
         entropy = pd.Series(index=y.index, dtype=float)
         y_pred = pd.Series(index=y.index, dtype=int)
@@ -75,10 +76,10 @@
             last_changed = changed
             entropy, y_pred = self.evaluate(X, y_corrected)
             it += 1
 
         
     
     def log_params(self):
-        mlflow.log_param('correction_alg', 'BE')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('n_folds', self.n_folds)
         mlflow.log_param('alpha', self.alpha)
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/cc.py` & `label_noise_correction-0.0.2/src/label_noise_correction/cc.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ----------
     n_iterations : int
         Number of iterations to run
     n_clusters : int
         Number of clusters to use
     """
     def __init__(self, n_iterations, n_clusters):
+        super().__init__('CC')
         self.n_iterations = n_iterations
         self.n_clusters = n_clusters
 
     def calc_weights(self, cluster_labels:pd.Series, label_dist, n_labels):
         d = [cluster_labels.value_counts().loc[l]/len(cluster_labels) if l in cluster_labels.value_counts().index else 0 for l in range(n_labels)]
         u = 1/n_labels
         multiplier = min(math.log(len(cluster_labels), 10), 2)
@@ -58,10 +59,10 @@
             for idx in X.index:
                 ins_weights[idx] += cluster_weights[C.labels_[idx]]
 
         y_corrected = [np.argmax(ins_weights[idx]) for idx in X.index]
         return pd.Series(y_corrected, index=original_index)
 
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Cluster-Based Correction')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('n_iterations', self.n_iterations)
         mlflow.log_param('n_clusters', self.n_clusters)
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/fair_obnc.py` & `label_noise_correction-0.0.2/src/label_noise_correction/fair_obnc.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ----------
     m : float
         Proportion of labels to correct
     sensitive_attr : str
         Name of sensitive attribute
     """
     def __init__(self, m, sensitive_attr):
-        super().__init__(m)
+        super().__init__('Fair-OBNC-rs', m)
         self.sensitive_attr = sensitive_attr
 
     def correct(self, X:pd.DataFrame, y:pd.Series):
         y_corrected = y.copy()
         X_fair = X.drop(columns=self.sensitive_attr)
 
         bagging = BaggingClassifier(n_estimators=100, random_state=42).fit(X_fair, y)
@@ -29,15 +29,15 @@
         margins = self.calculate_margins(X_fair.loc[y != y_pred], y.loc[y != y_pred], bagging).apply(lambda x: abs(x)).sort_values(ascending=False)
         index = margins.index[:int(self.m*len(margins))]
         y_corrected.loc[index] = y_pred.loc[index]
 
         return y_corrected
     
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Fair-OBNC-rs')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('m', self.m)
         mlflow.log_param('sensitive_attr', self.sensitive_attr)
 
 class FairOBNCOptimizeDemographicParity(OrderingBasedCorrection):
     """
     Fair Ordering-Based Correction algorithm (Fair-OBNC-dp)
 
@@ -47,15 +47,15 @@
         Proportion of labels to correct
     sensitive_attr : str
         Name of sensitive attribute
     prob : float
         Probability of correcting a label that does not contribute to balancing label distribution across sensitive groups
     """
     def __init__(self, m:float, sensitive_attr:str, prob:float):
-        super().__init__(m)
+        super().__init__('Fair-OBNC-dp', m)
         self.sensitive_attr = sensitive_attr
         self.prob = prob
 
     def dem_par_diff(self, X, y, attr):
         p_y1_g1 = len(y.loc[(X[attr] == 1) & (y == 1)]) / len(y.loc[X[attr] == 1])
         p_y1_g0 = len(y.loc[(X[attr] == 0) & (y == 1)]) / len(y.loc[X[attr] == 0])
 
@@ -89,15 +89,15 @@
                 
                 if corrected == n:
                     break
 
         return y_corrected
     
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Fair-OBNC-dp')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('m', self.m)
         mlflow.log_param('sensitive_attr', self.sensitive_attr)
         mlflow.log_param('prob', self.prob)
 
 class FairOBNC(FairOBNCOptimizeDemographicParity):
     """
     Fair Ordering-Based Correction algorithm (Fair-OBNC)
@@ -108,15 +108,15 @@
         Proportion of labels to correct
     sensitive_attr : str
         Name of sensitive attribute
     prob : float
         Probability of correcting a label that does not contribute to balancing label distribution across sensitive groups
     """
     def __init__(self, m:float, sensitive_attr:str, prob:float):
-        super().__init__(m, sensitive_attr, prob)
+        super().__init__('Fair-OBNC', m, sensitive_attr, prob)
 
     def correct(self, X:pd.DataFrame, y:pd.Series):
         y_corrected = y.copy()
         X_fair = X.drop(columns=self.sensitive_attr)
 
         bagging = BaggingClassifier(n_estimators=100, random_state=42).fit(X_fair, y)
         y_pred = pd.Series(bagging.predict(X_fair), index=y.index)
@@ -143,11 +143,11 @@
                 
                 if corrected == n:
                     break
 
         return y_corrected
     
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Fair-OBNC')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('m', self.m)
         mlflow.log_param('sensitive_attr', self.sensitive_attr)
         mlflow.log_param('prob', self.prob)
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/hlnc.py` & `label_noise_correction-0.0.2/src/label_noise_correction/hlnc.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     Attributes
     ----------
     n_clusters : int
         Number of clusters to use in KMeans clustering
     """
     def __init__(self, n_clusters):
+        super().__init__('HLNC')
         self.n_clusters = n_clusters
     
     def correct(self, X:pd.DataFrame, y:pd.Series):
         original_index = X.index
 
         X = X.reset_index(drop=True)
         y = y.reset_index(drop=True)
@@ -85,9 +86,9 @@
                     y_corrected.loc[low_conf[i]] = y_pred_dt[i]
                     
             low_conf = [x for x in low_conf if x not in high_conf]
 
         return pd.Series(y_corrected.values, index=original_index)
     
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Hybrid Label Noise Correction')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('n_clusters', self.n_clusters)
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/labelcorrection.py` & `label_noise_correction-0.0.2/src/label_noise_correction/labelcorrection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 import pandas as pd
 
 class LabelCorrectionModel(ABC):
-    def __init__(self) -> None:
-        pass
+    def __init__(self, name):
+        self.name = name
 
     @abstractmethod
     def correct(self, X:pd.DataFrame, y:pd.Series) -> pd.Series:
         """
         Corrects the labels of the given dataset
 
         Parameters
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/obnc.py` & `label_noise_correction-0.0.2/src/label_noise_correction/obnc.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     Attributes
     ----------
     m : float
         Proportion of labels to correct
     """
     def __init__(self, m):
+        super().__init__('OBNC')
         self.m = m
 
     def calculate_margins(self, X, y, bagging:BaggingClassifier):
         margins = pd.Series(dtype=float)
         for i in X.index:
             preds = [dt.predict(X.loc[i].values.reshape(1, -1))[0] for dt in bagging.estimators_]
             true_y = y.loc[i]
@@ -43,9 +44,9 @@
         margins = self.calculate_margins(X.loc[y != y_pred], y.loc[y != y_pred], bagging).apply(lambda x: abs(x)).sort_values(ascending=False)
         index = margins.index[:int(self.m*len(margins))]
         y_corrected.loc[index] = y_pred.loc[index]
 
         return y_corrected
     
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Ordering-Based Correction')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('m', self.m)
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/pl.py` & `label_noise_correction-0.0.2/src/label_noise_correction/pl.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ----------
     classifier
         Type of classifier to use
     n_folds : int
         Number of folds to use
     """
     def __init__(self, classifier, n_folds):
+        super().__init__('PL')
         self.classifier = classifier
         self.n_folds = n_folds
 
     def correct(self, X:pd.DataFrame, y:pd.Series):
         original_index = X.index
 
         X = X.reset_index(drop=True)
@@ -40,10 +41,10 @@
         y_corrected = X.apply(
             lambda x: 0 if np.mean([models[i].predict([x.values])[0] for i in range(self.n_folds)]) < 0.5 else 1, 
             axis=1).to_list()
         
         return pd.Series(y_corrected, index=original_index)
     
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Polishing Labels')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('correction_classifier', self.classifier.__name__)
         mlflow.log_param('n_folds', self.n_folds)
```

### Comparing `label_noise_correction-0.0.1/src/label_noise_correction/stc.py` & `label_noise_correction-0.0.2/src/label_noise_correction/stc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         Type of classifier to use 
     n_folds : int
         Number of folds to use
     correction_rate : float
         Percentage of labels to correct
     """
     def __init__(self, classifier, n_folds, correction_rate):
+        super().__init__('STC')
         self.classifier = classifier
         self.n_folds = n_folds
         self.correction_rate = correction_rate
 
     def correct(self, X:pd.DataFrame, y:pd.Series):
         original_index = X.index
 
@@ -81,11 +82,11 @@
         y_corrected = y.values
         for i in corrected.sort_values('y_prob', ascending=False)[:correction_n].index:
             y_corrected[i] = corrected.loc[i, 'y_pred']
 
         return pd.Series(y_corrected, index=original_index)
 
     def log_params(self):
-        mlflow.log_param('correction_alg', 'Self-Training Correction')
+        mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('correction_classifier', self.classifier.__name__)
         mlflow.log_param('n_folds', self.n_folds)
         mlflow.log_param('correction_rate', self.correction_rate)
```

### Comparing `label_noise_correction-0.0.1/.gitignore` & `label_noise_correction-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.1/LICENSE` & `label_noise_correction-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.1/README.md` & `label_noise_correction-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.1/pyproject.toml` & `label_noise_correction-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "label_noise_correction"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Inês Silva", email="inesoliveiraesilva@gmail.com" },
 ]
 description = "Label Noise Correction Methods"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `label_noise_correction-0.0.1/PKG-INFO` & `label_noise_correction-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: label_noise_correction
-Version: 0.0.1
+Version: 0.0.2
 Summary: Label Noise Correction Methods
 Project-URL: Homepage, https://github.com/reluzita/label-noise-correction
 Author-email: Inês Silva <inesoliveiraesilva@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


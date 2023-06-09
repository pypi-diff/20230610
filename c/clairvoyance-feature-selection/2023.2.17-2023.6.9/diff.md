# Comparing `tmp/clairvoyance_feature_selection-2023.2.17.tar.gz` & `tmp/clairvoyance_feature_selection-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clairvoyance_feature_selection-2023.2.17.tar", last modified: Fri Feb 17 21:37:47 2023, max compression
+gzip compressed data, was "clairvoyance_feature_selection-2023.6.9.tar", last modified: Fri Jun  9 22:37:52 2023, max compression
```

## Comparing `clairvoyance_feature_selection-2023.2.17.tar` & `clairvoyance_feature_selection-2023.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-02-17 21:37:47.835697 clairvoyance_feature_selection-2023.2.17/
--rw-------   0 jespinoz  (3456) staff       (20)     1563 2022-12-27 22:25:44.000000 clairvoyance_feature_selection-2023.2.17/LICENSE.txt
--rw-------   0 jespinoz  (3456) staff       (20)      197 2022-12-27 22:26:50.000000 clairvoyance_feature_selection-2023.2.17/MANIFEST.in
--rw-r--r--   0 jespinoz  (3456) staff       (20)      287 2023-02-17 21:37:47.835324 clairvoyance_feature_selection-2023.2.17/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)    11929 2023-01-11 01:25:40.000000 clairvoyance_feature_selection-2023.2.17/README.md
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-02-17 21:37:47.830560 clairvoyance_feature_selection-2023.2.17/bin/
--rw-------   0 jespinoz  (3456) staff       (20)    87658 2022-12-27 22:53:11.000000 clairvoyance_feature_selection-2023.2.17/bin/clairvoyance_v1.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-02-17 21:37:47.832580 clairvoyance_feature_selection-2023.2.17/clairvoyance/
--rw-------   0 jespinoz  (3456) staff       (20)     2910 2023-02-17 20:35:42.000000 clairvoyance_feature_selection-2023.2.17/clairvoyance/__init__.py
--rw-------   0 jespinoz  (3456) staff       (20)    89100 2023-02-17 21:36:37.000000 clairvoyance_feature_selection-2023.2.17/clairvoyance/clairvoyance.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-02-17 21:37:47.834879 clairvoyance_feature_selection-2023.2.17/clairvoyance_feature_selection.egg-info/
--rw-r--r--   0 jespinoz  (3456) staff       (20)      287 2023-02-17 21:37:47.000000 clairvoyance_feature_selection-2023.2.17/clairvoyance_feature_selection.egg-info/PKG-INFO
--rw-r--r--   0 jespinoz  (3456) staff       (20)      388 2023-02-17 21:37:47.000000 clairvoyance_feature_selection-2023.2.17/clairvoyance_feature_selection.egg-info/SOURCES.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)        1 2023-02-17 21:37:47.000000 clairvoyance_feature_selection-2023.2.17/clairvoyance_feature_selection.egg-info/dependency_links.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)      139 2023-02-17 21:37:47.000000 clairvoyance_feature_selection-2023.2.17/clairvoyance_feature_selection.egg-info/requires.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       13 2023-02-17 21:37:47.000000 clairvoyance_feature_selection-2023.2.17/clairvoyance_feature_selection.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-02-17 21:37:47.835802 clairvoyance_feature_selection-2023.2.17/setup.cfg
--rw-------   0 jespinoz  (3456) staff       (20)     1026 2022-12-27 22:38:27.000000 clairvoyance_feature_selection-2023.2.17/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.495942 clairvoyance_feature_selection-2023.6.9/
+-rw-------   0 jespinoz  (3456) staff       (20)     1563 2022-12-27 22:25:44.000000 clairvoyance_feature_selection-2023.6.9/LICENSE.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      197 2022-12-27 22:26:50.000000 clairvoyance_feature_selection-2023.6.9/MANIFEST.in
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      314 2023-06-09 22:37:52.495622 clairvoyance_feature_selection-2023.6.9/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)    11934 2023-06-09 22:36:15.000000 clairvoyance_feature_selection-2023.6.9/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.489595 clairvoyance_feature_selection-2023.6.9/bin/
+-rw-------   0 jespinoz  (3456) staff       (20)    87658 2022-12-27 22:53:11.000000 clairvoyance_feature_selection-2023.6.9/bin/clairvoyance_v1.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.491586 clairvoyance_feature_selection-2023.6.9/clairvoyance/
+-rw-------   0 jespinoz  (3456) staff       (20)     2968 2023-06-09 21:31:53.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance/__init__.py
+-rw-------   0 jespinoz  (3456) staff       (20)   106647 2023-06-09 21:31:32.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance/clairvoyance.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.495156 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      314 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      388 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      139 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       13 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-06-09 22:37:52.496064 clairvoyance_feature_selection-2023.6.9/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)     1026 2022-12-27 22:38:27.000000 clairvoyance_feature_selection-2023.6.9/setup.py
```

### Comparing `clairvoyance_feature_selection-2023.2.17/LICENSE.txt` & `clairvoyance_feature_selection-2023.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clairvoyance_feature_selection-2023.2.17/README.md` & `clairvoyance_feature_selection-2023.6.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Reimplementation for `Clairvoyance` from [Espinoza & Dupont et al. 2021](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008857).  The updated version includes regression support, support for all linear/tree-based models, and improved visualizations.  `Clairvoyance` is currently in active development.   
 
 
 #### Details:
 `import clairvoyance as cy`
 
-`__version__ = "2022.1.3"`
+`__version__ = "2023.6.9"`
 
 #### Installation
 
 ```
 # Stable:
 pip install clairvoyance_feature_selection
 conda install -c jolespin clairvoyance
@@ -26,15 +26,15 @@
 ```
 
 #### Citation
 
 Espinoza JL, Dupont CL, O’Rourke A, Beyhan S, Morales P, Spoering A, et al. (2021) Predicting antimicrobial mechanism-of-action from transcriptomes: A generalizable explainable artificial intelligence approach. PLoS Comput Biol 17(3): e1008857. https://doi.org/10.1371/journal.pcbi.1008857
 
 #### Development
-*Clairvoyance* is current in active development and undergoing a complete reimplementation from the ground up from the original publication.  The following includes a list of new features: 
+*Clairvoyance* is currently under active development and undergoing a complete reimplementation from the ground up from the original publication.  The following includes a list of new features: 
 
 *  Supports any linear or tree-based `Scikit-Learn` compatible model
 *  Supports any `Scikit-Learn` compatible performance metric
 *  Supports regression (in addition to classification as in original implementation)
 *  Properly implements transformations for compositional data (e.g., CLR and closure) based on the query features for each iteration
 *  Added option to remove zero weighted features and redundant feature sets
 *  Added asymmetric mode in addition to the symmetric mode from the original implementation
```

### Comparing `clairvoyance_feature_selection-2023.2.17/bin/clairvoyance_v1.py` & `clairvoyance_feature_selection-2023.6.9/bin/clairvoyance_v1.py`

 * *Files identical despite different names*

### Comparing `clairvoyance_feature_selection-2023.2.17/clairvoyance/__init__.py` & `clairvoyance_feature_selection-2023.6.9/clairvoyance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,33 @@
 #
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #
 # =======
 # Version
 # =======
-__version__= "2023.2.17"
+__version__= "2023.6.9"
 __author__ = "Josh L. Espinoza"
 __email__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"
 __url__ = "https://github.com/jolespin/clairvoyance"
 __cite__ = "https://github.com/jolespin/clairvoyance"
 __license__ = "BSD-3"
 __developmental__ = True
 
 functions = { 
   "format_stratify",
   "format_weights",
   "format_cross_validation",
   "get_feature_importance_attribute",
+  "get_balanced_class_subset",
   "recursive_feature_inclusion",
   "plot_scores_line","plot_weights_bar",
   "plot_weights_box",
   "plot_recursive_feature_selection",
+  "plot_scores_comparison",
 }
 classes = {
   "ClairvoyanceBase","ClairvoyanceClassification","ClairvoyanceRegression","ClairvoyanceRecursive",
 
 }
 __all__ = sorted(functions | classes)
 __doc__ = """
```

### Comparing `clairvoyance_feature_selection-2023.2.17/clairvoyance/clairvoyance.py` & `clairvoyance_feature_selection-2023.6.9/clairvoyance/clairvoyance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
+
 # Built-ins
+from ast import Or
 import os, sys, itertools, argparse, time, datetime, copy, warnings
 from collections import OrderedDict
 # from multiprocessing import cpu_count
 
 # PyData
 import pandas as pd
 import numpy as np
 import xarray as xr
 
 ## Plotting
-# from matplotlib import use as mpl_backend
-# mpl_backend("Agg")
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # Machine learning
 from scipy import stats
 from sklearn.metrics import get_scorer, make_scorer
 from sklearn.model_selection import cross_val_score, train_test_split, RepeatedStratifiedKFold, StratifiedKFold, RepeatedKFold, KFold
@@ -25,23 +25,30 @@
 from sklearn.exceptions import ConvergenceWarning, UndefinedMetricWarning
 
 # # Parallel
 # import ray
 # from ray.air.config import ScalingConfig
 # from ray.train.sklearn import SklearnTrainer
 
+# Clairvoyance 
+try:
+    from . import __version__ 
+except ImportError:
+    __version__ = None
+    warnings.warn("Unable to load version information")
+
 # Soothsayer Utils
 from soothsayer_utils import (
     assert_acceptable_arguments,
     format_header,
     format_duration,
-    read_dataframe,
+    # read_dataframe,
     read_object,
     write_object,
-    to_precision,
+    # to_precision,
     pv,
     flatten,
 )
 
 # Specify maximum number of threads
 # available_threads = cpu_count()
 
@@ -78,14 +85,15 @@
     X_transformed = X.copy()
 
     # Checks
     if X.ndim != 2:
         raise ValueError("Input matrix must have two dimensions")
     # if np.all(X == 0, axis=1).sum() > 0:
     #     raise ValueError("Input matrix cannot have rows with all zeros")
+
     # Transformed output
     if method is not None:
         if np.any(X.values < 0):
             raise ValueError("Cannot have negative values")
         if X.shape[1] > 1:
             if method == "closure":
                 X_transformed = closure(X)
@@ -102,14 +110,15 @@
         else:
             if verbose > 1:
                 print("Only 1 feature left.  Ignoring transformation.", file=log)
 
     # Transpose back
     if axis == 0:
         X_transformed = X_transformed.T
+
     return X_transformed
 
 def format_stratify(stratify, estimator_type:str, y:pd.Series):
     assert_acceptable_arguments(estimator_type, {"classifier", "regressor"})
     if isinstance(stratify, bool):
         if stratify is True:
             assert estimator_type == "classifier", "If `stratify=True` then the estimator must be a classifier.  Please provide a stratification grouping or select None for regressor."
@@ -257,49 +266,86 @@
             importance_getter = "coef_"
         if hasattr(estimator, "feature_importances_"):
             importance_getter = "feature_importances_"
         assert importance_getter is not None, "If `importance_getter='auto'`, `estimator` must be either a linear model with `.coef_` or a tree-based model with `.feature_importances_`"
     assert hasattr(estimator, importance_getter), "Fitted estimator does not have feature weight attribute: `{}`".format(importance_getter)
     return importance_getter
 
+def get_balanced_class_subset(y:pd.Series, size:float=0.1, random_state=None):
+    n = y.size
+    number_of_classes = y.nunique()
+    number_of_samples_in_subset = int(n * size)
+    subset_size_per_class = int(number_of_samples_in_subset/number_of_classes)
+    
+    index = list()
+    for id_class in y.unique():
+        class_samples = y[lambda x: x == id_class].index
+        assert len(class_samples) >= subset_size_per_class
+        subset = np.random.RandomState(random_state).choice(class_samples, size=subset_size_per_class, replace=False)
+        index += subset.tolist()
+    return index
 def recursive_feature_inclusion(
     estimator, 
     X:pd.DataFrame, 
     y:pd.Series, 
     scorer,
     initial_feature_weights:pd.Series, 
     initial_feature_weights_name:str="initial_feature_weights",
     feature_weight_attribute:str="auto",
     transformation=None,
     multiplicative_replacement="auto",
     metric=np.mean, 
     early_stopping=25, 
     minimum_improvement_in_score=0.0,
     additional_feature_penalty=None,
-    maximum_number_of_features=np.inf,
+    maximum_number_of_features="auto",
     target_score=-np.inf, 
     less_features_is_better=True,  
     random_state=0,
     n_jobs=1,
     cv=(5,3), 
     stratify=None, 
     training_column="training_index", 
     testing_column="testing_index", 
     cv_prefix="cv=",
     verbose=0,
     log=sys.stdout,
     progress_message="Recursive feature inclusion",
     remove_zero_weighted_features=True,
     maximum_tries_to_remove_zero_weighted_features=1000,
+    X_validation:pd.DataFrame=None,
+    y_validation:pd.Series=None,
+    # optimize_validation_score = "auto",
     ) -> pd.Series:
 
     assert len(set(X.columns)) == X.shape[1], "Cannot have duplicate feature names in `X`"
     if additional_feature_penalty is None:
         additional_feature_penalty = lambda number_of_features: 0.0
 
+    # Validation
+    X_validation_is_provided = X_validation is not None
+    y_validation_is_provided = y_validation is not None
+
+    if X_validation_is_provided is not None:
+        assert y_validation_is_provided is not None, "If `X_validation` is provided then `y_validation` must be provided"
+
+    if y_validation_is_provided is not None:
+        assert X_validation_is_provided is not None, "If `y_validation` is provided then `X_validation` must be provided"
+
+    validation_set_provided = False
+    if all([X_validation_is_provided, y_validation_is_provided]):
+        assert np.all(X_validation.index == y_validation.index), "X_validation.index and y_validation.index must have the same ordering"
+        assert np.all(X_validation.columns == X.columns), "X_validation.columns and X.columns must have the same ordering"
+        validation_set_provided = True
+    # if optimize_validation_score == "auto":
+    #     if validation_set_provided:
+    #         optimize_validation_score = True
+    #     else:
+    #         optimize_validation_score = False
+
     # Transformations
     assert_acceptable_arguments(transformation, {None,"clr","closure"})
     if multiplicative_replacement is None:
         multiplicative_replacement = 0.0
     if isinstance(multiplicative_replacement, str):
         assert multiplicative_replacement == "auto", "If `multiplicative_replacement` is a string, it must be `auto`"
     else:
@@ -315,42 +361,47 @@
     
     # Scorer
     if isinstance(scorer, str):
         scorer = get_scorer(scorer)
 
     # Maximum number of features
     if maximum_number_of_features == "auto":
-        maximum_number_of_features = int(X.shape[1]*0.6180339887)
+        maximum_number_of_features = min(X.shape)
     if maximum_number_of_features == -1:
         maximum_number_of_features = X.shape[1]
+    if maximum_number_of_features is None:
+        maximum_number_of_features = X.shape[1]
     assert maximum_number_of_features > 0, "maximum_number_of_features must be greater than 0"
 
     # Best results
     history = OrderedDict()
+    validation_scores = OrderedDict()
 
     best_features = None
     best_score = target_score
 
     # Feature tracker
     feature_tuples = list()
     unique_feature_sets = list()
     
     # Progress tracker
     no_progress = 0
+
     if progress_message is None:
         iterable = range(initial_feature_weights.size)
     else:
         iterable = pv(range(initial_feature_weights.size), description=progress_message)
+
     for i in iterable:
         features = initial_feature_weights.index[:i+1].tolist()
         X_rfi = X.loc[:,features]
 
         continue_algorithm = True
 
-        # Transform features
+        # Transform features (if transformation = None, then there is no transformation)
         if X_rfi.shape[1] > 1: 
             X_rfi = transform(X=X_rfi, method=transformation, multiplicative_replacement=multiplicative_replacement, axis=1)
         else:
             if transformation is not None:
                 continue_algorithm = False
             if verbose > 2:
                 print("Only 1 feature left.  Ignoring transformation.", file=log)
@@ -386,29 +437,57 @@
             if feature_set  in unique_feature_sets:
                 if verbose > 0:
                     print("Skipping iteration {} because removing zero-weighted features has produced a feature set that has already been evaluated: {}".format(i, set(feature_set)), file=log)
             else:
                 feature_tuples.append(tuple(features))
                 unique_feature_sets.append(feature_set)
 
+                # Training/Testing Scores
                 scores = cross_val_score(estimator=estimator, X=X_rfi, y=y, cv=cv_splits, n_jobs=n_jobs, scoring=scorer)
 
                 average_score = np.mean(scores)
                 history[i] = scores #{"average_score":average_score, "sem":sem}
-                
+
+                #! ---
+                # Validation Score
+                query_score = average_score
+                validation_score = np.nan
+                if validation_set_provided:
+                    estimator.fit(
+                        X=X_rfi, 
+                        y=y,
+                    )
+                    
+                    # Transform features (if transformation = None, then there is no transformation)
+                    X_validation_rfi = transform(X=X_validation.loc[:,features], method=transformation, multiplicative_replacement=multiplicative_replacement, axis=1)
+                    validation_score = scorer(estimator=estimator, X=X_validation_rfi, y_true=y_validation)
+                    validation_scores[i] = validation_score
+                    # if optimize_validation_score:
+                    #     query_score = validation_score
+                #! ---
+
                 # Add penalties to score target
                 penalty_adjusted_score_target = (best_score + minimum_improvement_in_score + additional_feature_penalty(len(features)))
                 
-                if average_score <= penalty_adjusted_score_target:
+                if query_score <= penalty_adjusted_score_target:
                     if verbose > 1:
-                        print("Current iteration {} of N={} features has not improved score: {} ≤ {}".format(i, len(features), average_score, best_score), file=log)
+                        # if optimize_validation_score:
+                        #     print("Current iteration {} of N={} features has not improved score: Validation Score[{} ≤ {}]".format(i, len(features), validation_score, best_score), file=log)
+                        # else:
+                        print("Current iteration {} of N={} features has not improved score: Average Score[{} ≤ {}]".format(i, len(features), average_score, best_score), file=log)
+
                     no_progress += 1
                 else:
+                    # if optimize_validation_score:
+                    #     if verbose > 0:
+                    #         print("Updating best score with N={} features : Validation Score[{} -> {}]".format(len(features), best_score, validation_score), file=log)
+                    #     best_score = validation_score
+                    # else:
                     if verbose > 0:
-                        print("Updating best score with N={} features : {} -> {}".format(len(features), best_score, average_score), file=log)
+                        print("Updating best score with N={} features : Average Score[{} -> {}]".format(len(features), best_score, average_score), file=log)
                     best_score = average_score
                     best_features = features
                     no_progress = 0
                 if no_progress >= early_stopping:
                     break
             if len(features) >= maximum_number_of_features:
                 if verbose > 0:
@@ -417,30 +496,61 @@
     if verbose > 0:
         if best_features is None:
             print("Terminating algorithm after {} iterations with a best score of {} as no feature set improved the score with current parameters".format(i+1, best_score), file=log)
         else:
             print("Terminating algorithm at N={} features after {} iterations with a best score of {}".format(len(best_features), i+1, best_score), file=log)
     
     history = pd.DataFrame(history, index=list(map(lambda x: ("splits", x), cv_labels))).T
+    # if validation_set_provided:
+    #     history[("validation","score")] = pd.Series(validation_scores)
     history.index = feature_tuples
     history.index.name = "features"
+    
+    # Summary
     average_scores = history.mean(axis=1)
     sems = history.sem(axis=1)
+    if validation_set_provided:
+        validation_scores = pd.Series(validation_scores)
+        validation_scores.index = feature_tuples
+    else:
+        validation_scores = pd.Series([np.nan]*len(feature_tuples), index=feature_tuples)
+    
     history.insert(loc=0, column=("summary", "number_of_features"),value = history.index.map(len))
     history.insert(loc=1, column=("summary", "average_score"),value = average_scores)
     history.insert(loc=2, column=("summary", "sem"),value = sems)
+    history.insert(loc=3, column=("summary", "validation_score"), value = validation_scores)
+    history.insert(loc=4, column=("summary", "∆(validation_score-average_score)"), value = average_scores - validation_scores)
+
     history.columns = pd.MultiIndex.from_tuples(history.columns)
+
     
     # Highest scoring features (not necessarily the best since there can be many features added with minimal gains)
+    # if optimize_validation_score:
+    #     highest_score = history[("summary", "validation_score")].max()
+    #     highest_scoring_features = list(history.loc[history[("summary", "validation_score")] == highest_score].sort_values(
+    #         by=[("summary", "average_score"), ("summary", "number_of_features")], 
+    #         ascending=[False, less_features_is_better]).index[0])
+    # else:
     highest_score = history[("summary", "average_score")].max()
     highest_scoring_features = list(history.loc[history[("summary", "average_score")] == highest_score, ("summary", "number_of_features")].sort_values(ascending=less_features_is_better).index[0])
     
-    # Best results
-    best_features = list(history.loc[history[("summary", "average_score")] == best_score, ("summary", "number_of_features")].sort_values(ascending=less_features_is_better).index[0])
+    # # Best results
+    # if optimize_validation_score:
+    #     # best_features = list(history.loc[history[("summary", "validation_score")] == best_score].sort_values(
+    #     #     by=[("summary", "average_score"), ("summary", "number_of_features")], 
+    #     #     ascending=[False, less_features_is_better]).index[0])
+    # else:
+    #     best_features = list(history.loc[history[("summary", "average_score")] == best_score, ("summary", "number_of_features")].sort_values(ascending=less_features_is_better).index[0])
+    best_features = list(history.loc[history[("summary", "average_score")] == best_score].sort_values(
+        by=[("summary", "validation_score"), ("summary", "average_score"), ("summary", "number_of_features")], 
+        ascending=[False, False, less_features_is_better]).index[0])
+    
     best_estimator_sem = history.loc[[tuple(best_features)],("summary","sem")].values[0]
+    best_estimator_validation_score = history.loc[[tuple(best_features)],("summary","validation_score")].values[0]
+
     best_estimator_rci = clone(estimator)
     X_best_features = transform(X=X.loc[:,best_features], method=transformation, multiplicative_replacement=multiplicative_replacement, axis=1)
 
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=ConvergenceWarning)
         best_estimator_rci.fit(X_best_features, y)
     
@@ -482,29 +592,33 @@
         best_features=best_features,
         best_estimator_rci=best_estimator_rci,
         feature_weights=feature_weights,
         highest_score=highest_score,
         highest_scoring_features=highest_scoring_features,
         cv_splits=cv_splits, 
         cv_labels=cv_labels,
+        validation_scores=validation_scores,
+        best_estimator_validation_score=best_estimator_validation_score,
         ),
         name="recursive_feature_elimination",
     )
 
 
 # Plotting
 def plot_scores_line(
     average_scores:pd.Series, 
     sem:pd.Series, 
+    validation_scores:pd.Series=None, 
     horizontal_lines=True,
     vertical_lines="auto",
     title=None,
     figsize=(13,3), 
     linecolor="black",
     errorcolor="gray",
+    validation_linecolor="red",
     style="seaborn-white",
     xlim=None,
     ylim=None,
     ax=None, 
     alpha=0.382, 
     xlabel="$N_{Features}$", 
     ylabel="Score", 
@@ -532,15 +646,18 @@
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = plt.gcf()
         
         average_scores.plot(ax=ax, color=linecolor, label="Average score", **kwargs)
         x_grid = np.arange(average_scores.size)
         ax.fill_between(x_grid, y1=average_scores-sem, y2=average_scores+sem, alpha=alpha, color=errorcolor, label="SEM")
-        
+        if validation_scores is not None:
+            if not np.all(validation_scores.isnull()):
+                validation_scores.plot(ax=ax, color=validation_linecolor, label="Validation score", **kwargs)
+
         rci = np.argmax(average_scores.values) 
         if vertical_lines == "auto":
             vertical_lines = rci
         if isinstance(vertical_lines, (float,np.floating, int, np.integer)):
             vertical_lines = [vertical_lines]
         
         for v in vertical_lines:
@@ -673,15 +790,14 @@
         _box_kws = dict( linewidth=1.0, boxprops={"facecolor": color}, medianprops={"color": linecolor})
         _box_kws.update(kwargs)
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = plt.gcf()
         
-
         feature_weights = feature_weights.dropna(how="all", axis=0)
         if ascending is not None:
             index = feature_weights.mean(axis=1).sort_values(ascending=ascending).index
             feature_weights = feature_weights.loc[index]
             
         # feature_weights.T.plot(ax=ax, color=color, label=ylabel, kind="box")
         
@@ -711,22 +827,24 @@
             ax.xaxis.grid(True)
         if show_ygrid:
             ax.yaxis.grid(True)
         return fig, ax
 
 def plot_recursive_feature_selection(
     number_of_features:pd.Series, 
-    scores:pd.Series, 
+    average_scores:pd.Series, 
     # sem:pd.Series=None, 
+    # validation_scores:pd.Series=None,
     min_features:int=None,
     max_features:int=None,
     min_score:float=None,
     max_score:float=None,
     ax=None,
     color="darkslategray",
+    color_validation="red",
     linewidth=0.618,
     alpha=0.618,
     edgecolor="black", 
     style="seaborn-white",
     figsize=(8,3),
     title=None,
     xlabel="$N_{Features}$",
@@ -740,62 +858,177 @@
     ylabel_kws=dict(), 
     xticklabel_kws=dict(), 
     yticklabel_kws=dict(),
     title_kws=dict(),
     legend_kws=dict(),
     **kwargs,
     ):
+
     assert isinstance(number_of_features, pd.Series)
-    assert isinstance(scores, pd.Series)
-    assert np.all(number_of_features.index == scores.index)
-    df = pd.DataFrame([number_of_features, scores], index=["number_of_features", "scores"]).T
+    assert isinstance(average_scores, pd.Series)
+    assert np.all(number_of_features.index == average_scores.index)
+    df = pd.DataFrame([number_of_features, average_scores], index=["number_of_features", "average_scores"]).T
     # if sem is not None:
     #     assert isinstance(sem, pd.Series)
     #     assert np.all(df.index == sem.index)
     #     df["sem"] = sem
     
     if min_features:
         df = df.query("number_of_features >= {}".format(min_features))
     if max_features:
         df = df.query("number_of_features <= {}".format(max_features))
     if min_score:
-        df = df.query("scores >= {}".format(min_score))
+        df = df.query("average_scores >= {}".format(min_score))
     if max_score:
-        df = df.query("scores <= {}".format(max_score))
+        df = df.query("average_scores <= {}".format(max_score))
         
     with plt.style.context(style):
         _title_kws = {"fontsize":16, "fontweight":"bold"}; _title_kws.update(title_kws)
         _xlabel_kws = {"fontsize":15}; _xlabel_kws.update(xlabel_kws)
         _ylabel_kws = {"fontsize":15}; _ylabel_kws.update(ylabel_kws)
         _xticklabel_kws = {"fontsize":12, "rotation":xtick_rotation}; _xticklabel_kws.update(xticklabel_kws)
         _yticklabel_kws = {"fontsize":12}; _yticklabel_kws.update(yticklabel_kws)
         _legend_kws = {"fontsize":12}; _legend_kws.update(legend_kws)
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = plt.gcf()
 
         # if sem is not None:
-        #     ax.errorbar(df["number_of_features"].values, df["scores"].values, yerr=df["sem"].values, alpha=0.1618, color=color)
-        ax.scatter(x=df["number_of_features"].values, y=df["scores"].values, edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
-        ax.set_xlabel(xlabel, fontsize=12)
-        ax.set_ylabel(ylabel, fontsize=12)
+        #     ax.errorbar(df["number_of_features"].values, df["average_scores"].values, yerr=df["sem"].values, alpha=0.1618, color=color)
+        ax.scatter(x=df["number_of_features"].values, y=df["average_scores"].values, edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
 
         ax.set_xlabel(xlabel, **_xlabel_kws)
         ax.set_ylabel(ylabel, **_ylabel_kws)
         # ax.set_yticklabels(map(lambda x:"%0.2f"%x, ax.get_yticks()), **_yticklabel_kws)
         if title:
             ax.set_title(title, **_title_kws)
         if show_legend:
             ax.legend(**_legend_kws)
         if show_xgrid:
             ax.xaxis.grid(True)
         if show_ygrid:
             ax.yaxis.grid(True)
         return fig, ax
+    
+def plot_scores_comparison(
+    number_of_features:pd.Series, 
+    average_scores:pd.Series, 
+    validation_scores:pd.Series=None,
+    min_features:int=None,
+    max_features:int=None,
+    min_score:float=None,
+    max_score:float=None,
+    ax=None,
+    color="darkslategray",
+    linewidth=0.618,
+    alpha=0.618,
+    edgecolor="black", 
+    style="seaborn-white",
+    figsize=(8,5),
+    title=None,
+    xlabel="Average Score",
+    ylabel="Validation Score",
+
+    feature_to_size_function = "auto",
+
+    xtick_rotation=0,
+    show_xgrid=False,
+    show_ygrid=True,
+    # show_zgrid=True,
+
+    show_xticks=True, 
+    show_legend=True,
+    xlabel_kws=dict(), 
+    ylabel_kws=dict(), 
+    # zlabel_kws=dict(), 
+
+    xticklabel_kws=dict(), 
+    yticklabel_kws=dict(),
+    # zticklabel_kws=dict(),
+
+    title_kws=dict(),
+    legend_kws=dict(),
+    **kwargs,
+    ):
+
+    assert isinstance(number_of_features, pd.Series)
+    assert isinstance(average_scores, pd.Series)
+    assert isinstance(validation_scores, pd.Series)
+
+    assert np.all(number_of_features.index == average_scores.index)
+    assert np.all(number_of_features.index == validation_scores.index)
+
+    df = pd.DataFrame([number_of_features, average_scores, validation_scores], index=["number_of_features", "average_scores", "validation_scores"]).T
+
+    if min_features:
+        df = df.query("number_of_features >= {}".format(min_features))
+    if max_features:
+        df = df.query("number_of_features <= {}".format(max_features))
+    if min_score:
+        df = df.query("average_scores >= {}".format(min_score))
+    if max_score:
+        df = df.query("average_scores <= {}".format(max_score))
+    if min_score:
+        df = df.query("validation_scores >= {}".format(min_score))
+    if max_score:
+        df = df.query("validation_scores <= {}".format(max_score))
+
+    if feature_to_size_function == "auto":
+        def feature_to_size_function(n):
+            return 100/n
+    assert hasattr(feature_to_size_function, "__call__")
+    s = feature_to_size_function(number_of_features)
+
+    with plt.style.context(style):
+        _title_kws = {"fontsize":16, "fontweight":"bold"}; _title_kws.update(title_kws)
+        _xlabel_kws = {"fontsize":15}; _xlabel_kws.update(xlabel_kws)
+        _ylabel_kws = {"fontsize":15}; _ylabel_kws.update(ylabel_kws)
+        # _zlabel_kws = {"fontsize":15}; _zlabel_kws.update(zlabel_kws)
+
+        _xticklabel_kws = {"fontsize":12, "rotation":xtick_rotation}; _xticklabel_kws.update(xticklabel_kws)
+        _yticklabel_kws = {"fontsize":12}; _yticklabel_kws.update(yticklabel_kws)
+        # _zticklabel_kws = {"fontsize":12}; _zticklabel_kws.update(zticklabel_kws)
+
+        _legend_kws = {"fontsize":12, "frameon":True, "title_fontsize":"x-large"}; _legend_kws.update(legend_kws)
+        if ax is None:
+            fig, ax = plt.subplots(figsize=figsize)
+
+        else:
+            fig = plt.gcf()
+
+
+        # ax.scatter(xs=df["number_of_features"].values, ys=df["average_scores"].values, zs=df["validation_scores"], edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
+        ax.scatter(x=df["average_scores"].values, y=df["validation_scores"], s=s, edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
+
+
+        ax.set_xlabel(xlabel, **_xlabel_kws)
+        ax.set_ylabel(ylabel, **_ylabel_kws)
+        # ax.set_zlabel(zlabel, **_zlabel_kws)
+
+        # ax.set_yticklabels(map(lambda x:"%0.2f"%x, ax.get_yticks()), **_yticklabel_kws)
+        if title:
+            ax.set_title(title, **_title_kws)
+        if show_legend:
+            legendary_features = number_of_features.describe()[["25%", "50%", "75%", "max"]].astype(int)
+            
+            legend_elements = list()
+            for n in legendary_features.values:
+                marker = plt.Line2D([], [], color=color, marker='o', linestyle='None', markersize=feature_to_size_function(n), label="$N$ = %d"%(n))
+                legend_elements.append(marker)
+
+            legend = ax.legend(handles=legend_elements, markerscale=1,title="$N_{Features}$",  **_legend_kws)
+            
+        if show_xgrid:
+            ax.xaxis.grid(True)
+        if show_ygrid:
+            ax.yaxis.grid(True)
+        # if show_zgrid:
+        #     ax.zaxis.grid(True)
+        return fig, ax
 
 # -------
 # Classes
 # -------
 class ClairvoyanceBase(object):
     def __init__(
         self,
@@ -857,14 +1090,15 @@
         # Set attributes
         self.name = name
         self.observation_type = observation_type
         self.feature_type = feature_type
         self.target_type = target_type
         self.is_fitted_weights = False
         self.is_fitted_rci = False
+        self.validation_set_provided = False
         self.n_draws = n_draws
         self.n_jobs = n_jobs
         self.random_state = random_state
         if isinstance(scorer, str):
             scorer = get_scorer(scorer)
         self.scorer = scorer
         self.scorer_name = scorer._score_func.__name__
@@ -1106,15 +1340,15 @@
             assert y.dtype != float
             self.y_ = y.astype("category")
             self.classes_ = sorted(y.unique())
         self.observation_ids_ = X.index
         self.feature_ids_ = X.columns
         self.number_of_observations_, self.number_of_initial_features_ = X.shape
         self.stratify_ = format_stratify(stratify, estimator_type=self.estimator_type, y=self.y_)
-    
+
         # Checks
         if sort_hyperparameters_by is not None:
             assert isinstance(sort_hyperparameters_by, list), "`sort_hyperparameters_by` must be a list of size n accompanied by an `ascending` list of n boolean vaues"
             assert isinstance(ascending, list), "`sort_hyperparameters_by` must be a list of size n accompanied by an `ascending` list of n boolean vaues"
             assert len(sort_hyperparameters_by) == len(ascending), "`sort_hyperparameters_by` must be a list of size n accompanied by an `ascending` list of n boolean vaues"
             assert all(map(lambda x: isinstance(x, bool), ascending)), "`sort_hyperparameters_by` must be a list of size n accompanied by an `ascending` list of n boolean vaues"
             assert set(sort_hyperparameters_by) <= set(self.param_grid.keys()), "`sort_hyperparameters_by` must contain a list of keys in `param_grid`"
@@ -1181,30 +1415,34 @@
         df.columns.name = "metrics"
         return df.squeeze()
     
     
     def recursive_feature_inclusion(
         self, 
         estimator=None, 
-        X=None, 
-        y=None, 
+        X:pd.DataFrame=None, 
+        y:pd.Series=None, 
+        X_validation:pd.DataFrame=None,
+        y_validation:pd.Series=None,
         cv=(5,3), 
         minimum_score=None, 
         metric=np.mean, 
         early_stopping=25, 
         target_score=-np.inf, 
         minimum_improvement_in_score=0.0, 
         additional_feature_penalty=None,
         maximum_number_of_features=np.inf,
         less_features_is_better=True, 
         training_column="training_index", 
         testing_column="testing_index", 
         cv_prefix="cv=", 
         copy_X_rci=True,
         progress_message="Recursive feature inclusion",
+        # optimize_validation_score = "auto",
+
         ):
         assert self.is_fitted_weights, "Please `fit` model before proceeding."
 
         if X is None:
             X = self.X_.copy()
         else:
             assert set(X.columns) == set(self.X_.columns), "`X.columns` must be a subset `.feature_ids`"
@@ -1213,18 +1451,35 @@
             y = self.y_.copy()
         else:
             if self.estimator_type == "classifier":
                 assert set(y.unique()) <= set(self.classes_), "`y` must be a subset `.classes_ = {}`".format(self.classes_)
 
         if estimator is None:
             estimator = self.best_estimator_
-            
+
         self.clairvoyance_feature_weights_ = self.get_weights(minimum_score=minimum_score, metrics=metric).sort_values(ascending=False)
         self.rci_parameters_ = {"estimator":estimator, "cv":cv, "minimum_score":minimum_score, "metric":metric, "early_stopping":early_stopping, "target_score":target_score, "less_features_is_better":less_features_is_better}
         
+        # Validation
+        X_validation_is_provided = X_validation is not None
+        y_validation_is_provided = y_validation is not None
+
+        if X_validation_is_provided is not None:
+            assert y_validation_is_provided is not None, "If `X_validation` is provided then `y_validation` must be provided"
+
+        if y_validation_is_provided is not None:
+            assert X_validation_is_provided is not None, "If `y_validation` is provided then `X_validation` must be provided"
+
+        self.validation_set_provided = False
+        if all([X_validation_is_provided, y_validation_is_provided]):
+            assert np.all(X_validation.index == y_validation.index), "X_validation.index and y_validation.index must have the same ordering"
+            assert np.all(X_validation.columns == X.columns), "X_validation.columns and X.columns must have the same ordering"
+            self.validation_set_provided = True
+
+
         # Recursive feature incusion
         rci_results = recursive_feature_inclusion(
             estimator=estimator, 
             X=X, 
             y=y, 
             scorer=self.scorer,
             initial_feature_weights=self.clairvoyance_feature_weights_, 
@@ -1246,26 +1501,34 @@
             training_column=training_column, 
             testing_column=testing_column, 
             cv_prefix=cv_prefix,
             verbose=self.verbose,
             progress_message=progress_message,
             remove_zero_weighted_features=self.remove_zero_weighted_features,
             maximum_tries_to_remove_zero_weighted_features=self.maximum_tries_to_remove_zero_weighted_features,
+            X_validation=X_validation,
+            y_validation=y_validation,
+            # optimize_validation_score=optimize_validation_score,
             )
         
         # Results
+        # self.validation_scores_ = rci_results["validation_scores"]
         self.history_ = rci_results["history"]
         if self.remove_zero_weighted_features:
-            self.history_ = self.history_.sort_values([("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, less_features_is_better])
+            if self.validation_set_provided:
+                self.history_ = self.history_.sort_values([("summary", "validation_score"), ("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, False, less_features_is_better])
+            else:
+                self.history_ = self.history_.sort_values([("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, less_features_is_better])
         self.highest_score_ = rci_results["highest_score"]
         self.highest_scoring_features_ = rci_results["highest_scoring_features"]
         self.best_score_ = rci_results["best_score"]
         self.best_estimator_sem_ = rci_results["best_estimator_sem"]
         self.best_features_ = rci_results["best_features"]
         self.best_estimator_rci_ = clone(estimator)
+        self.best_estimator_validation_score_ = rci_results["best_estimator_validation_score"]
 
         X_rci = transform(X=X.loc[:,self.best_features_], method=self.transformation, multiplicative_replacement=self.multiplicative_replacement, axis=1)
         with warnings.catch_warnings(): #!
             warnings.filterwarnings("ignore", category=ConvergenceWarning)
             self.best_estimator_rci_.fit(X_rci, y)
         self.feature_weights_ =  rci_results["feature_weights"]
         self.rci_feature_weights_ = rci_results["feature_weights"][("full_dataset", "rci_weights")].loc[self.best_features_]
@@ -1290,32 +1553,39 @@
         assert self.is_fitted_rci, "Please run `recursive_feature_inclusion` before proceeding."
         if self.best_score_ < self.highest_score_:
             vertical_lines = [len(self.best_features_)-1, len(self.highest_scoring_features_)-1]
         else:
             vertical_lines = [len(self.best_features_)-1]
 
         if self.remove_zero_weighted_features:
-            return plot_recursive_feature_selection(number_of_features=self.history_[("summary", "number_of_features")], scores=self.history_[("summary", "average_score")],  **kwargs)
+            return plot_recursive_feature_selection(number_of_features=self.history_[("summary", "number_of_features")], average_scores=self.history_[("summary", "average_score")],  **kwargs)
         else:
-            return plot_scores_line(average_scores=self.history_[("summary", "average_score")], sem=self.history_[("summary", "sem")], vertical_lines=vertical_lines, **kwargs)
+            return plot_scores_line(average_scores=self.history_[("summary", "average_score")], sem=self.history_[("summary", "sem")], validation_scores=self.history_[("summary", "validation_score")], vertical_lines=vertical_lines, **kwargs)
         
     def plot_weights(
         self,
         weight_type=("full_dataset","rci_weights"),
         **kwargs,
         ):
         assert self.is_fitted_rci, "Please run `recursive_feature_inclusion` before proceeding."
         assert_acceptable_arguments(weight_type, {("full_dataset","rci_weights"), ("full_dataset","clairvoyance_weights"), "cross_validation"})
         
-        
         if weight_type in {("full_dataset","rci_weights"), ("full_dataset","clairvoyance_weights")}:
             fig, ax = plot_weights_bar(feature_weights=self.feature_weights_[weight_type], **kwargs)
         if weight_type == "cross_validation":
             fig, ax = plot_weights_box(feature_weights=self.feature_weights_[weight_type], **kwargs)
         return fig, ax
+    
+    def plot_scores_comparison(
+        self,
+        **kwargs,
+        ):
+        assert self.is_fitted_rci, "Please run `recursive_feature_inclusion` before proceeding."
+        assert self.validation_set_provided, "Please run `recursive_feature_inclusion` with a validation set before proceeding."
+        return plot_recursive_feature_selection(number_of_features=self.history_[("summary", "number_of_features")], average_scores=self.history_[("summary", "average_score")],   validation_scores=self.history_[("summary", "validation_score")], **kwargs)
 
     def copy(self):
         return copy.deepcopy(self)
     
     # def to_file(self, path:str):
     #     write_object(self, path)  
         
@@ -1470,15 +1740,14 @@
         random_state=0,
         n_jobs=1,
         
         # Recursive feature inclusion
         early_stopping=25, 
         minimum_improvement_in_score=0.0, 
         additional_feature_penalty=None,
-        maximum_number_of_features=np.inf,
 
         #Iterative
         percentiles=[0.0,0.1,0.2,0.3,0.4,0.5,0.6,0.7,0.8,0.9,0.925,0.95,0.975,0.99],
         minimum_scores=[-np.inf],
         
         # Compositional data transformations
         transformation=None,
@@ -1541,14 +1810,15 @@
         # Set attributes
         self.name = name
         self.observation_type = observation_type
         self.feature_type = feature_type
         self.target_type = target_type
         # self.is_fitted_weights = False
         self.is_fitted_rci = False
+        self.validation_set_provided = False
         self.n_draws = n_draws
         self.n_jobs = n_jobs
         self.random_state = random_state
         if isinstance(scorer, str):
             scorer = get_scorer(scorer)
         self.scorer = scorer
         self.scorer_name = scorer._score_func.__name__
@@ -1566,15 +1836,14 @@
             minimum_scores = [minimum_scores]
         if minimum_scores[0] != -np.inf:
             minimum_scores = [-np.inf] + minimum_scores
         self.minimum_scores = sorted(minimum_scores)  
         self.early_stopping = early_stopping
         self.minimum_improvement_in_score = minimum_improvement_in_score
         self.additional_feature_penalty = additional_feature_penalty
-        self.maximum_number_of_features = maximum_number_of_features
         self.verbose = verbose
         self.log = log
         self.remove_zero_weighted_features = remove_zero_weighted_features
         self.maximum_tries_to_remove_zero_weighted_features = maximum_tries_to_remove_zero_weighted_features
 
     def __repr__(self):
         pad = 4
@@ -1620,39 +1889,59 @@
 
         return "\n".join(fields)
     
     def fit(
         self, 
         X:pd.DataFrame, 
         y:pd.Series, 
+        X_validation:pd.DataFrame=None,
+        y_validation:pd.Series=None,
         stratify="auto", 
         split_size=0.618033, 
         cv=(5,3),
         training_column="training_index", 
         testing_column="testing_index", 
         cv_prefix="cv=",
         sort_hyperparameters_by:list=None, 
         ascending:list=None,
         less_features_is_better=True,
         remove_redundancy=True,
+        maximum_number_of_features="auto",
         ):
 
         assert np.all(X.index == y.index), "X.index and y.index must have the same ordering"
         self.X_initial_ = X.copy()
         self.y_ = y.copy()
         if self.estimator_type == "classifier":
             assert y.dtype != float
             self.y_ = y.astype("category")       
             self.classes_ = sorted(y.unique())
         self.observation_ids_ = X.index
         self.feature_ids_initial_ = X.columns
         self.number_of_observations_, self.number_of_initial_features_ = X.shape
         self.stratify_ = format_stratify(stratify, estimator_type=self.estimator_type, y=self.y_)
         self.split_size = split_size
+        self.maximum_number_of_features = maximum_number_of_features
 
+        # Validation
+        X_validation_is_provided = X_validation is not None
+        y_validation_is_provided = y_validation is not None
+
+        if X_validation_is_provided is not None:
+            assert y_validation_is_provided is not None, "If `X_validation` is provided then `y_validation` must be provided"
+
+        if y_validation_is_provided is not None:
+            assert X_validation_is_provided is not None, "If `y_validation` is provided then `X_validation` must be provided"
+
+        self.validation_set_provided = False
+        if all([X_validation_is_provided, y_validation_is_provided]):
+            assert np.all(X_validation.index == y_validation.index), "X_validation.index and y_validation.index must have the same ordering"
+            assert np.all(X_validation.columns == X.columns), "X_validation.columns and X.columns must have the same ordering"
+            self.validation_set_provided = True
+            
         # Get cross-validation splits
         self.cv_splits_, self.cv_labels_ = format_cross_validation(cv, X, self.y_, stratify=self.stratify_, random_state=self.random_state, cv_prefix=cv_prefix, training_column=training_column, testing_column=testing_column)
 
         self.history_ = OrderedDict()
         self.results_ = OrderedDict()
         self.results_baseline_ = OrderedDict()
 
@@ -1725,58 +2014,77 @@
                         with warnings.catch_warnings():
                             warnings.filterwarnings("ignore", category=ConvergenceWarning)
                             baseline_rci_weights = getattr(estimator.fit(X_query, self.y_), self.feature_weight_attribute)
                         if np.all(baseline_rci_weights == 0):
                             if self.verbose > 2:
                                 print("Excluding results from [percentile={}, estimator_params={}] becaue baseline model could not be fit with parameter set".format(pctl, params), file=self.log)
                         else:
+
+                            baseline_validation_score = np.nan
+                            if self.validation_set_provided:
+                                # Transform features (if transformation = None, then there is no transformation)
+                                X_validation_query = transform(X=X_validation.loc[:,current_features_for_percentile], method=self.transformation, multiplicative_replacement=self.multiplicative_replacement, axis=1)
+                                baseline_validation_score = self.scorer(estimator=estimator, X=X_validation_query, y_true=y_validation)
+
                             baseline_rci_weights = format_weights(baseline_rci_weights)
                             self.results_baseline_[(pctl,"baseline", params)] = {
-                                "score":np.nanmean(baseline_scores_for_percentile), 
+                                "validation_score":baseline_validation_score,
+                                "average_score":np.nanmean(baseline_scores_for_percentile), 
                                 "sem":stats.sem(baseline_scores_for_percentile),
                                 "number_of_features":X_query.shape[1], 
                                 "features":X_query.columns.tolist(), 
                                 "clairvoyance_weights":np.nan,
                                 "rci_weights":baseline_rci_weights, 
                                 "estimator":estimator,
-
                             }
 
                             # Minimum score thresholds
                             for s in sorted(feature_ordering_from_minimum_scores):
                                 progress_message = {True:"Recursive feature inclusion [percentile={}, estimator_params={}, minimum_score={}]".format(pctl, params, s), False:None}[self.verbose > 1]
-                                rci_history = model.recursive_feature_inclusion(
-                                    estimator=estimator, 
-                                    X=self.X_initial_.loc[:,current_features_for_percentile], 
-                                    y=self.y_, 
-                                    cv=self.cv_splits_, 
-                                    minimum_score=s, 
-                                    metric=np.mean, 
-                                    early_stopping=self.early_stopping, 
-                                    minimum_improvement_in_score=self.minimum_improvement_in_score, 
-                                    additional_feature_penalty=self.additional_feature_penalty,
-                                    maximum_number_of_features=self.maximum_number_of_features,
-                                    target_score=-np.inf, 
-                                    less_features_is_better=less_features_is_better, 
-                                    progress_message=progress_message,
+                                rci_params =  dict(
+                                        estimator=estimator, 
+                                        X=self.X_initial_.loc[:,current_features_for_percentile], 
+                                        y=self.y_, 
+                                        cv=self.cv_splits_, 
+                                        minimum_score=s, 
+                                        metric=np.mean, 
+                                        early_stopping=self.early_stopping, 
+                                        minimum_improvement_in_score=self.minimum_improvement_in_score, 
+                                        additional_feature_penalty=self.additional_feature_penalty,
+                                        maximum_number_of_features=self.maximum_number_of_features,
+                                        target_score=-np.inf, 
+                                        less_features_is_better=less_features_is_better, 
+                                        progress_message=progress_message,
                                 )
+                                if self.validation_set_provided:
+                                    rci_params.update(
+                                        dict(
+                                        X_validation=X_validation.loc[:,current_features_for_percentile],
+                                        y_validation=y_validation,
+                                        )
+                                    )
+
+                                rci_history = model.recursive_feature_inclusion(**rci_params)
+
+
 
                                 #!
                                 # Update weights if applicable
                                 if model.best_score_ > best_score_for_percentile:
                                     best_score_for_percentile = model.best_score_
                                     best_hyperparameters_for_percentile = params
                                     best_minimum_score_for_percentile = s
                                     best_clairvoyance_feature_weights_for_percentile = model.clairvoyance_feature_weights_.copy()
 
                                 # Store results
                                 rci_feature_weights = model.rci_feature_weights_[model.best_features_]
                                 if not np.any(rci_feature_weights.isnull()) and np.any(rci_feature_weights > 0):
                                     self.results_[(pctl, params, s)] = {
-                                        "score":model.best_score_, 
+                                        "validation_score":model.best_estimator_validation_score_,
+                                        "average_score":model.best_score_, 
                                         "sem":model.best_estimator_sem_,
                                         "number_of_features":len(model.best_features_), 
                                         "features":list(model.best_features_), 
                                         "clairvoyance_weights":model.clairvoyance_feature_weights_[model.best_features_].values.tolist(),
                                         "rci_weights":rci_feature_weights.values.tolist(), 
                                         "estimator":estimator,
                                     }
@@ -1799,64 +2107,110 @@
                         if self.verbose > 0:
                             print("Terminating algorithm. Last percentile has been processed.", file=self.log)
                 else:
                     if self.verbose > 0:
                         print("Terminating algorithm. Only 1 feature remains.", file=self.log)
                     break
 
-            self.results_ = pd.DataFrame(self.results_).T.sort_values(["score", "number_of_features", "sem"], ascending=[False,less_features_is_better, True])
+            self.results_ = pd.DataFrame(self.results_).T.sort_values(["validation_score", "average_score", "number_of_features", "sem"], ascending=[False, False,less_features_is_better, True])
             self.results_.index.names = ["percentile", "hyperparameters", "minimum_score"]
-            self.results_ = self.results_.loc[:,["score", "sem", "number_of_features", "features", "clairvoyance_weights", "rci_weights", "estimator"]]
+
+            self.results_ = self.results_.loc[:,["validation_score", "average_score", "sem", "number_of_features", "features", "clairvoyance_weights", "rci_weights", "estimator"]]
 
             # Dtypes
-            for field in ["score", "sem"]:
+            for field in ["validation_score", "average_score", "sem"]:
                 self.results_[field] = self.results_[field].astype(float)
             for field in ["number_of_features"]:
                 self.results_[field] = self.results_[field].astype(int)
 
             # Remove redundancy
             if remove_redundancy:
                 unique_results = set()
                 unique_index = list()
                 for idx, row in pv(self.results_.iterrows(), "Removing duplicate results", total=self.results_.shape[0]):
-                    id_unique = frozenset([row["score"], row["sem"], tuple(row["features"])])
+                    id_unique = frozenset([row["average_score"], row["sem"], tuple(row["features"])])
                     if id_unique not in unique_results:
                         unique_results.add(id_unique)
                         unique_index.append(idx)
                     else:
                         if self.verbose > 2:
                             print("Removing duplicate result: {}".format(id_unique), file=self.log)
                 self.results_ = self.results_.loc[unique_index]
             self.results_baseline_ = pd.DataFrame(self.results_baseline_).T
             self.results_baseline_.index.names = ["percentile", "hyperparameters", "minimum_score"]
 
             self.is_fitted_rci = True
             return self
 
+    def get_history(self, sort_values_by=[("summary", "validation_score"), ("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, False, True]):
+        assert self.is_fitted_rci, "Please run `fit` before proceeding."
+
+        dataframes = list()
+        for params, df in self.history_.items(): # self.history_[(pctl,params, s)] = rci_history
+            df.index = df.index.map(lambda x: (*params, x))
+            df.index.names = ["percentile", "hyperparameters", "minimum_score", "features"]
+            dataframes.append(df)
+
+        df_concatenated = pd.concat(dataframes, axis=0)
+        if sort_values_by is not None:
+            df_concatenated = df_concatenated.sort_values(by=sort_values_by, ascending=ascending)
+            
+        return df_concatenated
+
+
     def plot_recursive_feature_selection(
         self,
         ylabel="auto",
+        comprehensive = "auto",
         include_baseline=False,
         **kwargs,
         ):
         if ylabel == "auto":
             ylabel = self.scorer_name
         kwargs["ylabel"] = ylabel
         assert self.is_fitted_rci, "Please run `fit` before proceeding."
         
-        number_of_features = self.results_["number_of_features"]
-        scores = self.results_["score"]
-        if include_baseline:
-            number_of_features = pd.concat([number_of_features, self.results_baseline_["number_of_features"]])
-            scores = pd.concat([scores, self.results_baseline_["score"]])
+        if comprehensive == "auto":
+            if self.validation_set_provided:
+                comprehensive = True 
+            else:
+                comprehensive = False
+            
+        if comprehensive:
+            df = self.get_history()
+            number_of_features = df[("summary","number_of_features")]
+            average_scores = df[("summary", "average_score")]
+            # validation_scores = df[("summary", "validation_score")]
+        else:
+            number_of_features = self.results_["number_of_features"]
+            average_scores = self.results_["average_score"]
+            validation_scores = self.results_["validation_score"]
+            if include_baseline:
+                number_of_features = pd.concat([number_of_features, self.results_baseline_["number_of_features"]])
+                average_scores = pd.concat([average_scores, self.results_baseline_["average_score"]])
+                # validation_scores = pd.concat([validation_scores, self.results_baseline_["validation_score"]])
 
-        return plot_recursive_feature_selection(number_of_features=number_of_features, scores=scores,  **kwargs)
+        return plot_recursive_feature_selection(number_of_features=number_of_features, average_scores=average_scores,  **kwargs)
+
+    def plot_scores_comparison(
+        self,
+        **kwargs,
+        ):
+        assert self.is_fitted_rci, "Please run `recursive_feature_inclusion` before proceeding."
+        assert self.validation_set_provided, "Please run `recursive_feature_inclusion` with a validation set before proceeding."
+        df = self.get_history()
+        number_of_features = df[("summary","number_of_features")]
+        average_scores = df[("summary", "average_score")]
+        validation_scores = df[("summary", "validation_score")]
+        return plot_scores_comparison(number_of_features=number_of_features, average_scores=average_scores,   validation_scores=validation_scores, **kwargs)
 
     def to_file(self, path:str):
         write_object(self, path)  
+
+
         
     @classmethod
     def from_file(cls, path:str):
         cls = read_object(path)
         return cls
 
 def main():
@@ -1881,15 +2235,15 @@
             X.columns = X.columns.map(lambda j: j.split(" (cm")[0].replace(" ","_"))
 
             # Relabel targets
             target_names = load_iris().target_names
             y = y.map(lambda i: target_names[i])
 
             # Add 996 noise features (total = 1000 features) in the same range of values as the original features
-            number_of_noise_features = 996
+            number_of_noise_features = 46
             vmin = X.values.ravel().min()
             vmax = X.values.ravel().max()
             X_noise = pd.DataFrame(
                 data=np.random.RandomState(0).randint(low=int(vmin*10), high=int(vmax*10), size=(150, number_of_noise_features))/10,
                 columns=map(lambda j:"noise_{}".format(j+1), range(number_of_noise_features)),
             )
 
@@ -1915,40 +2269,44 @@
             )
             clf.fit(X_normalized, y)#, sort_hyperparameters_by=["C", "penalty"], ascending=[True, False])
             history = clf.recursive_feature_inclusion(early_stopping=10)
             print(history.head(), file=sys.stdout)
 
             # Regression
             print("\nRunning test for `ClairvoyanceRegression`", file=sys.stderr)
-            from sklearn.datasets import load_boston
+            # from sklearn.datasets import fetch_openml
             from sklearn.tree import DecisionTreeRegressor
             from sklearn.model_selection import train_test_split
 
-            # Load Boston data
-            boston = load_boston()
-            X = pd.DataFrame(boston.data, columns=boston.feature_names)
-            y = pd.Series(boston.target)
+            # Load housing data
+            # housing = fetch_openml(name="house_prices", as_frame=True)
+            data_url = "http://lib.stat.cmu.edu/datasets/boston"
+            raw_df = pd.read_csv(data_url, sep="\s+", skiprows=22, header=None)
+            data = np.hstack([raw_df.values[::2, :], raw_df.values[1::2, :2]])
+            target = raw_df.values[1::2, 2]
+            X = pd.DataFrame(data, columns=['CRIM', 'ZN', 'INDUS', 'CHAS', 'NOX', 'RM', 'AGE', 'DIS', 'RAD', 'TAX', 'PTRATIO', 'B', 'LSTAT'])
+            y = pd.Series(target)
 
-            number_of_noise_features = 100 - X.shape[1]
+            number_of_noise_features = 50 - X.shape[1]
             X_noise = pd.DataFrame(np.random.RandomState(0).normal(size=(X.shape[0], number_of_noise_features)),  columns=map(lambda j: f"noise_{j}", range(number_of_noise_features)))
-            X_boston_with_noise = pd.concat([X, X_noise], axis=1)
-            X_normalized = X_boston_with_noise - X_boston_with_noise.mean(axis=0).values
+            X_housing_with_noise = pd.concat([X, X_noise], axis=1)
+            X_normalized = X_housing_with_noise - X_housing_with_noise.mean(axis=0).values
             X_normalized = X_normalized/X_normalized.std(axis=0).values
 
             # Let's fit the model but leave a held out validation set
             X_training, X_validation, y_training, y_validation = train_test_split(X_normalized, y, random_state=0, test_size=0.1618)
 
             # Get parameters
             estimator = DecisionTreeRegressor(random_state=0)
             param_grid = {"min_samples_leaf":[1,2,3,5,8],"min_samples_split":{ 0.1618, 0.382, 0.5, 0.618}}
 
             # Fit model
-            reg = ClairvoyanceRegression(name="Boston", n_jobs=-1, n_draws=10, estimator=estimator, param_grid=param_grid, verbose=1)
+            reg = ClairvoyanceRegression(name="Housing", n_jobs=-1, n_draws=10, estimator=estimator, param_grid=param_grid, verbose=1)
             reg.fit(X_training, y_training)
-            history = reg.recursive_feature_inclusion(early_stopping=10, X=X_validation, y=y_validation)
+            history = reg.recursive_feature_inclusion(early_stopping=10, X=X_training, y=y_training, X_validation=X_validation, y_validation=y_validation)
             print(history.head(), file=sys.stdout)
 
             # Recursive
             print("\nRunning test for `ClairvoyanceRecursive`", file=sys.stderr)
             from sklearn.tree import DecisionTreeClassifier
 
             X_normalized = X_iris_with_noise - X_iris_with_noise.mean(axis=0).values
```

### Comparing `clairvoyance_feature_selection-2023.2.17/setup.py` & `clairvoyance_feature_selection-2023.6.9/setup.py`

 * *Files identical despite different names*


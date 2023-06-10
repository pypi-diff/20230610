# Comparing `tmp/clust-learn-0.2.0.7.tar.gz` & `tmp/clust-learn-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clust-learn-0.2.0.7.tar", last modified: Sat Jun 10 08:17:48 2023, max compression
+gzip compressed data, was "clust-learn-0.2.0b0.tar", last modified: Sat May 27 07:19:34 2023, max compression
```

## Comparing `clust-learn-0.2.0.7.tar` & `clust-learn-0.2.0b0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29234 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/clearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/clearn/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/classifier/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/classifier/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/clearn/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27697 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/clustering/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/clustering/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/clustering/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/clustering/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/clearn/data_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/data_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/data_preprocessing/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/data_preprocessing/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/clearn/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/dimensionality_reduction/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/dimensionality_reduction/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/dimensionality_reduction/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/dimensionality_reduction/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/clearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/clust_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29234 2023-06-10 08:17:48.000000 clust-learn-0.2.0.7/clust_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-10 08:17:48.000000 clust-learn-0.2.0.7/clust_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 08:17:48.000000 clust-learn-0.2.0.7/clust_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 08:17:48.000000 clust-learn-0.2.0.7/clust_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 08:17:48.000000 clust-learn-0.2.0.7/clust_learn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 08:17:48.374241 clust-learn-0.2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:48.370241 clust-learn-0.2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-10 08:17:34.000000 clust-learn-0.2.0.7/tests/test_clearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27503 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16269 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clust_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/tests/test_clearn.py
```

### Comparing `clust-learn-0.2.0.7/LICENSE` & `clust-learn-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/PKG-INFO` & `clust-learn-0.2.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.2.0.7
+Version: 0.2.0b0
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -104,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0.7
+* Version: 0.2.0b
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.2.0.7/README.md` & `clust-learn-0.2.0b0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0.7
+* Version: 0.2.0b
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.2.0.7/clearn/classifier/classifier.py` & `clust-learn-0.2.0b0/clearn/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/classifier/utils.py` & `clust-learn-0.2.0b0/clearn/classifier/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/classifier/viz_utils.py` & `clust-learn-0.2.0b0/clearn/classifier/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/clustering/clustering.py` & `clust-learn-0.2.0b0/clearn/clustering/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,57 +62,56 @@
             else:
                 raise RuntimeWarning(f'Algorithm {str(algorithm)} does not comply with scikit-learn standard')
 
         self.scores_ = dict()
         self._initialize_scores()
 
         self.metric_ = 'inertia'
-        self.labels_ = None
         self.optimal_config_ = None
         self.weights_ = None
 
     def _initialize_scores(self):
         for algorithm in self.algorithms:
             self.scores_[algorithm] = []
 
     def _compute_clusters(self, algorithm, n_clusters, weights=None):
-        n_clusters_param_name = get_n_clusters_param_name(self.instances_[algorithm])
-        self.instances_[algorithm].set_params(**{n_clusters_param_name: n_clusters})
-        if accepts_param(self.instances_[algorithm].fit_predict, 'sample_weight'):
-            self.labels_ = self.instances_[algorithm].fit_predict(self.df[self.dimensions_], sample_weight=weights)
+        self.instances_[algorithm].set_params(n_clusters=n_clusters)
+        if accepts_param(self.instances_[algorithm].fit, 'sample_weight'):
+            self.instances_[algorithm].fit(self.df[self.dimensions_], sample_weight=weights)
         else:
-            self.labels_ = self.instances_[algorithm].fit_predict(self.df[self.dimensions_])
+            self.instances_[algorithm].fit(self.df[self.dimensions_])
+        self.labels_ = self.instances_[algorithm].labels_
 
     def _compute_optimal_clustering_config(self, metric, cluster_range, weights=None):
         optimal_list = []
         for algorithm in self.algorithms:
-            n_clusters_param_name = get_n_clusters_param_name(self.instances_[algorithm])
             for nc in range(*cluster_range):
-                self.instances_[algorithm].set_params(**{n_clusters_param_name: nc})
-
-                local_labels = None
-                if accepts_param(self.instances_[algorithm].fit_predict, 'sample_weight'):
-                    local_labels = self.instances_[algorithm].fit_predict(self.df[self.dimensions_],
-                                                                          sample_weight=weights)
+                self.instances_[algorithm].set_params(n_clusters=nc)
+                if accepts_param(self.instances_[algorithm].fit, 'sample_weight'):
+                    self.instances_[algorithm].fit(self.df[self.dimensions_], sample_weight=weights)
                 else:
-                    local_labels = self.instances_[algorithm].fit_predict(self.df[self.dimensions_])
+                    self.instances_[algorithm].fit(self.df[self.dimensions_])
 
                 if metric == 'inertia':
                     self.scores_[algorithm].append(
-                        weighted_sum_of_squared_distances(self.df[self.dimensions_], local_labels, weights))
+                        weighted_sum_of_squared_distances(self.df[self.dimensions_], self.instances_[algorithm].labels_,
+                                                          weights))
                 elif metric == 'davies_bouldin_score':
                     self.scores_[algorithm].append(
-                        1 if nc == 1 else davies_bouldin_score(self.df[self.dimensions_], local_labels))
+                        1 if nc == 1 else davies_bouldin_score(self.df[self.dimensions_],
+                                                               self.instances_[algorithm].labels_))
                 elif metric == 'silhouette_score':
                     self.scores_[algorithm].append(
-                        0 if nc == 1 else silhouette_score(self.df[self.dimensions_], local_labels))
+                        0 if nc == 1 else silhouette_score(self.df[self.dimensions_],
+                                                           self.instances_[algorithm].labels_))
 
                 elif metric == 'calinski_harabasz_score':
                     self.scores_[algorithm].append(
-                        1 if nc == 1 else calinski_harabasz_score(self.df[self.dimensions_], local_labels))
+                        1 if nc == 1 else calinski_harabasz_score(self.df[self.dimensions_],
+                                                                  self.instances_[algorithm].labels_))
 
             if len(range(*cluster_range)) > 1:
                 kl = KneeLocator(x=range(*cluster_range), y=self.scores_[algorithm], curve='convex',
                                  direction='decreasing')
                 optimal_list.append((algorithm, kl.knee, self.scores_[algorithm][kl.knee-cluster_range[0]]))
             else:
                 optimal_list.append((algorithm, cluster_range[0], self.scores_[algorithm][0]))
@@ -228,16 +227,14 @@
             variables.remove('cluster')
 
         if cluster_filter is None:
             cluster_filter = list(df_ext['cluster'].unique())
         if not isinstance(cluster_filter, list):
             cluster_filter = [cluster_filter]
 
-        if not isinstance(statistics, list):
-            statistics = [statistics]
         if 'wmean' in statistics:
             def wmean(x): return weighted_mean(x, self.weights_[x.index])
             statistics[statistics.index('wmean')] = wmean
         if 'wstd' in statistics:
             def wstd(x): return weighted_std(x, self.weights_[x.index])
             statistics[statistics.index('wstd')] = wstd
 
@@ -392,15 +389,15 @@
             The order of the observations must be the same as that of the base DataFrame.
 
         Returns
         ----------
         dict : dictionary
             Dictionary with the corresponding test statistics.
         """
-        contingency_t = self.describe_clusters_cat(cat_array, '')
+        contingency_t = self.describe_clusters_cat(cat_array)
         test_res = chi2_contingency(contingency_t.values)
         return dict(zip(['chi2', 'p', 'dof'], test_res[:-1]))
 
     def plot_score_comparison(self, output_path=None, savefig_kws=None):
         """
         Plots the comparison in performance between the different clustering algorithms.
 
@@ -449,17 +446,20 @@
         use_weights: bool
             Whether to use sample weights.
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
-        plot_clustercount(self.df, self.weights_, output_path, savefig_kws)
+        if use_weights:
+            plot_clustercount(self.df, self.weights_, output_path, savefig_kws)
+        else:
+            plot_clustercount(self.df, output_path, savefig_kws)
 
-    def plot_cluster_means_to_global_means_comparison(self, use_weights=False, df_original=None, xlabel=None, ylabel=None,
+    def plot_cluster_means_to_global_means_comparison(self, use_weights= False, df_original=None, xlabel=None, ylabel=None,
                                                       levels=[-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50],
                                                       output_path=None, savefig_kws=None):
         """
         Plots the normalized curve used for computing the optimal number of clusters.
 
         Parameters
         ----------
@@ -575,30 +575,28 @@
         hue = 'cluster_cat'
         weights = None
         if use_weights:
             weights = self.weights_
         plot_clusters_2D(coor1, coor2, hue, df_ext, weights, style_kwargs=style_kwargs, output_path=output_path,
                          savefig_kws=savefig_kws)
 
-    def plot_cat_distribution_by_cluster(self, cat_array, cat_label, cluster_label=None, use_weights=False,
-                                         output_path=None, savefig_kws=None):
+    def plot_cat_distribution_by_cluster(self, cat_array, cat_label=None, cluster_label=None, output_path=None,
+                                         savefig_kws=None):
         """
         Plots the relative contingency table of the clusters with a categorical variable as a stacked bar plot.
 
         Parameters
         ----------
         cat_array : `numpy.array` or list
             Array with categorical values.
             *Note its length must be the same as self.df and observations be in the same order*.
         cat_label : str, default=None
             Name/Description of the categorical variable to be displayed.
         cluster_label : str, default=None
             Name/Description of the cluster variable to be displayed.
-        use_weights : bool, default=False
-            Whether to use weights for centroid comparison.
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
-        ct = self.describe_clusters_cat(cat_array, cat_label, normalize=True, use_weights=use_weights)
+        ct = self.describe_clusters_cat(cat_array, normalize=True)
         plot_cat_distribution_by_cluster(ct, cat_label, cluster_label, output_path, savefig_kws)
```

### Comparing `clust-learn-0.2.0.7/clearn/clustering/table_utils.py` & `clust-learn-0.2.0b0/clearn/clustering/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/clustering/utils.py` & `clust-learn-0.2.0b0/clearn/clustering/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,23 +78,13 @@
     """
     average = np.average(data, weights=weights)
     variance = np.average((data-average)**2, weights=weights)
     return np.sqrt(variance)
 
 
 def is_sklearn_compatible(algorithm):
-    return 'fit_predict' in dir(algorithm) and 'set_params' in dir(algorithm)
+    return 'fit' in dir(algorithm) and 'set_params' in dir(algorithm)
 
 
 def accepts_param(function, param):
     args, varargs, varkw, defaults, kwonlyargs, kwonlydefaults, annotations = inspect.getfullargspec(function)
     return param in args
-
-
-def get_n_clusters_param_name(algorithm):
-    param_list = list(algorithm.get_params().keys())
-    if 'n_clusters' in param_list:
-        return 'n_clusters'
-    elif 'n_components' in param_list:
-        return 'n_components'
-    else:
-        return None
```

### Comparing `clust-learn-0.2.0.7/clearn/clustering/viz_utils.py` & `clust-learn-0.2.0b0/clearn/clustering/viz_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         If data are standardized, comparison to global mean is based solely on the mean per cluster.
     output_path : str, default=None
         Path to save figure as image.
     savefig_kws : dict, default=None
         Save figure options.
     """
     df_diff = compare_cluster_means_to_global_means(df, dimensions, weights, data_standardized=data_standardized)
-    colors = sns.color_palette("BrBG", n_colors=len(levels)+1)
+    colors = sns.color_palette("BrBG", n_colors=9)
     cmap, norm = matplotlib.colors.from_levels_and_colors(levels, colors, extend="both")
     width = min(len(dimensions), 20)
     height = min(df['cluster'].nunique(), 8)
     fig, ax = plt.subplots(figsize=(width, height))
     im = ax.imshow(df_diff[dimensions].values, cmap=cmap, norm=norm)
     ax.set(xticks=range(len(dimensions)), yticks=range(df_diff.shape[0]),
            xticklabels=list(map(str.upper, dimensions)), yticklabels=df_diff['cluster'])
@@ -317,15 +317,15 @@
         agg_method = wmean
     scatter_df = df.groupby(hue).agg(dict(zip([x, y], [agg_method] * 2))).reset_index()
 
     sns.scatterplot(x=x, y=y, hue=hue, data=scatter_df,
                     alpha=1, palette=palette, linewidth=0, marker='X', s=100, ax=axs[1])
 
     if kdeplot:
-        hue_order = np.sort(df[hue].unique())
+        hue_order = np.sort(df[hue].values)
         sns.kdeplot(x=x, y=y, hue=hue, data=df, levels=1, alpha=0.2, palette=palette,
                     weights=weights, hue_order=hue_order, ax=axs[1])
 
     axs[1].vlines(xmean, ymin=ymin, ymax=ymax, color=vline_color, linewidth=1, linestyles='--', label=xmean_label)
     axs[1].hlines(ymean, xmin=xmin, xmax=xmax, color=hline_color, linewidth=1, linestyles='--', label=ymean_label)
     axs[1].set_xlabel(x, fontsize=12)
     axs[1].set_ylabel(y, fontsize=12)
```

### Comparing `clust-learn-0.2.0.7/clearn/data_preprocessing/__init__.py` & `clust-learn-0.2.0b0/clearn/data_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/data_preprocessing/data_preprocessing.py` & `clust-learn-0.2.0b0/clearn/data_preprocessing/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/data_preprocessing/viz_utils.py` & `clust-learn-0.2.0b0/clearn/data_preprocessing/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/dimensionality_reduction/dimensionality_reduction.py` & `clust-learn-0.2.0b0/clearn/dimensionality_reduction/dimensionality_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Dimensionality Reduction with PCA as reference"""
 # Author: Miguel Alvarez-Garcia
 
-import numpy as np
 import prince
 
 from sklearn.decomposition import PCA, SparsePCA
 from sklearn.preprocessing import StandardScaler
 from .table_utils import *
-from .utils import *
 from .viz_utils import *
 
 
 class DimensionalityReduction:
     """
     Dimensionality Reduction class
 
@@ -170,18 +168,18 @@
         trans.columns = [f'dim_{str(i+1).zfill(idx_positions)}' for i in range(trans.shape[1])]
         return trans
 
     def _transform_cat(self, df, n_components_cat=None):
         self.cat_model.set_params(n_components=df.nunique().sum())
         self.cat_model.fit(df.astype(str))
 
-        explained_variance_ratio = self._get_explained_variance_ratio()
+        explained_variance_ratio = self.cat_model.explained_inertia_ / self.cat_model.explained_inertia_.sum()
         if n_components_cat is None and self.min_explained_variance_ratio_ is None:
             # Optimal number
-            kl = KneeLocator(x=range(1, df.nunique().sum()),
+            kl = KneeLocator(x=range(1, df.nunique().sum() + 1),
                              y=explained_variance_ratio,
                              curve='convex',
                              direction='decreasing')
             n_components_cat = np.maximum(kl.knee-1, 1)
 
         elif n_components_cat is None:
             # Based on explained variance
@@ -190,20 +188,14 @@
 
         trans = self.cat_model.transform(df.astype(str))
         trans = trans[trans.columns[:n_components_cat]]
         idx_positions = np.maximum(2, len(str(n_components_cat)))
         trans.columns = [f'dim_{str(i+1).zfill(idx_positions)}' for i in range(n_components_cat)]
         return trans
 
-    # We need to (temporarily) do this manually because prince is no longer applying these corrections with MCA
-    def _get_explained_variance_ratio(self):
-        benzecri_eigenvalues = apply_benzecri_eigenvalue_correction(self.cat_model.eigenvalues_, self.cat_model.K_)
-        greenacre_inertia = compute_greenacre_inertia(self.cat_model.eigenvalues_, self.cat_model.K_, self.cat_model.J_)
-        return benzecri_eigenvalues / greenacre_inertia
-
     def num_main_contributors(self, thres=0.5, n_contributors=None, dim_idx=None, component_description=None,
                               col_description=None, output_path=None):
         """
         Computes the original numerical variables with the strongest relation to the derived variable(s)
         (measured as Pearson correlation coefficient)
 
         Parameters
@@ -323,15 +315,15 @@
         plots : str or list, default='all'
             The following plots are supported: ['cumulative', 'ratio', 'normalized']
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
-        explained_variance_ratio = self._get_explained_variance_ratio()
+        explained_variance_ratio = self.cat_model.explained_inertia_ / self.cat_model.explained_inertia_.sum()
         plot_explained_variance(explained_variance_ratio, thres, plots, output_path, savefig_kws)
 
     def plot_num_main_contributors(self, thres=0.5, n_contributors=5, dim_idx=None, output_path=None, savefig_kws=None):
         """
         Plot main contributors (original variables with the strongest relation with derived variables) for
         every derived variable
```

### Comparing `clust-learn-0.2.0.7/clearn/dimensionality_reduction/table_utils.py` & `clust-learn-0.2.0b0/clearn/dimensionality_reduction/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clearn/dimensionality_reduction/viz_utils.py` & `clust-learn-0.2.0b0/clearn/dimensionality_reduction/viz_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
     j = 0
     for idx, row in mc.iterrows():
         var_name = row['var_name']
         nvalues = df[var_name].nunique()
 
         i = 0
         ax0 = None
-        for v in np.sort(df[var_name].unique()):
+        for v in df[var_name].unique():
             ax = fig.add_subplot(gs[i:i + int(nrows / nvalues), j], sharex=ax0, sharey=ax0)
             sns.kdeplot(data=df[df[var_name] == v], x=dim_name, color='blue', fill=True, ax=ax)
             ax.set_title(f'{var_name} = {v}', fontsize=10)
             ax.set_ylabel('')
 
             i += int(nrows / nvalues)
             if i < nrows:
```

### Comparing `clust-learn-0.2.0.7/clearn/utils.py` & `clust-learn-0.2.0b0/clearn/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0.7/clust_learn.egg-info/PKG-INFO` & `clust-learn-0.2.0b0/clust_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.2.0.7
+Version: 0.2.0b0
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -104,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0.7
+* Version: 0.2.0b
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.2.0.7/clust_learn.egg-info/SOURCES.txt` & `clust-learn-0.2.0b0/clust_learn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 clearn/clustering/viz_utils.py
 clearn/data_preprocessing/__init__.py
 clearn/data_preprocessing/data_preprocessing.py
 clearn/data_preprocessing/viz_utils.py
 clearn/dimensionality_reduction/__init__.py
 clearn/dimensionality_reduction/dimensionality_reduction.py
 clearn/dimensionality_reduction/table_utils.py
-clearn/dimensionality_reduction/utils.py
 clearn/dimensionality_reduction/viz_utils.py
 clust_learn.egg-info/PKG-INFO
 clust_learn.egg-info/SOURCES.txt
 clust_learn.egg-info/dependency_links.txt
 clust_learn.egg-info/requires.txt
 clust_learn.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `clust-learn-0.2.0.7/pyproject.toml` & `clust-learn-0.2.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clust-learn"
-version = "0.2.0.7"
+version = "0.2.0b"
 authors = [
   { name="Miguel Alvarez-Garcia", email="malvarez.statistics@gmail.com" },
 ]
 description = "A Python package for explainable cluster analysis"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `clust-learn-0.2.0.7/setup.py` & `clust-learn-0.2.0b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(os.path.join(ROOT, 'README.md')) as f:
     README = f.read()
 
 
 setup(
     name='clust-learn',
-    version="0.2.0.7",
+    version="0.2.0b",
     description="A Python package for explainable cluster analysis",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra",
     author_email="@gmail.com",
     url="https://github.com/malgar/clust-learn",
     packages=find_packages(),
@@ -27,17 +27,17 @@
     ],
     license='GPLv3',
     install_requires=[
         "kneed>=0.7.0",
         "matplotlib>=3.4.3",
         "networkx>=2.6.3",
         "numpy>=1.20.3",
-        "pandas>=1.3.4,<2.0",
-        "pingouin>=0.5.3",
-        "prince==0.10.4",
+        "pandas>=1.3.4",
+        "pingouin>=0.5.1",
+        "prince==0.7.0",
         "scikit-learn>=1.0.2",
         "scipy>=1.7.1",
         "seaborn>=0.11.2",
         "shap>=0.40.0",
         "statsmodels>=0.13.2",
         "xgboost>=1.5.2"
     ],
```


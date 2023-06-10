# Comparing `tmp/clust-learn-0.2.0b0.tar.gz` & `tmp/clust-learn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clust-learn-0.2.0b0.tar", last modified: Sat May 27 07:19:34 2023, max compression
+gzip compressed data, was "clust-learn-0.2.1.tar", last modified: Sat Jun 10 17:05:44 2023, max compression
```

## Comparing `clust-learn-0.2.0b0.tar` & `clust-learn-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27503 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16269 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/data_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clust_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/tests/test_clearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.246119 clust-learn-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-10 17:05:27.000000 clust-learn-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29327 2023-06-10 17:05:44.246119 clust-learn-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28474 2023-06-10 17:05:27.000000 clust-learn-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.238119 clust-learn-0.2.1/clearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.238119 clust-learn-0.2.1/clearn/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/classifier/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/classifier/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.242119 clust-learn-0.2.1/clearn/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27697 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/clustering/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/clustering/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/clustering/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/clustering/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.242119 clust-learn-0.2.1/clearn/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/data_preprocessing/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/data_preprocessing/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.242119 clust-learn-0.2.1/clearn/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/dimensionality_reduction/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/dimensionality_reduction/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/dimensionality_reduction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/dimensionality_reduction/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-10 17:05:27.000000 clust-learn-0.2.1/clearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.246119 clust-learn-0.2.1/clust_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29327 2023-06-10 17:05:44.000000 clust-learn-0.2.1/clust_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-10 17:05:44.000000 clust-learn-0.2.1/clust_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 17:05:44.000000 clust-learn-0.2.1/clust_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 17:05:44.000000 clust-learn-0.2.1/clust_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 17:05:44.000000 clust-learn-0.2.1/clust_learn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-10 17:05:27.000000 clust-learn-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 17:05:44.246119 clust-learn-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-10 17:05:27.000000 clust-learn-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:44.246119 clust-learn-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 17:05:27.000000 clust-learn-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-10 17:05:27.000000 clust-learn-0.2.1/tests/test_clearn.py
```

### Comparing `clust-learn-0.2.0b0/LICENSE` & `clust-learn-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/PKG-INFO` & `clust-learn-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.2.0b0
+Version: 0.2.1
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -77,15 +77,15 @@
 
 **Figue 1** shows the package layout with the functionalities covered by each module along with the techniques used, the
 explainability strategies available, and the main functions and class methods encapsulating these techniques and
 explainability strategies.
 
 <br/>
 
-![clust-learn package structure](https://github.com/malgar/clust-learn/blob/v0.0.8/images/package_structure.png?raw=true)
+![clust-learn package structure](https://github.com/malgar/clust-learn/blob/master/images/package_structure.png?raw=true)
 
 <br/>
 
 <h2 id="user-content-implementation">
 3. Implementation
 </h2>
 
@@ -104,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0b
+* Version: 0.2.1
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
 
@@ -409,15 +409,15 @@
 ```
 cl = Clustering(df, algorithms='kmeans', normalize=False)
 ```
 
 | Parameter | Type | Description |
 |:-|:-|:-|
 | `df` | `pandas.DataFrame` | Data frame containing the data to be clustered |
-| `algorithms` | `string` or `list` | Algorithms to be used for clustering. The current version supports k-means and agglomerative clustering |
+| `algorithms` | instance or `list` of instances | Algorithm instances to be used for clustering. They must implement the `fit` and `set_params` methods |
 | `normalize` | `bool` | Whether to apply data normalization for fair comparisons between variables. In case dimensionality reduction is applied beforehand, normalization should not be applied |
 | **Attribute** | **Type** | **Description** |
 | `dimensions_` | `list` | List of columns of they input data frame |
 | `instances_` | `dict` | Pairs of algorithm name and its instance |
 | `metric_` | `string` | The cluster validation metric used. Four metrics available: ['inertia', 'davies_bouldin_score', 'silhouette_score',  'calinski_harabasz_score'] |
 | `optimal_config_` | `tuple` | Tuple with the optimal configuration for clustering containing the algorithm name, number of clusters, and value of the chosen validation metric |
 | `scores_` | `dict` | Pairs of algorithm name and a list of values of the chosen validation metric for a cluster range |
@@ -457,15 +457,15 @@
 <h4 id="describe_clusters_cat">
 describe_clusters_cat()
 </h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L237)
 
 ```
-describe_clusters_cat(self, cat_array, cat_name=None, order=None, normalize=False, output_path=None)
+describe_clusters_cat(self, cat_array, cat_name, order=None, normalize=False, use_weights=False, output_path=None)
 ```
 
 Describes clusters based on  external *categorical* variables. The result is a contingency table.
 For continuous variables use [`describe_clusters()`](#describe_clusters).
 
 <h4>compare_cluster_means_to_global_means()</h4>
 
@@ -519,25 +519,25 @@
 Plots the normalized curve used for computing the optimal number of clusters.
 
 <h4>plot_clustercount()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L419)
 
 ```
-plot_clustercount(self, output_path=None, savefig_kws=None)
+plot_clustercount(self, use_weights=False, output_path=None, savefig_kws=None)
 ```
 
 Plots a bar plot with cluster counts.
 
 <h4>plot_cluster_means_to_global_means_comparison()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L432)
 
 ```
-plot_cluster_means_to_global_means_comparison(self, df_original=None, xlabel=None, ylabel=None,
+plot_cluster_means_to_global_means_comparison(self, use_weights= False, df_original=None, xlabel=None, ylabel=None,
                                               levels=[-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50],
                                               output_path=None, savefig_kws=None)
 ```
 
 Plots the normalized curve used for computing the optimal number of clusters.
 
 <h4>plot_distribution_comparison_by_cluster()</h4>
@@ -551,27 +551,27 @@
 Plots the violin plots per cluster and *continuous* variables of interest to understand differences in their distributions by cluster.
 
 <h4>plot_clusters_2D()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L498)
 
 ```
-plot_clusters_2D(self, coor1, coor2, style_kwargs=dict(), output_path=None, savefig_kws=None)
+plot_clusters_2D(self, coor1, coor2, use_weights=False, style_kwargs=dict(), output_path=None, savefig_kws=None)
 ```
 
 Plots two 2D plots:
 	 - A scatter plot styled by the categorical variable `hue`.
 	 - A 2D plot comparing cluster centroids and optionally the density area.
 	 
 <h4>plot_cat_distribution_by_cluster()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L545)
 
 ```
-plot_cat_distribution_by_cluster(self, cat_array, cat_label=None, cluster_label=None, output_path=None, savefig_kws=None)
+plot_cat_distribution_by_cluster(self, cat_array, cat_label, cluster_label=None, use_weights=False, output_path=None, savefig_kws=None)
 ```
 
 Plots the relative contingency table of the clusters with a categorical variable as a stacked bar plot.
 
 <h3 id="user-content-module-classifier">
 7.iv. Classifier
 </h3>
```

### Comparing `clust-learn-0.2.0b0/README.md` & `clust-learn-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 **Figue 1** shows the package layout with the functionalities covered by each module along with the techniques used, the
 explainability strategies available, and the main functions and class methods encapsulating these techniques and
 explainability strategies.
 
 <br/>
 
-![clust-learn package structure](https://github.com/malgar/clust-learn/blob/v0.0.8/images/package_structure.png?raw=true)
+![clust-learn package structure](https://github.com/malgar/clust-learn/blob/master/images/package_structure.png?raw=true)
 
 <br/>
 
 <h2 id="user-content-implementation">
 3. Implementation
 </h2>
 
@@ -84,15 +84,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0b
+* Version: 0.2.1
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
 
@@ -389,15 +389,15 @@
 ```
 cl = Clustering(df, algorithms='kmeans', normalize=False)
 ```
 
 | Parameter | Type | Description |
 |:-|:-|:-|
 | `df` | `pandas.DataFrame` | Data frame containing the data to be clustered |
-| `algorithms` | `string` or `list` | Algorithms to be used for clustering. The current version supports k-means and agglomerative clustering |
+| `algorithms` | instance or `list` of instances | Algorithm instances to be used for clustering. They must implement the `fit` and `set_params` methods |
 | `normalize` | `bool` | Whether to apply data normalization for fair comparisons between variables. In case dimensionality reduction is applied beforehand, normalization should not be applied |
 | **Attribute** | **Type** | **Description** |
 | `dimensions_` | `list` | List of columns of they input data frame |
 | `instances_` | `dict` | Pairs of algorithm name and its instance |
 | `metric_` | `string` | The cluster validation metric used. Four metrics available: ['inertia', 'davies_bouldin_score', 'silhouette_score',  'calinski_harabasz_score'] |
 | `optimal_config_` | `tuple` | Tuple with the optimal configuration for clustering containing the algorithm name, number of clusters, and value of the chosen validation metric |
 | `scores_` | `dict` | Pairs of algorithm name and a list of values of the chosen validation metric for a cluster range |
@@ -437,15 +437,15 @@
 <h4 id="describe_clusters_cat">
 describe_clusters_cat()
 </h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L237)
 
 ```
-describe_clusters_cat(self, cat_array, cat_name=None, order=None, normalize=False, output_path=None)
+describe_clusters_cat(self, cat_array, cat_name, order=None, normalize=False, use_weights=False, output_path=None)
 ```
 
 Describes clusters based on  external *categorical* variables. The result is a contingency table.
 For continuous variables use [`describe_clusters()`](#describe_clusters).
 
 <h4>compare_cluster_means_to_global_means()</h4>
 
@@ -499,25 +499,25 @@
 Plots the normalized curve used for computing the optimal number of clusters.
 
 <h4>plot_clustercount()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L419)
 
 ```
-plot_clustercount(self, output_path=None, savefig_kws=None)
+plot_clustercount(self, use_weights=False, output_path=None, savefig_kws=None)
 ```
 
 Plots a bar plot with cluster counts.
 
 <h4>plot_cluster_means_to_global_means_comparison()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L432)
 
 ```
-plot_cluster_means_to_global_means_comparison(self, df_original=None, xlabel=None, ylabel=None,
+plot_cluster_means_to_global_means_comparison(self, use_weights= False, df_original=None, xlabel=None, ylabel=None,
                                               levels=[-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50],
                                               output_path=None, savefig_kws=None)
 ```
 
 Plots the normalized curve used for computing the optimal number of clusters.
 
 <h4>plot_distribution_comparison_by_cluster()</h4>
@@ -531,27 +531,27 @@
 Plots the violin plots per cluster and *continuous* variables of interest to understand differences in their distributions by cluster.
 
 <h4>plot_clusters_2D()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L498)
 
 ```
-plot_clusters_2D(self, coor1, coor2, style_kwargs=dict(), output_path=None, savefig_kws=None)
+plot_clusters_2D(self, coor1, coor2, use_weights=False, style_kwargs=dict(), output_path=None, savefig_kws=None)
 ```
 
 Plots two 2D plots:
 	 - A scatter plot styled by the categorical variable `hue`.
 	 - A 2D plot comparing cluster centroids and optionally the density area.
 	 
 <h4>plot_cat_distribution_by_cluster()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L545)
 
 ```
-plot_cat_distribution_by_cluster(self, cat_array, cat_label=None, cluster_label=None, output_path=None, savefig_kws=None)
+plot_cat_distribution_by_cluster(self, cat_array, cat_label, cluster_label=None, use_weights=False, output_path=None, savefig_kws=None)
 ```
 
 Plots the relative contingency table of the clusters with a categorical variable as a stacked bar plot.
 
 <h3 id="user-content-module-classifier">
 7.iv. Classifier
 </h3>
```

### Comparing `clust-learn-0.2.0b0/clearn/classifier/classifier.py` & `clust-learn-0.2.1/clearn/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clearn/classifier/utils.py` & `clust-learn-0.2.1/clearn/classifier/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clearn/classifier/viz_utils.py` & `clust-learn-0.2.1/clearn/classifier/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clearn/clustering/clustering.py` & `clust-learn-0.2.1/clearn/clustering/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,56 +62,57 @@
             else:
                 raise RuntimeWarning(f'Algorithm {str(algorithm)} does not comply with scikit-learn standard')
 
         self.scores_ = dict()
         self._initialize_scores()
 
         self.metric_ = 'inertia'
+        self.labels_ = None
         self.optimal_config_ = None
         self.weights_ = None
 
     def _initialize_scores(self):
         for algorithm in self.algorithms:
             self.scores_[algorithm] = []
 
     def _compute_clusters(self, algorithm, n_clusters, weights=None):
-        self.instances_[algorithm].set_params(n_clusters=n_clusters)
-        if accepts_param(self.instances_[algorithm].fit, 'sample_weight'):
-            self.instances_[algorithm].fit(self.df[self.dimensions_], sample_weight=weights)
+        n_clusters_param_name = get_n_clusters_param_name(self.instances_[algorithm])
+        self.instances_[algorithm].set_params(**{n_clusters_param_name: n_clusters})
+        if accepts_param(self.instances_[algorithm].fit_predict, 'sample_weight'):
+            self.labels_ = self.instances_[algorithm].fit_predict(self.df[self.dimensions_], sample_weight=weights)
         else:
-            self.instances_[algorithm].fit(self.df[self.dimensions_])
-        self.labels_ = self.instances_[algorithm].labels_
+            self.labels_ = self.instances_[algorithm].fit_predict(self.df[self.dimensions_])
 
     def _compute_optimal_clustering_config(self, metric, cluster_range, weights=None):
         optimal_list = []
         for algorithm in self.algorithms:
+            n_clusters_param_name = get_n_clusters_param_name(self.instances_[algorithm])
             for nc in range(*cluster_range):
-                self.instances_[algorithm].set_params(n_clusters=nc)
-                if accepts_param(self.instances_[algorithm].fit, 'sample_weight'):
-                    self.instances_[algorithm].fit(self.df[self.dimensions_], sample_weight=weights)
+                self.instances_[algorithm].set_params(**{n_clusters_param_name: nc})
+
+                local_labels = None
+                if accepts_param(self.instances_[algorithm].fit_predict, 'sample_weight'):
+                    local_labels = self.instances_[algorithm].fit_predict(self.df[self.dimensions_],
+                                                                          sample_weight=weights)
                 else:
-                    self.instances_[algorithm].fit(self.df[self.dimensions_])
+                    local_labels = self.instances_[algorithm].fit_predict(self.df[self.dimensions_])
 
                 if metric == 'inertia':
                     self.scores_[algorithm].append(
-                        weighted_sum_of_squared_distances(self.df[self.dimensions_], self.instances_[algorithm].labels_,
-                                                          weights))
+                        weighted_sum_of_squared_distances(self.df[self.dimensions_], local_labels, weights))
                 elif metric == 'davies_bouldin_score':
                     self.scores_[algorithm].append(
-                        1 if nc == 1 else davies_bouldin_score(self.df[self.dimensions_],
-                                                               self.instances_[algorithm].labels_))
+                        1 if nc == 1 else davies_bouldin_score(self.df[self.dimensions_], local_labels))
                 elif metric == 'silhouette_score':
                     self.scores_[algorithm].append(
-                        0 if nc == 1 else silhouette_score(self.df[self.dimensions_],
-                                                           self.instances_[algorithm].labels_))
+                        0 if nc == 1 else silhouette_score(self.df[self.dimensions_], local_labels))
 
                 elif metric == 'calinski_harabasz_score':
                     self.scores_[algorithm].append(
-                        1 if nc == 1 else calinski_harabasz_score(self.df[self.dimensions_],
-                                                                  self.instances_[algorithm].labels_))
+                        1 if nc == 1 else calinski_harabasz_score(self.df[self.dimensions_], local_labels))
 
             if len(range(*cluster_range)) > 1:
                 kl = KneeLocator(x=range(*cluster_range), y=self.scores_[algorithm], curve='convex',
                                  direction='decreasing')
                 optimal_list.append((algorithm, kl.knee, self.scores_[algorithm][kl.knee-cluster_range[0]]))
             else:
                 optimal_list.append((algorithm, cluster_range[0], self.scores_[algorithm][0]))
@@ -227,14 +228,16 @@
             variables.remove('cluster')
 
         if cluster_filter is None:
             cluster_filter = list(df_ext['cluster'].unique())
         if not isinstance(cluster_filter, list):
             cluster_filter = [cluster_filter]
 
+        if not isinstance(statistics, list):
+            statistics = [statistics]
         if 'wmean' in statistics:
             def wmean(x): return weighted_mean(x, self.weights_[x.index])
             statistics[statistics.index('wmean')] = wmean
         if 'wstd' in statistics:
             def wstd(x): return weighted_std(x, self.weights_[x.index])
             statistics[statistics.index('wstd')] = wstd
 
@@ -389,15 +392,15 @@
             The order of the observations must be the same as that of the base DataFrame.
 
         Returns
         ----------
         dict : dictionary
             Dictionary with the corresponding test statistics.
         """
-        contingency_t = self.describe_clusters_cat(cat_array)
+        contingency_t = self.describe_clusters_cat(cat_array, '')
         test_res = chi2_contingency(contingency_t.values)
         return dict(zip(['chi2', 'p', 'dof'], test_res[:-1]))
 
     def plot_score_comparison(self, output_path=None, savefig_kws=None):
         """
         Plots the comparison in performance between the different clustering algorithms.
 
@@ -446,20 +449,17 @@
         use_weights: bool
             Whether to use sample weights.
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
-        if use_weights:
-            plot_clustercount(self.df, self.weights_, output_path, savefig_kws)
-        else:
-            plot_clustercount(self.df, output_path, savefig_kws)
+        plot_clustercount(self.df, self.weights_, output_path, savefig_kws)
 
-    def plot_cluster_means_to_global_means_comparison(self, use_weights= False, df_original=None, xlabel=None, ylabel=None,
+    def plot_cluster_means_to_global_means_comparison(self, use_weights=False, df_original=None, xlabel=None, ylabel=None,
                                                       levels=[-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50],
                                                       output_path=None, savefig_kws=None):
         """
         Plots the normalized curve used for computing the optimal number of clusters.
 
         Parameters
         ----------
@@ -575,28 +575,30 @@
         hue = 'cluster_cat'
         weights = None
         if use_weights:
             weights = self.weights_
         plot_clusters_2D(coor1, coor2, hue, df_ext, weights, style_kwargs=style_kwargs, output_path=output_path,
                          savefig_kws=savefig_kws)
 
-    def plot_cat_distribution_by_cluster(self, cat_array, cat_label=None, cluster_label=None, output_path=None,
-                                         savefig_kws=None):
+    def plot_cat_distribution_by_cluster(self, cat_array, cat_label, cluster_label=None, use_weights=False,
+                                         output_path=None, savefig_kws=None):
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
+        use_weights : bool, default=False
+            Whether to use weights for centroid comparison.
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
-        ct = self.describe_clusters_cat(cat_array, normalize=True)
+        ct = self.describe_clusters_cat(cat_array, cat_label, normalize=True, use_weights=use_weights)
         plot_cat_distribution_by_cluster(ct, cat_label, cluster_label, output_path, savefig_kws)
```

### Comparing `clust-learn-0.2.0b0/clearn/clustering/table_utils.py` & `clust-learn-0.2.1/clearn/clustering/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clearn/clustering/utils.py` & `clust-learn-0.2.1/clearn/clustering/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,13 +78,23 @@
     """
     average = np.average(data, weights=weights)
     variance = np.average((data-average)**2, weights=weights)
     return np.sqrt(variance)
 
 
 def is_sklearn_compatible(algorithm):
-    return 'fit' in dir(algorithm) and 'set_params' in dir(algorithm)
+    return 'fit_predict' in dir(algorithm) and 'set_params' in dir(algorithm)
 
 
 def accepts_param(function, param):
     args, varargs, varkw, defaults, kwonlyargs, kwonlydefaults, annotations = inspect.getfullargspec(function)
     return param in args
+
+
+def get_n_clusters_param_name(algorithm):
+    param_list = list(algorithm.get_params().keys())
+    if 'n_clusters' in param_list:
+        return 'n_clusters'
+    elif 'n_components' in param_list:
+        return 'n_components'
+    else:
+        return None
```

### Comparing `clust-learn-0.2.0b0/clearn/clustering/viz_utils.py` & `clust-learn-0.2.1/clearn/clustering/viz_utils.py`

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
-    colors = sns.color_palette("BrBG", n_colors=9)
+    colors = sns.color_palette("BrBG", n_colors=len(levels)+1)
     cmap, norm = matplotlib.colors.from_levels_and_colors(levels, colors, extend="both")
     width = min(len(dimensions), 20)
     height = min(df['cluster'].nunique(), 8)
     fig, ax = plt.subplots(figsize=(width, height))
     im = ax.imshow(df_diff[dimensions].values, cmap=cmap, norm=norm)
     ax.set(xticks=range(len(dimensions)), yticks=range(df_diff.shape[0]),
            xticklabels=list(map(str.upper, dimensions)), yticklabels=df_diff['cluster'])
@@ -208,15 +208,16 @@
 
     i = 0
     for col in df.columns:
         ax = get_axis(i, axs, ncols, nrows)
         sns.violinplot(y=df[col], x=cluster_labels, linewidth=1, ax=ax)
         plt.setp(ax.collections, alpha=.4)
         sns.boxplot(y=df[col], x=cluster_labels, width=0.2, linewidth=1, color='grey', ax=ax)
-        sns.stripplot(y=df[col], x=cluster_labels, alpha=0.7, size=3, ax=ax)
+        sns.stripplot(y=df[col], x=cluster_labels, hue=list(map(str,cluster_labels)), alpha=0.5, size=3, ax=ax,
+                      legend=None)
         ax.set_ylabel(col if ylabel is None else ylabel, fontsize=12, labelpad=15)
         if i // ncols == nrows-1:
             ax.set_xlabel('cluster' if xlabel is None else xlabel, fontsize=12, labelpad=15)
         i += 1
 
     while i < ncols * nrows:
         ax = get_axis(i, axs, ncols, nrows)
@@ -317,15 +318,15 @@
         agg_method = wmean
     scatter_df = df.groupby(hue).agg(dict(zip([x, y], [agg_method] * 2))).reset_index()
 
     sns.scatterplot(x=x, y=y, hue=hue, data=scatter_df,
                     alpha=1, palette=palette, linewidth=0, marker='X', s=100, ax=axs[1])
 
     if kdeplot:
-        hue_order = np.sort(df[hue].values)
+        hue_order = np.sort(df[hue].unique())
         sns.kdeplot(x=x, y=y, hue=hue, data=df, levels=1, alpha=0.2, palette=palette,
                     weights=weights, hue_order=hue_order, ax=axs[1])
 
     axs[1].vlines(xmean, ymin=ymin, ymax=ymax, color=vline_color, linewidth=1, linestyles='--', label=xmean_label)
     axs[1].hlines(ymean, xmin=xmin, xmax=xmax, color=hline_color, linewidth=1, linestyles='--', label=ymean_label)
     axs[1].set_xlabel(x, fontsize=12)
     axs[1].set_ylabel(y, fontsize=12)
```

### Comparing `clust-learn-0.2.0b0/clearn/data_preprocessing/__init__.py` & `clust-learn-0.2.1/clearn/data_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clearn/data_preprocessing/data_preprocessing.py` & `clust-learn-0.2.1/clearn/data_preprocessing/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clearn/data_preprocessing/viz_utils.py` & `clust-learn-0.2.1/clearn/data_preprocessing/viz_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,16 @@
     nrows = int(np.ceil(len(imputed_vars) / ncols))
 
     fig, axs = plt.subplots(nrows, ncols, figsize=(4 * ncols, 4 * nrows))
     df_prior_sample = df_prior.sample(frac=sample_frac, random_state=42)
     i = 0
     for ivar in imputed_vars:
         ax = get_axis(i, axs, ncols, nrows)
-        sns.kdeplot(ivar, data=df_prior_sample, label='Before imputation', ax=ax, **prior_kws)
-        sns.kdeplot(ivar, data=df_posterior.loc[df_prior_sample.index], label='After imputation', ax=ax,
+        sns.kdeplot(x=ivar, data=df_prior_sample, label='Before imputation', ax=ax, **prior_kws)
+        sns.kdeplot(x=ivar, data=df_posterior.loc[df_prior_sample.index], label='After imputation', ax=ax,
                     **posterior_kws)
         ax.legend()
         i += 1
 
     fig.tight_layout(pad=2)
     savefig(output_path=output_path, savefig_kws=savefig_kws)
```

### Comparing `clust-learn-0.2.0b0/clearn/dimensionality_reduction/dimensionality_reduction.py` & `clust-learn-0.2.1/clearn/dimensionality_reduction/dimensionality_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Dimensionality Reduction with PCA as reference"""
 # Author: Miguel Alvarez-Garcia
 
+import numpy as np
 import prince
 
 from sklearn.decomposition import PCA, SparsePCA
 from sklearn.preprocessing import StandardScaler
 from .table_utils import *
+from .utils import *
 from .viz_utils import *
 
 
 class DimensionalityReduction:
     """
     Dimensionality Reduction class
 
@@ -168,18 +170,18 @@
         trans.columns = [f'dim_{str(i+1).zfill(idx_positions)}' for i in range(trans.shape[1])]
         return trans
 
     def _transform_cat(self, df, n_components_cat=None):
         self.cat_model.set_params(n_components=df.nunique().sum())
         self.cat_model.fit(df.astype(str))
 
-        explained_variance_ratio = self.cat_model.explained_inertia_ / self.cat_model.explained_inertia_.sum()
+        explained_variance_ratio = self._get_explained_variance_ratio()
         if n_components_cat is None and self.min_explained_variance_ratio_ is None:
             # Optimal number
-            kl = KneeLocator(x=range(1, df.nunique().sum() + 1),
+            kl = KneeLocator(x=range(1, df.nunique().sum()),
                              y=explained_variance_ratio,
                              curve='convex',
                              direction='decreasing')
             n_components_cat = np.maximum(kl.knee-1, 1)
 
         elif n_components_cat is None:
             # Based on explained variance
@@ -188,14 +190,20 @@
 
         trans = self.cat_model.transform(df.astype(str))
         trans = trans[trans.columns[:n_components_cat]]
         idx_positions = np.maximum(2, len(str(n_components_cat)))
         trans.columns = [f'dim_{str(i+1).zfill(idx_positions)}' for i in range(n_components_cat)]
         return trans
 
+    # We need to (temporarily) do this manually because prince is no longer applying these corrections with MCA
+    def _get_explained_variance_ratio(self):
+        benzecri_eigenvalues = apply_benzecri_eigenvalue_correction(self.cat_model.eigenvalues_, self.cat_model.K_)
+        greenacre_inertia = compute_greenacre_inertia(self.cat_model.eigenvalues_, self.cat_model.K_, self.cat_model.J_)
+        return benzecri_eigenvalues / greenacre_inertia
+
     def num_main_contributors(self, thres=0.5, n_contributors=None, dim_idx=None, component_description=None,
                               col_description=None, output_path=None):
         """
         Computes the original numerical variables with the strongest relation to the derived variable(s)
         (measured as Pearson correlation coefficient)
 
         Parameters
@@ -315,15 +323,15 @@
         plots : str or list, default='all'
             The following plots are supported: ['cumulative', 'ratio', 'normalized']
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
-        explained_variance_ratio = self.cat_model.explained_inertia_ / self.cat_model.explained_inertia_.sum()
+        explained_variance_ratio = self._get_explained_variance_ratio()
         plot_explained_variance(explained_variance_ratio, thres, plots, output_path, savefig_kws)
 
     def plot_num_main_contributors(self, thres=0.5, n_contributors=5, dim_idx=None, output_path=None, savefig_kws=None):
         """
         Plot main contributors (original variables with the strongest relation with derived variables) for
         every derived variable
```

### Comparing `clust-learn-0.2.0b0/clearn/dimensionality_reduction/table_utils.py` & `clust-learn-0.2.1/clearn/dimensionality_reduction/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clearn/dimensionality_reduction/viz_utils.py` & `clust-learn-0.2.1/clearn/dimensionality_reduction/viz_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
     j = 0
     for idx, row in mc.iterrows():
         var_name = row['var_name']
         nvalues = df[var_name].nunique()
 
         i = 0
         ax0 = None
-        for v in df[var_name].unique():
+        for v in np.sort(df[var_name].unique()):
             ax = fig.add_subplot(gs[i:i + int(nrows / nvalues), j], sharex=ax0, sharey=ax0)
             sns.kdeplot(data=df[df[var_name] == v], x=dim_name, color='blue', fill=True, ax=ax)
             ax.set_title(f'{var_name} = {v}', fontsize=10)
             ax.set_ylabel('')
 
             i += int(nrows / nvalues)
             if i < nrows:
```

### Comparing `clust-learn-0.2.0b0/clearn/utils.py` & `clust-learn-0.2.1/clearn/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0b0/clust_learn.egg-info/PKG-INFO` & `clust-learn-0.2.1/clust_learn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.2.0b0
+Version: 0.2.1
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -77,15 +77,15 @@
 
 **Figue 1** shows the package layout with the functionalities covered by each module along with the techniques used, the
 explainability strategies available, and the main functions and class methods encapsulating these techniques and
 explainability strategies.
 
 <br/>
 
-![clust-learn package structure](https://github.com/malgar/clust-learn/blob/v0.0.8/images/package_structure.png?raw=true)
+![clust-learn package structure](https://github.com/malgar/clust-learn/blob/master/images/package_structure.png?raw=true)
 
 <br/>
 
 <h2 id="user-content-implementation">
 3. Implementation
 </h2>
 
@@ -104,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0b
+* Version: 0.2.1
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
 
@@ -409,15 +409,15 @@
 ```
 cl = Clustering(df, algorithms='kmeans', normalize=False)
 ```
 
 | Parameter | Type | Description |
 |:-|:-|:-|
 | `df` | `pandas.DataFrame` | Data frame containing the data to be clustered |
-| `algorithms` | `string` or `list` | Algorithms to be used for clustering. The current version supports k-means and agglomerative clustering |
+| `algorithms` | instance or `list` of instances | Algorithm instances to be used for clustering. They must implement the `fit` and `set_params` methods |
 | `normalize` | `bool` | Whether to apply data normalization for fair comparisons between variables. In case dimensionality reduction is applied beforehand, normalization should not be applied |
 | **Attribute** | **Type** | **Description** |
 | `dimensions_` | `list` | List of columns of they input data frame |
 | `instances_` | `dict` | Pairs of algorithm name and its instance |
 | `metric_` | `string` | The cluster validation metric used. Four metrics available: ['inertia', 'davies_bouldin_score', 'silhouette_score',  'calinski_harabasz_score'] |
 | `optimal_config_` | `tuple` | Tuple with the optimal configuration for clustering containing the algorithm name, number of clusters, and value of the chosen validation metric |
 | `scores_` | `dict` | Pairs of algorithm name and a list of values of the chosen validation metric for a cluster range |
@@ -457,15 +457,15 @@
 <h4 id="describe_clusters_cat">
 describe_clusters_cat()
 </h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L237)
 
 ```
-describe_clusters_cat(self, cat_array, cat_name=None, order=None, normalize=False, output_path=None)
+describe_clusters_cat(self, cat_array, cat_name, order=None, normalize=False, use_weights=False, output_path=None)
 ```
 
 Describes clusters based on  external *categorical* variables. The result is a contingency table.
 For continuous variables use [`describe_clusters()`](#describe_clusters).
 
 <h4>compare_cluster_means_to_global_means()</h4>
 
@@ -519,25 +519,25 @@
 Plots the normalized curve used for computing the optimal number of clusters.
 
 <h4>plot_clustercount()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L419)
 
 ```
-plot_clustercount(self, output_path=None, savefig_kws=None)
+plot_clustercount(self, use_weights=False, output_path=None, savefig_kws=None)
 ```
 
 Plots a bar plot with cluster counts.
 
 <h4>plot_cluster_means_to_global_means_comparison()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L432)
 
 ```
-plot_cluster_means_to_global_means_comparison(self, df_original=None, xlabel=None, ylabel=None,
+plot_cluster_means_to_global_means_comparison(self, use_weights= False, df_original=None, xlabel=None, ylabel=None,
                                               levels=[-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50],
                                               output_path=None, savefig_kws=None)
 ```
 
 Plots the normalized curve used for computing the optimal number of clusters.
 
 <h4>plot_distribution_comparison_by_cluster()</h4>
@@ -551,27 +551,27 @@
 Plots the violin plots per cluster and *continuous* variables of interest to understand differences in their distributions by cluster.
 
 <h4>plot_clusters_2D()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L498)
 
 ```
-plot_clusters_2D(self, coor1, coor2, style_kwargs=dict(), output_path=None, savefig_kws=None)
+plot_clusters_2D(self, coor1, coor2, use_weights=False, style_kwargs=dict(), output_path=None, savefig_kws=None)
 ```
 
 Plots two 2D plots:
 	 - A scatter plot styled by the categorical variable `hue`.
 	 - A 2D plot comparing cluster centroids and optionally the density area.
 	 
 <h4>plot_cat_distribution_by_cluster()</h4>
 
 [Source](https://github.com/malgar/clust-learn/blob/be4a2238670af01023bd419a0f8adaa7f9cee9f6/clearn/clustering/clustering.py#L545)
 
 ```
-plot_cat_distribution_by_cluster(self, cat_array, cat_label=None, cluster_label=None, output_path=None, savefig_kws=None)
+plot_cat_distribution_by_cluster(self, cat_array, cat_label, cluster_label=None, use_weights=False, output_path=None, savefig_kws=None)
 ```
 
 Plots the relative contingency table of the clusters with a categorical variable as a stacked bar plot.
 
 <h3 id="user-content-module-classifier">
 7.iv. Classifier
 </h3>
```

### Comparing `clust-learn-0.2.0b0/clust_learn.egg-info/SOURCES.txt` & `clust-learn-0.2.1/clust_learn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 clearn/clustering/viz_utils.py
 clearn/data_preprocessing/__init__.py
 clearn/data_preprocessing/data_preprocessing.py
 clearn/data_preprocessing/viz_utils.py
 clearn/dimensionality_reduction/__init__.py
 clearn/dimensionality_reduction/dimensionality_reduction.py
 clearn/dimensionality_reduction/table_utils.py
+clearn/dimensionality_reduction/utils.py
 clearn/dimensionality_reduction/viz_utils.py
 clust_learn.egg-info/PKG-INFO
 clust_learn.egg-info/SOURCES.txt
 clust_learn.egg-info/dependency_links.txt
 clust_learn.egg-info/requires.txt
 clust_learn.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `clust-learn-0.2.0b0/pyproject.toml` & `clust-learn-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clust-learn"
-version = "0.2.0b"
+version = "0.2.1"
 authors = [
   { name="Miguel Alvarez-Garcia", email="malvarez.statistics@gmail.com" },
 ]
 description = "A Python package for explainable cluster analysis"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `clust-learn-0.2.0b0/setup.py` & `clust-learn-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(os.path.join(ROOT, 'README.md')) as f:
     README = f.read()
 
 
 setup(
     name='clust-learn',
-    version="0.2.0b",
+    version="0.2.1",
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
-        "pandas>=1.3.4",
-        "pingouin>=0.5.1",
-        "prince==0.7.0",
+        "pandas>=1.3.4,<2.0",
+        "pingouin>=0.5.3",
+        "prince==0.10.4",
         "scikit-learn>=1.0.2",
         "scipy>=1.7.1",
         "seaborn>=0.11.2",
         "shap>=0.40.0",
         "statsmodels>=0.13.2",
         "xgboost>=1.5.2"
     ],
```


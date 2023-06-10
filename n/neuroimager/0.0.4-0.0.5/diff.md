# Comparing `tmp/neuroimager-0.0.4.tar.gz` & `tmp/neuroimager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroimager-0.0.4.tar", last modified: Mon Jun  5 13:46:29 2023, max compression
+gzip compressed data, was "neuroimager-0.0.5.tar", last modified: Sat Jun 10 05:37:07 2023, max compression
```

## Comparing `neuroimager-0.0.4.tar` & `neuroimager-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:46:29.357931 neuroimager-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 13:46:19.000000 neuroimager-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-05 13:46:29.357931 neuroimager-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 13:46:19.000000 neuroimager-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:46:29.353931 neuroimager-0.0.4/neuroimager/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:46:29.353931 neuroimager-0.0.4/neuroimager/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/pipes/brainage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/pipes/cca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:46:29.353931 neuroimager-0.0.4/neuroimager/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:46:29.353931 neuroimager-0.0.4/neuroimager/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/utils/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-05 13:46:19.000000 neuroimager-0.0.4/neuroimager/utils/fc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:46:29.353931 neuroimager-0.0.4/neuroimager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-05 13:46:29.000000 neuroimager-0.0.4/neuroimager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-05 13:46:29.000000 neuroimager-0.0.4/neuroimager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:46:29.000000 neuroimager-0.0.4/neuroimager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 13:46:29.000000 neuroimager-0.0.4/neuroimager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 13:46:29.000000 neuroimager-0.0.4/neuroimager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:46:29.357931 neuroimager-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-05 13:46:19.000000 neuroimager-0.0.4/setup.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-10 05:37:07.419255 neuroimager-0.0.5/
+-rw-r--r--   0 nij       (1000) nij       (1000)    35149 2023-06-05 13:40:29.000000 neuroimager-0.0.5/LICENSE
+-rw-r--r--   0 nij       (1000) nij       (1000)     2392 2023-06-10 05:37:07.419255 neuroimager-0.0.5/PKG-INFO
+-rw-r--r--   0 nij       (1000) nij       (1000)     1766 2023-06-10 04:15:11.000000 neuroimager-0.0.5/README.md
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-10 05:37:07.417255 neuroimager-0.0.5/neuroimager/
+-rw-r--r--   0 nij       (1000) nij       (1000)      149 2023-06-05 13:02:03.000000 neuroimager-0.0.5/neuroimager/__init__.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-10 05:37:07.418255 neuroimager-0.0.5/neuroimager/pipes/
+-rw-r--r--   0 nij       (1000) nij       (1000)        0 2023-06-05 13:00:13.000000 neuroimager-0.0.5/neuroimager/pipes/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     3188 2023-06-10 05:11:31.000000 neuroimager-0.0.5/neuroimager/pipes/bipartite.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     1212 2023-06-05 13:02:03.000000 neuroimager-0.0.5/neuroimager/pipes/brainage.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     7097 2023-06-08 17:19:10.000000 neuroimager-0.0.5/neuroimager/pipes/cca.py
+-rw-r--r--   0 nij       (1000) nij       (1000)    15619 2023-06-08 17:19:10.000000 neuroimager-0.0.5/neuroimager/pipes/explore.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     8830 2023-06-08 17:19:10.000000 neuroimager-0.0.5/neuroimager/pipes/hmm.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-10 05:37:07.418255 neuroimager-0.0.5/neuroimager/plotting/
+-rw-r--r--   0 nij       (1000) nij       (1000)      180 2023-06-08 17:13:31.000000 neuroimager-0.0.5/neuroimager/plotting/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     4530 2023-06-08 17:13:02.000000 neuroimager-0.0.5/neuroimager/plotting/plot.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-10 05:37:07.419255 neuroimager-0.0.5/neuroimager/stats/
+-rw-r--r--   0 nij       (1000) nij       (1000)       85 2023-06-08 17:03:02.000000 neuroimager-0.0.5/neuroimager/stats/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     5558 2023-06-09 10:11:35.000000 neuroimager-0.0.5/neuroimager/stats/correlation.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-10 05:37:07.419255 neuroimager-0.0.5/neuroimager/utils/
+-rw-r--r--   0 nij       (1000) nij       (1000)      560 2023-06-09 06:04:17.000000 neuroimager-0.0.5/neuroimager/utils/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     9900 2023-06-09 14:51:06.000000 neuroimager-0.0.5/neuroimager/utils/atlas.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     6704 2023-06-09 10:11:35.000000 neuroimager-0.0.5/neuroimager/utils/fc.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-10 05:37:07.418255 neuroimager-0.0.5/neuroimager.egg-info/
+-rw-r--r--   0 nij       (1000) nij       (1000)     2392 2023-06-10 05:37:07.000000 neuroimager-0.0.5/neuroimager.egg-info/PKG-INFO
+-rw-r--r--   0 nij       (1000) nij       (1000)      600 2023-06-10 05:37:07.000000 neuroimager-0.0.5/neuroimager.egg-info/SOURCES.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)        1 2023-06-10 05:37:07.000000 neuroimager-0.0.5/neuroimager.egg-info/dependency_links.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)       87 2023-06-10 05:37:07.000000 neuroimager-0.0.5/neuroimager.egg-info/requires.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)       12 2023-06-10 05:37:07.000000 neuroimager-0.0.5/neuroimager.egg-info/top_level.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)       38 2023-06-10 05:37:07.419255 neuroimager-0.0.5/setup.cfg
+-rw-r--r--   0 nij       (1000) nij       (1000)     1187 2023-06-10 05:30:09.000000 neuroimager-0.0.5/setup.py
```

### Comparing `neuroimager-0.0.4/LICENSE` & `neuroimager-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.4/neuroimager/pipes/brainage.py` & `neuroimager-0.0.5/neuroimager/pipes/brainage.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.4/neuroimager/pipes/cca.py` & `neuroimager-0.0.5/neuroimager/pipes/cca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 from sklearn.cross_decomposition import CCA
 import seaborn as sns
 from matplotlib import pyplot as plt
 from scipy.stats import pearsonr
-from plotting import density_scatter
+from neuroimager.plotting import density_scatter
 
 
 def permutation_test_cca(X, Y, n_components=1, n_permutations=1000, random_state=None):
     """
     Perform a permutation test for Canonical Correlation Analysis (CCA) to assess the significance
     of the correlation between two sets of features.
```


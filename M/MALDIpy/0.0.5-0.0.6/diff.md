# Comparing `tmp/MALDIpy-0.0.5.tar.gz` & `tmp/MALDIpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MALDIpy-0.0.5.tar", last modified: Sat Jun 10 02:22:34 2023, max compression
+gzip compressed data, was "MALDIpy-0.0.6.tar", last modified: Sat Jun 10 02:24:36 2023, max compression
```

## Comparing `MALDIpy-0.0.5.tar` & `MALDIpy-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:22:34.478377 MALDIpy-0.0.5/
--rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.0.5/LICENSE
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:22:34.474377 MALDIpy-0.0.5/MALDIpy/
--rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-10 02:22:10.000000 MALDIpy-0.0.5/MALDIpy/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     5030 2023-06-10 02:21:05.000000 MALDIpy-0.0.5/MALDIpy/featureplot.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.0.5/MALDIpy/msi_data.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.0.5/MALDIpy/multi_sample.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.0.5/MALDIpy/projection.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:22:34.474377 MALDIpy-0.0.5/MALDIpy/shell/
--rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.0.5/MALDIpy/shell/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.0.5/MALDIpy/shell/usage.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.0.5/MALDIpy/single_cell.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:22:34.478377 MALDIpy-0.0.5/MALDIpy/src/
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.5/MALDIpy/src/temp.txt
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:22:34.474377 MALDIpy-0.0.5/MALDIpy.egg-info/
--rw-r--r--   0 hli       (1002) labmem    (1001)      678 2023-06-10 02:22:34.000000 MALDIpy-0.0.5/MALDIpy.egg-info/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-10 02:22:34.000000 MALDIpy-0.0.5/MALDIpy.egg-info/SOURCES.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-10 02:22:34.000000 MALDIpy-0.0.5/MALDIpy.egg-info/dependency_links.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-10 02:22:34.000000 MALDIpy-0.0.5/MALDIpy.egg-info/entry_points.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-10 02:22:34.000000 MALDIpy-0.0.5/MALDIpy.egg-info/top_level.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.0.5/MALDIpy.egg-info/zip-safe
--rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.0.5/MANIFEST.in
--rw-r--r--   0 hli       (1002) labmem    (1001)      678 2023-06-10 02:22:34.478377 MALDIpy-0.0.5/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      250 2023-06-10 02:22:26.000000 MALDIpy-0.0.5/README.md
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.5/requirements.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-10 02:22:34.478377 MALDIpy-0.0.5/setup.cfg
--rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.0.5/setup.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:24:36.379239 MALDIpy-0.0.6/
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.0.6/LICENSE
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:24:36.379239 MALDIpy-0.0.6/MALDIpy/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-10 02:24:03.000000 MALDIpy-0.0.6/MALDIpy/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     5002 2023-06-10 02:24:28.000000 MALDIpy-0.0.6/MALDIpy/featureplot.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.0.6/MALDIpy/msi_data.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.0.6/MALDIpy/multi_sample.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.0.6/MALDIpy/projection.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:24:36.379239 MALDIpy-0.0.6/MALDIpy/shell/
+-rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.0.6/MALDIpy/shell/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.0.6/MALDIpy/shell/usage.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.0.6/MALDIpy/single_cell.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:24:36.379239 MALDIpy-0.0.6/MALDIpy/src/
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.6/MALDIpy/src/temp.txt
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:24:36.379239 MALDIpy-0.0.6/MALDIpy.egg-info/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      696 2023-06-10 02:24:36.000000 MALDIpy-0.0.6/MALDIpy.egg-info/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-10 02:24:36.000000 MALDIpy-0.0.6/MALDIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-10 02:24:36.000000 MALDIpy-0.0.6/MALDIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-10 02:24:36.000000 MALDIpy-0.0.6/MALDIpy.egg-info/entry_points.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-10 02:24:36.000000 MALDIpy-0.0.6/MALDIpy.egg-info/top_level.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.0.6/MALDIpy.egg-info/zip-safe
+-rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.0.6/MANIFEST.in
+-rw-r--r--   0 hli       (1002) labmem    (1001)      696 2023-06-10 02:24:36.379239 MALDIpy-0.0.6/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      252 2023-06-10 02:23:57.000000 MALDIpy-0.0.6/README.md
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.6/requirements.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-10 02:24:36.379239 MALDIpy-0.0.6/setup.cfg
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.0.6/setup.py
```

### Comparing `MALDIpy-0.0.5/LICENSE` & `MALDIpy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.5/MALDIpy/featureplot.py` & `MALDIpy-0.0.6/MALDIpy/featureplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
 import math
 from scipy import ndimage
 from scipy.spatial import distance_matrix
 import requests
 import matplotlib.colors as mcolors
 
-def plot1feature(tissue_obj, title='',cmap = "magma_r", mz_use=mz_use,
+def plot1feature(tissue_obj, title='',cmap = "magma_r", mz_use,
                               max_num=50000, min_num=0, figsize = (6,5)):
     print('Feature mz:',mz_use)
     tissue_mz = tissue_obj.to_img_mtx(mz=mz_use,smooth=False)
     df1=tissue_mz
     fig, ((ax1,axcb1)) = plt.subplots(1, 2, figsize = figsize,dpi = 300,gridspec_kw={'width_ratios':[1,0.05]})
     
 
@@ -36,15 +36,15 @@
                                fontproperties=fm.FontProperties(size=10))
 
 ##300um
     ax1.add_artist(scalebar1)
     plt.tight_layout()
     return fig
 
-def plot1feature_subset(tissue_obj, title='',cmap = "magma_r", mz_use=mz_use,
+def plot1feature_subset(tissue_obj, title='',cmap = "magma_r", mz_use,
                               max_num=50000, min_num=0, figsize = (6,5), subset=[95,185,35,175]):
     print('Feature mz:',mz_use)
     tissue_mz = tissue_obj.to_img_mtx(mz=mz_use,smooth=False)
     df1=tissue_mz.iloc[subset[0]:subset[1], subset[2]:subset[3]]
 
     fig, ((ax1)) = plt.subplots(1, 1, figsize = figsize,dpi = 300,gridspec_kw={'width_ratios':[1]})
     
@@ -57,15 +57,15 @@
     plt.tight_layout()
     return fig
 
 def twofeatureplot(
     tissue_obj, 
     title='',
     cmap = ["Reds", "Greens"], 
-    mz_use=mz_use,                 
+    mz_use,                 
     max_num_1=50000, min_num_1=0, 
     max_num_2=50000, min_num_2=0,
     alpha = [0.5, 0.5],
     figsize = (6,5)
 ):
     print('Feature mz:',mz_use)
     df1 = tissue_obj.to_img_mtx(mz=mz_use[0],smooth=False)
@@ -105,15 +105,15 @@
     return fig
 
 
 def twofeatureplot_subset(
     tissue_obj, 
     title='',
     cmap = ["Reds", "Greens"], 
-    mz_use=mz_use,                 
+    mz_use,                 
     max_num_1=50000, min_num_1=0, 
     max_num_2=50000, min_num_2=0,
     alpha = [0.5, 0.5],
     figsize = (6,5),subset=[95,185,35,175]
     
 ):
     print('Feature mz:',mz_use)
```

### Comparing `MALDIpy-0.0.5/MALDIpy/msi_data.py` & `MALDIpy-0.0.6/MALDIpy/msi_data.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.5/MALDIpy/multi_sample.py` & `MALDIpy-0.0.6/MALDIpy/multi_sample.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.5/MALDIpy/projection.py` & `MALDIpy-0.0.6/MALDIpy/projection.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.5/MALDIpy/single_cell.py` & `MALDIpy-0.0.6/MALDIpy/single_cell.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.5/MALDIpy.egg-info/PKG-INFO` & `MALDIpy-0.0.6/MALDIpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: MALDIpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: MALDI-MS data analysis at the single-cell level
 Home-page: https://github.com/TheHumphreysLab
 Author: Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys
 Author-email: haikuolibio@gmail.com
 License: UNKNOWN
-Description: Updates in MALDIpy v0.0.5; compared to v0.0.2:\n
-        1.New function: MALDIpy.projection.umap_projection_subset\n
-        2.New function: MALDIpy.featureplot, which includes four subfunctions (plot1feature,plot1feature_subset,twofeatureplot,twofeatureplot_subset)
+Description: Updates in MALDIpy v0.0.6; compared to v0.0.2:
+        
+        (1) New function: MALDIpy.projection.umap_projection_subset
+        
+        (2) New function: MALDIpy.featureplot, which includes four subfunctions (plot1feature,plot1feature_subset,twofeatureplot,twofeatureplot_subset)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `MALDIpy-0.0.5/PKG-INFO` & `MALDIpy-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: MALDIpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: MALDI-MS data analysis at the single-cell level
 Home-page: https://github.com/TheHumphreysLab
 Author: Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys
 Author-email: haikuolibio@gmail.com
 License: UNKNOWN
-Description: Updates in MALDIpy v0.0.5; compared to v0.0.2:\n
-        1.New function: MALDIpy.projection.umap_projection_subset\n
-        2.New function: MALDIpy.featureplot, which includes four subfunctions (plot1feature,plot1feature_subset,twofeatureplot,twofeatureplot_subset)
+Description: Updates in MALDIpy v0.0.6; compared to v0.0.2:
+        
+        (1) New function: MALDIpy.projection.umap_projection_subset
+        
+        (2) New function: MALDIpy.featureplot, which includes four subfunctions (plot1feature,plot1feature_subset,twofeatureplot,twofeatureplot_subset)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `MALDIpy-0.0.5/setup.py` & `MALDIpy-0.0.6/setup.py`

 * *Files identical despite different names*


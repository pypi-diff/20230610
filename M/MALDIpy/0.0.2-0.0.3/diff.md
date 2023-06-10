# Comparing `tmp/MALDIpy-0.0.2.tar.gz` & `tmp/MALDIpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MALDIpy-0.0.2.tar", last modified: Thu Apr  6 21:03:02 2023, max compression
+gzip compressed data, was "MALDIpy-0.0.3.tar", last modified: Sat Jun 10 02:09:15 2023, max compression
```

## Comparing `MALDIpy-0.0.2.tar` & `MALDIpy-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-04-06 21:03:02.830432 MALDIpy-0.0.2/
--rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.0.2/LICENSE
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-04-06 21:03:02.830432 MALDIpy-0.0.2/MALDIpy/
--rw-r--r--   0 hli       (1002) labmem    (1001)      168 2023-04-06 21:02:56.000000 MALDIpy-0.0.2/MALDIpy/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.0.2/MALDIpy/msi_data.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.0.2/MALDIpy/multi_sample.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     5687 2023-04-06 18:38:13.000000 MALDIpy-0.0.2/MALDIpy/projection.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-04-06 21:03:02.830432 MALDIpy-0.0.2/MALDIpy/shell/
--rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.0.2/MALDIpy/shell/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.0.2/MALDIpy/shell/usage.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.0.2/MALDIpy/single_cell.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-04-06 21:03:02.830432 MALDIpy-0.0.2/MALDIpy/src/
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.2/MALDIpy/src/temp.txt
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-04-06 21:03:02.830432 MALDIpy-0.0.2/MALDIpy.egg-info/
--rw-r--r--   0 hli       (1002) labmem    (1001)      420 2023-04-06 21:03:02.000000 MALDIpy-0.0.2/MALDIpy.egg-info/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      418 2023-04-06 21:03:02.000000 MALDIpy-0.0.2/MALDIpy.egg-info/SOURCES.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-06 21:03:02.000000 MALDIpy-0.0.2/MALDIpy.egg-info/dependency_links.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-04-06 21:03:02.000000 MALDIpy-0.0.2/MALDIpy.egg-info/entry_points.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-04-06 21:03:02.000000 MALDIpy-0.0.2/MALDIpy.egg-info/top_level.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.0.2/MALDIpy.egg-info/zip-safe
--rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.0.2/MANIFEST.in
--rw-r--r--   0 hli       (1002) labmem    (1001)      420 2023-04-06 21:03:02.830432 MALDIpy-0.0.2/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)       17 2023-04-06 20:06:12.000000 MALDIpy-0.0.2/README.md
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.2/requirements.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-04-06 21:03:02.830432 MALDIpy-0.0.2/setup.cfg
--rw-r--r--   0 hli       (1002) labmem    (1001)     1913 2023-04-06 20:06:15.000000 MALDIpy-0.0.2/setup.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.0.3/LICENSE
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      168 2023-06-10 01:44:59.000000 MALDIpy-0.0.3/MALDIpy/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     5090 2023-06-10 02:02:01.000000 MALDIpy-0.0.3/MALDIpy/featureplot.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.0.3/MALDIpy/msi_data.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.0.3/MALDIpy/multi_sample.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.0.3/MALDIpy/projection.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy/shell/
+-rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.0.3/MALDIpy/shell/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.0.3/MALDIpy/shell/usage.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.0.3/MALDIpy/single_cell.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy/src/
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.3/MALDIpy/src/temp.txt
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy.egg-info/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      674 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/entry_points.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/top_level.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.0.3/MALDIpy.egg-info/zip-safe
+-rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.0.3/MANIFEST.in
+-rw-r--r--   0 hli       (1002) labmem    (1001)      674 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      246 2023-06-10 02:02:57.000000 MALDIpy-0.0.3/README.md
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.3/requirements.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/setup.cfg
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.0.3/setup.py
```

### Comparing `MALDIpy-0.0.2/LICENSE` & `MALDIpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.2/MALDIpy/msi_data.py` & `MALDIpy-0.0.3/MALDIpy/msi_data.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.2/MALDIpy/multi_sample.py` & `MALDIpy-0.0.3/MALDIpy/multi_sample.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.2/MALDIpy/projection.py` & `MALDIpy-0.0.3/MALDIpy/projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,34 @@
     
     if add_scalebar==True:
         scalebar1 = AnchoredSizeBar(ax1.transData, 30, '300 µm', 'lower right',frameon=False,size_vertical=2,sep=5,
                                fontproperties=fm.FontProperties(size=8))
         ax1.add_artist(scalebar1)
     plt.show()
     
+def umap_projection_subset(adata_name, file_name='', leiden_key_added='leiden', pltcmap='',figtitle='',figdpi=100, fig_size=(5,4),
+                           subset=[95,185,35,175]):
+    loc_df = create_loc(file_name)
+    num_celltype = len(set(adata_name.obs[leiden_key_added]))
+    df = adata_name.obs
+    for i in range(1,num_celltype+1): ##changed
+        tmp = df[df[leiden_key_added] == str(i)].index.str.split('_').tolist() ##changed
+        for idx in tmp:
+            loc_df.loc[idx[1],idx[0]] = i
+    loc_df = transform(loc_df)
+    loc_df=loc_df.iloc[subset[0]:subset[1], subset[2]:subset[3]]
+    fig, ax1 = plt.subplots(1,1, figsize = fig_size, dpi = figdpi)
+    g1 = sns.heatmap(loc_df,
+                     mask=(loc_df==0),cmap=pltcmap,
+                     ax=ax1,cbar=False)
+    g1.set_title(figtitle, fontsize=14)
+    g1.set_ylabel('');g1.set_xlabel('');g1.set_xticks([]);g1.set_yticks([])
+    
+    plt.show()
+    
 def project3tissues(raw_file1,raw_file2,raw_file3, adata_name, leiden_key='leiden',suffix1='data1',suffix2='data2',suffix3='data3',
                     cmap = "magma_r",figdpi=100, fig_size=(15,5), add_scalebar=True,
                    subtitle1='',subtitle2='',subtitle3=''):
     file1_df = create_loc(raw_file1)
     file2_df = create_loc(raw_file2)
     file3_df = create_loc(raw_file3)
     num_celltype=len(set(adata_name.obs[leiden_key]))
```

### Comparing `MALDIpy-0.0.2/MALDIpy/single_cell.py` & `MALDIpy-0.0.3/MALDIpy/single_cell.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.2/setup.py` & `MALDIpy-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 NAME = "MALDIpy"
-AUTHOR = "Haikuo Li; Qiao Xuanyuan; Benjamin Humphreys"
+AUTHOR = "Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys"
 EMAIL = "haikuolibio@gmail.com"
 URL = "https://github.com/TheHumphreysLab"
 #LICENSE = "your license"
 DESCRIPTION = "MALDI-MS data analysis at the single-cell level"
 
 if sys.version_info < (3, 6, 0):
     raise RuntimeError(f"{NAME} requires Python >=3.6.0, but yours is {sys.version}!")
```


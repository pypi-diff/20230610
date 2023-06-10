# Comparing `tmp/MALDIpy-0.0.3.tar.gz` & `tmp/MALDIpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MALDIpy-0.0.3.tar", last modified: Sat Jun 10 02:09:15 2023, max compression
+gzip compressed data, was "MALDIpy-0.0.4.tar", last modified: Sat Jun 10 02:17:46 2023, max compression
```

## Comparing `MALDIpy-0.0.3.tar` & `MALDIpy-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/
--rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.0.3/LICENSE
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy/
--rw-r--r--   0 hli       (1002) labmem    (1001)      168 2023-06-10 01:44:59.000000 MALDIpy-0.0.3/MALDIpy/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     5090 2023-06-10 02:02:01.000000 MALDIpy-0.0.3/MALDIpy/featureplot.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.0.3/MALDIpy/msi_data.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.0.3/MALDIpy/multi_sample.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.0.3/MALDIpy/projection.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy/shell/
--rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.0.3/MALDIpy/shell/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.0.3/MALDIpy/shell/usage.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.0.3/MALDIpy/single_cell.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy/src/
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.3/MALDIpy/src/temp.txt
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/MALDIpy.egg-info/
--rw-r--r--   0 hli       (1002) labmem    (1001)      674 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/SOURCES.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/dependency_links.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/entry_points.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-10 02:09:15.000000 MALDIpy-0.0.3/MALDIpy.egg-info/top_level.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.0.3/MALDIpy.egg-info/zip-safe
--rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.0.3/MANIFEST.in
--rw-r--r--   0 hli       (1002) labmem    (1001)      674 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      246 2023-06-10 02:02:57.000000 MALDIpy-0.0.3/README.md
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.3/requirements.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-10 02:09:15.871821 MALDIpy-0.0.3/setup.cfg
--rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.0.3/setup.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:17:46.308241 MALDIpy-0.0.4/
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.0.4/LICENSE
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:17:46.308241 MALDIpy-0.0.4/MALDIpy/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-10 02:17:41.000000 MALDIpy-0.0.4/MALDIpy/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     5090 2023-06-10 02:02:01.000000 MALDIpy-0.0.4/MALDIpy/featureplot.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.0.4/MALDIpy/msi_data.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.0.4/MALDIpy/multi_sample.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.0.4/MALDIpy/projection.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:17:46.308241 MALDIpy-0.0.4/MALDIpy/shell/
+-rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.0.4/MALDIpy/shell/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.0.4/MALDIpy/shell/usage.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.0.4/MALDIpy/single_cell.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:17:46.308241 MALDIpy-0.0.4/MALDIpy/src/
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.4/MALDIpy/src/temp.txt
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:17:46.308241 MALDIpy-0.0.4/MALDIpy.egg-info/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      674 2023-06-10 02:17:46.000000 MALDIpy-0.0.4/MALDIpy.egg-info/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-10 02:17:46.000000 MALDIpy-0.0.4/MALDIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-10 02:17:46.000000 MALDIpy-0.0.4/MALDIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-10 02:17:46.000000 MALDIpy-0.0.4/MALDIpy.egg-info/entry_points.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-10 02:17:46.000000 MALDIpy-0.0.4/MALDIpy.egg-info/top_level.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.0.4/MALDIpy.egg-info/zip-safe
+-rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.0.4/MANIFEST.in
+-rw-r--r--   0 hli       (1002) labmem    (1001)      674 2023-06-10 02:17:46.308241 MALDIpy-0.0.4/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      246 2023-06-10 02:16:22.000000 MALDIpy-0.0.4/README.md
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.0.4/requirements.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-10 02:17:46.308241 MALDIpy-0.0.4/setup.cfg
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.0.4/setup.py
```

### Comparing `MALDIpy-0.0.3/LICENSE` & `MALDIpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.3/MALDIpy/featureplot.py` & `MALDIpy-0.0.4/MALDIpy/featureplot.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.3/MALDIpy/msi_data.py` & `MALDIpy-0.0.4/MALDIpy/msi_data.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.3/MALDIpy/multi_sample.py` & `MALDIpy-0.0.4/MALDIpy/multi_sample.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.3/MALDIpy/projection.py` & `MALDIpy-0.0.4/MALDIpy/projection.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.3/MALDIpy/single_cell.py` & `MALDIpy-0.0.4/MALDIpy/single_cell.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.0.3/MALDIpy.egg-info/PKG-INFO` & `MALDIpy-0.0.4/MALDIpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: MALDIpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: MALDI-MS data analysis at the single-cell level
 Home-page: https://github.com/TheHumphreysLab
 Author: Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys
 Author-email: haikuolibio@gmail.com
 License: UNKNOWN
-Description: Updates in MALDIpy v0.0.3; compared to v0.0.2:
+Description: Updates in MALDIpy v0.0.4; compared to v0.0.2:
         1.New function: MALDIpy.projection.umap_projection_subset
         2.New function: MALDIpy.featureplot, which includes four subfunctions (plot1feature,plot1feature_subset,twofeatureplot,twofeatureplot_subset)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `MALDIpy-0.0.3/PKG-INFO` & `MALDIpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: MALDIpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: MALDI-MS data analysis at the single-cell level
 Home-page: https://github.com/TheHumphreysLab
 Author: Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys
 Author-email: haikuolibio@gmail.com
 License: UNKNOWN
-Description: Updates in MALDIpy v0.0.3; compared to v0.0.2:
+Description: Updates in MALDIpy v0.0.4; compared to v0.0.2:
         1.New function: MALDIpy.projection.umap_projection_subset
         2.New function: MALDIpy.featureplot, which includes four subfunctions (plot1feature,plot1feature_subset,twofeatureplot,twofeatureplot_subset)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `MALDIpy-0.0.3/setup.py` & `MALDIpy-0.0.4/setup.py`

 * *Files identical despite different names*


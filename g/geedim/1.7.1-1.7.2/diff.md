# Comparing `tmp/geedim-1.7.1.tar.gz` & `tmp/geedim-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geedim-1.7.1.tar", last modified: Wed May 10 13:45:37 2023, max compression
+gzip compressed data, was "geedim-1.7.2.tar", last modified: Sat Jun 10 19:53:53 2023, max compression
```

## Comparing `geedim-1.7.1.tar` & `geedim-1.7.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.539969 geedim-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 13:45:21.000000 geedim-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-10 13:45:37.539969 geedim-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-10 13:45:21.000000 geedim-1.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.535969 geedim-1.7.1/geedim/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37237 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.539969 geedim-1.7.1/geedim/data/
--rw-r--r--   0 runner    (1001) docker     (123)   119884 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/data/ee_stac_urls.json
--rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/medoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.535969 geedim-1.7.1/geedim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 13:45:21.000000 geedim-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:45:37.539969 geedim-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-10 13:45:21.000000 geedim-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.539969 geedim-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26863 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:53:53.906471 geedim-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 19:53:37.000000 geedim-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-10 19:53:53.906471 geedim-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-10 19:53:37.000000 geedim-1.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:53:53.902471 geedim-1.7.2/geedim/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37237 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:53:53.902471 geedim-1.7.2/geedim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   122757 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/data/ee_stac_urls.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46656 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/medoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 19:53:37.000000 geedim-1.7.2/geedim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:53:53.902471 geedim-1.7.2/geedim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-10 19:53:53.000000 geedim-1.7.2/geedim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-10 19:53:53.000000 geedim-1.7.2/geedim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:53:53.000000 geedim-1.7.2/geedim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-10 19:53:53.000000 geedim-1.7.2/geedim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-10 19:53:53.000000 geedim-1.7.2/geedim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 19:53:53.000000 geedim-1.7.2/geedim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-10 19:53:37.000000 geedim-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:53:53.906471 geedim-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-10 19:53:37.000000 geedim-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:53:53.906471 geedim-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    26863 2023-06-10 19:53:37.000000 geedim-1.7.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-06-10 19:53:37.000000 geedim-1.7.2/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-06-10 19:53:37.000000 geedim-1.7.2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-06-10 19:53:37.000000 geedim-1.7.2/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-10 19:53:37.000000 geedim-1.7.2/tests/test_stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-10 19:53:37.000000 geedim-1.7.2/tests/test_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-10 19:53:37.000000 geedim-1.7.2/tests/test_utils.py
```

### Comparing `geedim-1.7.1/LICENSE` & `geedim-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/PKG-INFO` & `geedim-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geedim
-Version: 1.7.1
+Version: 1.7.2
 Summary: Search, composite and download Google Earth Engine imagery.
 Home-page: https://github.com/leftfield-geospatial/geedim
 Author: Dugal Harris
 Author-email: dugalh@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://geedim.readthedocs.io
 Project-URL: Source, https://github.com/leftfield-geospatial/geedim
```

### Comparing `geedim-1.7.1/README.rst` & `geedim-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/__init__.py` & `geedim-1.7.2/geedim/__init__.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/cli.py` & `geedim-1.7.2/geedim/cli.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/collection.py` & `geedim-1.7.2/geedim/collection.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/data/ee_stac_urls.json` & `geedim-1.7.2/geedim/data/ee_stac_urls.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9738219895287958%*

 * *Differences: {"'CSIC/SPEI/2_8'": "'https://storage.googleapis.com/earthengine-stac/catalog/CSIC/CSIC_SPEI_2_8.json'",*

 * * "'ECMWF/ERA5_LAND/DAILY_AGGR'": "'https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_DAILY_AGGR.json'",*

 * * "'Estonia/Maamet/orthos/mono'": "'https://storage.googleapis.com/earthengine-stac/catalog/Estonia/Estonia_Maamet_orthos_mono.json'",*

 * * "'Estonia/Maamet/orthos/rgb'": "'https://storage.googleapis.com/earthengine-stac/catalog/Estonia/Estonia_Maamet_orthos_rgb.json'",*

 * * "'Latvia […]*

```diff
@@ -57,14 +57,15 @@
     "COPERNICUS/S5P/OFFL/L3_CO": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S5P_OFFL_L3_CO.json",
     "COPERNICUS/S5P/OFFL/L3_HCHO": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S5P_OFFL_L3_HCHO.json",
     "COPERNICUS/S5P/OFFL/L3_NO2": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S5P_OFFL_L3_NO2.json",
     "COPERNICUS/S5P/OFFL/L3_O3": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S5P_OFFL_L3_O3.json",
     "COPERNICUS/S5P/OFFL/L3_O3_TCL": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S5P_OFFL_L3_O3_TCL.json",
     "COPERNICUS/S5P/OFFL/L3_SO2": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S5P_OFFL_L3_SO2.json",
     "CPOM/CryoSat2/ANTARCTICA_DEM": "https://storage.googleapis.com/earthengine-stac/catalog/CPOM/CPOM_CryoSat2_ANTARCTICA_DEM.json",
+    "CSIC/SPEI/2_8": "https://storage.googleapis.com/earthengine-stac/catalog/CSIC/CSIC_SPEI_2_8.json",
     "CSIRO/SLGA": "https://storage.googleapis.com/earthengine-stac/catalog/CSIRO/CSIRO_SLGA.json",
     "CSP/ERGo/1_0/Global/ALOS_CHILI": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_Global_ALOS_CHILI.json",
     "CSP/ERGo/1_0/Global/ALOS_landforms": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_Global_ALOS_landforms.json",
     "CSP/ERGo/1_0/Global/ALOS_mTPI": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_Global_ALOS_mTPI.json",
     "CSP/ERGo/1_0/Global/ALOS_topoDiversity": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_Global_ALOS_topoDiversity.json",
     "CSP/ERGo/1_0/Global/SRTM_CHILI": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_Global_SRTM_CHILI.json",
     "CSP/ERGo/1_0/Global/SRTM_landforms": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_Global_SRTM_landforms.json",
@@ -79,24 +80,26 @@
     "CSP/ERGo/1_0/US/topoDiversity": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_US_topoDiversity.json",
     "CSP/HM/GlobalHumanModification": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_HM_GlobalHumanModification.json",
     "DLR/WSF/WSF2015/v1": "https://storage.googleapis.com/earthengine-stac/catalog/DLR/DLR_WSF_WSF2015_v1.json",
     "DOE/ORNL/LandScan_HD/Ukraine_202201": "https://storage.googleapis.com/earthengine-stac/catalog/DOE/DOE_ORNL_LandScan_HD_Ukraine_202201.json",
     "ECMWF/CAMS/NRT": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_CAMS_NRT.json",
     "ECMWF/ERA5/DAILY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_DAILY.json",
     "ECMWF/ERA5/MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_MONTHLY.json",
-    "ECMWF/ERA5_LAND/DAILY_RAW": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_DAILY_RAW.json",
+    "ECMWF/ERA5_LAND/DAILY_AGGR": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_DAILY_AGGR.json",
     "ECMWF/ERA5_LAND/HOURLY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_HOURLY.json",
     "ECMWF/ERA5_LAND/MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_MONTHLY.json",
     "ECMWF/ERA5_LAND/MONTHLY_AGGR": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_MONTHLY_AGGR.json",
     "ECMWF/ERA5_LAND/MONTHLY_BY_HOUR": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_MONTHLY_BY_HOUR.json",
     "EO1/HYPERION": "https://storage.googleapis.com/earthengine-stac/catalog/EO1/EO1_HYPERION.json",
     "ESA/CCI/FireCCI/5_1": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_CCI_FireCCI_5_1.json",
     "ESA/GLOBCOVER_L4_200901_200912_V2_3": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_GLOBCOVER_L4_200901_200912_V2_3.json",
     "ESA/WorldCover/v100": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_WorldCover_v100.json",
     "ESA/WorldCover/v200": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_WorldCover_v200.json",
+    "Estonia/Maamet/orthos/mono": "https://storage.googleapis.com/earthengine-stac/catalog/Estonia/Estonia_Maamet_orthos_mono.json",
+    "Estonia/Maamet/orthos/rgb": "https://storage.googleapis.com/earthengine-stac/catalog/Estonia/Estonia_Maamet_orthos_rgb.json",
     "FAO/GHG/1/DROSA_A": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_GHG_1_DROSA_A.json",
     "FAO/GHG/1/DROSE_A": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_GHG_1_DROSE_A.json",
     "FAO/SOFO/1/FPP": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_SOFO_1_FPP.json",
     "FAO/SOFO/1/TPP": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_SOFO_1_TPP.json",
     "FAO/WAPOR/2/L1_AETI_D": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_AETI_D.json",
     "FAO/WAPOR/2/L1_E_D": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_E_D.json",
     "FAO/WAPOR/2/L1_I_D": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_I_D.json",
@@ -537,14 +540,16 @@
     "LANDSAT/LT5_L1T_ANNUAL_TOA": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_LT5_L1T_ANNUAL_TOA.json",
     "LANDSAT/LT5_L1T_TOA": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_LT5_L1T_TOA.json",
     "LANDSAT/MANGROVE_FORESTS": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_MANGROVE_FORESTS.json",
     "LARSE/GEDI/GEDI02_A_002_MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI02_A_002_MONTHLY.json",
     "LARSE/GEDI/GEDI02_B_002_MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI02_B_002_MONTHLY.json",
     "LARSE/GEDI/GEDI04_A_002_MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI04_A_002_MONTHLY.json",
     "LARSE/GEDI/GEDI04_B_002": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI04_B_002.json",
+    "Latvia/Maamet/orthos/cir": "https://storage.googleapis.com/earthengine-stac/catalog/Latvia/Latvia_Maamet_orthos_cir.json",
+    "Latvia/Maamet/orthos/rgb": "https://storage.googleapis.com/earthengine-stac/catalog/Latvia/Latvia_Maamet_orthos_rgb.json",
     "MERIT/DEM/v1_0_3": "https://storage.googleapis.com/earthengine-stac/catalog/MERIT/MERIT_DEM_v1_0_3.json",
     "MERIT/Hydro/v1_0_1": "https://storage.googleapis.com/earthengine-stac/catalog/MERIT/MERIT_Hydro_v1_0_1.json",
     "MERIT/Hydro_reduced/v1_0_1": "https://storage.googleapis.com/earthengine-stac/catalog/MERIT/MERIT_Hydro_reduced_v1_0_1.json",
     "MODIS/006/MCD12Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MCD12Q1.json",
     "MODIS/006/MCD12Q2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MCD12Q2.json",
     "MODIS/006/MCD15A3H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MCD15A3H.json",
     "MODIS/006/MCD19A2_GRANULES": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MCD19A2_GRANULES.json",
@@ -594,45 +599,49 @@
     "MODIS/006/MYD17A3HGF": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYD17A3HGF.json",
     "MODIS/006/MYDOCGA": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYDOCGA.json",
     "MODIS/055/MOD17A3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_055_MOD17A3.json",
     "MODIS/061/MCD12Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD12Q1.json",
     "MODIS/061/MCD12Q2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD12Q2.json",
     "MODIS/061/MCD15A3H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD15A3H.json",
     "MODIS/061/MCD18C2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD18C2.json",
+    "MODIS/061/MCD19A2_GRANULES": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD19A2_GRANULES.json",
     "MODIS/061/MCD43A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A1.json",
     "MODIS/061/MCD43A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A2.json",
     "MODIS/061/MCD43A3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A3.json",
     "MODIS/061/MCD43A4": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A4.json",
     "MODIS/061/MCD43C3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43C3.json",
     "MODIS/061/MCD64A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD64A1.json",
     "MODIS/061/MOD08_M3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD08_M3.json",
     "MODIS/061/MOD09A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09A1.json",
     "MODIS/061/MOD09CMG": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09CMG.json",
     "MODIS/061/MOD09GA": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09GA.json",
     "MODIS/061/MOD09GQ": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09GQ.json",
     "MODIS/061/MOD09Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09Q1.json",
+    "MODIS/061/MOD10A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD10A1.json",
     "MODIS/061/MOD11A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD11A1.json",
     "MODIS/061/MOD11A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD11A2.json",
     "MODIS/061/MOD13A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD13A1.json",
     "MODIS/061/MOD13A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD13A2.json",
     "MODIS/061/MOD13Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD13Q1.json",
     "MODIS/061/MOD14A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD14A1.json",
     "MODIS/061/MOD14A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD14A2.json",
     "MODIS/061/MOD15A2H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD15A2H.json",
+    "MODIS/061/MOD16A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD16A2.json",
     "MODIS/061/MOD17A3HGF": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD17A3HGF.json",
     "MODIS/061/MOD21A1D": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21A1D.json",
     "MODIS/061/MOD21A1N": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21A1N.json",
     "MODIS/061/MOD21C1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21C1.json",
     "MODIS/061/MOD21C2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21C2.json",
     "MODIS/061/MOD21C3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21C3.json",
     "MODIS/061/MYD08_M3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD08_M3.json",
     "MODIS/061/MYD09A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09A1.json",
     "MODIS/061/MYD09GA": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09GA.json",
     "MODIS/061/MYD09GQ": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09GQ.json",
     "MODIS/061/MYD09Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09Q1.json",
+    "MODIS/061/MYD10A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD10A1.json",
     "MODIS/061/MYD11A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD11A1.json",
     "MODIS/061/MYD11A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD11A2.json",
     "MODIS/061/MYD13A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD13A1.json",
     "MODIS/061/MYD13A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD13A2.json",
     "MODIS/061/MYD13Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD13Q1.json",
     "MODIS/061/MYD14A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD14A1.json",
     "MODIS/061/MYD14A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD14A2.json",
@@ -782,29 +791,37 @@
     "NOAA/VIIRS/001/VNP09H1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP09H1.json",
     "NOAA/VIIRS/001/VNP13A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP13A1.json",
     "NOAA/VIIRS/001/VNP14A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP14A1.json",
     "NOAA/VIIRS/001/VNP15A2H": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP15A2H.json",
     "NOAA/VIIRS/001/VNP21A1D": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP21A1D.json",
     "NOAA/VIIRS/001/VNP21A1N": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP21A1N.json",
     "NOAA/VIIRS/001/VNP22Q2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP22Q2.json",
+    "NOAA/VIIRS/001/VNP43IA1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP43IA1.json",
+    "NOAA/VIIRS/001/VNP43IA2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP43IA2.json",
+    "NOAA/VIIRS/001/VNP46A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP46A1.json",
     "NOAA/VIIRS/001/VNP46A2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP46A2.json",
     "NOAA/VIIRS/001/VNP64A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP64A1.json",
     "NOAA/VIIRS/DNB/MONTHLY_V1/VCMCFG": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_DNB_MONTHLY_V1_VCMCFG.json",
     "NOAA/VIIRS/DNB/MONTHLY_V1/VCMSLCFG": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_DNB_MONTHLY_V1_VCMSLCFG.json",
     "NRCan/CDEM": "https://storage.googleapis.com/earthengine-stac/catalog/NRCan/NRCan_CDEM.json",
     "OREGONSTATE/PRISM/AN81d": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_AN81d.json",
     "OREGONSTATE/PRISM/AN81m": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_AN81m.json",
     "OREGONSTATE/PRISM/Norm81m": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_Norm81m.json",
     "OREGONSTATE/PRISM/Norm91m": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_Norm91m.json",
-    "ORTHO/Switzerland/SWISSIMAGE/10cm": "https://storage.googleapis.com/earthengine-stac/catalog/ORTHO/ORTHO_Switzerland_SWISSIMAGE_10cm.json",
     "OSU/GIMP/2000_ICE_OCEAN_MASK": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_2000_ICE_OCEAN_MASK.json",
     "OSU/GIMP/2000_IMAGERY_MOSAIC": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_2000_IMAGERY_MOSAIC.json",
     "OSU/GIMP/DEM": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_DEM.json",
     "OSU/GIMP/ICE_VELOCITY_OPT": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_ICE_VELOCITY_OPT.json",
+    "OpenET/DISALEXI/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_DISALEXI_CONUS_GRIDMET_MONTHLY_v2_0.json",
+    "OpenET/EEMETRIC/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_EEMETRIC_CONUS_GRIDMET_MONTHLY_v2_0.json",
     "OpenET/ENSEMBLE/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_ENSEMBLE_CONUS_GRIDMET_MONTHLY_v2_0.json",
+    "OpenET/GEESEBAL/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_GEESEBAL_CONUS_GRIDMET_MONTHLY_v2_0.json",
+    "OpenET/PTJPL/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_PTJPL_CONUS_GRIDMET_MONTHLY_v2_0.json",
+    "OpenET/SIMS/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_SIMS_CONUS_GRIDMET_MONTHLY_v2_0.json",
+    "OpenET/SSEBOP/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_SSEBOP_CONUS_GRIDMET_MONTHLY_v2_0.json",
     "OpenLandMap/CLM/CLM_LST_MOD11A2-DAYNIGHT_M/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_LST_MOD11A2-DAYNIGHT_M_v01.json",
     "OpenLandMap/CLM/CLM_LST_MOD11A2-DAY_M/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_LST_MOD11A2-DAY_M_v01.json",
     "OpenLandMap/CLM/CLM_LST_MOD11A2-DAY_SD/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_LST_MOD11A2-DAY_SD_v01.json",
     "OpenLandMap/CLM/CLM_PRECIPITATION_SM2RAIN_M/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_PRECIPITATION_SM2RAIN_M_v01.json",
     "OpenLandMap/PNV/PNV_BIOME-TYPE_BIOME00K_C/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_PNV_PNV_BIOME-TYPE_BIOME00K_C_v01.json",
     "OpenLandMap/PNV/PNV_FAPAR_PROBA-V_D/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_PNV_PNV_FAPAR_PROBA-V_D_v01.json",
     "OpenLandMap/SOL/SOL_BULKDENS-FINEEARTH_USDA-4A1H_M/v02": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_SOL_SOL_BULKDENS-FINEEARTH_USDA-4A1H_M_v02.json",
@@ -827,14 +844,15 @@
     "Oxford/MAP/friction_surface_2015_v1_0": "https://storage.googleapis.com/earthengine-stac/catalog/Oxford/Oxford_MAP_friction_surface_2015_v1_0.json",
     "Oxford/MAP/friction_surface_2019": "https://storage.googleapis.com/earthengine-stac/catalog/Oxford/Oxford_MAP_friction_surface_2019.json",
     "RUB/RUBCLIM/LCZ/global_lcz_map/v1": "https://storage.googleapis.com/earthengine-stac/catalog/RUB/RUB_RUBCLIM_LCZ_global_lcz_map_v1.json",
     "SKYSAT/GEN-A/PUBLIC/ORTHO/MULTISPECTRAL": "https://storage.googleapis.com/earthengine-stac/catalog/SKYSAT/SKYSAT_GEN-A_PUBLIC_ORTHO_MULTISPECTRAL.json",
     "SKYSAT/GEN-A/PUBLIC/ORTHO/RGB": "https://storage.googleapis.com/earthengine-stac/catalog/SKYSAT/SKYSAT_GEN-A_PUBLIC_ORTHO_RGB.json",
     "SNU/ESL/BESS/Rad/v1": "https://storage.googleapis.com/earthengine-stac/catalog/SNU/SNU_ESL_BESS_Rad_v1.json",
     "Spain/PNOA/PNOA10": "https://storage.googleapis.com/earthengine-stac/catalog/Spain/Spain_PNOA_PNOA10.json",
+    "Switzerland/SWISSIMAGE/orthos/10cm": "https://storage.googleapis.com/earthengine-stac/catalog/Switzerland/Switzerland_SWISSIMAGE_orthos_10cm.json",
     "TERN/AET/CMRSET_LANDSAT_V2_1": "https://storage.googleapis.com/earthengine-stac/catalog/TERN/TERN_AET_CMRSET_LANDSAT_V2_1.json",
     "TERN/AET/CMRSET_LANDSAT_V2_2": "https://storage.googleapis.com/earthengine-stac/catalog/TERN/TERN_AET_CMRSET_LANDSAT_V2_2.json",
     "TOMS/MERGED": "https://storage.googleapis.com/earthengine-stac/catalog/TOMS/TOMS_MERGED.json",
     "TRMM/3B42": "https://storage.googleapis.com/earthengine-stac/catalog/TRMM/TRMM_3B42.json",
     "TRMM/3B43V7": "https://storage.googleapis.com/earthengine-stac/catalog/TRMM/TRMM_3B43V7.json",
     "TUBerlin/BigEarthNet/v1": "https://storage.googleapis.com/earthengine-stac/catalog/TUBerlin/TUBerlin_BigEarthNet_v1.json",
     "Tsinghua/DESS/ChinaTerraceMap/v1": "https://storage.googleapis.com/earthengine-stac/catalog/Tsinghua/Tsinghua_DESS_ChinaTerraceMap_v1.json",
@@ -848,14 +866,15 @@
     "UMD/hansen/global_forest_change_2015_v1_3": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2015_v1_3.json",
     "UMD/hansen/global_forest_change_2016_v1_4": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2016_v1_4.json",
     "UMD/hansen/global_forest_change_2017_v1_5": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2017_v1_5.json",
     "UMD/hansen/global_forest_change_2018_v1_6": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2018_v1_6.json",
     "UMD/hansen/global_forest_change_2019_v1_7": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2019_v1_7.json",
     "UMD/hansen/global_forest_change_2020_v1_8": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2020_v1_8.json",
     "UMD/hansen/global_forest_change_2021_v1_9": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2021_v1_9.json",
+    "UMD/hansen/global_forest_change_2022_v1_10": "https://storage.googleapis.com/earthengine-stac/catalog/UMD/UMD_hansen_global_forest_change_2022_v1_10.json",
     "UMN/PGC/ArcticDEM/V2/2m": "https://storage.googleapis.com/earthengine-stac/catalog/UMN/UMN_PGC_ArcticDEM_V2_2m.json",
     "UMN/PGC/ArcticDEM/V2/5m": "https://storage.googleapis.com/earthengine-stac/catalog/UMN/UMN_PGC_ArcticDEM_V2_5m.json",
     "UMN/PGC/ArcticDEM/V3/2m": "https://storage.googleapis.com/earthengine-stac/catalog/UMN/UMN_PGC_ArcticDEM_V3_2m.json",
     "UMN/PGC/ArcticDEM/V3/2m_mosaic": "https://storage.googleapis.com/earthengine-stac/catalog/UMN/UMN_PGC_ArcticDEM_V3_2m_mosaic.json",
     "UMN/PGC/REMA/V1/2m": "https://storage.googleapis.com/earthengine-stac/catalog/UMN/UMN_PGC_REMA_V1_2m.json",
     "UMN/PGC/REMA/V1/8m": "https://storage.googleapis.com/earthengine-stac/catalog/UMN/UMN_PGC_REMA_V1_8m.json",
     "UMN/PGC/REMA/V1_1/8m": "https://storage.googleapis.com/earthengine-stac/catalog/UMN/UMN_PGC_REMA_V1_1_8m.json",
@@ -868,14 +887,15 @@
     "UQ/murray/Intertidal/v1_1/global_intertidal": "https://storage.googleapis.com/earthengine-stac/catalog/UQ/UQ_murray_Intertidal_v1_1_global_intertidal.json",
     "UQ/murray/Intertidal/v1_1/qa_pixel_count": "https://storage.googleapis.com/earthengine-stac/catalog/UQ/UQ_murray_Intertidal_v1_1_qa_pixel_count.json",
     "USDA/NAIP/DOQQ": "https://storage.googleapis.com/earthengine-stac/catalog/USDA/USDA_NAIP_DOQQ.json",
     "USDA/NASS/CDL": "https://storage.googleapis.com/earthengine-stac/catalog/USDA/USDA_NASS_CDL.json",
     "USFS/GTAC/LCMS/v2020-5": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_LCMS_v2020-5.json",
     "USFS/GTAC/LCMS/v2020-6": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_LCMS_v2020-6.json",
     "USFS/GTAC/LCMS/v2021-7": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_LCMS_v2021-7.json",
+    "USFS/GTAC/LCMS/v2022-8": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_LCMS_v2022-8.json",
     "USFS/GTAC/MTBS/annual_burn_severity_mosaics/v1": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_MTBS_annual_burn_severity_mosaics_v1.json",
     "USGS/3DEP/10m": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_3DEP_10m.json",
     "USGS/3DEP/1m": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_3DEP_1m.json",
     "USGS/GAP/AK/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_AK_2001.json",
     "USGS/GAP/CONUS/2011": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_CONUS_2011.json",
     "USGS/GAP/HI/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_HI_2001.json",
     "USGS/GAP/PR/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_PR_2001.json",
@@ -924,11 +944,12 @@
     "WorldPop/POP": "https://storage.googleapis.com/earthengine-stac/catalog/WorldPop/WorldPop_POP.json",
     "YALE/YCEO/UHI/Summer_UHI_yearly_pixel/v4": "https://storage.googleapis.com/earthengine-stac/catalog/YALE/YALE_YCEO_UHI_Summer_UHI_yearly_pixel_v4.json",
     "YALE/YCEO/UHI/UHI_all_averaged/v4": "https://storage.googleapis.com/earthengine-stac/catalog/YALE/YALE_YCEO_UHI_UHI_all_averaged_v4.json",
     "YALE/YCEO/UHI/UHI_monthly_averaged/v4": "https://storage.googleapis.com/earthengine-stac/catalog/YALE/YALE_YCEO_UHI_UHI_monthly_averaged_v4.json",
     "YALE/YCEO/UHI/UHI_yearly_averaged/v4": "https://storage.googleapis.com/earthengine-stac/catalog/YALE/YALE_YCEO_UHI_UHI_yearly_averaged_v4.json",
     "YALE/YCEO/UHI/UHI_yearly_pixel/v4": "https://storage.googleapis.com/earthengine-stac/catalog/YALE/YALE_YCEO_UHI_UHI_yearly_pixel_v4.json",
     "YALE/YCEO/UHI/Winter_UHI_yearly_pixel/v4": "https://storage.googleapis.com/earthengine-stac/catalog/YALE/YALE_YCEO_UHI_Winter_UHI_yearly_pixel_v4.json",
+    "projects/ngis-cat/assets/DEA/NIDEM": "https://storage.googleapis.com/earthengine-stac/catalog/ngis-cat/projects_ngis-cat_assets_DEA_NIDEM.json",
     "projects/planet-nicfi/assets/basemaps/africa": "https://storage.googleapis.com/earthengine-stac/catalog/planet-nicfi/projects_planet-nicfi_assets_basemaps_africa.json",
     "projects/planet-nicfi/assets/basemaps/americas": "https://storage.googleapis.com/earthengine-stac/catalog/planet-nicfi/projects_planet-nicfi_assets_basemaps_americas.json",
     "projects/planet-nicfi/assets/basemaps/asia": "https://storage.googleapis.com/earthengine-stac/catalog/planet-nicfi/projects_planet-nicfi_assets_basemaps_asia.json"
 }
```

### Comparing `geedim-1.7.1/geedim/download.py` & `geedim-1.7.2/geedim/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,27 +609,33 @@
             tile_size = tile_shape[0] * tile_shape[1] * pixel_size
 
         tile_shape[tile_shape > max_tile_dim] = max_tile_dim
         num_tiles = int(np.product(np.ceil(image_shape / tile_shape)))
         tile_shape = tuple(tile_shape.tolist())
         return tile_shape, num_tiles
 
-    @staticmethod
-    def _build_overviews(dataset: rio.io.DatasetWriter, max_num_levels: int = 8, min_ovw_pixels: int = 256):
-        """ Build internal overviews, downsampled by successive powers of 2, for an open rasterio dataset. """
-        if dataset.closed:
-            raise IOError('Image dataset is closed')
+    def _build_overviews(self, filename: Union[str, pathlib.Path], max_num_levels: int = 8, min_ovw_pixels: int = 256):
+        """ Build internal overviews, downsampled by successive powers of 2, for a given filename. """
 
-        # limit overviews so that the highest level has at least 2**8=256 pixels along the shortest dimension,
-        # and so there are no more than 8 levels.
-        max_ovw_levels = int(np.min(np.log2(dataset.shape)))
-        min_level_shape_pow2 = int(np.log2(min_ovw_pixels))
-        num_ovw_levels = np.min([max_num_levels, max_ovw_levels - min_level_shape_pow2])
-        ovw_levels = [2**m for m in range(1, num_ovw_levels + 1)]
-        dataset.build_overviews(ovw_levels, RioResampling.average)
+        # TODO: revisit multi-threaded overviews on gdal update
+        # build overviews in a single threaded environment (currently gdal reports errors when building overviews
+        # with GDAL_NUM_THREADS='ALL_CPUs' - see https://github.com/OSGeo/gdal/issues/7921)
+        env_dict = dict(GTIFF_FORCE_RGBA=False, COMPRESS_OVERVIEW='DEFLATE')
+        if self.size >= 4e9:
+            env_dict.update(BIGTIFF_OVERVIEW=True)
+
+        with rio.Env(**env_dict), rio.open(filename, 'r+') as ds:
+            # limit overviews so that the highest level has at least 2**8=256 pixels along the shortest dimension,
+            # and so there are no more than 8 levels.
+            max_ovw_levels = int(np.min(np.log2(ds.shape)))
+            min_level_shape_pow2 = int(np.log2(min_ovw_pixels))
+            num_ovw_levels = np.min([max_num_levels, max_ovw_levels - min_level_shape_pow2])
+            ovw_levels = [2**m for m in range(1, num_ovw_levels + 1)]
+            with utils.suppress_rio_logs(logging.CRITICAL):
+                ds.build_overviews(ovw_levels, RioResampling.average)
 
     def _write_metadata(self, dataset: rio.io.DatasetWriter):
         """ Write Earth Engine and STAC metadata to an open rasterio dataset. """
         if dataset.closed:
             raise IOError('Image dataset is closed')
 
         # replace 'system:*' property keys with 'system-*', and remove footprint if its there
@@ -945,10 +951,12 @@
                         future.result()
                 except Exception as ex:
                     logger.info(f'Exception: {str(ex)}\nCancelling...')
                     executor.shutdown(wait=False)
                     raise ex
 
             bar.update(bar.total - bar.n)   # ensure the bar reaches 100%
-            # populate GeoTIFF metadata and build overviews
+            # populate GeoTIFF metadata
             exp_image._write_metadata(out_ds)
-            BaseImage._build_overviews(out_ds)
+
+        # build overviews
+        exp_image._build_overviews(filename)
```

### Comparing `geedim-1.7.1/geedim/enums.py` & `geedim-1.7.2/geedim/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 
     asset = 'asset'
     """ Export to an Earth Engine asset. """
 
     cloud = 'cloud'
     """ Export to Google Cloud Storage. """
 
+
 class SpectralDistanceMetric(str, Enum):
     """ Enumeration for the spectral distance metric. """
     sam = 'sam'
     """ Spectral angle mapper. """
 
     sid = 'sid'
     """ Spectral information divergence. """
```

### Comparing `geedim-1.7.1/geedim/errors.py` & `geedim-1.7.2/geedim/errors.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/mask.py` & `geedim-1.7.2/geedim/mask.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/medoid.py` & `geedim-1.7.2/geedim/medoid.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/schema.py` & `geedim-1.7.2/geedim/schema.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/stac.py` & `geedim-1.7.2/geedim/stac.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/geedim/tile.py` & `geedim-1.7.2/geedim/tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         # extract geotiff from zipped buffer into another buffer
         zip_file = zipfile.ZipFile(zip_buffer)
         ext_buffer = BytesIO(zip_file.read(zip_file.filelist[0]))
 
         # read the geotiff with a rasterio memory file
         env = rio.Env(GDAL_NUM_THREADS='ALL_CPUs', GTIFF_FORCE_RGBA=False)
-        with utils.suppress_rio_warn_logs(), env, MemoryFile(ext_buffer) as mem_file:
+        with utils.suppress_rio_logs(), env, MemoryFile(ext_buffer) as mem_file:
             with mem_file.open() as ds:
                 array = ds.read()
                 if (array.dtype == np.dtype('float32')) or (array.dtype == np.dtype('float64')):
                     # GEE sets nodata to -inf for float data types, (but does not populate the nodata field).
                     # rasterio won't allow nodata=-inf, so this is a workaround to change nodata to nan at source.
                     array[np.isinf(array)] = np.nan
```

### Comparing `geedim-1.7.1/geedim/utils.py` & `geedim-1.7.2/geedim/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,21 +105,21 @@
         return None, None
     index = image_id.split("/")[-1]
     ee_coll_name = "/".join(image_id.split("/")[:-1])
     return ee_coll_name, index
 
 
 @contextmanager
-def suppress_rio_warn_logs():
-    """ A context manager that sets the `rasterio` logging level to ERROR, then returns it to its original value. """
+def suppress_rio_logs(level: int = logging.ERROR):
+    """ A context manager that sets the `rasterio` logging level, then returns it to its original value. """
     try:
         # GEE sets GeoTIFF `colorinterp` tags incorrectly. This suppresses `rasterio` warning relating to this:
         # 'Sum of Photometric type-related color channels and ExtraSamples doesn't match SamplesPerPixel'
         rio_level = logging.getLogger('rasterio').getEffectiveLevel()
-        logging.getLogger('rasterio').setLevel(logging.ERROR)
+        logging.getLogger('rasterio').setLevel(level)
         yield
     finally:
         logging.getLogger('rasterio').setLevel(rio_level)
 
 
 def get_bounds(filename: pathlib.Path, expand: float = 5):
     """
@@ -133,15 +133,15 @@
         Percentage (0-100) by which to expand the bounds (default: 5).
 
     Returns
     -------
     dict
         Geojson polygon.
     """
-    with suppress_rio_warn_logs(), rio.Env(GTIFF_FORCE_RGBA=False), rio.open(filename) as im:
+    with suppress_rio_logs(), rio.Env(GTIFF_FORCE_RGBA=False), rio.open(filename) as im:
         bbox = im.bounds
         if (im.crs.linear_units == "metre") and (expand > 0):  # expand the bounding box
             expand_x = (bbox.right - bbox.left) * expand / 100.0
             expand_y = (bbox.top - bbox.bottom) * expand / 100.0
             bbox_expand = rio.coords.BoundingBox(
                 bbox.left - expand_x, bbox.bottom - expand_y, bbox.right + expand_x, bbox.top + expand_y
             )
```

### Comparing `geedim-1.7.1/geedim.egg-info/PKG-INFO` & `geedim-1.7.2/geedim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geedim
-Version: 1.7.1
+Version: 1.7.2
 Summary: Search, composite and download Google Earth Engine imagery.
 Home-page: https://github.com/leftfield-geospatial/geedim
 Author: Dugal Harris
 Author-email: dugalh@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://geedim.readthedocs.io
 Project-URL: Source, https://github.com/leftfield-geospatial/geedim
```

### Comparing `geedim-1.7.1/geedim.egg-info/SOURCES.txt` & `geedim-1.7.2/geedim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/setup.py` & `geedim-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/tests/test_cli.py` & `geedim-1.7.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/tests/test_collection.py` & `geedim-1.7.2/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/tests/test_download.py` & `geedim-1.7.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/tests/test_mask.py` & `geedim-1.7.2/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/tests/test_stac.py` & `geedim-1.7.2/tests/test_stac.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/tests/test_tile.py` & `geedim-1.7.2/tests/test_tile.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.1/tests/test_utils.py` & `geedim-1.7.2/tests/test_utils.py`

 * *Files identical despite different names*


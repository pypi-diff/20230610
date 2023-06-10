# Comparing `tmp/momlevel-0.0.8.tar.gz` & `tmp/momlevel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momlevel-0.0.8.tar", last modified: Wed Apr 19 20:24:22 2023, max compression
+gzip compressed data, was "momlevel-0.0.9.tar", last modified: Sat Jun 10 12:33:07 2023, max compression
```

## Comparing `momlevel-0.0.8.tar` & `momlevel-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-19 20:24:10.000000 momlevel-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-19 20:24:22.621268 momlevel-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-19 20:24:10.000000 momlevel-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 20:24:10.000000 momlevel-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:24:22.621268 momlevel-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/momlevel/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/momlevel/eos/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/eos/wright.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/resources/
--rw-r--r--   0 runner    (1001) docker     (123) 18167522 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/CM4_historical.nc
--rw-r--r--   0 runner    (1001) docker     (123)   801596 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/NWA12_grid_dataframe.csv
--rw-r--r--   0 runner    (1001) docker     (123)  3377003 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/NWA12_sample_grid_data.nc
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/geolocate_points_reference.csv
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/global_tide_gauges.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/us_tide_gauges.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/spice/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/spice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/spice/flament.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/steric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/test_data/tripolar/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/tripolar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/tripolar/horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/tripolar/vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/tidegauge.py
--rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/trend.py
--rw-r--r--   0 runner    (1001) docker     (123)    23591 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/momlevel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_derived.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_flament.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_steric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_tidegauge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_trend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_wright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.604174 momlevel-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-10 12:32:49.000000 momlevel-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-10 12:33:07.604174 momlevel-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-10 12:32:49.000000 momlevel-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-10 12:32:49.000000 momlevel-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 12:33:07.604174 momlevel-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.576173 momlevel-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.580174 momlevel-0.0.9/src/momlevel/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-10 12:32:49.000000 momlevel-0.0.9/src/momlevel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24885 2023-06-10 12:32:49.000000 momlevel-0.0.9/src/momlevel/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-10 12:32:49.000000 momlevel-0.0.9/src/momlevel/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.580174 momlevel-0.0.9/src/momlevel/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-10 12:32:49.000000 momlevel-0.0.9/src/momlevel/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-10 12:32:49.000000 momlevel-0.0.9/src/momlevel/eos/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-10 12:32:49.000000 momlevel-0.0.9/src/momlevel/eos/wright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-10 12:32:49.000000 momlevel-0.0.9/src/momlevel/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.600174 momlevel-0.0.9/src/momlevel/resources/
+-rw-r--r--   0 runner    (1001) docker     (123) 18167522 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/resources/CM4_historical.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   801596 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/resources/NWA12_grid_dataframe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  3377003 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/resources/NWA12_sample_grid_data.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/resources/geolocate_points_reference.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/resources/global_tide_gauges.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/resources/us_tide_gauges.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.600174 momlevel-0.0.9/src/momlevel/spice/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/spice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/spice/flament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/steric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.600174 momlevel-0.0.9/src/momlevel/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/test_data/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.600174 momlevel-0.0.9/src/momlevel/test_data/tripolar/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/test_data/tripolar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/test_data/tripolar/horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/test_data/tripolar/vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/tidegauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23591 2023-06-10 12:32:50.000000 momlevel-0.0.9/src/momlevel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.580174 momlevel-0.0.9/src/momlevel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-10 12:33:07.000000 momlevel-0.0.9/src/momlevel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-10 12:33:07.000000 momlevel-0.0.9/src/momlevel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 12:33:07.000000 momlevel-0.0.9/src/momlevel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 12:33:07.000000 momlevel-0.0.9/src/momlevel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 12:33:07.000000 momlevel-0.0.9/src/momlevel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 12:33:07.604174 momlevel-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_flament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_steric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_tidegauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-10 12:32:50.000000 momlevel-0.0.9/tests/test_wright.py
```

### Comparing `momlevel-0.0.8/LICENSE.txt` & `momlevel-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/PKG-INFO` & `momlevel-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momlevel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to diagnose sea level in the MOM Ocean Model
 Author-email: John Krasting <john.krasting@noaa.gov>
 License: Software code created by U.S. Government employees is not subject to copyright in the United States (17 U.S.C. §105).
         The United States/Department of Commerce reserve all rights to seek and obtain copyright protection in countries
         otherthan the United States for Software authored in its entirety by the Department of Commerce. To this end, the
         Department of Commerce hereby grants to Recipient a royalty-free, nonexclusive license to use, copy, and create 
         derivative works of the Software outside of the United States.”
```

### Comparing `momlevel-0.0.8/README.md` & `momlevel-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/pyproject.toml` & `momlevel-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/__init__.py` & `momlevel-0.0.9/src/momlevel/__init__.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/derived.py` & `momlevel-0.0.9/src/momlevel/derived.py`

 * *Files 5% similar despite different names*

```diff
@@ -242,29 +242,38 @@
         "standard_name": "ocean_relative_vorticity",
         "long_name": "Ocean relative vorticity",
         "units": "s-1",
     }
     return relvort
 
 
-def calc_dz(levels, interfaces, depth, fraction=False):
+def calc_dz(levels, interfaces, depth, top=0.0, bottom=None, fraction=False):
     """Function to calculate dz that accounts for partial bottom cells
 
     This function uses the 2-dimensional bathymetry and the vertical
     coordinate levels and interfaces to calculate a 3-dimensional
     dz field that properly accounts for partial bottom cells.
 
+    A specific depth range can be provided using the `top` and `bottom`
+    arguments to request dz over a specified depth range.
+
     Parameters
     ----------
     levels : xarray.core.dataarray.DataArray
         Vertical coordinate cell centers (1-dimensional)
     interfaces : xarray.core.dataarray.DataArray
         Vertical coordinate cell interfaces (1-dimensional)
     depth : xarray.core.dataarray.DataArray
         Bathymetry field in same units as coordinate (2-dimensional)
+    top : float
+        Upper bound if a specific depth range is requested.
+        Must be in the same units as `depth`, by default 0.0
+    bottom : float
+        Lower bound if a specific depth range is requested.
+        Must be in the same units as `depth`, by default None
     fraction : bool
         If True, return fraction of cell. If False, return raw dz,
         by default False
 
     Returns
     -------
     xarray.core.dataarray.DataArray
@@ -281,30 +290,37 @@
     assert bool(
         np.all(interfaces >= 0)
     ), "Vertical coordinate interfaces must all be positive-definite"
 
     # fill missing values with zero
     depth = depth.fillna(0.0)
 
+    # use bottom boundary if depth range is specified
+    depth = np.minimum(depth, bottom) if bottom is not None else depth
+
     # broadcast to common dimensions
     ztop = xr.DataArray(interfaces[0:-1].values, coords=levels.coords)
     _, ztop = xr.broadcast(depth, ztop)
     zbot = xr.DataArray(interfaces[1::].values, coords=levels.coords)
     _, zbot = xr.broadcast(depth, zbot)
     depth = depth.broadcast_like(levels)
 
     # get pure dz
     dz_field = zbot - ztop
 
-    # calculate partial cell
+    # calculate partial cell based on bottom boundary
     part = depth - ztop
     part = xr.where(part < 0.0, 0.0, part)
-
     result = np.minimum(part, dz_field)
 
+    # calculate partial cell based on top boundary
+    part = zbot - top
+    part = xr.where(part < 0.0, 0.0, part)
+    result = np.minimum(part, result)
+
     if fraction:
         _dz_field = xr.where(dz_field == 0, np.nan, dz_field)
         _dz_part = xr.where(result == 0, np.nan, result)
         result = _dz_part / _dz_field
 
     return result
```

### Comparing `momlevel-0.0.8/src/momlevel/dynamic.py` & `momlevel-0.0.9/src/momlevel/dynamic.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/eos/wright.py` & `momlevel-0.0.9/src/momlevel/eos/wright.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/reference.py` & `momlevel-0.0.9/src/momlevel/reference.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/resources/CM4_historical.nc` & `momlevel-0.0.9/src/momlevel/resources/CM4_historical.nc`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/resources/NWA12_grid_dataframe.csv` & `momlevel-0.0.9/src/momlevel/resources/NWA12_grid_dataframe.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/resources/NWA12_sample_grid_data.nc` & `momlevel-0.0.9/src/momlevel/resources/NWA12_sample_grid_data.nc`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/resources/geolocate_points_reference.csv` & `momlevel-0.0.9/src/momlevel/resources/geolocate_points_reference.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/resources/global_tide_gauges.csv` & `momlevel-0.0.9/src/momlevel/resources/global_tide_gauges.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/resources/us_tide_gauges.csv` & `momlevel-0.0.9/src/momlevel/resources/us_tide_gauges.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/spice/flament.py` & `momlevel-0.0.9/src/momlevel/spice/flament.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/steric.py` & `momlevel-0.0.9/src/momlevel/steric.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/test_data/__init__.py` & `momlevel-0.0.9/src/momlevel/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/test_data/time.py` & `momlevel-0.0.9/src/momlevel/test_data/time.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/test_data/tripolar/horizontal.py` & `momlevel-0.0.9/src/momlevel/test_data/tripolar/horizontal.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/test_data/tripolar/vertical.py` & `momlevel-0.0.9/src/momlevel/test_data/tripolar/vertical.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/tidegauge.py` & `momlevel-0.0.9/src/momlevel/tidegauge.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/trend.py` & `momlevel-0.0.9/src/momlevel/trend.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel/util.py` & `momlevel-0.0.9/src/momlevel/util.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/src/momlevel.egg-info/PKG-INFO` & `momlevel-0.0.9/src/momlevel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momlevel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to diagnose sea level in the MOM Ocean Model
 Author-email: John Krasting <john.krasting@noaa.gov>
 License: Software code created by U.S. Government employees is not subject to copyright in the United States (17 U.S.C. §105).
         The United States/Department of Commerce reserve all rights to seek and obtain copyright protection in countries
         otherthan the United States for Software authored in its entirety by the Department of Commerce. To this end, the
         Department of Commerce hereby grants to Recipient a royalty-free, nonexclusive license to use, copy, and create 
         derivative works of the Software outside of the United States.”
```

### Comparing `momlevel-0.0.8/src/momlevel.egg-info/SOURCES.txt` & `momlevel-0.0.9/src/momlevel.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/momlevel/util.py
 src/momlevel.egg-info/PKG-INFO
 src/momlevel.egg-info/SOURCES.txt
 src/momlevel.egg-info/dependency_links.txt
 src/momlevel.egg-info/requires.txt
 src/momlevel.egg-info/top_level.txt
 src/momlevel/eos/__init__.py
+src/momlevel/eos/linear.py
 src/momlevel/eos/wright.py
 src/momlevel/resources/CM4_historical.nc
 src/momlevel/resources/NWA12_grid_dataframe.csv
 src/momlevel/resources/NWA12_sample_grid_data.nc
 src/momlevel/resources/geolocate_points_reference.csv
 src/momlevel/resources/global_tide_gauges.csv
 src/momlevel/resources/us_tide_gauges.csv
@@ -28,14 +29,15 @@
 src/momlevel/test_data/time.py
 src/momlevel/test_data/tripolar/__init__.py
 src/momlevel/test_data/tripolar/horizontal.py
 src/momlevel/test_data/tripolar/vertical.py
 tests/test_derived.py
 tests/test_dynamic.py
 tests/test_flament.py
+tests/test_linear.py
 tests/test_reference.py
 tests/test_steric.py
 tests/test_testdata.py
 tests/test_tidegauge.py
 tests/test_trend.py
 tests/test_util.py
 tests/test_wright.py
```

### Comparing `momlevel-0.0.8/tests/test_derived.py` & `momlevel-0.0.9/tests/test_derived.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 def test_calc_dz_3():
     deptho = dset2.deptho.copy()
     deptho[4, 4] = -200.0
     with pytest.raises(Exception):
         derived.calc_dz(dset2.z_l, dset2.z_i, deptho)
 
 
+def test_calc_dz_4():
+    dz = derived.calc_dz(dset2.z_l, dset2.z_i, dset2.deptho, top=12., bottom=33.)
+    assert np.allclose(dz.sum(), 363.71725794)
+
+
 def test_calc_rho():
     rho = derived.calc_rho(dset1.thetao, dset1.so, dset1.z_l * 1.0e4, eos="Wright")
     pytest.rho = rho
     assert np.allclose(rho.sum(), 643872.59725673)
 
 
 def test_calc_n2_1():
```

### Comparing `momlevel-0.0.8/tests/test_steric.py` & `momlevel-0.0.9/tests/test_steric.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/tests/test_testdata.py` & `momlevel-0.0.9/tests/test_testdata.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/tests/test_tidegauge.py` & `momlevel-0.0.9/tests/test_tidegauge.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/tests/test_trend.py` & `momlevel-0.0.9/tests/test_trend.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/tests/test_util.py` & `momlevel-0.0.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.8/tests/test_wright.py` & `momlevel-0.0.9/tests/test_wright.py`

 * *Files identical despite different names*


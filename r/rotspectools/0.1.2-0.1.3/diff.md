# Comparing `tmp/rotspectools-0.1.2.tar.gz` & `tmp/rotspectools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.2.tar", max compression
+gzip compressed data, was "rotspectools-0.1.3.tar", max compression
```

## Comparing `rotspectools-0.1.2.tar` & `rotspectools-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.2/LICENSE
--rw-r--r--   0        0        0      974 2023-06-09 22:48:57.252972 rotspectools-0.1.2/README.rst
--rw-r--r--   0        0        0      439 2023-06-10 00:32:53.804098 rotspectools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.2/rotspectools/.DS_Store
--rw-r--r--   0        0        0      146 2023-06-09 22:48:57.256906 rotspectools-0.1.2/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.2/rotspectools/cli.py
--rw-r--r--   0        0        0    19389 2023-06-09 20:41:27.276958 rotspectools-0.1.2/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 rotspectools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.3/LICENSE
+-rw-r--r--   0        0        0      974 2023-06-09 22:48:57.252972 rotspectools-0.1.3/README.rst
+-rw-r--r--   0        0        0      439 2023-06-10 01:01:12.417223 rotspectools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.3/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-06-09 22:48:57.256906 rotspectools-0.1.3/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.3/rotspectools/cli.py
+-rw-r--r--   0        0        0    19502 2023-06-10 00:59:18.180483 rotspectools-0.1.3/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 rotspectools-0.1.3/PKG-INFO
```

### Comparing `rotspectools-0.1.2/LICENSE` & `rotspectools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.2/README.rst` & `rotspectools-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.2/rotspectools/.DS_Store` & `rotspectools-0.1.3/rotspectools/.DS_Store`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.2/rotspectools/rotspectools.py` & `rotspectools-0.1.3/rotspectools/rotspectools.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scienceplots
 from matplotlib.legend_handler import HandlerPatch
 from pandas import DataFrame
+from inspect import currentframe, getframeinfo
 
 mpl.rc("text", usetex=True)
 plt.style.use(["science", "ieee"])
 
 
 class Experiment:
     def __init__(
         self,
         num_lines: int,
         molecule_type: str,
         file_name: str,
-        file_path_res: str = "", 
+        file_path_res: str = "",
         file_path_lin: str = "",
         res_dataframe: DataFrame = pd.DataFrame(),
         lin_dataframe: DataFrame = pd.DataFrame(),
     ):
         self.num_lines = num_lines
         self.molecule_type = molecule_type
         self.file_name = file_name
@@ -35,15 +36,16 @@
         self.lin_dataframe = lin_dataframe
         self.rel_file_path()
         self.read_res()
         self.df_error = self.res_dataframe.copy(deep=True)
         self.read_lin()
 
     def rel_file_path(self) -> str:
-        base_path = Path(__file__).parent
+        filename = getframeinfo(currentframe()).filename
+        base_path = Path(filename).resolve().parent
         file_name_res = self.file_name + ".res"
         file_name_lin = self.file_name + ".lin"
         self.file_path_res = (base_path / file_name_res).resolve()
         self.file_path_lin = (base_path / file_name_lin).resolve()
 
     def read_lin(self) -> DataFrame:
         line_width = len(str(self.num_lines)) + 1
```

### Comparing `rotspectools-0.1.2/PKG-INFO` & `rotspectools-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotspectools
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Dairen Jean
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


# Comparing `tmp/rotspectools-0.1.3.tar.gz` & `tmp/rotspectools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.3.tar", max compression
+gzip compressed data, was "rotspectools-0.1.4.tar", max compression
```

## Comparing `rotspectools-0.1.3.tar` & `rotspectools-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.3/LICENSE
--rw-r--r--   0        0        0      974 2023-06-09 22:48:57.252972 rotspectools-0.1.3/README.rst
--rw-r--r--   0        0        0      439 2023-06-10 01:01:12.417223 rotspectools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.3/rotspectools/.DS_Store
--rw-r--r--   0        0        0      146 2023-06-09 22:48:57.256906 rotspectools-0.1.3/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.3/rotspectools/cli.py
--rw-r--r--   0        0        0    19502 2023-06-10 00:59:18.180483 rotspectools-0.1.3/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 rotspectools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.4/LICENSE
+-rw-r--r--   0        0        0      974 2023-06-09 22:48:57.252972 rotspectools-0.1.4/README.rst
+-rw-r--r--   0        0        0      459 2023-06-10 01:51:52.249953 rotspectools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.4/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-06-09 22:48:57.256906 rotspectools-0.1.4/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.4/rotspectools/cli.py
+-rw-r--r--   0        0        0    19459 2023-06-10 01:50:31.482562 rotspectools-0.1.4/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 rotspectools-0.1.4/PKG-INFO
```

### Comparing `rotspectools-0.1.3/LICENSE` & `rotspectools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.3/README.rst` & `rotspectools-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.3/rotspectools/.DS_Store` & `rotspectools-0.1.4/rotspectools/.DS_Store`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.3/rotspectools/rotspectools.py` & `rotspectools-0.1.4/rotspectools/rotspectools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import sys
 from pathlib import Path
 from typing import Tuple
 
 import matplotlib as mpl
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
@@ -36,16 +37,15 @@
         self.lin_dataframe = lin_dataframe
         self.rel_file_path()
         self.read_res()
         self.df_error = self.res_dataframe.copy(deep=True)
         self.read_lin()
 
     def rel_file_path(self) -> str:
-        filename = getframeinfo(currentframe()).filename
-        base_path = Path(filename).resolve().parent
+        base_path = Path(sys.argv[0]).resolve().parent
         file_name_res = self.file_name + ".res"
         file_name_lin = self.file_name + ".lin"
         self.file_path_res = (base_path / file_name_res).resolve()
         self.file_path_lin = (base_path / file_name_lin).resolve()
 
     def read_lin(self) -> DataFrame:
         line_width = len(str(self.num_lines)) + 1
```

### Comparing `rotspectools-0.1.3/PKG-INFO` & `rotspectools-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rotspectools
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Dairen Jean
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SciencePlots (>=2.1.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Description-Content-Type: text/x-rst
 
 =============================
 Rotational Spectroscopy Tools
 =============================
```


# Comparing `tmp/omniplate-0.9.9.tar.gz` & `tmp/omniplate-0.9.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-0.9.9.tar", max compression
+gzip compressed data, was "omniplate-0.9.91.tar", max compression
```

## Comparing `omniplate-0.9.9.tar` & `omniplate-0.9.91.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.9/README.md
--rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.9/om_code/__init__.py
--rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.000000 omniplate-0.9.9/om_code/admin.py
--rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.907067 omniplate-0.9.9/om_code/clogger.py
--rw-r--r--   0        0        0    23910 2023-06-10 14:52:08.047214 omniplate-0.9.9/om_code/corrections.py
--rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.087062 omniplate-0.9.9/om_code/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.122549 omniplate-0.9.9/om_code/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     7681 2023-06-10 14:52:08.058039 omniplate-0.9.9/om_code/getfitnesspenalty.py
--rw-r--r--   0        0        0     3470 2023-05-26 11:17:09.852745 omniplate-0.9.9/om_code/loaddata.py
--rw-r--r--   0        0        0     5187 2023-06-10 14:52:08.069421 omniplate-0.9.9/om_code/midlog.py
--rw-r--r--   0        0        0     2577 2023-05-26 11:17:09.866642 omniplate-0.9.9/om_code/old_analyseOldTecan.py
--rw-r--r--   0        0        0     1771 2023-05-26 11:17:09.866955 omniplate-0.9.9/om_code/old_analyseSunrise.py
--rw-r--r--   0        0        0     2609 2023-05-26 11:17:09.867263 omniplate-0.9.9/om_code/old_analyseTecan.py
--rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.9/om_code/omerrors.py
--rw-r--r--   0        0        0    11866 2023-06-10 14:52:08.126153 omniplate-0.9.9/om_code/omfitderiv.py
--rw-r--r--   0        0        0     3925 2023-06-10 14:52:08.317129 omniplate-0.9.9/om_code/omgenutils.py
--rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.000000 omniplate-0.9.9/om_code/omplot.py
--rw-r--r--   0        0        0     6781 2023-06-10 14:52:08.375378 omniplate-0.9.9/om_code/omstats.py
--rw-r--r--   0        0        0     4256 2023-06-10 14:52:08.413530 omniplate-0.9.9/om_code/parseplate.py
--rw-r--r--   0        0        0     6068 2023-06-10 14:52:08.481613 omniplate-0.9.9/om_code/runfitderiv.py
--rw-r--r--   0        0        0     6211 2023-05-16 09:18:38.727419 omniplate-0.9.9/om_code/sunder.py
--rw-r--r--   0        0        0    93614 2023-06-10 14:52:08.661990 omniplate-0.9.9/omniplate/Omniplate.py
--rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.9/omniplate/__init__.py
--rw-r--r--   0        0        0     1115 2023-06-10 14:52:08.693966 omniplate-0.9.9/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 omniplate-0.9.9/setup.py
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 omniplate-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.91/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.91/om_code/__init__.py
+-rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.000000 omniplate-0.9.91/om_code/admin.py
+-rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.907067 omniplate-0.9.91/om_code/clogger.py
+-rw-r--r--   0        0        0    23910 2023-06-10 14:52:08.047214 omniplate-0.9.91/om_code/corrections.py
+-rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.087062 omniplate-0.9.91/om_code/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.122549 omniplate-0.9.91/om_code/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     7681 2023-06-10 14:52:08.058039 omniplate-0.9.91/om_code/getfitnesspenalty.py
+-rw-r--r--   0        0        0     3470 2023-06-10 16:06:46.513087 omniplate-0.9.91/om_code/loaddata.py
+-rw-r--r--   0        0        0     5187 2023-06-10 14:52:08.069421 omniplate-0.9.91/om_code/midlog.py
+-rw-r--r--   0        0        0     2577 2023-05-26 11:17:09.866642 omniplate-0.9.91/om_code/old_analyseOldTecan.py
+-rw-r--r--   0        0        0     1771 2023-05-26 11:17:09.866955 omniplate-0.9.91/om_code/old_analyseSunrise.py
+-rw-r--r--   0        0        0     2609 2023-05-26 11:17:09.867263 omniplate-0.9.91/om_code/old_analyseTecan.py
+-rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.91/om_code/omerrors.py
+-rw-r--r--   0        0        0    11866 2023-06-10 14:52:08.126153 omniplate-0.9.91/om_code/omfitderiv.py
+-rw-r--r--   0        0        0     3925 2023-06-10 14:52:08.317129 omniplate-0.9.91/om_code/omgenutils.py
+-rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.000000 omniplate-0.9.91/om_code/omplot.py
+-rw-r--r--   0        0        0     6781 2023-06-10 14:52:08.375378 omniplate-0.9.91/om_code/omstats.py
+-rw-r--r--   0        0        0     4211 2023-06-10 16:06:35.568372 omniplate-0.9.91/om_code/parseplate.py
+-rw-r--r--   0        0        0     6068 2023-06-10 14:52:08.481613 omniplate-0.9.91/om_code/runfitderiv.py
+-rw-r--r--   0        0        0     6211 2023-05-16 09:18:38.727419 omniplate-0.9.91/om_code/sunder.py
+-rw-r--r--   0        0        0    93615 2023-06-10 16:11:05.939987 omniplate-0.9.91/omniplate/Omniplate.py
+-rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.91/omniplate/__init__.py
+-rw-r--r--   0        0        0     1116 2023-06-10 16:11:20.579802 omniplate-0.9.91/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 omniplate-0.9.91/setup.py
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 omniplate-0.9.91/PKG-INFO
```

### Comparing `omniplate-0.9.9/om_code/admin.py` & `omniplate-0.9.91/om_code/admin.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/clogger.py` & `omniplate-0.9.91/om_code/clogger.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/corrections.py` & `omniplate-0.9.91/om_code/corrections.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/dilution_data_lucia.tsv` & `omniplate-0.9.91/om_code/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/dilution_data_xiao.tsv` & `omniplate-0.9.91/om_code/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/getfitnesspenalty.py` & `omniplate-0.9.91/om_code/getfitnesspenalty.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/loaddata.py` & `omniplate-0.9.91/om_code/loaddata.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     # import and parse plate contents file
     allconditions, allstrains, alldata, wellcontents = analyseContentsofWells(
         wdirpath, experiment, aname, asheetnumber
     )
     # import and parse data file created by plate reader
     try:
-        print("loading", dname)
+        print("Loading", dname)
         rdf = parseplate(dname, platereadertype, wdirpath, dsheetnumber)
     except FileNotFoundError:
         raise errors.FileNotFound(str(wdirpath / dname))
 
     # get datatypes
     cols = rdf.columns.to_list()
     datatypes = [col for col in cols if col != "time" and col != "well"]
```

### Comparing `omniplate-0.9.9/om_code/midlog.py` & `omniplate-0.9.91/om_code/midlog.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/old_analyseOldTecan.py` & `omniplate-0.9.91/om_code/old_analyseOldTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/old_analyseSunrise.py` & `omniplate-0.9.91/om_code/old_analyseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/old_analyseTecan.py` & `omniplate-0.9.91/om_code/old_analyseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/omfitderiv.py` & `omniplate-0.9.91/om_code/omfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/omgenutils.py` & `omniplate-0.9.91/om_code/omgenutils.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/omplot.py` & `omniplate-0.9.91/om_code/omplot.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/omstats.py` & `omniplate-0.9.91/om_code/omstats.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/parseplate.py` & `omniplate-0.9.91/om_code/parseplate.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     # create a dict to store data
     rdict = {}
     rdict["time"] = []
     rdict["well"] = []
 
     if platereadertype == "tidy":
         print(
-            "Columns must be labelled 'time', 'well', 'OD', etc.,"
+            "Columns must be labelled 'time', 'well', 'OD', etc., "
             "and time must be in units of hours."
         )
         try:
             if ".tsv" in platereaderfile:
                 rdf = pd.read_csv(str(wdirpath / platereaderfile), sep="\t")
             else:
                 rdf = pd.read_csv(str(wdirpath / platereaderfile))
@@ -60,15 +60,14 @@
             raise errors.FileNotFound(str(wdirpath / platereaderfile))
         if rdf.time.max() > 100:
             print("Warning: time does not appear to be in hours.")
         return rdf
 
     elif platereadertype == "Tecan":
         try:
-            print("loading", platereaderfile)
             dfd = pd.read_excel(
                 str(wdirpath / platereaderfile), sheet_name=sheetnumber
             )
         except FileNotFoundError:
             raise errors.FileNotFound(str(wdirpath / platereaderfile))
         # extract datatypes
         datatypes = (
```

### Comparing `omniplate-0.9.9/om_code/runfitderiv.py` & `omniplate-0.9.91/om_code/runfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/om_code/sunder.py` & `omniplate-0.9.91/om_code/sunder.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.9/omniplate/Omniplate.py` & `omniplate-0.9.91/omniplate/Omniplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import om_code.omgenutils as gu
 import om_code.omplot as omplot
 import om_code.sunder as sunder
 import pandas as pd
 import seaborn as sns
 from om_code.runfitderiv import runfitderiv
 
-version = "0.9.9"
+version = "0.9.91"
 
 plt.rcParams["figure.max_open_warning"] = 0
 sns.set()
 
 
 class platereader:
     """
```

### Comparing `omniplate-0.9.9/pyproject.toml` & `omniplate-0.9.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "0.9.9"
+version = "0.9.91"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
```

### Comparing `omniplate-0.9.9/setup.py` & `omniplate-0.9.91/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pandas>=1.5.1',
  'scipy>=1.10.1,<2.0.0',
  'seaborn>=0.11.2',
  'statsmodels>=0.13.1']
 
 setup_kwargs = {
     'name': 'omniplate',
-    'version': '0.9.9',
+    'version': '0.9.91',
     'description': 'For analysing and meta-analysing plate-reader data',
     'long_description': 'A Python package for analysing data from plate-reader studies of growing biological cells. Users can correct for autofluorescence, determine growth rates and the amount of fluorescence per cell, and simultaneously analyse multiple experiments.\n',
     'author': 'Peter Swain',
     'author_email': 'peter.swain@ed.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://swainlab.bio.ed.ac.uk/software/omniplate',
```

### Comparing `omniplate-0.9.9/PKG-INFO` & `omniplate-0.9.91/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 0.9.9
+Version: 0.9.91
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
```


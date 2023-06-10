# Comparing `tmp/expt-0.4.1.tar.gz` & `tmp/expt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expt-0.4.1.tar", last modified: Sun Oct  2 00:33:39 2022, max compression
+gzip compressed data, was "expt-0.4.2.tar", last modified: Sat Jun 10 02:32:16 2023, max compression
```

## Comparing `expt-0.4.1.tar` & `expt-0.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.174570 expt-0.4.1/
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.165922 expt-0.4.1/.github/
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.167229 expt-0.4.1/.github/workflows/
--rw-r--r--   0 wookayin   (501) staff       (20)      929 2022-09-30 14:59:58.000000 expt-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0 wookayin   (501) staff       (20)     1821 2022-09-30 14:59:58.000000 expt-0.4.1/.gitignore
--rw-r--r--   0 wookayin   (501) staff       (20)      323 2022-09-30 14:59:58.000000 expt-0.4.1/.pylintrc
--rw-r--r--   0 wookayin   (501) staff       (20)       47 2022-09-30 14:59:58.000000 expt-0.4.1/.style.yapf
--rw-r--r--   0 wookayin   (501) staff       (20)     1079 2020-06-29 03:12:25.000000 expt-0.4.1/LICENSE
--rw-r--r--   0 wookayin   (501) staff       (20)       34 2020-06-29 03:12:56.000000 expt-0.4.1/MANIFEST.in
--rw-r--r--   0 wookayin   (501) staff       (20)     1671 2022-10-02 00:33:39.174715 expt-0.4.1/PKG-INFO
--rw-r--r--   0 wookayin   (501) staff       (20)     1000 2022-09-30 14:59:58.000000 expt-0.4.1/README.md
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.168489 expt-0.4.1/examples/
--rw-r--r--   0 wookayin   (501) staff       (20)        5 2022-02-14 00:43:52.000000 expt-0.4.1/examples/.gitignore
--rw-r--r--   0 wookayin   (501) staff       (20)   197516 2021-10-22 22:17:39.000000 expt-0.4.1/examples/demo-figure.png
--rw-r--r--   0 wookayin   (501) staff       (20)  3020990 2022-09-30 15:00:02.000000 expt-0.4.1/examples/quick-tour.ipynb
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.173283 expt-0.4.1/expt/
--rw-r--r--   0 wookayin   (501) staff       (20)      506 2022-10-02 00:32:44.000000 expt-0.4.1/expt/__init__.py
--rw-r--r--   0 wookayin   (501) staff       (20)     2080 2022-09-30 14:59:58.000000 expt-0.4.1/expt/colors.py
--rw-r--r--   0 wookayin   (501) staff       (20)    36398 2022-10-01 23:34:32.000000 expt-0.4.1/expt/data.py
--rw-r--r--   0 wookayin   (501) staff       (20)    20952 2022-10-01 23:39:00.000000 expt-0.4.1/expt/data_loader.py
--rw-r--r--   0 wookayin   (501) staff       (20)     5639 2022-09-30 14:59:58.000000 expt-0.4.1/expt/data_loader_test.py
--rw-r--r--   0 wookayin   (501) staff       (20)    15468 2022-10-01 23:00:39.000000 expt-0.4.1/expt/data_test.py
--rw-r--r--   0 wookayin   (501) staff       (20)     4948 2022-09-30 14:59:58.000000 expt-0.4.1/expt/path_util.py
--rw-r--r--   0 wookayin   (501) staff       (20)    37507 2022-09-30 15:00:02.000000 expt-0.4.1/expt/plot.py
--rw-r--r--   0 wookayin   (501) staff       (20)    15538 2022-09-30 15:00:02.000000 expt-0.4.1/expt/plot_test.py
--rw-r--r--   0 wookayin   (501) staff       (20)     2196 2022-09-30 14:59:58.000000 expt-0.4.1/expt/util.py
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.174056 expt-0.4.1/expt.egg-info/
--rw-r--r--   0 wookayin   (501) staff       (20)     1671 2022-10-02 00:33:38.000000 expt-0.4.1/expt.egg-info/PKG-INFO
--rw-r--r--   0 wookayin   (501) staff       (20)      566 2022-10-02 00:33:39.000000 expt-0.4.1/expt.egg-info/SOURCES.txt
--rw-r--r--   0 wookayin   (501) staff       (20)        1 2022-10-02 00:33:38.000000 expt-0.4.1/expt.egg-info/dependency_links.txt
--rw-r--r--   0 wookayin   (501) staff       (20)        1 2020-06-29 03:10:21.000000 expt-0.4.1/expt.egg-info/not-zip-safe
--rw-r--r--   0 wookayin   (501) staff       (20)      175 2022-10-02 00:33:38.000000 expt-0.4.1/expt.egg-info/requires.txt
--rw-r--r--   0 wookayin   (501) staff       (20)        5 2022-10-02 00:33:38.000000 expt-0.4.1/expt.egg-info/top_level.txt
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.174170 expt-0.4.1/fixtures/
--rw-r--r--   0 wookayin   (501) staff       (20)       13 2022-09-30 14:59:58.000000 expt-0.4.1/fixtures/.gitignore
-drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2022-10-02 00:33:39.174295 expt-0.4.1/fixtures/sample_csv/
--rw-r--r--   0 wookayin   (501) staff       (20)     1634 2022-09-30 14:59:58.000000 expt-0.4.1/fixtures/sample_csv/progress.csv
--rw-r--r--   0 wookayin   (501) staff       (20)      129 2022-10-02 00:33:39.175050 expt-0.4.1/setup.cfg
--rw-r--r--   0 wookayin   (501) staff       (20)     3450 2022-10-02 00:32:30.000000 expt-0.4.1/setup.py
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.791484 expt-0.4.2/
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.784478 expt-0.4.2/.github/
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.786071 expt-0.4.2/.github/workflows/
+-rw-r--r--   0 wookayin   (501) staff       (20)      928 2023-06-10 02:30:09.000000 expt-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 wookayin   (501) staff       (20)     1821 2023-06-10 02:30:09.000000 expt-0.4.2/.gitignore
+-rw-r--r--   0 wookayin   (501) staff       (20)      323 2023-06-10 02:30:09.000000 expt-0.4.2/.pylintrc
+-rw-r--r--   0 wookayin   (501) staff       (20)       47 2023-06-10 02:30:01.000000 expt-0.4.2/.style.yapf
+-rw-r--r--   0 wookayin   (501) staff       (20)     1079 2023-06-10 02:30:01.000000 expt-0.4.2/LICENSE
+-rw-r--r--   0 wookayin   (501) staff       (20)       34 2023-06-10 02:30:09.000000 expt-0.4.2/MANIFEST.in
+-rw-r--r--   0 wookayin   (501) staff       (20)     1671 2023-06-10 02:32:16.791578 expt-0.4.2/PKG-INFO
+-rw-r--r--   0 wookayin   (501) staff       (20)     1000 2023-06-10 02:30:01.000000 expt-0.4.2/README.md
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.786619 expt-0.4.2/examples/
+-rw-r--r--   0 wookayin   (501) staff       (20)        5 2023-06-10 02:30:01.000000 expt-0.4.2/examples/.gitignore
+-rw-r--r--   0 wookayin   (501) staff       (20)   197516 2023-06-10 02:30:01.000000 expt-0.4.2/examples/demo-figure.png
+-rw-r--r--   0 wookayin   (501) staff       (20)  3021000 2023-06-10 02:30:01.000000 expt-0.4.2/examples/quick-tour.ipynb
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.790126 expt-0.4.2/expt/
+-rw-r--r--   0 wookayin   (501) staff       (20)      506 2023-06-10 02:31:14.000000 expt-0.4.2/expt/__init__.py
+-rw-r--r--   0 wookayin   (501) staff       (20)     2080 2023-06-10 02:30:09.000000 expt-0.4.2/expt/colors.py
+-rw-r--r--   0 wookayin   (501) staff       (20)    36396 2023-06-10 02:30:09.000000 expt-0.4.2/expt/data.py
+-rw-r--r--   0 wookayin   (501) staff       (20)    20952 2023-06-10 02:30:09.000000 expt-0.4.2/expt/data_loader.py
+-rw-r--r--   0 wookayin   (501) staff       (20)     5639 2023-06-10 02:30:09.000000 expt-0.4.2/expt/data_loader_test.py
+-rw-r--r--   0 wookayin   (501) staff       (20)    15468 2023-06-10 02:30:09.000000 expt-0.4.2/expt/data_test.py
+-rw-r--r--   0 wookayin   (501) staff       (20)     4948 2023-06-10 02:30:09.000000 expt-0.4.2/expt/path_util.py
+-rw-r--r--   0 wookayin   (501) staff       (20)    37477 2023-06-10 02:30:09.000000 expt-0.4.2/expt/plot.py
+-rw-r--r--   0 wookayin   (501) staff       (20)    15538 2023-06-10 02:30:09.000000 expt-0.4.2/expt/plot_test.py
+-rw-r--r--   0 wookayin   (501) staff       (20)     2196 2023-06-10 02:30:09.000000 expt-0.4.2/expt/util.py
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.791079 expt-0.4.2/expt.egg-info/
+-rw-r--r--   0 wookayin   (501) staff       (20)     1671 2023-06-10 02:32:16.000000 expt-0.4.2/expt.egg-info/PKG-INFO
+-rw-r--r--   0 wookayin   (501) staff       (20)      566 2023-06-10 02:32:16.000000 expt-0.4.2/expt.egg-info/SOURCES.txt
+-rw-r--r--   0 wookayin   (501) staff       (20)        1 2023-06-10 02:32:16.000000 expt-0.4.2/expt.egg-info/dependency_links.txt
+-rw-r--r--   0 wookayin   (501) staff       (20)        1 2023-06-10 02:32:16.000000 expt-0.4.2/expt.egg-info/not-zip-safe
+-rw-r--r--   0 wookayin   (501) staff       (20)      175 2023-06-10 02:32:16.000000 expt-0.4.2/expt.egg-info/requires.txt
+-rw-r--r--   0 wookayin   (501) staff       (20)        5 2023-06-10 02:32:16.000000 expt-0.4.2/expt.egg-info/top_level.txt
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.791206 expt-0.4.2/fixtures/
+-rw-r--r--   0 wookayin   (501) staff       (20)       13 2023-06-10 02:30:09.000000 expt-0.4.2/fixtures/.gitignore
+drwxr-xr-x   0 wookayin   (501) staff       (20)        0 2023-06-10 02:32:16.791370 expt-0.4.2/fixtures/sample_csv/
+-rw-r--r--   0 wookayin   (501) staff       (20)     1634 2023-06-10 02:30:01.000000 expt-0.4.2/fixtures/sample_csv/progress.csv
+-rw-r--r--   0 wookayin   (501) staff       (20)      129 2023-06-10 02:32:16.791815 expt-0.4.2/setup.cfg
+-rw-r--r--   0 wookayin   (501) staff       (20)     3450 2023-06-10 02:30:09.000000 expt-0.4.2/setup.py
```

### Comparing `expt-0.4.1/.gitignore` & `expt-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/LICENSE` & `expt-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/PKG-INFO` & `expt-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expt
-Version: 0.4.1
+Version: 0.4.2
 Summary: EXperiment. Plot. Tabulate.
 Home-page: https://github.com/wookayin/expt
 Author: Jongwook Choi
 Author-email: wookayin@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `expt-0.4.1/README.md` & `expt-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/examples/demo-figure.png` & `expt-0.4.2/examples/demo-figure.png`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/examples/quick-tour.ipynb` & `expt-0.4.2/examples/quick-tour.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997427983539094%*

 * *Differences: {"'cells'": "{2: {'metadata': {'jupyter': OrderedDict([('source_hidden', True)]), delete: "*

 * *            "['jp-MarkdownHeadingCollapsed']}}}"}*

```diff
@@ -13,15 +13,17 @@
             "source": [
                 "DISCLAIMER: Many things including API and default behaviors are subject to change."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "jp-MarkdownHeadingCollapsed": true,
+                "jupyter": {
+                    "source_hidden": true
+                },
                 "tags": []
             },
             "source": [
                 "## 0. Data Preparation Part (can be skipped)"
             ]
         },
         {
```

### Comparing `expt-0.4.1/expt/colors.py` & `expt-0.4.2/expt/colors.py`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/expt/data.py` & `expt-0.4.2/expt/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,15 +647,15 @@
   """An Experiment is a collection of Hypotheses, structured with
   hierarchical MultiIndex."""
 
   @typechecked
   def __init__(
       self,
       name: Optional[str] = None,
-      hypotheses: Iterable[Hypothesis] = None,
+      hypotheses: Iterable[Hypothesis] = (),
   ):
     self._name = name if name is not None else ""
     self._hypotheses: MutableMapping[str, Hypothesis]
     self._hypotheses = collections.OrderedDict()
 
     if isinstance(hypotheses, np.ndarray):
       hypotheses = list(hypotheses)
```

### Comparing `expt-0.4.1/expt/data_loader.py` & `expt-0.4.2/expt/data_loader.py`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/expt/data_loader_test.py` & `expt-0.4.2/expt/data_loader_test.py`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/expt/data_test.py` & `expt-0.4.2/expt/data_test.py`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/expt/path_util.py` & `expt-0.4.2/expt/path_util.py`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/expt/plot.py` & `expt-0.4.2/expt/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
                ignore_unknown: bool = False,
                legend: Union[bool, int, str, Dict[str, Any]] = False,
                prettify_labels: bool = False,
                suptitle: Optional[str] = None,
                grid: Optional[GridPlot] = None,
                ax: Optional[Union[Axes, np.ndarray]] = None,
                tight_layout: bool = True,
-               **kwargs) -> 'holoviews.core.layout.NdLayout':  # type: ignore
+               **kwargs) -> GridPlot:
     '''Hypothesis.plot based on matplotlib.
 
     This can work in two different modes:
     (1) Plot (several or all) columns as separate subplots (subplots=True)
     (2) Plot (several or all) columns in a single axesplot (subplots=False)
 
     Additional keyword arguments:
@@ -515,16 +515,16 @@
 
   def _validate_ax_with_y(self, ax, y):
     assert not isinstance(y, str)
     if not isinstance(ax, (Axes, np.ndarray)):
       raise TypeError("`ax` must be a single Axes or a ndarray of Axes, "
                       "but given {}".format(ax))
     if isinstance(ax, Axes):
-      ax = np.asarray([ax], dtype=object)
-    if len(ax) != len(y):
+      ax = np.asarray([[ax]], dtype=object)
+    if len(ax.ravel()) != len(y):
       raise ValueError("The length of `ax` and `y` must be equal: "
                        "ax = {}, y = {}".format(len(ax), len(y)))
 
   def _do_plot(
       self,
       y: List[str],
       representative: pd.DataFrame,  # usually mean
```

### Comparing `expt-0.4.1/expt/plot_test.py` & `expt-0.4.2/expt/plot_test.py`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/expt/util.py` & `expt-0.4.2/expt/util.py`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/expt.egg-info/PKG-INFO` & `expt-0.4.2/expt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expt
-Version: 0.4.1
+Version: 0.4.2
 Summary: EXperiment. Plot. Tabulate.
 Home-page: https://github.com/wookayin/expt
 Author: Jongwook Choi
 Author-email: wookayin@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `expt-0.4.1/expt.egg-info/SOURCES.txt` & `expt-0.4.2/expt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/fixtures/sample_csv/progress.csv` & `expt-0.4.2/fixtures/sample_csv/progress.csv`

 * *Files identical despite different names*

### Comparing `expt-0.4.1/setup.py` & `expt-0.4.2/setup.py`

 * *Files identical despite different names*


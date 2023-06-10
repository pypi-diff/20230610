# Comparing `tmp/tiafork-1.2.1.tar.gz` & `tmp/tiafork-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiafork-1.2.1.tar", last modified: Sat Jun 10 16:46:37 2023, max compression
+gzip compressed data, was "tiafork-1.2.2.tar", last modified: Sat Jun 10 16:54:21 2023, max compression
```

## Comparing `tiafork-1.2.1.tar` & `tiafork-1.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.687994 tiafork-1.2.1/
--rw-rw-rw-   0        0        0     1659 2023-06-10 05:31:16.000000 tiafork-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     3329 2023-06-10 16:46:37.686998 tiafork-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2427 2023-06-10 16:42:23.000000 tiafork-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 16:46:37.687994 tiafork-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1820 2023-06-10 16:42:35.000000 tiafork-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.663743 tiafork-1.2.1/tiafork/
--rw-rw-rw-   0        0        0       23 2023-06-10 16:43:26.000000 tiafork-1.2.1/tiafork/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.670511 tiafork-1.2.1/tiafork/analysis/
--rw-rw-rw-   0        0        0       66 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.674833 tiafork-1.2.1/tiafork/analysis/model/
--rw-rw-rw-   0        0        0      342 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/analysis/model/__init__.py
--rw-rw-rw-   0        0        0    15668 2023-06-10 03:57:51.000000 tiafork-1.2.1/tiafork/analysis/model/ins.py
--rw-rw-rw-   0        0        0     3407 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/analysis/model/interface.py
--rw-rw-rw-   0        0        0    22576 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/analysis/model/pl.py
--rw-rw-rw-   0        0        0    13761 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/analysis/model/port.py
--rw-rw-rw-   0        0        0    11797 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/analysis/model/pos.py
--rw-rw-rw-   0        0        0    21045 2023-06-10 03:57:51.000000 tiafork-1.2.1/tiafork/analysis/model/ret.py
--rw-rw-rw-   0        0        0     3448 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/analysis/model/trd.py
--rw-rw-rw-   0        0        0     5311 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/analysis/model/txn.py
--rw-rw-rw-   0        0        0    12643 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/analysis/pdf_rpts.py
--rw-rw-rw-   0        0        0    19390 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/analysis/perf.py
--rw-rw-rw-   0        0        0     3127 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/analysis/plots.py
--rw-rw-rw-   0        0        0    12511 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/analysis/ta.py
--rw-rw-rw-   0        0        0    22716 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/analysis/talib_wrapper.py
--rw-rw-rw-   0        0        0     4463 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/analysis/util.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.676826 tiafork-1.2.1/tiafork/bbg/
--rw-rw-rw-   0        0        0      117 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/bbg/__init__.py
--rw-rw-rw-   0        0        0    25838 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/bbg/bbg_com.py
--rw-rw-rw-   0        0        0    18197 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/bbg/datamgr.py
--rw-rw-rw-   0        0        0     2323 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/bbg/example.py
--rw-rw-rw-   0        0        0    38217 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/bbg/v3api.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.680019 tiafork-1.2.1/tiafork/rlab/
--rw-rw-rw-   0        0        0      196 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/rlab/__init__.py
--rw-rw-rw-   0        0        0    11291 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/rlab/builder.py
--rw-rw-rw-   0        0        0     4287 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/rlab/components.py
--rw-rw-rw-   0        0        0      417 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/rlab/font.py
--rw-rw-rw-   0        0        0     2252 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/rlab/patch.py
--rw-rw-rw-   0        0        0     7101 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/rlab/sample.py
--rw-rw-rw-   0        0        0    41202 2023-06-10 03:57:51.000000 tiafork-1.2.1/tiafork/rlab/table.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.683011 tiafork-1.2.1/tiafork/tests/
--rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/tests/__init__.py
--rw-rw-rw-   0        0        0     6410 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/tests/test_analysis.py
--rw-rw-rw-   0        0        0     6790 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/tests/test_datamgr.py
--rw-rw-rw-   0        0        0     4728 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/tests/test_fmt.py
--rw-rw-rw-   0        0        0     5101 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/tests/test_rlab_table.py
--rw-rw-rw-   0        0        0     1556 2023-06-10 03:57:52.000000 tiafork-1.2.1/tiafork/tests/test_ta.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.686998 tiafork-1.2.1/tiafork/util/
--rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/util/__init__.py
--rw-rw-rw-   0        0        0     1381 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/util/decorator.py
--rw-rw-rw-   0        0        0    12795 2023-06-10 03:57:51.000000 tiafork-1.2.1/tiafork/util/fmt.py
--rw-rw-rw-   0        0        0     1195 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/util/log.py
--rw-rw-rw-   0        0        0     6666 2023-06-10 03:57:53.000000 tiafork-1.2.1/tiafork/util/mplot.py
--rw-rw-rw-   0        0        0     3783 2023-06-10 03:56:02.000000 tiafork-1.2.1/tiafork/util/windows.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:46:37.666736 tiafork-1.2.1/tiafork.egg-info/
--rw-rw-rw-   0        0        0     3329 2023-06-10 16:46:37.000000 tiafork-1.2.1/tiafork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1258 2023-06-10 16:46:37.000000 tiafork-1.2.1/tiafork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 16:46:37.000000 tiafork-1.2.1/tiafork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 16:46:37.000000 tiafork-1.2.1/tiafork.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 16:46:37.000000 tiafork-1.2.1/tiafork.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.529158 tiafork-1.2.2/
+-rw-rw-rw-   0        0        0     1659 2023-06-10 05:31:16.000000 tiafork-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3370 2023-06-10 16:54:21.529158 tiafork-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2427 2023-06-10 16:42:23.000000 tiafork-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 16:54:21.529158 tiafork-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2023-06-10 16:53:19.000000 tiafork-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.508694 tiafork-1.2.2/tiafork/
+-rw-rw-rw-   0        0        0       23 2023-06-10 16:54:09.000000 tiafork-1.2.2/tiafork/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.513677 tiafork-1.2.2/tiafork/analysis/
+-rw-rw-rw-   0        0        0       66 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.518276 tiafork-1.2.2/tiafork/analysis/model/
+-rw-rw-rw-   0        0        0      342 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/model/__init__.py
+-rw-rw-rw-   0        0        0    15668 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/analysis/model/ins.py
+-rw-rw-rw-   0        0        0     3407 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/analysis/model/interface.py
+-rw-rw-rw-   0        0        0    22576 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/model/pl.py
+-rw-rw-rw-   0        0        0    13761 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/model/port.py
+-rw-rw-rw-   0        0        0    11797 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/model/pos.py
+-rw-rw-rw-   0        0        0    21045 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/analysis/model/ret.py
+-rw-rw-rw-   0        0        0     3448 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/analysis/model/trd.py
+-rw-rw-rw-   0        0        0     5311 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/model/txn.py
+-rw-rw-rw-   0        0        0    12643 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/pdf_rpts.py
+-rw-rw-rw-   0        0        0    19390 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/perf.py
+-rw-rw-rw-   0        0        0     3127 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/plots.py
+-rw-rw-rw-   0        0        0    12511 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/ta.py
+-rw-rw-rw-   0        0        0    22716 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/talib_wrapper.py
+-rw-rw-rw-   0        0        0     4463 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/analysis/util.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.520269 tiafork-1.2.2/tiafork/bbg/
+-rw-rw-rw-   0        0        0      117 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/bbg/__init__.py
+-rw-rw-rw-   0        0        0    25838 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/bbg/bbg_com.py
+-rw-rw-rw-   0        0        0    18197 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/bbg/datamgr.py
+-rw-rw-rw-   0        0        0     2323 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/bbg/example.py
+-rw-rw-rw-   0        0        0    38217 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/bbg/v3api.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.523517 tiafork-1.2.2/tiafork/rlab/
+-rw-rw-rw-   0        0        0      196 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/rlab/__init__.py
+-rw-rw-rw-   0        0        0    11291 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/rlab/builder.py
+-rw-rw-rw-   0        0        0     4287 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/rlab/components.py
+-rw-rw-rw-   0        0        0      417 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/rlab/font.py
+-rw-rw-rw-   0        0        0     2252 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/rlab/patch.py
+-rw-rw-rw-   0        0        0     7101 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/rlab/sample.py
+-rw-rw-rw-   0        0        0    41202 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/rlab/table.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.526508 tiafork-1.2.2/tiafork/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/tests/__init__.py
+-rw-rw-rw-   0        0        0     6410 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/tests/test_analysis.py
+-rw-rw-rw-   0        0        0     6790 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_datamgr.py
+-rw-rw-rw-   0        0        0     4728 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_fmt.py
+-rw-rw-rw-   0        0        0     5101 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_rlab_table.py
+-rw-rw-rw-   0        0        0     1556 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_ta.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.529158 tiafork-1.2.2/tiafork/util/
+-rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/__init__.py
+-rw-rw-rw-   0        0        0     1381 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/decorator.py
+-rw-rw-rw-   0        0        0    12795 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/util/fmt.py
+-rw-rw-rw-   0        0        0     1195 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/log.py
+-rw-rw-rw-   0        0        0     6666 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/util/mplot.py
+-rw-rw-rw-   0        0        0     3783 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/windows.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.510687 tiafork-1.2.2/tiafork.egg-info/
+-rw-rw-rw-   0        0        0     3370 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1258 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/top_level.txt
```

### Comparing `tiafork-1.2.1/LICENSE` & `tiafork-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/PKG-INFO` & `tiafork-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiafork
-Version: 1.2.1
+Version: 1.2.2
 Summary: Fork of tia: Toolkit for integration and analysis
 Home-page: https://github.com/nathanramoscfa/tiafork
 Download-URL: https://github.com/nathanramoscfa/tiafork
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: BSD (3-clause)
 Keywords: bloomberg,backtesting,technical analysis,pdf
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tiafork: Toolkit for Integration and Analysis (Fork of a Fork)
 
 ## This is a Fork of a Fork!
 This project is a fork of the Python 3 compliant version of the `tia` toolkit made by [PaulMest](https://github.com/PaulMest/tia). I've named it `tiafork`.
```

### Comparing `tiafork-1.2.1/README.md` & `tiafork-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/setup.py` & `tiafork-1.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 setuptools.setup(
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     description=PACKAGE_DESC,
     include_package_data=True,
     install_requires=REQUIRED,
     long_description=LONG_DESC,
+    long_description_content_type="text/markdown",
     name=PACKAGE,
     packages=['tiafork', 'tiafork.analysis', 'tiafork.bbg', 'tiafork.rlab', 'tiafork.tests',
               'tiafork.util', 'tiafork.analysis.model'],
     package_dir={'tiafork': 'tiafork'},
     test_suite='tiafork.tests',
     tests_require=REQUIRED_FOR_TESTS,
     url=URL,
```

### Comparing `tiafork-1.2.1/tiafork/analysis/model/ins.py` & `tiafork-1.2.2/tiafork/analysis/model/ins.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/model/interface.py` & `tiafork-1.2.2/tiafork/analysis/model/interface.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/model/pl.py` & `tiafork-1.2.2/tiafork/analysis/model/pl.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/model/port.py` & `tiafork-1.2.2/tiafork/analysis/model/port.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/model/pos.py` & `tiafork-1.2.2/tiafork/analysis/model/pos.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/model/ret.py` & `tiafork-1.2.2/tiafork/analysis/model/ret.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/model/trd.py` & `tiafork-1.2.2/tiafork/analysis/model/trd.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/model/txn.py` & `tiafork-1.2.2/tiafork/analysis/model/txn.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/pdf_rpts.py` & `tiafork-1.2.2/tiafork/analysis/pdf_rpts.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/perf.py` & `tiafork-1.2.2/tiafork/analysis/perf.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/plots.py` & `tiafork-1.2.2/tiafork/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/ta.py` & `tiafork-1.2.2/tiafork/analysis/ta.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/talib_wrapper.py` & `tiafork-1.2.2/tiafork/analysis/talib_wrapper.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/analysis/util.py` & `tiafork-1.2.2/tiafork/analysis/util.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/bbg/bbg_com.py` & `tiafork-1.2.2/tiafork/bbg/bbg_com.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/bbg/datamgr.py` & `tiafork-1.2.2/tiafork/bbg/datamgr.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/bbg/example.py` & `tiafork-1.2.2/tiafork/bbg/example.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/bbg/v3api.py` & `tiafork-1.2.2/tiafork/bbg/v3api.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/rlab/builder.py` & `tiafork-1.2.2/tiafork/rlab/builder.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/rlab/components.py` & `tiafork-1.2.2/tiafork/rlab/components.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/rlab/patch.py` & `tiafork-1.2.2/tiafork/rlab/patch.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/rlab/sample.py` & `tiafork-1.2.2/tiafork/rlab/sample.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/rlab/table.py` & `tiafork-1.2.2/tiafork/rlab/table.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/tests/test_analysis.py` & `tiafork-1.2.2/tiafork/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/tests/test_datamgr.py` & `tiafork-1.2.2/tiafork/tests/test_datamgr.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/tests/test_fmt.py` & `tiafork-1.2.2/tiafork/tests/test_fmt.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/tests/test_rlab_table.py` & `tiafork-1.2.2/tiafork/tests/test_rlab_table.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/tests/test_ta.py` & `tiafork-1.2.2/tiafork/tests/test_ta.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/util/decorator.py` & `tiafork-1.2.2/tiafork/util/decorator.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/util/fmt.py` & `tiafork-1.2.2/tiafork/util/fmt.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/util/log.py` & `tiafork-1.2.2/tiafork/util/log.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/util/mplot.py` & `tiafork-1.2.2/tiafork/util/mplot.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork/util/windows.py` & `tiafork-1.2.2/tiafork/util/windows.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.1/tiafork.egg-info/PKG-INFO` & `tiafork-1.2.2/tiafork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiafork
-Version: 1.2.1
+Version: 1.2.2
 Summary: Fork of tia: Toolkit for integration and analysis
 Home-page: https://github.com/nathanramoscfa/tiafork
 Download-URL: https://github.com/nathanramoscfa/tiafork
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: BSD (3-clause)
 Keywords: bloomberg,backtesting,technical analysis,pdf
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tiafork: Toolkit for Integration and Analysis (Fork of a Fork)
 
 ## This is a Fork of a Fork!
 This project is a fork of the Python 3 compliant version of the `tia` toolkit made by [PaulMest](https://github.com/PaulMest/tia). I've named it `tiafork`.
```

### Comparing `tiafork-1.2.1/tiafork.egg-info/SOURCES.txt` & `tiafork-1.2.2/tiafork.egg-info/SOURCES.txt`

 * *Files identical despite different names*


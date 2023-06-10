# Comparing `tmp/tiafork-1.2.2.tar.gz` & `tmp/tiafork-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiafork-1.2.2.tar", last modified: Sat Jun 10 16:54:21 2023, max compression
+gzip compressed data, was "tiafork-1.2.3.tar", last modified: Sat Jun 10 18:09:55 2023, max compression
```

## Comparing `tiafork-1.2.2.tar` & `tiafork-1.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.529158 tiafork-1.2.2/
--rw-rw-rw-   0        0        0     1659 2023-06-10 05:31:16.000000 tiafork-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3370 2023-06-10 16:54:21.529158 tiafork-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2427 2023-06-10 16:42:23.000000 tiafork-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 16:54:21.529158 tiafork-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1872 2023-06-10 16:53:19.000000 tiafork-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.508694 tiafork-1.2.2/tiafork/
--rw-rw-rw-   0        0        0       23 2023-06-10 16:54:09.000000 tiafork-1.2.2/tiafork/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.513677 tiafork-1.2.2/tiafork/analysis/
--rw-rw-rw-   0        0        0       66 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.518276 tiafork-1.2.2/tiafork/analysis/model/
--rw-rw-rw-   0        0        0      342 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/model/__init__.py
--rw-rw-rw-   0        0        0    15668 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/analysis/model/ins.py
--rw-rw-rw-   0        0        0     3407 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/analysis/model/interface.py
--rw-rw-rw-   0        0        0    22576 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/model/pl.py
--rw-rw-rw-   0        0        0    13761 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/model/port.py
--rw-rw-rw-   0        0        0    11797 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/model/pos.py
--rw-rw-rw-   0        0        0    21045 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/analysis/model/ret.py
--rw-rw-rw-   0        0        0     3448 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/analysis/model/trd.py
--rw-rw-rw-   0        0        0     5311 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/model/txn.py
--rw-rw-rw-   0        0        0    12643 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/pdf_rpts.py
--rw-rw-rw-   0        0        0    19390 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/perf.py
--rw-rw-rw-   0        0        0     3127 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/plots.py
--rw-rw-rw-   0        0        0    12511 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/analysis/ta.py
--rw-rw-rw-   0        0        0    22716 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/analysis/talib_wrapper.py
--rw-rw-rw-   0        0        0     4463 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/analysis/util.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.520269 tiafork-1.2.2/tiafork/bbg/
--rw-rw-rw-   0        0        0      117 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/bbg/__init__.py
--rw-rw-rw-   0        0        0    25838 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/bbg/bbg_com.py
--rw-rw-rw-   0        0        0    18197 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/bbg/datamgr.py
--rw-rw-rw-   0        0        0     2323 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/bbg/example.py
--rw-rw-rw-   0        0        0    38217 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/bbg/v3api.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.523517 tiafork-1.2.2/tiafork/rlab/
--rw-rw-rw-   0        0        0      196 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/rlab/__init__.py
--rw-rw-rw-   0        0        0    11291 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/rlab/builder.py
--rw-rw-rw-   0        0        0     4287 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/rlab/components.py
--rw-rw-rw-   0        0        0      417 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/rlab/font.py
--rw-rw-rw-   0        0        0     2252 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/rlab/patch.py
--rw-rw-rw-   0        0        0     7101 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/rlab/sample.py
--rw-rw-rw-   0        0        0    41202 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/rlab/table.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.526508 tiafork-1.2.2/tiafork/tests/
--rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/tests/__init__.py
--rw-rw-rw-   0        0        0     6410 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/tests/test_analysis.py
--rw-rw-rw-   0        0        0     6790 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_datamgr.py
--rw-rw-rw-   0        0        0     4728 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_fmt.py
--rw-rw-rw-   0        0        0     5101 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_rlab_table.py
--rw-rw-rw-   0        0        0     1556 2023-06-10 03:57:52.000000 tiafork-1.2.2/tiafork/tests/test_ta.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.529158 tiafork-1.2.2/tiafork/util/
--rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/__init__.py
--rw-rw-rw-   0        0        0     1381 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/decorator.py
--rw-rw-rw-   0        0        0    12795 2023-06-10 03:57:51.000000 tiafork-1.2.2/tiafork/util/fmt.py
--rw-rw-rw-   0        0        0     1195 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/log.py
--rw-rw-rw-   0        0        0     6666 2023-06-10 03:57:53.000000 tiafork-1.2.2/tiafork/util/mplot.py
--rw-rw-rw-   0        0        0     3783 2023-06-10 03:56:02.000000 tiafork-1.2.2/tiafork/util/windows.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:54:21.510687 tiafork-1.2.2/tiafork.egg-info/
--rw-rw-rw-   0        0        0     3370 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1258 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 16:54:21.000000 tiafork-1.2.2/tiafork.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.762722 tiafork-1.2.3/
+-rw-rw-rw-   0        0        0     1659 2023-06-10 05:31:16.000000 tiafork-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3370 2023-06-10 18:09:55.762722 tiafork-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2427 2023-06-10 16:42:23.000000 tiafork-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 18:09:55.762722 tiafork-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2023-06-10 16:53:19.000000 tiafork-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.737711 tiafork-1.2.3/tiafork/
+-rw-rw-rw-   0        0        0       23 2023-06-10 18:05:57.000000 tiafork-1.2.3/tiafork/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.744002 tiafork-1.2.3/tiafork/analysis/
+-rw-rw-rw-   0        0        0       66 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.749861 tiafork-1.2.3/tiafork/analysis/model/
+-rw-rw-rw-   0        0        0      342 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/analysis/model/__init__.py
+-rw-rw-rw-   0        0        0    15668 2023-06-10 03:57:51.000000 tiafork-1.2.3/tiafork/analysis/model/ins.py
+-rw-rw-rw-   0        0        0     3407 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/analysis/model/interface.py
+-rw-rw-rw-   0        0        0    22576 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/analysis/model/pl.py
+-rw-rw-rw-   0        0        0    13761 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/analysis/model/port.py
+-rw-rw-rw-   0        0        0    11797 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/analysis/model/pos.py
+-rw-rw-rw-   0        0        0    21041 2023-06-10 18:01:56.000000 tiafork-1.2.3/tiafork/analysis/model/ret.py
+-rw-rw-rw-   0        0        0     3448 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/analysis/model/trd.py
+-rw-rw-rw-   0        0        0     5311 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/analysis/model/txn.py
+-rw-rw-rw-   0        0        0    12643 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/analysis/pdf_rpts.py
+-rw-rw-rw-   0        0        0    19390 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/analysis/perf.py
+-rw-rw-rw-   0        0        0     3127 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/analysis/plots.py
+-rw-rw-rw-   0        0        0    12511 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/analysis/ta.py
+-rw-rw-rw-   0        0        0    22712 2023-06-10 18:01:56.000000 tiafork-1.2.3/tiafork/analysis/talib_wrapper.py
+-rw-rw-rw-   0        0        0     4463 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/analysis/util.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.751854 tiafork-1.2.3/tiafork/bbg/
+-rw-rw-rw-   0        0        0      117 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/bbg/__init__.py
+-rw-rw-rw-   0        0        0    25830 2023-06-10 18:01:56.000000 tiafork-1.2.3/tiafork/bbg/bbg_com.py
+-rw-rw-rw-   0        0        0    18197 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/bbg/datamgr.py
+-rw-rw-rw-   0        0        0     2323 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/bbg/example.py
+-rw-rw-rw-   0        0        0    38217 2023-06-10 18:02:28.000000 tiafork-1.2.3/tiafork/bbg/v3api.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.754844 tiafork-1.2.3/tiafork/rlab/
+-rw-rw-rw-   0        0        0      196 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/rlab/__init__.py
+-rw-rw-rw-   0        0        0    11291 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/rlab/builder.py
+-rw-rw-rw-   0        0        0     4287 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/rlab/components.py
+-rw-rw-rw-   0        0        0      417 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/rlab/font.py
+-rw-rw-rw-   0        0        0     2252 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/rlab/patch.py
+-rw-rw-rw-   0        0        0     7101 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/rlab/sample.py
+-rw-rw-rw-   0        0        0    41202 2023-06-10 03:57:51.000000 tiafork-1.2.3/tiafork/rlab/table.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.758384 tiafork-1.2.3/tiafork/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/tests/__init__.py
+-rw-rw-rw-   0        0        0     6410 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/tests/test_analysis.py
+-rw-rw-rw-   0        0        0     6790 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/tests/test_datamgr.py
+-rw-rw-rw-   0        0        0     4728 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/tests/test_fmt.py
+-rw-rw-rw-   0        0        0     5101 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/tests/test_rlab_table.py
+-rw-rw-rw-   0        0        0     1556 2023-06-10 03:57:52.000000 tiafork-1.2.3/tiafork/tests/test_ta.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.761725 tiafork-1.2.3/tiafork/util/
+-rw-rw-rw-   0        0        0        0 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/util/__init__.py
+-rw-rw-rw-   0        0        0     1381 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/util/decorator.py
+-rw-rw-rw-   0        0        0    12781 2023-06-10 18:01:56.000000 tiafork-1.2.3/tiafork/util/fmt.py
+-rw-rw-rw-   0        0        0     1195 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/util/log.py
+-rw-rw-rw-   0        0        0     6666 2023-06-10 03:57:53.000000 tiafork-1.2.3/tiafork/util/mplot.py
+-rw-rw-rw-   0        0        0     3783 2023-06-10 03:56:02.000000 tiafork-1.2.3/tiafork/util/windows.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:09:55.740013 tiafork-1.2.3/tiafork.egg-info/
+-rw-rw-rw-   0        0        0     3370 2023-06-10 18:09:55.000000 tiafork-1.2.3/tiafork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1258 2023-06-10 18:09:55.000000 tiafork-1.2.3/tiafork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 18:09:55.000000 tiafork-1.2.3/tiafork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 18:09:55.000000 tiafork-1.2.3/tiafork.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 18:09:55.000000 tiafork-1.2.3/tiafork.egg-info/top_level.txt
```

### Comparing `tiafork-1.2.2/LICENSE` & `tiafork-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/PKG-INFO` & `tiafork-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiafork
-Version: 1.2.2
+Version: 1.2.3
 Summary: Fork of tia: Toolkit for integration and analysis
 Home-page: https://github.com/nathanramoscfa/tiafork
 Download-URL: https://github.com/nathanramoscfa/tiafork
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: BSD (3-clause)
 Keywords: bloomberg,backtesting,technical analysis,pdf
```

### Comparing `tiafork-1.2.2/README.md` & `tiafork-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/setup.py` & `tiafork-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/model/ins.py` & `tiafork-1.2.3/tiafork/analysis/model/ins.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/model/interface.py` & `tiafork-1.2.3/tiafork/analysis/model/interface.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/model/pl.py` & `tiafork-1.2.3/tiafork/analysis/model/pl.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/model/port.py` & `tiafork-1.2.3/tiafork/analysis/model/port.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/model/pos.py` & `tiafork-1.2.3/tiafork/analysis/model/pos.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/model/ret.py` & `tiafork-1.2.3/tiafork/analysis/model/ret.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from tiafork.util.mplot import AxesFormat
 from tiafork.util.fmt import PercentFormatter, new_percent_formatter, new_float_formatter
 
 
 __all__ = ['RoiiRetCalculator', 'AumRetCalculator', 'FixedAumRetCalculator', 'CumulativeRets', 'Performance']
 
 
-def return_on_initiaforkl_capital(capital, period_pl, leverage=None):
+def return_on_initial_capital(capital, period_pl, leverage=None):
     """Return the daily return series based on the capital"""
     if capital <= 0:
         raise ValueError('cost must be a positive number not %s' % capital)
     leverage = leverage or 1.
     eod = capital + (leverage * period_pl.cumsum())
     ltd_rets = (eod / capital) - 1.
     dly_rets = ltd_rets
```

### Comparing `tiafork-1.2.2/tiafork/analysis/model/trd.py` & `tiafork-1.2.3/tiafork/analysis/model/trd.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/model/txn.py` & `tiafork-1.2.3/tiafork/analysis/model/txn.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/pdf_rpts.py` & `tiafork-1.2.3/tiafork/analysis/pdf_rpts.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/perf.py` & `tiafork-1.2.3/tiafork/analysis/perf.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/plots.py` & `tiafork-1.2.3/tiafork/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/ta.py` & `tiafork-1.2.3/tiafork/analysis/ta.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/analysis/talib_wrapper.py` & `tiafork-1.2.3/tiafork/analysis/talib_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 
 def ADXR(frame, n=14, high_col='high', low_col='low', close_col='close'):
     return _frame_to_series(frame, [high_col, low_col, close_col], talib.ADXR, n)
 
 
 def APO(series, fast=12, slow=26, matype=0):
-    """double exponentiaforkl moving average"""
+    """double exponential moving average"""
     return _series_to_series(series, talib.APO, fast, slow, matype)
 
 
 def AROON(frame, n=14, high_col='high', low_col='low'):
     return _frame_to_frame(frame, [high_col, low_col], ['AroonDown', 'AroonUp'], talib.AROON, n)
```

### Comparing `tiafork-1.2.2/tiafork/analysis/util.py` & `tiafork-1.2.3/tiafork/analysis/util.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/bbg/bbg_com.py` & `tiafork-1.2.3/tiafork/bbg/bbg_com.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             return errors
         else:
             return None
 
 
 def debug_event(evt):
     print('unhandled event: %s' % evt.EventType)
-    if evt.EventType in [constants.RESPONSE, constants.PARtiaforkL_RESPONSE]:
+    if evt.EventType in [constants.RESPONSE, constants.PARTIAL_RESPONSE]:
         print('messages:')
         for msg in XmlHelper.message_iter(evt):
             print(msg.Print)
 
 
 class ResponseHandler(object):
     def do_init(self, handler):
@@ -189,15 +189,15 @@
             evt = CastTo(evt, 'Event')
             if not self.handler:
                 debug_event(evt)
 
             if evt.EventType == constants.RESPONSE:
                 self.handler.on_event(evt, is_final=True)
                 self.waiting = False
-            elif evt.EventType == constants.PARtiaforkL_RESPONSE:
+            elif evt.EventType == constants.PARTIAL_RESPONSE:
                 self.handler.on_event(evt, is_final=False)
             else:
                 self.handler.on_admin_event(evt)
         except Exception:
             import sys
 
             self.waiting = False
```

### Comparing `tiafork-1.2.2/tiafork/bbg/datamgr.py` & `tiafork-1.2.3/tiafork/bbg/datamgr.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/bbg/example.py` & `tiafork-1.2.3/tiafork/bbg/example.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/bbg/v3api.py` & `tiafork-1.2.3/tiafork/bbg/v3api.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 __all__ = ['Terminal']
 
 
 class XmlHelper(object):
     @staticmethod
     def security_iter(nodearr):
-        """ provide a security data iterator by returning a tuple of (Element, SecurityError) which are mutually exclusive """
+        """ provide a security data iterator by returning a tuple of (Element, SecurityError) which are mutually
+        exclusive"""
         assert nodearr.name() == 'securityData' and nodearr.isArray()
         for i in range(nodearr.numValues()):
             node = nodearr.getValue(i)
             err = XmlHelper.get_security_error(node)
             result = (None, err) if err else (node, None)
             yield result
 
@@ -180,15 +181,15 @@
             return errors
         else:
             return None
 
 
 def debug_event(evt):
     print('unhandled event: %s' % evt.EventType)
-    if evt.EventType in [blpapi.Event.RESPONSE, blpapi.Event.PARtiaforkL_RESPONSE]:
+    if evt.EventType in [blpapi.Event.RESPONSE, blpapi.Event.PARTIAL_RESPONSE]:
         print('messages:')
         for msg in XmlHelper.message_iter(evt):
             print(msg.Print)
 
 
 class Request(object):
     def __init__(self, svcname, ignore_security_error=0, ignore_field_error=0):
@@ -718,15 +719,15 @@
             request.new_response()
             session.sendRequest(asbbg)
             while True:
                 evt = session.nextEvent(500)
                 if evt.eventType() == blpapi.Event.RESPONSE:
                     request.on_event(evt, is_final=True)
                     break
-                elif evt.eventType() == blpapi.Event.PARtiaforkL_RESPONSE:
+                elif evt.eventType() == blpapi.Event.PARTIAL_RESPONSE:
                     request.on_event(evt, is_final=False)
                 else:
                     request.on_admin_event(evt)
             request.has_exception and request.raise_exception()
             return request.response
         finally:
             session.stop()
```

### Comparing `tiafork-1.2.2/tiafork/rlab/builder.py` & `tiafork-1.2.3/tiafork/rlab/builder.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/rlab/components.py` & `tiafork-1.2.3/tiafork/rlab/components.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/rlab/patch.py` & `tiafork-1.2.3/tiafork/rlab/patch.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/rlab/sample.py` & `tiafork-1.2.3/tiafork/rlab/sample.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/rlab/table.py` & `tiafork-1.2.3/tiafork/rlab/table.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/tests/test_analysis.py` & `tiafork-1.2.3/tiafork/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/tests/test_datamgr.py` & `tiafork-1.2.3/tiafork/tests/test_datamgr.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/tests/test_fmt.py` & `tiafork-1.2.3/tiafork/tests/test_fmt.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/tests/test_rlab_table.py` & `tiafork-1.2.3/tiafork/tests/test_rlab_table.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/tests/test_ta.py` & `tiafork-1.2.3/tiafork/tests/test_ta.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/util/decorator.py` & `tiafork-1.2.3/tiafork/util/decorator.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/util/fmt.py` & `tiafork-1.2.3/tiafork/util/fmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 pd_is_datetime_arraylike = None
 try:
     from pandas.core.common import is_datetime_arraylike as pd_is_datetime_arraylike
 except:
     pass
 
-from functools import partiaforkl
+from functools import partial
 
 
 def is_datetime_arraylike(arr):
     if isinstance(arr, pd.DataFrame):
         return arr.apply(pd_is_datetime_arraylike).all()
     elif pd_is_datetime_arraylike is not None:
         return pd_is_datetime_arraylike(arr)
@@ -84,15 +84,15 @@
 
     def __call__(self, value, **kwargs):
         # apply any overrides
         for k, v in kwargs.items():
             if hasattr(self, k):
                 setattr(self, k, v)
 
-        self_with_args = partiaforkl(self.__call__, **kwargs)
+        self_with_args = partial(self.__call__, **kwargs)
 
         if isinstance(value, pd.Series):
             return value.apply(self_with_args)
         elif isinstance(value, pd.DataFrame):
             return value.applymap(self_with_args)
         elif isinstance(value, (list, tuple)):
             return list(map(self_with_args, value))
@@ -265,23 +265,22 @@
         :return:
         """
         if method and method not in ('cell', 'col', 'row'):
             raise ValueError('method must be None, cell, row, or col')
         self.formatter_args = formatter_args
         self.method = method
 
-
     def __call__(self, value, **kwargs):
         for k in list(kwargs.keys()):
             if hasattr(self, k):
                 setattr(self, k, kwargs[k])
                 kwargs.pop(k)
         method = self.method
 
-        self_with_args = partiaforkl(self.__call__, **kwargs)
+        self_with_args = partial(self.__call__, **kwargs)
 
         if method is not None and isinstance(value, pd.DataFrame):
             if method == 'cell':
                 return value.applymap(self_with_args)
             elif method == 'row':
                 return value.T.apply(self_with_args).T
             else:
```

### Comparing `tiafork-1.2.2/tiafork/util/log.py` & `tiafork-1.2.3/tiafork/util/log.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/util/mplot.py` & `tiafork-1.2.3/tiafork/util/mplot.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork/util/windows.py` & `tiafork-1.2.3/tiafork/util/windows.py`

 * *Files identical despite different names*

### Comparing `tiafork-1.2.2/tiafork.egg-info/PKG-INFO` & `tiafork-1.2.3/tiafork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiafork
-Version: 1.2.2
+Version: 1.2.3
 Summary: Fork of tia: Toolkit for integration and analysis
 Home-page: https://github.com/nathanramoscfa/tiafork
 Download-URL: https://github.com/nathanramoscfa/tiafork
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: BSD (3-clause)
 Keywords: bloomberg,backtesting,technical analysis,pdf
```

### Comparing `tiafork-1.2.2/tiafork.egg-info/SOURCES.txt` & `tiafork-1.2.3/tiafork.egg-info/SOURCES.txt`

 * *Files identical despite different names*


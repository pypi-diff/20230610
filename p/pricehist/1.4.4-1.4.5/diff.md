# Comparing `tmp/pricehist-1.4.4.tar.gz` & `tmp/pricehist-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pricehist-1.4.4.tar", max compression
+gzip compressed data, was "pricehist-1.4.5.tar", max compression
```

## Comparing `pricehist-1.4.4.tar` & `pricehist-1.4.5.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     1071 2021-02-25 10:47:20.182855 pricehist-1.4.4/LICENSE
--rw-r--r--   0        0        0    18287 2022-04-04 15:00:57.327024 pricehist-1.4.4/README.md
--rw-r--r--   0        0        0    32357 2021-08-11 15:07:51.569519 pricehist-1.4.4/example-gnuplot.png
--rw-r--r--   0        0        0     1028 2023-01-25 10:51:57.538251 pricehist-1.4.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-01-25 10:52:01.041604 pricehist-1.4.4/src/pricehist/__init__.py
--rw-r--r--   0        0        0     2486 2021-08-19 18:52:25.316893 pricehist-1.4.4/src/pricehist/beanprice/__init__.py
--rw-r--r--   0        0        0      131 2021-07-21 13:20:19.305599 pricehist-1.4.4/src/pricehist/beanprice/alphavantage.py
--rw-r--r--   0        0        0      131 2021-12-26 21:09:06.732942 pricehist-1.4.4/src/pricehist/beanprice/bankofcanada.py
--rw-r--r--   0        0        0      128 2021-08-23 11:16:49.689972 pricehist-1.4.4/src/pricehist/beanprice/coinbasepro.py
--rw-r--r--   0        0        0      119 2021-08-10 11:13:52.406963 pricehist-1.4.4/src/pricehist/beanprice/coindesk.py
--rw-r--r--   0        0        0      134 2021-07-21 13:20:34.735690 pricehist-1.4.4/src/pricehist/beanprice/coinmarketcap.py
--rw-r--r--   0        0        0      104 2021-07-21 13:20:45.325752 pricehist-1.4.4/src/pricehist/beanprice/ecb.py
--rw-r--r--   0        0        0      143 2022-05-15 12:48:06.721091 pricehist-1.4.4/src/pricehist/beanprice/exchangeratehost.py
--rw-r--r--   0        0        0      110 2021-07-21 13:20:57.255822 pricehist-1.4.4/src/pricehist/beanprice/yahoo.py
--rw-r--r--   0        0        0    10630 2022-04-04 15:00:25.073491 pricehist-1.4.4/src/pricehist/cli.py
--rw-r--r--   0        0        0     2840 2021-12-26 23:12:39.908013 pricehist-1.4.4/src/pricehist/exceptions.py
--rw-r--r--   0        0        0     2716 2021-08-23 14:43:14.334311 pricehist-1.4.4/src/pricehist/fetch.py
--rw-r--r--   0        0        0     1892 2022-04-04 14:48:35.312436 pricehist-1.4.4/src/pricehist/format.py
--rw-r--r--   0        0        0     3379 2022-09-23 15:07:14.780903 pricehist-1.4.4/src/pricehist/isocurrencies.py
--rw-r--r--   0        0        0      850 2022-04-04 14:29:02.488423 pricehist-1.4.4/src/pricehist/logger.py
--rw-r--r--   0        0        0      327 2022-04-04 11:39:57.464444 pricehist-1.4.4/src/pricehist/outputs/__init__.py
--rw-r--r--   0        0        0      316 2021-08-04 10:40:11.475843 pricehist-1.4.4/src/pricehist/outputs/baseoutput.py
--rw-r--r--   0        0        0     1202 2021-07-30 12:23:11.850869 pricehist-1.4.4/src/pricehist/outputs/beancount.py
--rw-r--r--   0        0        0     1340 2021-06-11 19:29:03.394043 pricehist-1.4.4/src/pricehist/outputs/csv.py
--rw-r--r--   0        0        0     6525 2022-11-24 12:49:57.294701 pricehist-1.4.4/src/pricehist/outputs/gnucashsql.py
--rw-r--r--   0        0        0     1302 2022-04-04 14:50:55.533306 pricehist-1.4.4/src/pricehist/outputs/json.py
--rw-r--r--   0        0        0     1439 2021-07-30 12:22:53.977329 pricehist-1.4.4/src/pricehist/outputs/ledger.py
--rw-r--r--   0        0        0      135 2021-05-26 13:13:22.917056 pricehist-1.4.4/src/pricehist/price.py
--rw-r--r--   0        0        0        0 2021-04-22 11:12:27.944070 pricehist-1.4.4/src/pricehist/resources/__init__.py
--rw-r--r--   0        0        0     2052 2021-08-24 11:48:42.317971 pricehist-1.4.4/src/pricehist/resources/gnucash.sql
--rw-r--r--   0        0        0    47640 2023-01-25 10:45:37.000000 pricehist-1.4.4/src/pricehist/resources/list-one.xml
--rw-r--r--   0        0        0    29515 2023-01-25 10:46:06.000000 pricehist-1.4.4/src/pricehist/resources/list-three.xml
--rw-r--r--   0        0        0     1416 2021-09-14 06:38:59.436958 pricehist-1.4.4/src/pricehist/series.py
--rw-r--r--   0        0        0      613 2023-01-25 10:51:14.278009 pricehist-1.4.4/src/pricehist/sources/__init__.py
--rw-r--r--   0        0        0    13211 2022-11-24 14:04:17.568956 pricehist-1.4.4/src/pricehist/sources/alphavantage.py
--rw-r--r--   0        0        0     3665 2021-12-26 21:20:16.239801 pricehist-1.4.4/src/pricehist/sources/bankofcanada.py
--rw-r--r--   0        0        0     3797 2021-09-14 06:57:40.980843 pricehist-1.4.4/src/pricehist/sources/basesource.py
--rw-r--r--   0        0        0     5710 2021-08-23 16:39:06.225980 pricehist-1.4.4/src/pricehist/sources/coinbasepro.py
--rw-r--r--   0        0        0     4261 2022-11-24 14:29:25.062199 pricehist-1.4.4/src/pricehist/sources/coindesk.py
--rw-r--r--   0        0        0     7229 2021-07-17 16:40:53.502235 pricehist-1.4.4/src/pricehist/sources/coinmarketcap.py
--rw-r--r--   0        0        0     2989 2021-07-14 11:10:14.211009 pricehist-1.4.4/src/pricehist/sources/ecb.py
--rw-r--r--   0        0        0     4057 2022-05-15 12:54:38.734173 pricehist-1.4.4/src/pricehist/sources/exchangeratehost.py
--rw-r--r--   0        0        0     6731 2021-11-12 12:53:22.622927 pricehist-1.4.4/src/pricehist/sources/yahoo.py
--rw-r--r--   0        0        0    19821 1970-01-01 00:00:00.000000 pricehist-1.4.4/setup.py
--rw-r--r--   0        0        0    19202 1970-01-01 00:00:00.000000 pricehist-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-02-25 10:47:20.182855 pricehist-1.4.5/LICENSE
+-rw-r--r--   0        0        0    18287 2023-05-29 12:16:33.195814 pricehist-1.4.5/README.md
+-rw-r--r--   0        0        0    32357 2021-08-11 15:07:51.569519 pricehist-1.4.5/example-gnuplot.png
+-rw-r--r--   0        0        0     1028 2023-06-10 11:35:06.421097 pricehist-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-10 11:35:10.357477 pricehist-1.4.5/src/pricehist/__init__.py
+-rw-r--r--   0        0        0     2486 2021-08-19 18:52:25.316893 pricehist-1.4.5/src/pricehist/beanprice/__init__.py
+-rw-r--r--   0        0        0      131 2021-07-21 13:20:19.305599 pricehist-1.4.5/src/pricehist/beanprice/alphavantage.py
+-rw-r--r--   0        0        0      131 2021-12-26 21:09:06.732942 pricehist-1.4.5/src/pricehist/beanprice/bankofcanada.py
+-rw-r--r--   0        0        0      128 2021-08-23 11:16:49.689972 pricehist-1.4.5/src/pricehist/beanprice/coinbasepro.py
+-rw-r--r--   0        0        0      119 2021-08-10 11:13:52.406963 pricehist-1.4.5/src/pricehist/beanprice/coindesk.py
+-rw-r--r--   0        0        0      134 2021-07-21 13:20:34.735690 pricehist-1.4.5/src/pricehist/beanprice/coinmarketcap.py
+-rw-r--r--   0        0        0      104 2021-07-21 13:20:45.325752 pricehist-1.4.5/src/pricehist/beanprice/ecb.py
+-rw-r--r--   0        0        0      143 2022-05-15 12:48:06.721091 pricehist-1.4.5/src/pricehist/beanprice/exchangeratehost.py
+-rw-r--r--   0        0        0      110 2021-07-21 13:20:57.255822 pricehist-1.4.5/src/pricehist/beanprice/yahoo.py
+-rw-r--r--   0        0        0    10630 2022-04-04 15:00:25.073491 pricehist-1.4.5/src/pricehist/cli.py
+-rw-r--r--   0        0        0     2840 2021-12-26 23:12:39.908013 pricehist-1.4.5/src/pricehist/exceptions.py
+-rw-r--r--   0        0        0     2716 2021-08-23 14:43:14.334311 pricehist-1.4.5/src/pricehist/fetch.py
+-rw-r--r--   0        0        0     1892 2022-04-04 14:48:35.312436 pricehist-1.4.5/src/pricehist/format.py
+-rw-r--r--   0        0        0     3493 2023-06-10 11:06:16.207889 pricehist-1.4.5/src/pricehist/isocurrencies.py
+-rw-r--r--   0        0        0      850 2022-04-04 14:29:02.488423 pricehist-1.4.5/src/pricehist/logger.py
+-rw-r--r--   0        0        0      327 2022-04-04 11:39:57.464444 pricehist-1.4.5/src/pricehist/outputs/__init__.py
+-rw-r--r--   0        0        0      316 2021-08-04 10:40:11.475843 pricehist-1.4.5/src/pricehist/outputs/baseoutput.py
+-rw-r--r--   0        0        0     1202 2021-07-30 12:23:11.850869 pricehist-1.4.5/src/pricehist/outputs/beancount.py
+-rw-r--r--   0        0        0     1340 2021-06-11 19:29:03.394043 pricehist-1.4.5/src/pricehist/outputs/csv.py
+-rw-r--r--   0        0        0     6629 2023-06-10 11:07:50.047796 pricehist-1.4.5/src/pricehist/outputs/gnucashsql.py
+-rw-r--r--   0        0        0     1302 2022-04-04 14:50:55.533306 pricehist-1.4.5/src/pricehist/outputs/json.py
+-rw-r--r--   0        0        0     1439 2021-07-30 12:22:53.977329 pricehist-1.4.5/src/pricehist/outputs/ledger.py
+-rw-r--r--   0        0        0      135 2021-05-26 13:13:22.917056 pricehist-1.4.5/src/pricehist/price.py
+-rw-r--r--   0        0        0        0 2021-04-22 11:12:27.944070 pricehist-1.4.5/src/pricehist/resources/__init__.py
+-rw-r--r--   0        0        0     2052 2021-08-24 11:48:42.317971 pricehist-1.4.5/src/pricehist/resources/gnucash.sql
+-rw-r--r--   0        0        0    47640 2023-05-26 15:19:35.000000 pricehist-1.4.5/src/pricehist/resources/list-one.xml
+-rw-r--r--   0        0        0    29515 2023-05-26 15:31:08.000000 pricehist-1.4.5/src/pricehist/resources/list-three.xml
+-rw-r--r--   0        0        0     1416 2021-09-14 06:38:59.436958 pricehist-1.4.5/src/pricehist/series.py
+-rw-r--r--   0        0        0      613 2023-01-25 10:51:14.278009 pricehist-1.4.5/src/pricehist/sources/__init__.py
+-rw-r--r--   0        0        0    13211 2022-11-24 14:04:17.568956 pricehist-1.4.5/src/pricehist/sources/alphavantage.py
+-rw-r--r--   0        0        0     3665 2021-12-26 21:20:16.239801 pricehist-1.4.5/src/pricehist/sources/bankofcanada.py
+-rw-r--r--   0        0        0     3797 2021-09-14 06:57:40.980843 pricehist-1.4.5/src/pricehist/sources/basesource.py
+-rw-r--r--   0        0        0     5710 2021-08-23 16:39:06.225980 pricehist-1.4.5/src/pricehist/sources/coinbasepro.py
+-rw-r--r--   0        0        0     4261 2022-11-24 14:29:25.062199 pricehist-1.4.5/src/pricehist/sources/coindesk.py
+-rw-r--r--   0        0        0     7229 2021-07-17 16:40:53.502235 pricehist-1.4.5/src/pricehist/sources/coinmarketcap.py
+-rw-r--r--   0        0        0     2989 2021-07-14 11:10:14.211009 pricehist-1.4.5/src/pricehist/sources/ecb.py
+-rw-r--r--   0        0        0     4057 2022-05-15 12:54:38.734173 pricehist-1.4.5/src/pricehist/sources/exchangeratehost.py
+-rw-r--r--   0        0        0     6841 2023-06-10 11:24:49.696986 pricehist-1.4.5/src/pricehist/sources/yahoo.py
+-rw-r--r--   0        0        0    19202 1970-01-01 00:00:00.000000 pricehist-1.4.5/PKG-INFO
```

### Comparing `pricehist-1.4.4/LICENSE` & `pricehist-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/README.md` & `pricehist-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/example-gnuplot.png` & `pricehist-1.4.5/example-gnuplot.png`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/pyproject.toml` & `pricehist-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pricehist"
-version = "1.4.4"
+version = "1.4.5"
 description = "Fetch and format historical price data"
 authors = ["Chris Berkhout <chris@chrisberkhout.com>"]
 license = "MIT"
 keywords = ["historical", "prices", "plaintext", "accounting", "csv", "gnucash", "ledger", "hledger", "beancount"]
 readme = "README.md"
 homepage = "https://gitlab.com/chrisberkhout/pricehist"
 repository = "https://gitlab.com/chrisberkhout/pricehist"
```

### Comparing `pricehist-1.4.4/src/pricehist/beanprice/__init__.py` & `pricehist-1.4.5/src/pricehist/beanprice/__init__.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/cli.py` & `pricehist-1.4.5/src/pricehist/cli.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/exceptions.py` & `pricehist-1.4.5/src/pricehist/exceptions.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/fetch.py` & `pricehist-1.4.5/src/pricehist/fetch.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/format.py` & `pricehist-1.4.5/src/pricehist/format.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/isocurrencies.py` & `pricehist-1.4.5/src/pricehist/isocurrencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     current_data_date() -> str
     historical_data_date() -> str
     by_code() -> dict[str, ISOCurrency]
 
 """
 
 from dataclasses import dataclass, field
-from importlib.resources import read_binary
+from importlib.resources import files
 from typing import List
 
 from lxml import etree
 
 
 @dataclass(frozen=False)
 class ISOCurrency:
@@ -39,28 +39,36 @@
     is_fund: bool = False
     countries: List[str] = field(default_factory=list)
     historical: bool = False
     withdrawal_date: str = None
 
 
 def current_data_date():
-    one = etree.fromstring(read_binary("pricehist.resources", "list-one.xml"))
+    one = etree.fromstring(
+        files("pricehist.resources").joinpath("list-one.xml").read_bytes()
+    )
     return one.cssselect("ISO_4217")[0].attrib["Pblshd"]
 
 
 def historical_data_date():
-    three = etree.fromstring(read_binary("pricehist.resources", "list-three.xml"))
+    three = etree.fromstring(
+        files("pricehist.resources").joinpath("list-three.xml").read_bytes()
+    )
     return three.cssselect("ISO_4217")[0].attrib["Pblshd"]
 
 
 def by_code():
     result = {}
 
-    one = etree.fromstring(read_binary("pricehist.resources", "list-one.xml"))
-    three = etree.fromstring(read_binary("pricehist.resources", "list-three.xml"))
+    one = etree.fromstring(
+        files("pricehist.resources").joinpath("list-one.xml").read_bytes()
+    )
+    three = etree.fromstring(
+        files("pricehist.resources").joinpath("list-three.xml").read_bytes()
+    )
 
     for entry in three.cssselect("HstrcCcyNtry") + one.cssselect("CcyNtry"):
         if currency := _parse(entry):
             if existing := result.get(currency.code):
                 existing.code = currency.code
                 existing.number = currency.number
                 existing.minor_units = currency.minor_units
```

### Comparing `pricehist-1.4.4/src/pricehist/logger.py` & `pricehist-1.4.5/src/pricehist/logger.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/outputs/beancount.py` & `pricehist-1.4.5/src/pricehist/outputs/beancount.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/outputs/csv.py` & `pricehist-1.4.5/src/pricehist/outputs/csv.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/outputs/gnucashsql.py` & `pricehist-1.4.5/src/pricehist/outputs/gnucashsql.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 """
 
 import hashlib
 import logging
 from datetime import datetime
 from decimal import Decimal
-from importlib.resources import read_text
+from importlib.resources import files
 
 from pricehist import __version__
 from pricehist.format import Format
 
 from .baseoutput import BaseOutput
 
 
@@ -115,21 +115,26 @@
                 "This SQL contains numbers outside of the int64 range required "
                 "by GnuCash for the numerators and denominators of prices. "
                 "Using the --quantize option to limit the number of decimal "
                 "places will usually reduce the size of the rational form as "
                 "well."
             )
 
-        sql = read_text("pricehist.resources", "gnucash.sql").format(
-            version=__version__,
-            timestamp=datetime.utcnow().isoformat() + "Z",
-            base=self._sql_str(base),
-            quote=self._sql_str(quote),
-            values_comment=values_comment,
-            values=values,
+        sql = (
+            files("pricehist.resources")
+            .joinpath("gnucash.sql")
+            .read_text()
+            .format(
+                version=__version__,
+                timestamp=datetime.utcnow().isoformat() + "Z",
+                base=self._sql_str(base),
+                quote=self._sql_str(quote),
+                values_comment=values_comment,
+                values=values,
+            )
         )
 
         return sql
 
     def _warn_about_backslashes(self, fields):
         hits = [name for name, value in fields.items() if "\\" in value]
         if hits:
```

### Comparing `pricehist-1.4.4/src/pricehist/outputs/json.py` & `pricehist-1.4.5/src/pricehist/outputs/json.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/outputs/ledger.py` & `pricehist-1.4.5/src/pricehist/outputs/ledger.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/resources/gnucash.sql` & `pricehist-1.4.5/src/pricehist/resources/gnucash.sql`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/resources/list-one.xml` & `pricehist-1.4.5/src/pricehist/resources/list-one.xml`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/resources/list-three.xml` & `pricehist-1.4.5/src/pricehist/resources/list-three.xml`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/series.py` & `pricehist-1.4.5/src/pricehist/series.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/__init__.py` & `pricehist-1.4.5/src/pricehist/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/alphavantage.py` & `pricehist-1.4.5/src/pricehist/sources/alphavantage.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/bankofcanada.py` & `pricehist-1.4.5/src/pricehist/sources/bankofcanada.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/basesource.py` & `pricehist-1.4.5/src/pricehist/sources/basesource.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/coinbasepro.py` & `pricehist-1.4.5/src/pricehist/sources/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/coindesk.py` & `pricehist-1.4.5/src/pricehist/sources/coindesk.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/coinmarketcap.py` & `pricehist-1.4.5/src/pricehist/sources/coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/ecb.py` & `pricehist-1.4.5/src/pricehist/sources/ecb.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/exchangeratehost.py` & `pricehist-1.4.5/src/pricehist/sources/exchangeratehost.py`

 * *Files identical despite different names*

### Comparing `pricehist-1.4.4/src/pricehist/sources/yahoo.py` & `pricehist-1.4.5/src/pricehist/sources/yahoo.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         )
         end_ts = int(
             datetime.strptime(series.end, "%Y-%m-%d")
             .replace(tzinfo=timezone.utc)
             .timestamp()
         ) + (
             24 * 60 * 60
-        )  # round up to include the last day
+        )  # some symbols require padding on the end timestamp
 
         history_url = f"{base_url}/download/{series.base}"
         history_params = {
             "period1": start_ts,
             "period2": end_ts,
             "interval": "1d",
             "events": "history",
@@ -187,8 +187,10 @@
             history = csv.DictReader(history_lines, delimiter=",")
         except Exception as e:
             raise exceptions.ResponseParsingError(str(e)) from e
 
         if history_lines[0] != "date,open,high,low,close,adjclose,volume":
             raise exceptions.ResponseParsingError("Unexpected CSV format")
 
-        return (quote, history)
+        requested_history = [row for row in history if row["date"] <= series.end]
+
+        return (quote, requested_history)
```

### Comparing `pricehist-1.4.4/setup.py` & `pricehist-1.4.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,485 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pricehist
+Version: 1.4.5
+Summary: Fetch and format historical price data
+Home-page: https://gitlab.com/chrisberkhout/pricehist
+License: MIT
+Keywords: historical,prices,plaintext,accounting,csv,gnucash,ledger,hledger,beancount
+Author: Chris Berkhout
+Author-email: chris@chrisberkhout.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cssselect (>=1.1.0,<2.0.0)
+Requires-Dist: curlify (>=2.2.1,<3.0.0)
+Requires-Dist: lxml (>=4.6.2,<5.0.0)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Project-URL: Repository, https://gitlab.com/chrisberkhout/pricehist
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# pricehist
 
-packages = \
-['pricehist',
- 'pricehist.beanprice',
- 'pricehist.outputs',
- 'pricehist.resources',
- 'pricehist.sources']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cssselect>=1.1.0,<2.0.0',
- 'curlify>=2.2.1,<3.0.0',
- 'lxml>=4.6.2,<5.0.0',
- 'requests>=2.25.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['pricehist = pricehist.cli:cli']}
-
-setup_kwargs = {
-    'name': 'pricehist',
-    'version': '1.4.4',
-    'description': 'Fetch and format historical price data',
-    'long_description': '# pricehist\n\nA command-line tool for fetching and formatting historical price data, with\nsupport for multiple data sources and output formats.\n\n[![Pipeline status](https://gitlab.com/chrisberkhout/pricehist/badges/master/pipeline.svg)](https://gitlab.com/chrisberkhout/pricehist/-/commits/master)\n[![Coverage report](https://gitlab.com/chrisberkhout/pricehist/badges/master/coverage.svg)](https://gitlab.com/chrisberkhout/pricehist/-/commits/master)\n[![PyPI version](https://badge.fury.io/py/pricehist.svg)](https://badge.fury.io/py/pricehist)\n[![Downloads](https://pepy.tech/badge/pricehist)](https://pepy.tech/project/pricehist)\n[![License](https://img.shields.io/pypi/l/pricehist)](https://gitlab.com/chrisberkhout/pricehist/-/blob/master/LICENSE)\n[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgitlab.com%2Fchrisberkhout%2Fpricehist&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)\n\n## Installation\n\nInstall via pip or\n[pipx](https://pypa.github.io/pipx/).\n\n```\npipx install pricehist\n```\n\n## Sources\n\n- **`alphavantage`**: [Alpha Vantage](https://www.alphavantage.co/)\n- **`bankofcanada`**: [Bank of Canada daily exchange rates](https://www.bankofcanada.ca/valet/docs)\n- **`coinbasepro`**: [Coinbase Pro](https://pro.coinbase.com/)\n- **`coindesk`**: [CoinDesk Bitcoin Price Index](https://www.coindesk.com/coindesk-api)\n- **`coinmarketcap`**: [CoinMarketCap](https://coinmarketcap.com/)\n- **`ecb`**: [European Central Bank Euro foreign exchange reference rates](https://www.ecb.europa.eu/stats/exchange/eurofxref/html/index.en.html)\n- **`yahoo`**: [Yahoo! Finance](https://finance.yahoo.com/)\n\n## Output formats\n\n- **`beancount`**: [Beancount](http://furius.ca/beancount/)\n- **`csv`**: [Comma-separated values](https://en.wikipedia.org/wiki/Comma-separated_values)\n- **`json`**: [JSON](https://en.wikipedia.org/wiki/JSON)\n- **`jsonl`**: [JSON lines](https://en.wikipedia.org/wiki/JSON_streaming)\n- **`gnucash-sql`**: [GnuCash](https://www.gnucash.org/) SQL\n- **`ledger`**: [Ledger](https://www.ledger-cli.org/) and [hledger](https://hledger.org/)\n\n## Reactions\n\n> This is my new favourite price fetcher, by far.  \n> -- _Simon Michael, creator of [hledger](https://hledger.org/) ([ref](https://groups.google.com/g/hledger/c/SCLbNiKl9D8/m/0ReYmDppAAAJ))_\n\n> This is great!  \n> -- _Martin Blais, creator of [Beancount](https://beancount.github.io/) ([ref](https://groups.google.com/g/beancount/c/cCJc9OhIlNg/m/QGRvNowcAwAJ))_\n\n## How to\n\n### Fetch prices\n\nFetch prices by choosing a source, a pair and, optionally, a time interval.\n\n```\npricehist fetch ecb EUR/AUD -s 2021-01-04 -e 2021-01-08\n```\n```\ndate,base,quote,amount,source,type\n2021-01-04,EUR,AUD,1.5928,ecb,reference\n2021-01-05,EUR,AUD,1.5927,ecb,reference\n2021-01-06,EUR,AUD,1.5824,ecb,reference\n2021-01-07,EUR,AUD,1.5836,ecb,reference\n2021-01-08,EUR,AUD,1.5758,ecb,reference\n```\n\nThe default output format is CSV, which is suitable for use in spreadsheets and\nwith other tools. For example, you can generate a price chart from the command\nline as follows (or using [an alias](https://gitlab.com/-/snippets/2163031)).\n\n```\npricehist fetch coindesk BTC/USD -s 2021-01-01 | \\\n  sed 1d | \\\n  cut -d, -f1,4 | \\\n  gnuplot -p -e \'\n    set datafile separator ",";\n    set xdata time;\n    set timefmt "%Y-%m-%d";\n    set format x "%b\\n%Y";\n    plot "/dev/stdin" using 1:2 with lines title "BTC/USD"\n  \'\n```\n\n![BTC/USD prices](https://gitlab.com/chrisberkhout/pricehist/-/raw/master/example-gnuplot.png)\n\n### Show usage information\n\nAdd `-h` to any command to see usage information.\n\n```\npricehist fetch -h\n```\n```\nusage: pricehist fetch SOURCE PAIR [-h] [-vvv] [-t TYPE] [-s DATE | -sx DATE] [-e DATE | -ex DATE]\n[-o beancount|csv|json|jsonl|gnucash-sql|ledger] [--invert] [--quantize INT]\n[--fmt-base SYM] [--fmt-quote SYM] [--fmt-time TIME] [--fmt-decimal CHAR] [--fmt-thousands CHAR]\n[--fmt-symbol rightspace|right|leftspace|left] [--fmt-datesep CHAR]\n[--fmt-csvdelim CHAR] [--fmt-jsonnums]\n\npositional arguments:\n  SOURCE                   the source identifier\n  PAIR                     pair, usually BASE/QUOTE, e.g. BTC/USD\n\noptional arguments:\n  -h, --help               show this help message and exit\n  -vvv, --verbose          show all log messages\n  -t TYPE, --type TYPE     price type, e.g. close\n  -s DATE, --start DATE    start date, inclusive (default: source start)\n  -sx DATE, --startx DATE  start date, exclusive\n  -e DATE, --end DATE      end date, inclusive (default: today)\n  -ex DATE, --endx DATE    end date, exclusive\n  -o FMT, --output FMT     output format (default: csv)\n  --invert                 invert the price, swapping base and quote\n  --quantize INT           round to the given number of decimal places\n  --fmt-base SYM           rename the base symbol in output\n  --fmt-quote SYM          rename the quote symbol in output\n  --fmt-time TIME          set a particular time of day in output (default: 00:00:00)\n  --fmt-decimal CHAR       decimal point in output (default: \'.\')\n  --fmt-thousands CHAR     thousands separator in output (default: \'\')\n  --fmt-symbol LOCATION    commodity symbol placement in output (default: rightspace)\n  --fmt-datesep CHAR       date separator in output (default: \'-\')\n  --fmt-csvdelim CHAR      field delimiter for CSV output (default: \',\')\n  --fmt-jsonnums           numbers not strings for JSON output (default: False)\n```\n\n### Choose and customize the output format\n\nAs the output format you can choose one of `beancount`, `csv`, `json`, `jsonl`,\n`ledger` or `gnucash-sql`.\n\n```\npricehist fetch ecb EUR/AUD -s 2021-01-04 -e 2021-01-08 -o ledger\n```\n```\nP 2021-01-04 00:00:00 EUR 1.5928 AUD\nP 2021-01-05 00:00:00 EUR 1.5927 AUD\nP 2021-01-06 00:00:00 EUR 1.5824 AUD\nP 2021-01-07 00:00:00 EUR 1.5836 AUD\nP 2021-01-08 00:00:00 EUR 1.5758 AUD\n```\n\nFormatting options let you control certain details of the output.\n\n```\npricehist fetch ecb EUR/AUD -s 2021-01-04 -e 2021-01-08 -o ledger \\\n  --fmt-time \'\' --fmt-datesep / --fmt-base € --fmt-quote $ --fmt-symbol left\n```\n```\nP 2021/01/04 € $1.5928\nP 2021/01/05 € $1.5927\nP 2021/01/06 € $1.5824\nP 2021/01/07 € $1.5836\nP 2021/01/08 € $1.5758\n```\n\n### Fetch new prices only\n\nYou can update an existing file without refetching the prices you already have.\nFirst find the date of the last price, then fetch from there, drop the header\nline if present and append the rest to the existing file.\n\n```\nlast=$(tail -1 prices-eur-usd.csv | cut -d, -f1)\npricehist fetch ecb EUR/USD -sx $last -o csv | sed 1d >> prices-eur-usd.csv\n```\n\n### Load prices into GnuCash\n\nYou can generate SQL for a GnuCash database and apply it immediately with one\nof the following commands.\n\n```\npricehist fetch ecb EUR/AUD -s 2021-01-01 -o gnucash-sql | sqlite3 Accounts.gnucash\npricehist fetch ecb EUR/AUD -s 2021-01-01 -o gnucash-sql | mysql -u username -p -D databasename\npricehist fetch ecb EUR/AUD -s 2021-01-01 -o gnucash-sql | psql -U username -d databasename -v ON_ERROR_STOP=1\n```\n\nBeware that the GnuCash project itself does not support integration at the\ndatabase level, so there is a risk that the SQL generated by `pricehist` will\nbe ineffective or even damaging for some version of GnuCash. In practice, this\nstrategy has been used successfully by other projects. Reading the SQL and\nkeeping regular database backups is recommended.\n\nThe GnuCash database must already contain commodities with mnemonics matching\nthe base and quote of new prices, otherwise the SQL will fail without making\nchanges.\n\nEach price entry is given a GUID based on its content (date, base, quote,\nsource, type and amount) and existing GUIDs are skipped in the final insert, so\nyou can apply identical or overlapping SQL files multiple times without\ncreating duplicate entries in the database.\n\n### Show source information\n\nThe `source` command shows information about a source.\n\n```\npricehist source alphavantage\n```\n```\nID          : alphavantage\nName        : Alpha Vantage\nDescription : Provider of market data for stocks, forex and cryptocurrencies\nURL         : https://www.alphavantage.co/\nStart       : 1995-01-01\nTypes       : close, open, high, low, adjclose, mid\nNotes       : Alpha Vantage has data on...\n```\n\nAvailable symbols can be listed for most sources, either as full pairs or as\nseparate base and quote symbols that will work in certain combinations.\n\n```\npricehist source ecb --symbols\n```\n```\nEUR/AUD    Euro against Australian Dollar\nEUR/BGN    Euro against Bulgarian Lev\nEUR/BRL    Euro against Brazilian Real\nEUR/CAD    Euro against Canadian Dollar\nEUR/CHF    Euro against Swiss Franc\n...\n```\n\nIt may also be possible to search for symbols.\n\n```\npricehist source alphavantage --search Tesla\n```\n```\nTL0.DEX       Tesla, Equity, XETRA, EUR\nTL0.FRK       Tesla, Equity, Frankfurt, EUR\nTSLA34.SAO    Tesla, Equity, Brazil/Sao Paolo, BRL\nTSLA          Tesla Inc, Equity, United States, USD\nTXLZF         Tesla Exploration Ltd, Equity, United States, USD\n```\n\n### Inspect source interactions\n\nYou can see extra information by adding the verbose option (`--verbose` or\n`-vvv`), including `curl` commands that reproduce each request to a source.\n\n```\npricehist fetch coindesk BTC/USD -s 2021-01-01 -e 2021-01-05 -vvv\n```\n```\nDEBUG Began pricehist run at 2021-08-12 14:38:26.630357.\nDEBUG Starting new HTTPS connection (1): api.coindesk.com:443\nDEBUG https://api.coindesk.com:443 "GET /v1/bpi/historical/close.json?currency=USD&start=2021-01-01&end=2021-01-05 HTTP/1.1" 200 319\nDEBUG curl -X GET -H \'Accept: */*\' -H \'Accept-Encoding: gzip, deflate\' -H \'Connection: keep-alive\' -H \'User-Agent: python-requests/2.25.1\' --compressed \'https://api.coindesk.com/v1/bpi/historical/close.json?currency=USD&start=2021-01-01&end=2021-01-05\'\nDEBUG Available data covers the interval [2021-01-01--2021-01-05], as requested.\ndate,base,quote,amount,source,type\n2021-01-01,BTC,USD,29391.775,coindesk,close\n2021-01-02,BTC,USD,32198.48,coindesk,close\n2021-01-03,BTC,USD,33033.62,coindesk,close\n2021-01-04,BTC,USD,32017.565,coindesk,close\n2021-01-05,BTC,USD,34035.0067,coindesk,close\nDEBUG Ended pricehist run at 2021-08-12 14:38:26.709428.\n```\n\nRunning a logged `curl` command shows exactly what data is returned by the\nsource.\n\n```\npricehist fetch coindesk BTC/USD -s 2021-01-01 -e 2021-01-05 -vvv 2>&1 \\\n  | grep \'^DEBUG curl\' | sed \'s/^DEBUG //\' | bash | jq .\n```\n```json\n{\n  "bpi": {\n    "2021-01-01": 29391.775,\n    "2021-01-02": 32198.48,\n    "2021-01-03": 33033.62,\n    "2021-01-04": 32017.565,\n    "2021-01-05": 34035.0067\n  },\n  "disclaimer": "This data was produced from the CoinDesk Bitcoin Price Index. BPI value data returned as USD.",\n  "time": {\n    "updated": "Jan 6, 2021 00:03:00 UTC",\n    "updatedISO": "2021-01-06T00:03:00+00:00"\n  }\n}\n```\n\n### Use via `bean-price`\n\nBeancount users may wish to use `pricehist` sources via `bean-price`. To do so,\nensure the `pricehist` package is installed in an accessible location.\n\nYou can fetch the latest price directly from the command line.\n\n```\nbean-price -e "USD:pricehist.beanprice.coindesk/BTC:USD"\n```\n```\n2021-08-18 price BTC:USD                          44725.12 USD\n```\n\nYou can fetch a series of prices by providing a Beancount file as input.\n\n```\n; input.beancount\n2021-08-14 commodity BTC\n  price: "USD:pricehist.beanprice.coindesk/BTC:USD:close"\n```\n\n```\nbean-price input.beancount --update --update-rate daily --inactive --clear-cache\n```\n```\n2021-08-14 price BTC                            47098.2633 USD\n2021-08-15 price BTC                            47018.9017 USD\n2021-08-16 price BTC                             45927.405 USD\n2021-08-17 price BTC                            44686.3333 USD\n2021-08-18 price BTC                              44725.12 USD\n```\n\nAdding `-v` will print progress information, `-vv` will print debug information,\nincluding that from `pricehist`.\n\nA source map specification for `bean-price` has the form\n`<currency>:<module>/[^]<ticker>`. Additional `<module>/[^]<ticker>` parts can\nbe appended, separated by commas.\n\nThe module name will be of the form `pricehist.beanprice.<source_id>`.\n\nThe ticker symbol will be of the form `BASE:QUOTE:TYPE`.\n\nAny non-alphanumeric characters except the equals sign (`=`), hyphen (`-`),\nperiod (`.`), or parentheses (`(` or `)`) are special characters that need to\nbe encoded as their a two-digit hexadecimal code prefixed with an underscore,\nbecause `bean-price` ticker symbols don\'t allow all the characters used by\n`pricehist` pairs.\n[This page](https://replit.com/@chrisberkhout/bpticker) will do it for you.\n\nFor example, the Yahoo! Finance symbol for the Dow Jones Industrial Average is\n`^DJI`, and would have the source map specification\n`USD:pricehist.beanprice.yahoo/_5eDJI`, or for the daily high price\n`USD:pricehist.beanprice.yahoo/_5eDJI::high`.\n\n### Use as a library\n\nYou may find `pricehist`\'s source classes useful in your own scripts.\n\n```\n$\xa0python\nPython 3.9.6 (default, Jun 30 2021, 10:22:16)\n[GCC 11.1.0] on linux\nType "help", "copyright", "credits" or "license" for more information.\n>>> from pricehist.series import Series\n>>> from pricehist.sources.ecb import ECB\n>>> series = ECB().fetch(Series("EUR", "AUD", "reference", "2021-01-04", "2021-01-08"))\n>>> series.prices\n[Price(date=\'2021-01-04\', amount=Decimal(\'1.5928\')), Price(date=\'2021-01-05\', amount=Decimal(\'1.5927\')), Price(date=\'2021-01-06\', amount=Decimal(\'1.5824\')), Price(date=\'2021-01-07\', amount=Decimal(\'1.5836\')), Price(date=\'2021-01-08\', amount=Decimal(\'1.5758\'))]\n```\n\nA subclass of `pricehist.exceptions.SourceError` will be raised for any error.\n\n### Contribute\n\nContributions are welcome! If you discover a bug or want to work on a\nnon-trivial change, please open a\n[GitLab issue](https://gitlab.com/chrisberkhout/pricehist/-/issues)\nto discuss it.\n\nRun `make install-pre-commit-hook` set up local pre-commit checks.\nSet up your editor to run\n[isort](https://pycqa.github.io/isort/),\n[Black](https://black.readthedocs.io/en/stable/) and\n[Flake8](https://flake8.pycqa.org/en/latest/),\nor run them manually via `make format lint`.\n\n## Terminology\n\nA **source** is an upstream service that can provide a series of prices.\n\nEach **series** of prices is for one pair and price type.\n\nThe [**pair**](https://en.wikipedia.org/wiki/Currency_pair) is made up of a\nbase and a quote, each given as a symbol. Sometimes you will give the base\nonly, and the quote will be determined with information from the source. The\navailable pairs, the symbols used in them and the available price types all\ndepend on the particular source used.\n\nThe **base** is the currency or commodity being valued. Each price expresses\nthe value of one unit of the base.\n\nThe **quote** is the unit used to express the value of the base.\n\nA **symbol** is a code or abbreviation for a currency or commodity.\n\nThe **prices** in a series each have a date and an amount.\n\nThe **amount** is the number of units of the quote that are equal to one unit\nof the base.\n\nConsider the following command.\n\n```\npricehist fetch coindesk BTC/USD --type close\n```\n\n- **`coindesk`** is the ID of the CoinDesk Bitcoin Price Index source.\n- **`BTC`** is the symbol for Bitcoin, used here as the base.\n- **`USD`** is the symbol for the United States Dollar, used here as the quote.\n- **`BTC/USD`** is the pair Bitcoin against United States Dollar.\n- **`close`** is the price type for the last price of each day.\n\nA BTC/USD price of the amount 29,391.775 can be written as\n"BTC/USD = 29391.775" or "BTC 29391.775 USD", and means that one Bitcoin is\nworth 29,391.775 United States Dollars.\n\n## Initial design choices\n\nTo keep things simple, `pricehist` provides only univariate time series of\ndaily historical prices. It doesn\'t provide other types of market, financial or\neconomic data, real-time prices, or other temporal resolutions. Multiple or\nmultivariate series require multiple invocations.\n\n## Potential features\n\nIn the future, `pricehist` may be extended to cover some of the following\nfeatures:\n\n- **Time of day**: Sources sometimes provide specific times for each day\'s\n  high/low prices and these could be preserved for output. This would require\n  changes to how dates are handled internally, clarification of time zone\n  handling and extension of the time formatting option.\n- **Alternate resolutions**: Some sources can provide higher or lower\n  resolution data, such as hourly or weekly. These could be supported where\n  available. For other cases an option could be provided for downsampling data\n  before output.\n- **Real-time prices**: These generally come from different source endpoints\n  than the historical data. Real-time prices will usually have a different\n  price type, such as `last`, `bid` or `ask`. Support for real-time prices\n  would allow adding sources that don\'t provide historical data. Start and end\n  times are irrelevant when requesting real-time prices. A "follow" option\n  could continuously poll for new prices.\n- **Related non-price data**: Trading volume, spreads, split and dividend\n  events and other related data could be supported. The base/quote/type model\n  used for prices would work for some of this. Other things may require\n  extending the model.\n- **Multivariate series**: Would allow, for example, fetching\n  high/low/open/close prices in a single invocation.\n- **`format` command**: A command for rewriting existing CSV data into one of\n  the other output formats.\n\n## Alternatives\n\nBeancount\'s [`bean-price`](https://github.com/beancount/beanprice) tool fetches\nprices and addresses other workflow concerns in a Beancount-specific manner,\ngenerally requiring a Beancount file as input.\n\nThe [Piecash](https://piecash.readthedocs.io/) library is a pythonic interface\nto GnuCash files stored in SQL which has a\n[`Commodity.update_prices`](https://piecash.readthedocs.io/en/master/api/piecash.core.commodity.html?highlight=update_prices#piecash.core.commodity.Commodity.update_prices)\nmethod for fetching historical prices.\nThe GnuCash wiki documents [wrapper scripts](https://wiki.gnucash.org/wiki/Stocks/get_prices)\nfor the [Finance::QuoteHist](https://metacpan.org/pod/Finance::QuoteHist) Perl\nmodule.\n',
-    'author': 'Chris Berkhout',
-    'author_email': 'chris@chrisberkhout.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/chrisberkhout/pricehist',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+A command-line tool for fetching and formatting historical price data, with
+support for multiple data sources and output formats.
+
+[![Pipeline status](https://gitlab.com/chrisberkhout/pricehist/badges/master/pipeline.svg)](https://gitlab.com/chrisberkhout/pricehist/-/commits/master)
+[![Coverage report](https://gitlab.com/chrisberkhout/pricehist/badges/master/coverage.svg)](https://gitlab.com/chrisberkhout/pricehist/-/commits/master)
+[![PyPI version](https://badge.fury.io/py/pricehist.svg)](https://badge.fury.io/py/pricehist)
+[![Downloads](https://pepy.tech/badge/pricehist)](https://pepy.tech/project/pricehist)
+[![License](https://img.shields.io/pypi/l/pricehist)](https://gitlab.com/chrisberkhout/pricehist/-/blob/master/LICENSE)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgitlab.com%2Fchrisberkhout%2Fpricehist&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+
+## Installation
+
+Install via pip or
+[pipx](https://pypa.github.io/pipx/).
+
+```
+pipx install pricehist
+```
+
+## Sources
+
+- **`alphavantage`**: [Alpha Vantage](https://www.alphavantage.co/)
+- **`bankofcanada`**: [Bank of Canada daily exchange rates](https://www.bankofcanada.ca/valet/docs)
+- **`coinbasepro`**: [Coinbase Pro](https://pro.coinbase.com/)
+- **`coindesk`**: [CoinDesk Bitcoin Price Index](https://www.coindesk.com/coindesk-api)
+- **`coinmarketcap`**: [CoinMarketCap](https://coinmarketcap.com/)
+- **`ecb`**: [European Central Bank Euro foreign exchange reference rates](https://www.ecb.europa.eu/stats/exchange/eurofxref/html/index.en.html)
+- **`yahoo`**: [Yahoo! Finance](https://finance.yahoo.com/)
+
+## Output formats
+
+- **`beancount`**: [Beancount](http://furius.ca/beancount/)
+- **`csv`**: [Comma-separated values](https://en.wikipedia.org/wiki/Comma-separated_values)
+- **`json`**: [JSON](https://en.wikipedia.org/wiki/JSON)
+- **`jsonl`**: [JSON lines](https://en.wikipedia.org/wiki/JSON_streaming)
+- **`gnucash-sql`**: [GnuCash](https://www.gnucash.org/) SQL
+- **`ledger`**: [Ledger](https://www.ledger-cli.org/) and [hledger](https://hledger.org/)
+
+## Reactions
+
+> This is my new favourite price fetcher, by far.  
+> -- _Simon Michael, creator of [hledger](https://hledger.org/) ([ref](https://groups.google.com/g/hledger/c/SCLbNiKl9D8/m/0ReYmDppAAAJ))_
+
+> This is great!  
+> -- _Martin Blais, creator of [Beancount](https://beancount.github.io/) ([ref](https://groups.google.com/g/beancount/c/cCJc9OhIlNg/m/QGRvNowcAwAJ))_
+
+## How to
+
+### Fetch prices
+
+Fetch prices by choosing a source, a pair and, optionally, a time interval.
+
+```
+pricehist fetch ecb EUR/AUD -s 2021-01-04 -e 2021-01-08
+```
+```
+date,base,quote,amount,source,type
+2021-01-04,EUR,AUD,1.5928,ecb,reference
+2021-01-05,EUR,AUD,1.5927,ecb,reference
+2021-01-06,EUR,AUD,1.5824,ecb,reference
+2021-01-07,EUR,AUD,1.5836,ecb,reference
+2021-01-08,EUR,AUD,1.5758,ecb,reference
+```
+
+The default output format is CSV, which is suitable for use in spreadsheets and
+with other tools. For example, you can generate a price chart from the command
+line as follows (or using [an alias](https://gitlab.com/-/snippets/2163031)).
+
+```
+pricehist fetch coindesk BTC/USD -s 2021-01-01 | \
+  sed 1d | \
+  cut -d, -f1,4 | \
+  gnuplot -p -e '
+    set datafile separator ",";
+    set xdata time;
+    set timefmt "%Y-%m-%d";
+    set format x "%b\n%Y";
+    plot "/dev/stdin" using 1:2 with lines title "BTC/USD"
+  '
+```
+
+![BTC/USD prices](https://gitlab.com/chrisberkhout/pricehist/-/raw/master/example-gnuplot.png)
+
+### Show usage information
+
+Add `-h` to any command to see usage information.
+
+```
+pricehist fetch -h
+```
+```
+usage: pricehist fetch SOURCE PAIR [-h] [-vvv] [-t TYPE] [-s DATE | -sx DATE] [-e DATE | -ex DATE]
+[-o beancount|csv|json|jsonl|gnucash-sql|ledger] [--invert] [--quantize INT]
+[--fmt-base SYM] [--fmt-quote SYM] [--fmt-time TIME] [--fmt-decimal CHAR] [--fmt-thousands CHAR]
+[--fmt-symbol rightspace|right|leftspace|left] [--fmt-datesep CHAR]
+[--fmt-csvdelim CHAR] [--fmt-jsonnums]
+
+positional arguments:
+  SOURCE                   the source identifier
+  PAIR                     pair, usually BASE/QUOTE, e.g. BTC/USD
+
+optional arguments:
+  -h, --help               show this help message and exit
+  -vvv, --verbose          show all log messages
+  -t TYPE, --type TYPE     price type, e.g. close
+  -s DATE, --start DATE    start date, inclusive (default: source start)
+  -sx DATE, --startx DATE  start date, exclusive
+  -e DATE, --end DATE      end date, inclusive (default: today)
+  -ex DATE, --endx DATE    end date, exclusive
+  -o FMT, --output FMT     output format (default: csv)
+  --invert                 invert the price, swapping base and quote
+  --quantize INT           round to the given number of decimal places
+  --fmt-base SYM           rename the base symbol in output
+  --fmt-quote SYM          rename the quote symbol in output
+  --fmt-time TIME          set a particular time of day in output (default: 00:00:00)
+  --fmt-decimal CHAR       decimal point in output (default: '.')
+  --fmt-thousands CHAR     thousands separator in output (default: '')
+  --fmt-symbol LOCATION    commodity symbol placement in output (default: rightspace)
+  --fmt-datesep CHAR       date separator in output (default: '-')
+  --fmt-csvdelim CHAR      field delimiter for CSV output (default: ',')
+  --fmt-jsonnums           numbers not strings for JSON output (default: False)
+```
+
+### Choose and customize the output format
+
+As the output format you can choose one of `beancount`, `csv`, `json`, `jsonl`,
+`ledger` or `gnucash-sql`.
+
+```
+pricehist fetch ecb EUR/AUD -s 2021-01-04 -e 2021-01-08 -o ledger
+```
+```
+P 2021-01-04 00:00:00 EUR 1.5928 AUD
+P 2021-01-05 00:00:00 EUR 1.5927 AUD
+P 2021-01-06 00:00:00 EUR 1.5824 AUD
+P 2021-01-07 00:00:00 EUR 1.5836 AUD
+P 2021-01-08 00:00:00 EUR 1.5758 AUD
+```
+
+Formatting options let you control certain details of the output.
+
+```
+pricehist fetch ecb EUR/AUD -s 2021-01-04 -e 2021-01-08 -o ledger \
+  --fmt-time '' --fmt-datesep / --fmt-base € --fmt-quote $ --fmt-symbol left
+```
+```
+P 2021/01/04 € $1.5928
+P 2021/01/05 € $1.5927
+P 2021/01/06 € $1.5824
+P 2021/01/07 € $1.5836
+P 2021/01/08 € $1.5758
+```
+
+### Fetch new prices only
+
+You can update an existing file without refetching the prices you already have.
+First find the date of the last price, then fetch from there, drop the header
+line if present and append the rest to the existing file.
+
+```
+last=$(tail -1 prices-eur-usd.csv | cut -d, -f1)
+pricehist fetch ecb EUR/USD -sx $last -o csv | sed 1d >> prices-eur-usd.csv
+```
+
+### Load prices into GnuCash
+
+You can generate SQL for a GnuCash database and apply it immediately with one
+of the following commands.
+
+```
+pricehist fetch ecb EUR/AUD -s 2021-01-01 -o gnucash-sql | sqlite3 Accounts.gnucash
+pricehist fetch ecb EUR/AUD -s 2021-01-01 -o gnucash-sql | mysql -u username -p -D databasename
+pricehist fetch ecb EUR/AUD -s 2021-01-01 -o gnucash-sql | psql -U username -d databasename -v ON_ERROR_STOP=1
+```
+
+Beware that the GnuCash project itself does not support integration at the
+database level, so there is a risk that the SQL generated by `pricehist` will
+be ineffective or even damaging for some version of GnuCash. In practice, this
+strategy has been used successfully by other projects. Reading the SQL and
+keeping regular database backups is recommended.
+
+The GnuCash database must already contain commodities with mnemonics matching
+the base and quote of new prices, otherwise the SQL will fail without making
+changes.
+
+Each price entry is given a GUID based on its content (date, base, quote,
+source, type and amount) and existing GUIDs are skipped in the final insert, so
+you can apply identical or overlapping SQL files multiple times without
+creating duplicate entries in the database.
+
+### Show source information
+
+The `source` command shows information about a source.
+
+```
+pricehist source alphavantage
+```
+```
+ID          : alphavantage
+Name        : Alpha Vantage
+Description : Provider of market data for stocks, forex and cryptocurrencies
+URL         : https://www.alphavantage.co/
+Start       : 1995-01-01
+Types       : close, open, high, low, adjclose, mid
+Notes       : Alpha Vantage has data on...
+```
+
+Available symbols can be listed for most sources, either as full pairs or as
+separate base and quote symbols that will work in certain combinations.
+
+```
+pricehist source ecb --symbols
+```
+```
+EUR/AUD    Euro against Australian Dollar
+EUR/BGN    Euro against Bulgarian Lev
+EUR/BRL    Euro against Brazilian Real
+EUR/CAD    Euro against Canadian Dollar
+EUR/CHF    Euro against Swiss Franc
+...
+```
+
+It may also be possible to search for symbols.
+
+```
+pricehist source alphavantage --search Tesla
+```
+```
+TL0.DEX       Tesla, Equity, XETRA, EUR
+TL0.FRK       Tesla, Equity, Frankfurt, EUR
+TSLA34.SAO    Tesla, Equity, Brazil/Sao Paolo, BRL
+TSLA          Tesla Inc, Equity, United States, USD
+TXLZF         Tesla Exploration Ltd, Equity, United States, USD
+```
+
+### Inspect source interactions
+
+You can see extra information by adding the verbose option (`--verbose` or
+`-vvv`), including `curl` commands that reproduce each request to a source.
+
+```
+pricehist fetch coindesk BTC/USD -s 2021-01-01 -e 2021-01-05 -vvv
+```
+```
+DEBUG Began pricehist run at 2021-08-12 14:38:26.630357.
+DEBUG Starting new HTTPS connection (1): api.coindesk.com:443
+DEBUG https://api.coindesk.com:443 "GET /v1/bpi/historical/close.json?currency=USD&start=2021-01-01&end=2021-01-05 HTTP/1.1" 200 319
+DEBUG curl -X GET -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'User-Agent: python-requests/2.25.1' --compressed 'https://api.coindesk.com/v1/bpi/historical/close.json?currency=USD&start=2021-01-01&end=2021-01-05'
+DEBUG Available data covers the interval [2021-01-01--2021-01-05], as requested.
+date,base,quote,amount,source,type
+2021-01-01,BTC,USD,29391.775,coindesk,close
+2021-01-02,BTC,USD,32198.48,coindesk,close
+2021-01-03,BTC,USD,33033.62,coindesk,close
+2021-01-04,BTC,USD,32017.565,coindesk,close
+2021-01-05,BTC,USD,34035.0067,coindesk,close
+DEBUG Ended pricehist run at 2021-08-12 14:38:26.709428.
+```
+
+Running a logged `curl` command shows exactly what data is returned by the
+source.
+
+```
+pricehist fetch coindesk BTC/USD -s 2021-01-01 -e 2021-01-05 -vvv 2>&1 \
+  | grep '^DEBUG curl' | sed 's/^DEBUG //' | bash | jq .
+```
+```json
+{
+  "bpi": {
+    "2021-01-01": 29391.775,
+    "2021-01-02": 32198.48,
+    "2021-01-03": 33033.62,
+    "2021-01-04": 32017.565,
+    "2021-01-05": 34035.0067
+  },
+  "disclaimer": "This data was produced from the CoinDesk Bitcoin Price Index. BPI value data returned as USD.",
+  "time": {
+    "updated": "Jan 6, 2021 00:03:00 UTC",
+    "updatedISO": "2021-01-06T00:03:00+00:00"
+  }
 }
+```
+
+### Use via `bean-price`
+
+Beancount users may wish to use `pricehist` sources via `bean-price`. To do so,
+ensure the `pricehist` package is installed in an accessible location.
+
+You can fetch the latest price directly from the command line.
+
+```
+bean-price -e "USD:pricehist.beanprice.coindesk/BTC:USD"
+```
+```
+2021-08-18 price BTC:USD                          44725.12 USD
+```
+
+You can fetch a series of prices by providing a Beancount file as input.
+
+```
+; input.beancount
+2021-08-14 commodity BTC
+  price: "USD:pricehist.beanprice.coindesk/BTC:USD:close"
+```
+
+```
+bean-price input.beancount --update --update-rate daily --inactive --clear-cache
+```
+```
+2021-08-14 price BTC                            47098.2633 USD
+2021-08-15 price BTC                            47018.9017 USD
+2021-08-16 price BTC                             45927.405 USD
+2021-08-17 price BTC                            44686.3333 USD
+2021-08-18 price BTC                              44725.12 USD
+```
+
+Adding `-v` will print progress information, `-vv` will print debug information,
+including that from `pricehist`.
+
+A source map specification for `bean-price` has the form
+`<currency>:<module>/[^]<ticker>`. Additional `<module>/[^]<ticker>` parts can
+be appended, separated by commas.
+
+The module name will be of the form `pricehist.beanprice.<source_id>`.
+
+The ticker symbol will be of the form `BASE:QUOTE:TYPE`.
+
+Any non-alphanumeric characters except the equals sign (`=`), hyphen (`-`),
+period (`.`), or parentheses (`(` or `)`) are special characters that need to
+be encoded as their a two-digit hexadecimal code prefixed with an underscore,
+because `bean-price` ticker symbols don't allow all the characters used by
+`pricehist` pairs.
+[This page](https://replit.com/@chrisberkhout/bpticker) will do it for you.
+
+For example, the Yahoo! Finance symbol for the Dow Jones Industrial Average is
+`^DJI`, and would have the source map specification
+`USD:pricehist.beanprice.yahoo/_5eDJI`, or for the daily high price
+`USD:pricehist.beanprice.yahoo/_5eDJI::high`.
+
+### Use as a library
+
+You may find `pricehist`'s source classes useful in your own scripts.
+
+```
+$ python
+Python 3.9.6 (default, Jun 30 2021, 10:22:16)
+[GCC 11.1.0] on linux
+Type "help", "copyright", "credits" or "license" for more information.
+>>> from pricehist.series import Series
+>>> from pricehist.sources.ecb import ECB
+>>> series = ECB().fetch(Series("EUR", "AUD", "reference", "2021-01-04", "2021-01-08"))
+>>> series.prices
+[Price(date='2021-01-04', amount=Decimal('1.5928')), Price(date='2021-01-05', amount=Decimal('1.5927')), Price(date='2021-01-06', amount=Decimal('1.5824')), Price(date='2021-01-07', amount=Decimal('1.5836')), Price(date='2021-01-08', amount=Decimal('1.5758'))]
+```
+
+A subclass of `pricehist.exceptions.SourceError` will be raised for any error.
+
+### Contribute
+
+Contributions are welcome! If you discover a bug or want to work on a
+non-trivial change, please open a
+[GitLab issue](https://gitlab.com/chrisberkhout/pricehist/-/issues)
+to discuss it.
+
+Run `make install-pre-commit-hook` set up local pre-commit checks.
+Set up your editor to run
+[isort](https://pycqa.github.io/isort/),
+[Black](https://black.readthedocs.io/en/stable/) and
+[Flake8](https://flake8.pycqa.org/en/latest/),
+or run them manually via `make format lint`.
+
+## Terminology
+
+A **source** is an upstream service that can provide a series of prices.
+
+Each **series** of prices is for one pair and price type.
+
+The [**pair**](https://en.wikipedia.org/wiki/Currency_pair) is made up of a
+base and a quote, each given as a symbol. Sometimes you will give the base
+only, and the quote will be determined with information from the source. The
+available pairs, the symbols used in them and the available price types all
+depend on the particular source used.
+
+The **base** is the currency or commodity being valued. Each price expresses
+the value of one unit of the base.
+
+The **quote** is the unit used to express the value of the base.
+
+A **symbol** is a code or abbreviation for a currency or commodity.
+
+The **prices** in a series each have a date and an amount.
+
+The **amount** is the number of units of the quote that are equal to one unit
+of the base.
+
+Consider the following command.
+
+```
+pricehist fetch coindesk BTC/USD --type close
+```
+
+- **`coindesk`** is the ID of the CoinDesk Bitcoin Price Index source.
+- **`BTC`** is the symbol for Bitcoin, used here as the base.
+- **`USD`** is the symbol for the United States Dollar, used here as the quote.
+- **`BTC/USD`** is the pair Bitcoin against United States Dollar.
+- **`close`** is the price type for the last price of each day.
+
+A BTC/USD price of the amount 29,391.775 can be written as
+"BTC/USD = 29391.775" or "BTC 29391.775 USD", and means that one Bitcoin is
+worth 29,391.775 United States Dollars.
+
+## Initial design choices
+
+To keep things simple, `pricehist` provides only univariate time series of
+daily historical prices. It doesn't provide other types of market, financial or
+economic data, real-time prices, or other temporal resolutions. Multiple or
+multivariate series require multiple invocations.
+
+## Potential features
+
+In the future, `pricehist` may be extended to cover some of the following
+features:
+
+- **Time of day**: Sources sometimes provide specific times for each day's
+  high/low prices and these could be preserved for output. This would require
+  changes to how dates are handled internally, clarification of time zone
+  handling and extension of the time formatting option.
+- **Alternate resolutions**: Some sources can provide higher or lower
+  resolution data, such as hourly or weekly. These could be supported where
+  available. For other cases an option could be provided for downsampling data
+  before output.
+- **Real-time prices**: These generally come from different source endpoints
+  than the historical data. Real-time prices will usually have a different
+  price type, such as `last`, `bid` or `ask`. Support for real-time prices
+  would allow adding sources that don't provide historical data. Start and end
+  times are irrelevant when requesting real-time prices. A "follow" option
+  could continuously poll for new prices.
+- **Related non-price data**: Trading volume, spreads, split and dividend
+  events and other related data could be supported. The base/quote/type model
+  used for prices would work for some of this. Other things may require
+  extending the model.
+- **Multivariate series**: Would allow, for example, fetching
+  high/low/open/close prices in a single invocation.
+- **`format` command**: A command for rewriting existing CSV data into one of
+  the other output formats.
+
+## Alternatives
+
+Beancount's [`bean-price`](https://github.com/beancount/beanprice) tool fetches
+prices and addresses other workflow concerns in a Beancount-specific manner,
+generally requiring a Beancount file as input.
 
+The [Piecash](https://piecash.readthedocs.io/) library is a pythonic interface
+to GnuCash files stored in SQL which has a
+[`Commodity.update_prices`](https://piecash.readthedocs.io/en/master/api/piecash.core.commodity.html?highlight=update_prices#piecash.core.commodity.Commodity.update_prices)
+method for fetching historical prices.
+The GnuCash wiki documents [wrapper scripts](https://wiki.gnucash.org/wiki/Stocks/get_prices)
+for the [Finance::QuoteHist](https://metacpan.org/pod/Finance::QuoteHist) Perl
+module.
 
-setup(**setup_kwargs)
```


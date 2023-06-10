# Comparing `tmp/gitfarts-0.1.1.tar.gz` & `tmp/gitfarts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitfarts-0.1.1.tar", max compression
+gzip compressed data, was "gitfarts-0.1.2.tar", max compression
```

## Comparing `gitfarts-0.1.1.tar` & `gitfarts-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-10 12:31:52.561550 gitfarts-0.1.1/gitfarts/__init__.py
--rw-r--r--   0        0        0     4593 2023-06-10 12:35:12.503966 gitfarts-0.1.1/gitfarts/main.py
--rw-r--r--   0        0        0      316 2023-06-10 12:35:47.130673 gitfarts-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 gitfarts-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-10 12:31:52.561550 gitfarts-0.1.2/gitfarts/__init__.py
+-rw-r--r--   0        0        0     4775 2023-06-10 12:38:38.993088 gitfarts-0.1.2/gitfarts/main.py
+-rw-r--r--   0        0        0      334 2023-06-10 12:39:03.724361 gitfarts-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 gitfarts-0.1.2/PKG-INFO
```

### Comparing `gitfarts-0.1.1/gitfarts/main.py` & `gitfarts-0.1.2/gitfarts/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,24 +13,31 @@
 """
 
 import sys
 import argparse
 import datetime
 from subprocess import check_output
 from collections import OrderedDict
+import pandas
 
 import pkg_resources
 __version__ = pkg_resources.require("git-bars")[0].version
 
 def print_bars(items, block=u"\u2580", width=50):
     """Print unicode bar representations of dates and scores."""
-    for i in items:
+    # Get the maximum score.
+
+    df = pandas.DataFrame(columns=["Date", "Commits"])
+
+    for index, i in enumerate(items):
         num = str(items[i]["commits"])
+        df.loc[index] = [i, num]
 
-        print(f"{i}, {num}")
+    df = df.set_index("Date")
+    df.to_csv("gitfarts.csv")
         
 
 
 
 def filter(items, periodicity="day", author=""):
     """Filter entries by periodicity and author."""
     bars = OrderedDict()
```


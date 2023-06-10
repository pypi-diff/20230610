# Comparing `tmp/iggcli-0.1.0.tar.gz` & `tmp/iggcli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iggcli-0.1.0.tar", max compression
+gzip compressed data, was "iggcli-0.1.1.tar", max compression
```

## Comparing `iggcli-0.1.0.tar` & `iggcli-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0       25 2023-03-21 02:39:12.934353 iggcli-0.1.0/README.md
--rw-r--r--   0        0        0      200 2023-03-21 02:55:17.687500 iggcli-0.1.0/iggcli/__init__.py
--rw-r--r--   0        0        0       37 2023-03-21 02:37:43.633133 iggcli-0.1.0/iggcli/__main__.py
--rw-r--r--   0        0        0       96 2023-03-21 03:22:12.773529 iggcli-0.1.0/iggcli/calls/__init__.py
--rw-r--r--   0        0        0      225 2023-03-21 03:40:04.312108 iggcli-0.1.0/iggcli/calls/credits.py
--rw-r--r--   0        0        0     1073 2023-03-21 04:02:55.494727 iggcli-0.1.0/iggcli/calls/search.py
--rw-r--r--   0        0        0      276 2023-03-21 03:24:33.695452 iggcli-0.1.0/iggcli/cli.py
--rw-r--r--   0        0        0        0 2023-03-21 03:05:35.291921 iggcli-0.1.0/iggcli/core/__init__.py
--rw-r--r--   0        0        0      470 2023-03-21 03:41:51.109555 iggcli-0.1.0/iggcli/core/scrap.py
--rw-r--r--   0        0        0       99 2023-03-21 02:37:43.621133 iggcli-0.1.0/iggcli/main.py
--rw-r--r--   0        0        0       45 2023-03-21 03:03:36.710304 iggcli-0.1.0/iggcli/values/__init__.py
--rw-r--r--   0        0        0      223 2023-03-21 03:56:49.773755 iggcli-0.1.0/iggcli/values/search.py
--rw-r--r--   0        0        0       40 2023-03-21 03:08:06.249980 iggcli-0.1.0/iggcli/values/web.py
--rw-r--r--   0        0        0     1078 2023-03-21 04:24:12.332143 iggcli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 iggcli-0.1.0/setup.py
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 iggcli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-06-10 18:43:04.756648 iggcli-0.1.1/README.md
+-rw-r--r--   0        0        0      213 2023-06-10 18:44:33.827502 iggcli-0.1.1/iggcli/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-10 18:43:04.756648 iggcli-0.1.1/iggcli/__main__.py
+-rw-r--r--   0        0        0       96 2023-06-10 18:43:04.756648 iggcli-0.1.1/iggcli/calls/__init__.py
+-rw-r--r--   0        0        0      225 2023-06-10 18:44:21.180664 iggcli-0.1.1/iggcli/calls/credits.py
+-rw-r--r--   0        0        0     1088 2023-06-10 18:46:01.262377 iggcli-0.1.1/iggcli/calls/search.py
+-rw-r--r--   0        0        0      293 2023-06-10 18:46:04.100340 iggcli-0.1.1/iggcli/cli.py
+-rw-r--r--   0        0        0        0 2023-06-10 18:43:04.756648 iggcli-0.1.1/iggcli/core/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-10 18:46:01.264377 iggcli-0.1.1/iggcli/core/scrap.py
+-rw-r--r--   0        0        0       99 2023-06-10 18:43:04.756648 iggcli-0.1.1/iggcli/main.py
+-rw-r--r--   0        0        0       45 2023-06-10 18:43:04.756648 iggcli-0.1.1/iggcli/values/__init__.py
+-rw-r--r--   0        0        0      225 2023-06-10 18:46:01.076379 iggcli-0.1.1/iggcli/values/search.py
+-rw-r--r--   0        0        0       41 2023-06-10 18:46:01.072379 iggcli-0.1.1/iggcli/values/web.py
+-rw-r--r--   0        0        0     1078 2023-06-10 18:46:47.569781 iggcli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 iggcli-0.1.1/PKG-INFO
```

### Comparing `iggcli-0.1.0/iggcli/calls/search.py` & `iggcli-0.1.1/iggcli/calls/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+from datetime import datetime as dt
+
+from bs4 import BeautifulSoup, Tag
 from rich import print
 from rich.table import Table
 
-from bs4 import Tag, BeautifulSoup
-from datetime import datetime as dt
-
 from iggcli.core import scrap
 from iggcli.values import search as E
 
+
 def call(query: str, page: int) -> None:
     parse: BeautifulSoup = scrap.parse(["page", str(page)], {"s": query})
 
     table: Table = Table(title=f"Results for '{query}'", border_style="black")
 
     table.add_column("Title", style="green")
     table.add_column("Posted by")
     table.add_column("Genres")
     table.add_column("Release")
 
     for el in parse.select(E["elems"]):
-        title: str = el.select_one(E["title"]).text # type: ignore
+        title: str = el.select_one(E["title"]).text  # type: ignore
         meta: list[Tag] = el.select(E["meta"])
 
         posted_by: str = meta[0].text
         genres: list[str] = [x.text for x in meta[1:]]
-        date: str | dt = el.select_one(E["date"])["datetime"] # type: ignore
+        date: str | dt = el.select_one(E["date"])["datetime"]  # type: ignore
 
         title = title.split("Free")[0]
-        date = dt.fromisoformat(date) # type: ignore
-        
-        table.add_row(title, posted_by, ", ".join(genres) + ".", date.strftime("%d/%m/%Y"))
-    
-    print(table)
+        date = dt.fromisoformat(date)  # type: ignore
+
+        table.add_row(
+            title, posted_by, ", ".join(genres) + ".", date.strftime("%d/%m/%Y")
+        )
+
+    print(table)
```

### Comparing `iggcli-0.1.0/pyproject.toml` & `iggcli-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iggcli"
-version = "0.1.0"
+version = "0.1.1"
 description = "Download your games from Igg Games more easily."
 authors = ["Alekyo4 <alexsandergomes4742@gmail.com>"]
 license = "BeerWare"
 readme = "README.md"
 
 classifiers = [
     "Natural Language :: Portuguese (Brazilian)",
```

### Comparing `iggcli-0.1.0/PKG-INFO` & `iggcli-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: iggcli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Download your games from Igg Games more easily.
 License: Beerware
 Author: Alekyo4
 Author-email: alexsandergomes4742@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Customer Service
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Requires-Dist: beautifulsoup4 (>=4.12.0,<5.0.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: bug, https://github.com/alekyo4/iggcli/issues
```


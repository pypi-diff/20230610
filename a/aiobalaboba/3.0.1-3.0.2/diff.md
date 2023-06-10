# Comparing `tmp/aiobalaboba-3.0.1.tar.gz` & `tmp/aiobalaboba-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobalaboba-3.0.1.tar", max compression
+gzip compressed data, was "aiobalaboba-3.0.2.tar", max compression
```

## Comparing `aiobalaboba-3.0.1.tar` & `aiobalaboba-3.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/LICENSE
--rw-r--r--   0        0        0     1158 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/README.md
--rw-r--r--   0        0        0      141 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/__init__.py
--rw-r--r--   0        0        0     3022 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/_balaboba.py
--rw-r--r--   0        0        0     1582 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/_http.py
--rw-r--r--   0        0        0      147 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/_text_type.py
--rw-r--r--   0        0        0        0 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/aiobalaboba/py.typed
--rw-r--r--   0        0        0     2883 2023-05-31 10:59:29.088018 aiobalaboba-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 aiobalaboba-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/LICENSE
+-rw-r--r--   0        0        0     1158 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/README.md
+-rw-r--r--   0        0        0      141 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/__init__.py
+-rw-r--r--   0        0        0     3022 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/_balaboba.py
+-rw-r--r--   0        0        0     1582 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/_http.py
+-rw-r--r--   0        0        0      147 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/_text_type.py
+-rw-r--r--   0        0        0        0 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/aiobalaboba/py.typed
+-rw-r--r--   0        0        0     2883 2023-06-10 08:45:44.630547 aiobalaboba-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 aiobalaboba-3.0.2/PKG-INFO
```

### Comparing `aiobalaboba-3.0.1/LICENSE` & `aiobalaboba-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobalaboba-3.0.1/README.md` & `aiobalaboba-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aiobalaboba-3.0.1/aiobalaboba/_balaboba.py` & `aiobalaboba-3.0.2/aiobalaboba/_balaboba.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,28 +50,28 @@
             headers=self._get_balaboba_headers(query, intro),
         )
         return "{}{}".format(response["query"], response["text"])
 
     def _get_text_types_headers(self) -> Dict[str, str]:
         return {
             "User-Agent": (
-                "Mozilla/5.0 (Windows NT 10.0; rv:113.0) Gecko/20100101 Firefox/113.0"
+                "Mozilla/5.0 (Windows NT 10.0; rv:114.0) Gecko/20100101 Firefox/114.0"
             ),
             "Accept-Language": "en-US,en;q=0.5",
             "Referer": "https://yandex.ru/lab/yalm",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "TE": "trailers",
         }
 
     def _get_balaboba_headers(self, query: str, text_type: int) -> Dict[str, str]:
         return {
             "User-Agent": (
-                "Mozilla/5.0 (Windows NT 10.0; rv:113.0) Gecko/20100101 Firefox/113.0"
+                "Mozilla/5.0 (Windows NT 10.0; rv:114.0) Gecko/20100101 Firefox/114.0"
             ),
             "Accept-Language": "en-US,en;q=0.5",
             "Referer": f"https://yandex.ru/lab/yalm?style={text_type}",
             "X-Requested-With": "XMLHttpRequest",
             "X-Retpath-Y": (
                 "https://yandex.ru/lab/yalm?style={}&input={}&skipCurtain=1".format(
                     text_type, urllib.parse.quote_plus(query)
```

### Comparing `aiobalaboba-3.0.1/aiobalaboba/_http.py` & `aiobalaboba-3.0.2/aiobalaboba/_http.py`

 * *Files identical despite different names*

### Comparing `aiobalaboba-3.0.1/pyproject.toml` & `aiobalaboba-3.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiobalaboba"
-version = "3.0.1"
+version = "3.0.2"
 description = "Asynchronous wrapper for Yandex Balaboba"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/aiobalaboba"
 keywords = ["yalm"]
 classifiers = [
@@ -34,15 +34,15 @@
 black = "23.3.0"
 covdefaults = "2.3.0"
 mypy = "1.3.0"
 pre-commit = "2.21.0"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 coverage = { version = "7.2.7", extras = ["toml"] }
-ruff = "0.0.270"
+ruff = "0.0.272"
 
 [tool.black]
 target-version = ["py37"]
 skip-magic-trailing-comma = true
 preview = true
 
 [tool.coverage.report]
```

### Comparing `aiobalaboba-3.0.1/PKG-INFO` & `aiobalaboba-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobalaboba
-Version: 3.0.1
+Version: 3.0.2
 Summary: Asynchronous wrapper for Yandex Balaboba
 Home-page: https://github.com/monosans/aiobalaboba
 License: MIT
 Keywords: yalm
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
```


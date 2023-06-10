# Comparing `tmp/balaboba-3.0.1.tar.gz` & `tmp/balaboba-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balaboba-3.0.1.tar", max compression
+gzip compressed data, was "balaboba-3.0.2.tar", max compression
```

## Comparing `balaboba-3.0.1.tar` & `balaboba-3.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-31 10:59:20.692139 balaboba-3.0.1/LICENSE
--rw-r--r--   0        0        0     1041 2023-05-31 10:59:20.692139 balaboba-3.0.1/README.md
--rw-r--r--   0        0        0      128 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/__init__.py
--rw-r--r--   0        0        0     2935 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/_balaboba.py
--rw-r--r--   0        0        0     1442 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/_http.py
--rw-r--r--   0        0        0      147 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/_text_type.py
--rw-r--r--   0        0        0        0 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/py.typed
--rw-r--r--   0        0        0     2818 2023-05-31 10:59:20.696138 balaboba-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 balaboba-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-10 08:45:42.647279 balaboba-3.0.2/LICENSE
+-rw-r--r--   0        0        0     1041 2023-06-10 08:45:42.647279 balaboba-3.0.2/README.md
+-rw-r--r--   0        0        0      128 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/__init__.py
+-rw-r--r--   0        0        0     2935 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/_balaboba.py
+-rw-r--r--   0        0        0     1442 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/_http.py
+-rw-r--r--   0        0        0      147 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/_text_type.py
+-rw-r--r--   0        0        0        0 2023-06-10 08:45:42.647279 balaboba-3.0.2/balaboba/py.typed
+-rw-r--r--   0        0        0     2818 2023-06-10 08:45:42.651279 balaboba-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 balaboba-3.0.2/PKG-INFO
```

### Comparing `balaboba-3.0.1/LICENSE` & `balaboba-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `balaboba-3.0.1/README.md` & `balaboba-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `balaboba-3.0.1/balaboba/_balaboba.py` & `balaboba-3.0.2/balaboba/_balaboba.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,28 @@
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

### Comparing `balaboba-3.0.1/balaboba/_http.py` & `balaboba-3.0.2/balaboba/_http.py`

 * *Files identical despite different names*

### Comparing `balaboba-3.0.1/pyproject.toml` & `balaboba-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balaboba"
-version = "3.0.1"
+version = "3.0.2"
 description = "Wrapper for Yandex Balaboba"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/balaboba"
 keywords = ["yalm"]
 classifiers = [
@@ -32,15 +32,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 covdefaults = "2.3.0"
 mypy = "1.3.0"
 pre-commit = "2.21.0"
 pytest = "7.3.1"
 coverage = { version = "7.2.7", extras = ["toml"] }
-ruff = "0.0.270"
+ruff = "0.0.272"
 types-requests = "2.31.0.1"
 
 [tool.black]
 target-version = ["py37"]
 skip-magic-trailing-comma = true
 preview = true
```

### Comparing `balaboba-3.0.1/PKG-INFO` & `balaboba-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balaboba
-Version: 3.0.1
+Version: 3.0.2
 Summary: Wrapper for Yandex Balaboba
 Home-page: https://github.com/monosans/balaboba
 License: MIT
 Keywords: yalm
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
```


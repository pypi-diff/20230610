# Comparing `tmp/nutorious-0.1.2.tar.gz` & `tmp/nutorious-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutorious-0.1.2.tar", max compression
+gzip compressed data, was "nutorious-0.1.3.tar", max compression
```

## Comparing `nutorious-0.1.2.tar` & `nutorious-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      707 2023-06-10 17:01:08.764467 nutorious-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1173 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/__main__.py
--rw-r--r--   0        0        0      754 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/cli/__init__.py
--rw-r--r--   0        0        0     1187 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/config/__init__.py
--rw-r--r--   0        0        0      376 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/config/default.yml
--rw-r--r--   0        0        0      204 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/context/__init__.py
--rw-r--r--   0        0        0     4436 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/journal/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/__init__.py
--rw-r--r--   0        0        0      830 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/base.py
--rw-r--r--   0        0        0     2556 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/daily.py
--rw-r--r--   0        0        0        0 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/report/diff.py
--rw-r--r--   0        0        0     1094 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/ui/__init__.py
--rw-r--r--   0        0        0      503 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/ui/ui.py
--rw-r--r--   0        0        0      337 2023-06-10 17:01:08.764467 nutorious-0.1.2/src/nutorious/utils/collections.py
--rw-r--r--   0        0        0      197 2023-06-10 17:01:08.768467 nutorious-0.1.2/src/nutorious/utils/commons.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 nutorious-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-06-10 17:47:06.826712 nutorious-0.1.3/README.md
+-rw-r--r--   0        0        0      804 2023-06-10 17:47:06.826712 nutorious-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1173 2023-06-10 17:47:06.826712 nutorious-0.1.3/src/nutorious/__init__.py
+-rw-r--r--   0        0        0      754 2023-06-10 17:47:06.826712 nutorious-0.1.3/src/nutorious/cli/__init__.py
+-rw-r--r--   0        0        0     1187 2023-06-10 17:47:06.826712 nutorious-0.1.3/src/nutorious/config/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-10 17:47:06.826712 nutorious-0.1.3/src/nutorious/config/default.yml
+-rw-r--r--   0        0        0      204 2023-06-10 17:47:06.826712 nutorious-0.1.3/src/nutorious/context/__init__.py
+-rw-r--r--   0        0        0     4436 2023-06-10 17:47:06.826712 nutorious-0.1.3/src/nutorious/journal/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/report/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/report/base.py
+-rw-r--r--   0        0        0     2556 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/report/daily.py
+-rw-r--r--   0        0        0        0 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/report/diff.py
+-rw-r--r--   0        0        0     1094 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/ui/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/ui/ui.py
+-rw-r--r--   0        0        0      337 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/utils/collections.py
+-rw-r--r--   0        0        0      197 2023-06-10 17:47:06.830712 nutorious-0.1.3/src/nutorious/utils/commons.py
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 nutorious-0.1.3/PKG-INFO
```

### Comparing `nutorious-0.1.2/pyproject.toml` & `nutorious-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "nutorious"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Dzmitry Paulenka <paulenka.dk@gmail.com>"]
-# readme = "README.md"
+readme = "README.md"
+# TODO: what does this next line actually do ?
 # packages = [{include = "nutorious"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "^13.4.1"
 pyyaml = "^6.0"
 attrs = "^23.1.0"
@@ -16,14 +17,17 @@
 pydash = "^7.0.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-watch = "^4.2.0"
 
+[tool.poetry.scripts]
+nutorious = "nutorious:main"
+
 [tool.poe.tasks]
 nutorios = 'python3 -m nutorious report'
 watch = 'python3 -m nutorious report --w'
 today = 'python3 -m nutorious report'
 todayw = 'python3 -m nutorious report --w'
 
 [build-system]
```

### Comparing `nutorious-0.1.2/src/nutorious/__main__.py` & `nutorious-0.1.3/src/nutorious/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.2/src/nutorious/cli/__init__.py` & `nutorious-0.1.3/src/nutorious/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.2/src/nutorious/config/__init__.py` & `nutorious-0.1.3/src/nutorious/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.2/src/nutorious/journal/__init__.py` & `nutorious-0.1.3/src/nutorious/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.2/src/nutorious/model/__init__.py` & `nutorious-0.1.3/src/nutorious/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.2/src/nutorious/report/base.py` & `nutorious-0.1.3/src/nutorious/report/base.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.2/src/nutorious/report/daily.py` & `nutorious-0.1.3/src/nutorious/report/daily.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.2/src/nutorious/ui/__init__.py` & `nutorious-0.1.3/src/nutorious/ui/__init__.py`

 * *Files identical despite different names*


# Comparing `tmp/lazy_calculator-0.1.4.tar.gz` & `tmp/lazy_calculator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_calculator-0.1.4.tar", max compression
+gzip compressed data, was "lazy_calculator-0.1.5.tar", max compression
```

## Comparing `lazy_calculator-0.1.4.tar` & `lazy_calculator-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-09 15:23:49.150279 lazy_calculator-0.1.4/LICENSE
--rw-r--r--   0        0        0       18 2023-06-09 15:53:10.167861 lazy_calculator-0.1.4/README.md
--rw-r--r--   0        0        0      129 2023-06-09 16:21:00.964299 lazy_calculator-0.1.4/lazy_calculator/__init__.py
--rw-r--r--   0        0        0      432 2023-06-09 16:09:35.194791 lazy_calculator-0.1.4/lazy_calculator/factorial.py
--rw-r--r--   0        0        0      607 2023-06-09 16:24:49.881564 lazy_calculator-0.1.4/lazy_calculator/fibonacci.py
--rw-r--r--   0        0        0      420 2023-06-09 16:28:50.932410 lazy_calculator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 lazy_calculator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 15:23:49.150279 lazy_calculator-0.1.5/LICENSE
+-rw-r--r--   0        0        0       18 2023-06-09 15:53:10.167861 lazy_calculator-0.1.5/README.md
+-rw-r--r--   0        0        0      129 2023-06-09 16:21:00.964299 lazy_calculator-0.1.5/lazy_calculator/__init__.py
+-rw-r--r--   0        0        0      417 2023-06-10 10:18:53.713329 lazy_calculator-0.1.5/lazy_calculator/factorial.py
+-rw-r--r--   0        0        0      607 2023-06-09 16:24:49.881564 lazy_calculator-0.1.5/lazy_calculator/fibonacci.py
+-rw-r--r--   0        0        0      420 2023-06-10 10:19:43.716756 lazy_calculator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 lazy_calculator-0.1.5/PKG-INFO
```

### Comparing `lazy_calculator-0.1.4/LICENSE` & `lazy_calculator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy_calculator-0.1.4/lazy_calculator/fibonacci.py` & `lazy_calculator-0.1.5/lazy_calculator/fibonacci.py`

 * *Files identical despite different names*


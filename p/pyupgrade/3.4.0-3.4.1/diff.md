# Comparing `tmp/pyupgrade-3.4.0.tar.gz` & `tmp/pyupgrade-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyupgrade-3.4.0.tar", last modified: Sat May  6 21:09:25 2023, max compression
+gzip compressed data, was "pyupgrade-3.4.1.tar", last modified: Sat Jun 10 20:48:20 2023, max compression
```

## Comparing `pyupgrade-3.4.0.tar` & `pyupgrade-3.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.927491 pyupgrade-3.4.0/pyupgrade/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11784 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/pyupgrade/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/collections_abc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/datetime_utc_alias.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1465 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/default_encoding.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/dict_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1769 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/format_locals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4398 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/fstrings.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1543 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/identity_equality.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    20494 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/io_open.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/legacy.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2447 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/lru_cache.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/metaclass_type.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/mock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2331 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/native_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/new_style_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4031 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/open_mode.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/oserror_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9476 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/percent_format.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/set_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_base_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6522 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_metaclasses.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_remove_decorators.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_simple.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/subprocess_run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1413 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/type_of_primitive.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8423 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4877 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep563.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep585.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5787 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep604.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep646_unpack.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_text.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/unittest_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1073 2023-05-06 20:39:40.000000 pyupgrade-3.4.0/pyupgrade/_plugins/unpack_list_comprehension.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6490 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/versioned_branches.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_string_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    14591 2023-05-06 20:39:40.000000 pyupgrade-3.4.0/pyupgrade/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.927491 pyupgrade-3.4.0/pyupgrade.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1199 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:48:20.382423 pyupgrade-3.4.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-06-10 20:48:20.382423 pyupgrade-3.4.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:48:20.374423 pyupgrade-3.4.1/pyupgrade/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11830 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:48:20.382423 pyupgrade-3.4.1/pyupgrade/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/collections_abc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/datetime_utc_alias.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1465 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/default_encoding.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/dict_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1769 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/format_locals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4398 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/fstrings.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1543 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/identity_equality.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    20494 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/io_open.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/legacy.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2447 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/lru_cache.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/metaclass_type.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/mock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2438 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade/_plugins/native_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/new_style_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4031 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/open_mode.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/oserror_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9476 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/percent_format.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/set_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/six_base_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6522 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/six_calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/six_metaclasses.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/six_remove_decorators.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/six_simple.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/subprocess_run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1413 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/type_of_primitive.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8320 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade/_plugins/typing_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4877 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep563.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep585.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5787 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep604.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep646_unpack.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/typing_text.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/unittest_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1073 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/unpack_list_comprehension.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6490 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_plugins/versioned_branches.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_string_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14591 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/pyupgrade/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:48:20.378423 pyupgrade-3.4.1/pyupgrade.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-06-10 20:48:20.000000 pyupgrade-3.4.1/pyupgrade.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1200 2023-06-10 20:48:20.382423 pyupgrade-3.4.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:34:09.000000 pyupgrade-3.4.1/setup.py
```

### Comparing `pyupgrade-3.4.0/LICENSE` & `pyupgrade-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/PKG-INFO` & `pyupgrade-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.4.0
+Version: 3.4.1
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+    rev: v3.4.1
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.4.0/README.md` & `pyupgrade-3.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+    rev: v3.4.1
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.4.0/pyupgrade/_ast_helpers.py` & `pyupgrade-3.4.1/pyupgrade/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_data.py` & `pyupgrade-3.4.1/pyupgrade/_data.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_main.py` & `pyupgrade-3.4.1/pyupgrade/_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 def _fix_format_literal(tokens: list[Token], end: int) -> None:
     parts = rfind_string_parts(tokens, end)
     parsed_parts = []
     last_int = -1
     for i in parts:
         # f'foo {0}'.format(...) would get turned into a SyntaxError
         prefix, _ = parse_string_literal(tokens[i].src)
-        if 'f' in prefix.lower():
+        if 'f' in prefix.lower():  # pragma: <3.12 cover
             return
 
         try:
             parsed = parse_format(tokens[i].src)
         except ValueError:
             # the format literal was malformed, skip it
             return
@@ -240,15 +240,15 @@
             i + 3 < len(tokens) and
             tokens[i + 1].src == '(' and
             tokens[i + 2].name == 'STRING' and
             tokens[i + 3].src == ')'
     ):
         victims = slice(i - 1, i + 4)
         prefix, rest = parse_string_literal(tokens[i + 2].src)
-        if 'f' in prefix.lower():
+        if 'f' in prefix.lower():  # pragma: <3.12 cover
             return
         encoding = ast.literal_eval(prefix + rest)
         if is_codec(encoding, 'ascii') or is_codec(encoding, 'utf-8'):
             latin1_ok = False
         elif is_codec(encoding, 'iso8859-1'):
             latin1_ok = True
         else:
```

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/collections_abc.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/collections_abc.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/datetime_utc_alias.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/datetime_utc_alias.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/default_encoding.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/default_encoding.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/dict_literals.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/dict_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/format_locals.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/format_locals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/fstrings.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/fstrings.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/identity_equality.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/identity_equality.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/imports.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/imports.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/io_open.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/io_open.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/legacy.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/legacy.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/lru_cache.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/lru_cache.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/metaclass_type.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/metaclass_type.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/mock.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/mock.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/native_literals.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/native_literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,13 +62,16 @@
     if is_a_native_literal_call(node, state.from_imports):
         func = functools.partial(_fix_literal, empty="''")
         yield ast_to_offset(node), func
     elif (
             isinstance(node.func, ast.Name) and node.func.id == 'bytes' and
             not node.keywords and not has_starargs(node) and
             (
-                len(node.args) == 0 or
-                (len(node.args) == 1 and isinstance(node.args[0], ast.Bytes))
+                len(node.args) == 0 or (
+                    len(node.args) == 1 and
+                    isinstance(node.args[0], ast.Constant) and
+                    isinstance(node.args[0].value, bytes)
+                )
             )
     ):
         func = functools.partial(_fix_literal, empty="b''")
         yield ast_to_offset(node), func
```

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/new_style_classes.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/new_style_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/open_mode.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/open_mode.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/oserror_aliases.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/oserror_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/percent_format.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/percent_format.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/set_literals.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/set_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/six_base_classes.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/six_base_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/six_calls.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/six_calls.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/six_metaclasses.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/six_metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/six_remove_decorators.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/six_remove_decorators.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/six_simple.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/six_simple.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/subprocess_run.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/type_of_primitive.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/type_of_primitive.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/typing_classes.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/typing_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,18 +216,15 @@
                 ) and
                 len(node.value.args) == 2 and
                 (
                     not node.value.keywords or
                     (
                         len(node.value.keywords) == 1 and
                         node.value.keywords[0].arg == 'total' and
-                        isinstance(
-                            node.value.keywords[0].value,
-                            (ast.Constant, ast.NameConstant),
-                        )
+                        isinstance(node.value.keywords[0].value, ast.Constant)
                     )
                 ) and
                 isinstance(node.value.args[1], ast.Dict) and
                 node.value.args[1].keys and
                 all(
                     isinstance(k, ast.Constant) and
                     isinstance(k.value, str) and
```

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep563.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep563.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep585.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep585.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep604.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep604.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep646_unpack.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/typing_pep646_unpack.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/typing_text.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/typing_text.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/unittest_aliases.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/unittest_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/unpack_list_comprehension.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/unpack_list_comprehension.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_plugins/versioned_branches.py` & `pyupgrade-3.4.1/pyupgrade/_plugins/versioned_branches.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_string_helpers.py` & `pyupgrade-3.4.1/pyupgrade/_string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade/_token_helpers.py` & `pyupgrade-3.4.1/pyupgrade/_token_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/pyupgrade.egg-info/PKG-INFO` & `pyupgrade-3.4.1/pyupgrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.4.0
+Version: 3.4.1
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+    rev: v3.4.1
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.4.0/pyupgrade.egg-info/SOURCES.txt` & `pyupgrade-3.4.1/pyupgrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.4.0/setup.cfg` & `pyupgrade-3.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = pyupgrade
-version = 3.4.0
+version = 3.4.1
 description = A tool to automatically upgrade syntax for newer versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/pyupgrade
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
```


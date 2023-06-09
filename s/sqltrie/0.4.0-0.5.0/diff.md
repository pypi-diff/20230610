# Comparing `tmp/sqltrie-0.4.0.tar.gz` & `tmp/sqltrie-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqltrie-0.4.0.tar", last modified: Tue Jun  6 11:53:39 2023, max compression
+gzip compressed data, was "sqltrie-0.5.0.tar", last modified: Fri Jun  9 23:45:30 2023, max compression
```

## Comparing `sqltrie-0.4.0.tar` & `sqltrie-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-06 11:53:16.000000 sqltrie-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-06 11:53:16.000000 sqltrie-0.4.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-06 11:53:16.000000 sqltrie-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-06 11:53:16.000000 sqltrie-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 11:53:16.000000 sqltrie-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-06 11:53:39.364030 sqltrie-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-06 11:53:16.000000 sqltrie-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-06 11:53:16.000000 sqltrie-0.4.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-06 11:53:16.000000 sqltrie-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-06 11:53:39.368030 sqltrie-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.360029 sqltrie-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/src/sqltrie/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/src/sqltrie/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/__pyinstaller/hook-sqltrie.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/pygtrie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/serialized.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/src/sqltrie/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/sqlite/diff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/sqlite/init.sql
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/sqlite/items.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/sqlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/sqlite/steps.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-06 11:53:16.000000 sqltrie-0.4.0/src/sqltrie/trie.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/src/sqltrie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-06 11:53:39.000000 sqltrie-0.4.0/src/sqltrie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-06 11:53:39.000000 sqltrie-0.4.0/src/sqltrie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:53:39.000000 sqltrie-0.4.0/src/sqltrie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-06 11:53:39.000000 sqltrie-0.4.0/src/sqltrie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:53:38.000000 sqltrie-0.4.0/src/sqltrie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-06 11:53:39.000000 sqltrie-0.4.0/src/sqltrie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 11:53:39.000000 sqltrie-0.4.0/src/sqltrie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 11:53:16.000000 sqltrie-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:53:39.364030 sqltrie-0.4.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-06 11:53:16.000000 sqltrie-0.4.0/tests/benchmarks/test_sqltrie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-06 11:53:16.000000 sqltrie-0.4.0/tests/test_sqltrie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-09 23:45:06.000000 sqltrie-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-09 23:45:06.000000 sqltrie-0.5.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-09 23:45:06.000000 sqltrie-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-09 23:45:06.000000 sqltrie-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 23:45:06.000000 sqltrie-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-09 23:45:30.102771 sqltrie-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-09 23:45:06.000000 sqltrie-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-09 23:45:06.000000 sqltrie-0.5.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-09 23:45:06.000000 sqltrie-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-09 23:45:30.106771 sqltrie-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.098771 sqltrie-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/src/sqltrie/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/src/sqltrie/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/__pyinstaller/hook-sqltrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/pygtrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/serialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/src/sqltrie/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/sqlite/diff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/sqlite/init.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/sqlite/items.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/sqlite/steps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-09 23:45:06.000000 sqltrie-0.5.0/src/sqltrie/trie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/src/sqltrie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-09 23:45:29.000000 sqltrie-0.5.0/src/sqltrie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-09 23:45:30.000000 sqltrie-0.5.0/src/sqltrie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:45:29.000000 sqltrie-0.5.0/src/sqltrie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 23:45:29.000000 sqltrie-0.5.0/src/sqltrie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:45:29.000000 sqltrie-0.5.0/src/sqltrie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 23:45:29.000000 sqltrie-0.5.0/src/sqltrie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 23:45:29.000000 sqltrie-0.5.0/src/sqltrie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 23:45:06.000000 sqltrie-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:45:30.102771 sqltrie-0.5.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-09 23:45:06.000000 sqltrie-0.5.0/tests/benchmarks/test_sqltrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-09 23:45:06.000000 sqltrie-0.5.0/tests/test_sqltrie.py
```

### Comparing `sqltrie-0.4.0/.cruft.json` & `sqltrie-0.5.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/.github/dependabot.yml` & `sqltrie-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/.github/workflows/release.yml` & `sqltrie-0.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/.github/workflows/tests.yml` & `sqltrie-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/.gitignore` & `sqltrie-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/.pre-commit-config.yaml` & `sqltrie-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/CODE_OF_CONDUCT.rst` & `sqltrie-0.5.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/CONTRIBUTING.rst` & `sqltrie-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/LICENSE` & `sqltrie-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/PKG-INFO` & `sqltrie-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqltrie
-Version: 0.4.0
+Version: 0.5.0
 Summary: SQL-based prefix tree inspired by pygtrie and python-diskcache
 Home-page: https://github.com/iterative/sqltrie
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Keywords: sqlite,sqlite3,sql,trie,prefix tree,data-science,diskcache
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqltrie-0.4.0/README.rst` & `sqltrie-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/noxfile.py` & `sqltrie-0.5.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/pyproject.toml` & `sqltrie-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/setup.cfg` & `sqltrie-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py` & `sqltrie-0.5.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/src/sqltrie/pygtrie.py` & `sqltrie-0.5.0/src/sqltrie/pygtrie.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 
     def __len__(self):
         return len(self._trie)
 
     def has_node(self, key):
         return bool(self._trie.has_node(key))
 
+    def delete_node(self, key):
+        raise NotImplementedError
+
     def items(self, prefix=None, shallow=False):
         kwargs = {"shallow": shallow}
         if prefix is not None:
             kwargs["prefix"] = prefix
 
         yield from self._trie.iteritems(**kwargs)
```

### Comparing `sqltrie-0.4.0/src/sqltrie/serialized.py` & `sqltrie-0.5.0/src/sqltrie/serialized.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
     def diff(self, *args, **kwargs):
         yield from self._trie.diff(*args, **kwargs)
 
     def has_node(self, key):
         return self._trie.has_node(key)
 
+    def delete_node(self, key):
+        return self._trie.delete_node(key)
+
     def shortest_prefix(self, key):
         sprefix = self._trie.shortest_prefix(key)
         if sprefix is None:
             return None
 
         skey, raw = sprefix
         return key, self._load(skey, raw)
```

### Comparing `sqltrie-0.4.0/src/sqltrie/sqlite/diff.sql` & `sqltrie-0.5.0/src/sqltrie/sqlite/diff.sql`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/src/sqltrie/sqlite/items.sql` & `sqltrie-0.5.0/src/sqltrie/sqlite/items.sql`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/src/sqltrie/sqlite/sqlite.py` & `sqltrie-0.5.0/src/sqltrie/sqlite/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,24 +145,14 @@
         return self._conn.execute(  # nosec
             f"""
             SELECT * FROM nodes WHERE nodes.pid == ? {limit_sql}
             """,
             (node["id"],),
         ).fetchall()
 
-    def _delete_node(self, key):
-        node = self._get_node(key)
-        del self._ids[key]
-        self._conn.execute(
-            """
-            DELETE FROM nodes WHERE id = ?
-            """,
-            (node["id"],),
-        )
-
     def __setitem__(self, key, value):
         pid = self._create_node(key[:-1])
 
         if HAS_UPSERT:
             self._conn.execute(
                 """
                 INSERT INTO
@@ -286,14 +276,24 @@
     def has_node(self, key: TrieKey) -> bool:
         try:
             self._get_node(key)
             return True
         except KeyError:
             return False
 
+    def delete_node(self, key: TrieKey):
+        node = self._get_node(key)
+        del self._ids[key]
+        self._conn.execute(
+            """
+            DELETE FROM nodes WHERE id = ?
+            """,
+            (node["id"],),
+        )
+
     def ls(
         self, key: TrieKey, with_values: Optional[bool] = False
     ) -> Iterator[Union[TrieKey, TrieNode]]:
         if with_values:
             yield from (  # type: ignore
                 ((*key, row["name"]), row["value"]) for row in self._get_children(key)
             )
```

### Comparing `sqltrie-0.4.0/src/sqltrie/sqlite/steps.sql` & `sqltrie-0.5.0/src/sqltrie/sqlite/steps.sql`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/src/sqltrie/trie.py` & `sqltrie-0.5.0/src/sqltrie/trie.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,19 @@
         pass
 
     @abstractmethod
     def has_node(self, key: TrieKey) -> bool:
         pass
 
     @abstractmethod
+    def delete_node(self, key: TrieKey) -> bool:
+        # NOTE: this will leave orphans down the tree
+        pass
+
+    @abstractmethod
     def prefixes(self, key: TrieKey) -> Iterator[TrieStep]:
         pass
 
     @abstractmethod
     def shortest_prefix(self, key: TrieKey) -> Optional[TrieStep]:
         pass
```

### Comparing `sqltrie-0.4.0/src/sqltrie.egg-info/PKG-INFO` & `sqltrie-0.5.0/src/sqltrie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqltrie
-Version: 0.4.0
+Version: 0.5.0
 Summary: SQL-based prefix tree inspired by pygtrie and python-diskcache
 Home-page: https://github.com/iterative/sqltrie
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Keywords: sqlite,sqlite3,sql,trie,prefix tree,data-science,diskcache
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqltrie-0.4.0/src/sqltrie.egg-info/SOURCES.txt` & `sqltrie-0.5.0/src/sqltrie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/tests/benchmarks/test_sqltrie.py` & `sqltrie-0.5.0/tests/benchmarks/test_sqltrie.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.4.0/tests/test_sqltrie.py` & `sqltrie-0.5.0/tests/test_sqltrie.py`

 * *Files identical despite different names*


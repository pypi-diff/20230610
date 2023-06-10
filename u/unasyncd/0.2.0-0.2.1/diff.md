# Comparing `tmp/unasyncd-0.2.0.tar.gz` & `tmp/unasyncd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unasyncd-0.2.0.tar", max compression
+gzip compressed data, was "unasyncd-0.2.1.tar", max compression
```

## Comparing `unasyncd-0.2.0.tar` & `unasyncd-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-10 09:21:40.873681 unasyncd-0.2.0/LICENSE
--rw-r--r--   0        0        0    16076 2023-06-10 09:21:40.873681 unasyncd-0.2.0/README.md
--rw-r--r--   0        0        0      908 2023-06-10 09:21:40.873681 unasyncd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/__init__.py
--rw-r--r--   0        0        0     3836 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/cli.py
--rw-r--r--   0        0        0     2482 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/config.py
--rw-r--r--   0        0        0    10306 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/main.py
--rw-r--r--   0        0        0    37782 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/transformers.py
--rw-r--r--   0        0        0    16786 1970-01-01 00:00:00.000000 unasyncd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-10 12:20:34.638068 unasyncd-0.2.1/LICENSE
+-rw-r--r--   0        0        0    15986 2023-06-10 12:20:34.638068 unasyncd-0.2.1/README.md
+-rw-r--r--   0        0        0      908 2023-06-10 12:20:34.638068 unasyncd-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/__init__.py
+-rw-r--r--   0        0        0     3836 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/cli.py
+-rw-r--r--   0        0        0     2482 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/config.py
+-rw-r--r--   0        0        0    10306 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/main.py
+-rw-r--r--   0        0        0    36834 2023-06-10 12:20:34.638068 unasyncd-0.2.1/unasyncd/transformers.py
+-rw-r--r--   0        0        0    16696 1970-01-01 00:00:00.000000 unasyncd-0.2.1/PKG-INFO
```

### Comparing `unasyncd-0.2.0/LICENSE` & `unasyncd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unasyncd-0.2.0/README.md` & `unasyncd-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
       * [File](#file)
       * [CLI options](#cli-options)
       * [Exclusions](#exclusions)
       * [Extending name replacements](#extending-name-replacements)
     * [Handling of imports](#handling-of-imports)
-    * [Integration with linters and formatters](#integration-with-linters-and-formatters)
     * [Limitations](#limitations)
     * [Disclaimer](#disclaimer)
 <!-- TOC -->
 
 ## What can be transformed?
 
 Unasyncd supports a wide variety of transformation, ranging from simple name
@@ -394,15 +393,15 @@
 
 ### As a pre-commit hook
 
 Unasyncd is available as a pre-commit hook:
 
 ```yaml
 - repo: https://github.com/provinzkraut/unasyncd
-  rev: v0.1.0
+  rev: v0.2.0
   hooks:
     - id: unasyncd
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
```

### Comparing `unasyncd-0.2.0/pyproject.toml` & `unasyncd-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unasyncd"
-version = "0.2.0"
+version = "0.2.1"
 description = "A tool to transform asynchronous Python code to synchronous Python code."
 authors = ["Janek Nouvertné <j.a.nouvertne@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `unasyncd-0.2.0/unasyncd/cli.py` & `unasyncd-0.2.1/unasyncd/cli.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.2.0/unasyncd/config.py` & `unasyncd-0.2.1/unasyncd/config.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.2.0/unasyncd/main.py` & `unasyncd-0.2.1/unasyncd/main.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.2.0/unasyncd/transformers.py` & `unasyncd-0.2.1/unasyncd/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -952,17 +952,14 @@
         if self._should_transform_docstrings and self._should_transform_current_node:
             updated_node = self._transform_docstring(updated_node)
 
         return updated_node
 
 
 class _ImportTransformer(cst.CSTTransformer):
-    # partly taken from
-    # https://cst.readthedocs.io/en/latest/scope_tutorial.html#Automatically-Remove-Unused-Import
-
     def __init__(
         self,
         *,
         imports_to_update: dict[cst.ImportFrom, set[str]],
         if_type_checking_node: cst.If | None,
         type_checking_imports_to_add: Iterable[AnyImport],
     ) -> None:
@@ -989,34 +986,14 @@
                 *[
                     cst.SimpleStatementLine([import_])
                     for import_ in self.type_checking_imports_to_add
                 ],
             ],
         )
 
-    def leave_import_alike(
-        self, original_node: AnyImportT, updated_node: AnyImportT
-    ) -> AnyImportT | cst.RemovalSentinel:
-        if isinstance(updated_node.names, cst.ImportStar):
-            return updated_node
-
-        names_to_keep = []
-        for name in updated_node.names:
-            names_to_keep.append(name.with_changes(comma=cst.MaybeSentinel.DEFAULT))
-
-        if len(names_to_keep) == 0:
-            return cst.RemoveFromParent()
-        else:
-            return updated_node.with_changes(names=names_to_keep)  # type: ignore[return-value]  # noqa: E501
-
-    def leave_Import(
-        self, original_node: cst.Import, updated_node: cst.Import
-    ) -> cst.Import | cst.RemovalSentinel:
-        return self.leave_import_alike(original_node, updated_node)
-
     def leave_ImportFrom(
         self, original_node: cst.ImportFrom, updated_node: cst.ImportFrom
     ) -> cst.ImportFrom | cst.RemovalSentinel:
         aliases_to_add = self.imports_to_update.get(original_node)
         if aliases_to_add:
             new_aliases = [cst.ImportAlias(cst.Name(name)) for name in aliases_to_add]
 
@@ -1026,15 +1003,15 @@
                 else [updated_node.names]  # type: ignore[list-item]
             )
 
             updated_node = updated_node.with_changes(
                 names=[*current_names, *new_aliases]
             )
 
-        return self.leave_import_alike(original_node, updated_node)
+        return updated_node
 
     # since we're only interested in module level imports, we don't need to visit
     # class and function definitions
 
     def visit_ClassDef(self, node: cst.ClassDef) -> bool:
         return False
```

### Comparing `unasyncd-0.2.0/PKG-INFO` & `unasyncd-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unasyncd
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to transform asynchronous Python code to synchronous Python code.
 License: MIT
 Author: Janek Nouvertné
 Author-email: j.a.nouvertne@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,14 @@
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
       * [File](#file)
       * [CLI options](#cli-options)
       * [Exclusions](#exclusions)
       * [Extending name replacements](#extending-name-replacements)
     * [Handling of imports](#handling-of-imports)
-    * [Integration with linters and formatters](#integration-with-linters-and-formatters)
     * [Limitations](#limitations)
     * [Disclaimer](#disclaimer)
 <!-- TOC -->
 
 ## What can be transformed?
 
 Unasyncd supports a wide variety of transformation, ranging from simple name
@@ -414,15 +413,15 @@
 
 ### As a pre-commit hook
 
 Unasyncd is available as a pre-commit hook:
 
 ```yaml
 - repo: https://github.com/provinzkraut/unasyncd
-  rev: v0.1.0
+  rev: v0.2.0
   hooks:
     - id: unasyncd
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
```


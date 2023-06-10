# Comparing `tmp/wildered-0.1.1.tar.gz` & `tmp/wildered-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildered-0.1.1.tar", max compression
+gzip compressed data, was "wildered-0.1.2.tar", max compression
```

## Comparing `wildered-0.1.1.tar` & `wildered-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-06-02 11:38:41.913835 wildered-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      361 2023-06-09 13:00:36.185459 wildered-0.1.1/README.md
--rw-r--r--   0        0        0     1098 2023-06-10 02:01:45.696707 wildered-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 11:40:57.382603 wildered-0.1.1/wildered/__init__.py
--rw-r--r--   0        0        0       88 2023-06-04 10:18:18.194534 wildered-0.1.1/wildered/ast/__init__.py
--rw-r--r--   0        0        0    10144 2023-06-09 12:59:42.355472 wildered-0.1.1/wildered/ast/directive_parser.py
--rw-r--r--   0        0        0     9802 2023-06-07 10:24:21.755536 wildered-0.1.1/wildered/ast/source_code.py
--rw-r--r--   0        0        0    11189 2023-06-07 11:14:39.823997 wildered-0.1.1/wildered/ast/utils.py
--rw-r--r--   0        0        0        0 2023-06-04 10:19:18.785349 wildered-0.1.1/wildered/cst/__init__.py
--rw-r--r--   0        0        0     8767 2023-06-06 11:40:58.617603 wildered-0.1.1/wildered/cst/directive_parser.py
--rw-r--r--   0        0        0     3259 2023-06-06 11:40:59.841769 wildered-0.1.1/wildered/cst/source_code.py
--rw-r--r--   0        0        0     2306 2023-06-04 10:15:09.997931 wildered-0.1.1/wildered/cst/utils.py
--rw-r--r--   0        0        0     3749 2023-06-06 10:52:50.865918 wildered-0.1.1/wildered/directive.py
--rw-r--r--   0        0        0      802 2023-06-04 10:14:04.553786 wildered-0.1.1/wildered/group.py
--rw-r--r--   0        0        0     3774 2023-06-06 12:13:20.600427 wildered-0.1.1/wildered/models.py
--rw-r--r--   0        0        0     1313 2023-05-31 10:45:03.731806 wildered-0.1.1/wildered/utils.py
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 wildered-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-02 11:38:41.913835 wildered-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      361 2023-06-09 13:00:36.185459 wildered-0.1.2/README.md
+-rw-r--r--   0        0        0     1098 2023-06-10 04:10:20.753080 wildered-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 11:40:57.382603 wildered-0.1.2/wildered/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-04 10:18:18.194534 wildered-0.1.2/wildered/ast/__init__.py
+-rw-r--r--   0        0        0    10144 2023-06-09 12:59:42.355472 wildered-0.1.2/wildered/ast/directive_parser.py
+-rw-r--r--   0        0        0     9738 2023-06-10 04:08:39.688938 wildered-0.1.2/wildered/ast/source_code.py
+-rw-r--r--   0        0        0    10057 2023-06-10 04:08:36.655605 wildered-0.1.2/wildered/ast/utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:19:18.785349 wildered-0.1.2/wildered/cst/__init__.py
+-rw-r--r--   0        0        0     8767 2023-06-06 11:40:58.617603 wildered-0.1.2/wildered/cst/directive_parser.py
+-rw-r--r--   0        0        0     3259 2023-06-06 11:40:59.841769 wildered-0.1.2/wildered/cst/source_code.py
+-rw-r--r--   0        0        0     2306 2023-06-04 10:15:09.997931 wildered-0.1.2/wildered/cst/utils.py
+-rw-r--r--   0        0        0     3749 2023-06-06 10:52:50.865918 wildered-0.1.2/wildered/directive.py
+-rw-r--r--   0        0        0      802 2023-06-04 10:14:04.553786 wildered-0.1.2/wildered/group.py
+-rw-r--r--   0        0        0     3774 2023-06-06 12:13:20.600427 wildered-0.1.2/wildered/models.py
+-rw-r--r--   0        0        0     1313 2023-05-31 10:45:03.731806 wildered-0.1.2/wildered/utils.py
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 wildered-0.1.2/PKG-INFO
```

### Comparing `wildered-0.1.1/LICENSE.md` & `wildered-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/pyproject.toml` & `wildered-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wildered"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["engkheng <ongengkheng929@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `wildered-0.1.1/wildered/ast/directive_parser.py` & `wildered-0.1.2/wildered/ast/directive_parser.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/wildered/ast/source_code.py` & `wildered-0.1.2/wildered/ast/source_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,23 +159,21 @@
             directive_prefix=directive_prefix,
             drop_implementation=drop_implementation,
             return_global_import=return_global_import,
         )
 
     def get_entity(
         self,
-        entity_path: List[str],
+        entity_name: str,
         drop_directive: bool = False,
         directive_prefix: str = "",
         drop_implementation: bool = False,
         return_global_import: bool = False,
     ) -> str:
-        entity_node: ast.AST = self.node
-        for i in entity_path:
-            entity_node = locate_entity(code=entity_node, entity_name=i)
+        entity_node: ast.AST = locate_entity(code=self.node, entity_name=entity_name)
 
         return self._unparse(
             node=entity_node,
             drop_directive=drop_directive,
             directive_prefix=directive_prefix,
             drop_implementation=drop_implementation,
             return_global_import=return_global_import,
```

### Comparing `wildered-0.1.1/wildered/ast/utils.py` & `wildered-0.1.2/wildered/ast/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+from collections import defaultdict
 from typing import Dict, List, Optional, Tuple, Union
 
 from typing_extensions import assert_never
 
 
 def get_call_name(call_node: ast.Call) -> str:
     if hasattr(call_node.func, "id"):
@@ -282,60 +283,33 @@
     return imports
 
 
 class NodeFinder(ast.NodeVisitor):
     def __init__(
         self,
         entity_list: Optional[List[str]] = None,
-        func_list: Optional[List[str]] = None,
-        class_list: Optional[List[str]] = None,
-        method_list: Optional[Dict[str, List[str]]] = None,
     ) -> None:
         """
         Initialize the NodeFinder class.
         Args:
-            entity_list (Optional[List[str]]): A list of entities to search for.
-            func_list (Optional[List[str]]): A list of function names to search for.
-            class_list (Optional[List[str]]): A list of class names to search for.
-            method_list (Optional[Dict[str, List[str]]]): A dictionary mapping class names to a list of method names.
+            entity_list: Optional[List[str]] = None
         """
         self.entity_list = entity_list if entity_list else []
-        self.func_list = func_list if func_list else []
-        self.class_list = class_list if class_list else []
-        self.method_list = method_list if method_list else {}
-        self.cur_class = None
-        self.pure = True
-        self.found_node = {}
+        self.found_node = defaultdict(lambda: None)
 
     def visit_FunctionDef(self, node):
-        if (
-            (node.name in self.entity_list)
-            or (node.name in self.func_list)
-            or (
-                self.cur_class
-                and (self.cur_class in self.method_list)
-                and (node.name in self.method_list[self.cur_class])
-            )
-        ):
+        if node.name in self.entity_list:
             self.found_node[node.name] = node
 
-        elif not self.cur_class:
-            self.pure = False
-
         self.generic_visit(node)
 
     def visit_ClassDef(self, node):
-        if (node.name in self.entity_list) or (node.name in self.class_list):
+        if node.name in self.entity_list:
             self.found_node[node.name] = node
 
-        elif node.name not in self.method_list:
-            self.pure = False
-
-        self.cur_class = node.name
         self.generic_visit(node)
-        self.cur_class = None
 
 
 def locate_entity(code: ast.AST, entity_name: str):
     finder = NodeFinder(entity_name)
     finder.visit(code)
-    return finder.found_node
+    return finder.found_node[entity_name]
```

### Comparing `wildered-0.1.1/wildered/cst/directive_parser.py` & `wildered-0.1.2/wildered/cst/directive_parser.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/wildered/cst/source_code.py` & `wildered-0.1.2/wildered/cst/source_code.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/wildered/cst/utils.py` & `wildered-0.1.2/wildered/cst/utils.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/wildered/directive.py` & `wildered-0.1.2/wildered/directive.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/wildered/group.py` & `wildered-0.1.2/wildered/group.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/wildered/models.py` & `wildered-0.1.2/wildered/models.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/wildered/utils.py` & `wildered-0.1.2/wildered/utils.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.1/PKG-INFO` & `wildered-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildered
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: engkheng
 Author-email: ongengkheng929@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


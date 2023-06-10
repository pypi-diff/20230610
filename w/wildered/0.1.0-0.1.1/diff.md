# Comparing `tmp/wildered-0.1.0.tar.gz` & `tmp/wildered-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildered-0.1.0.tar", max compression
+gzip compressed data, was "wildered-0.1.1.tar", max compression
```

## Comparing `wildered-0.1.0.tar` & `wildered-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-06-02 11:38:41.913835 wildered-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      358 2023-06-02 11:36:16.562991 wildered-0.1.0/README.md
--rw-r--r--   0        0        0     1098 2023-06-04 10:18:02.507873 wildered-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 11:40:57.382603 wildered-0.1.0/wildered/__init__.py
--rw-r--r--   0        0        0       88 2023-06-04 10:18:18.194534 wildered-0.1.0/wildered/ast/__init__.py
--rw-r--r--   0        0        0     9707 2023-06-06 12:05:22.178879 wildered-0.1.0/wildered/ast/directive_parser.py
--rw-r--r--   0        0        0     9954 2023-06-06 11:41:03.904268 wildered-0.1.0/wildered/ast/source_code.py
--rw-r--r--   0        0        0    10453 2023-06-04 10:15:09.987098 wildered-0.1.0/wildered/ast/utils.py
--rw-r--r--   0        0        0        0 2023-06-04 10:19:18.785349 wildered-0.1.0/wildered/cst/__init__.py
--rw-r--r--   0        0        0     8767 2023-06-06 11:40:58.617603 wildered-0.1.0/wildered/cst/directive_parser.py
--rw-r--r--   0        0        0     3259 2023-06-06 11:40:59.841769 wildered-0.1.0/wildered/cst/source_code.py
--rw-r--r--   0        0        0     2306 2023-06-04 10:15:09.997931 wildered-0.1.0/wildered/cst/utils.py
--rw-r--r--   0        0        0     3749 2023-06-06 10:52:50.865918 wildered-0.1.0/wildered/directive.py
--rw-r--r--   0        0        0      802 2023-06-04 10:14:04.553786 wildered-0.1.0/wildered/group.py
--rw-r--r--   0        0        0     3774 2023-06-06 12:13:20.600427 wildered-0.1.0/wildered/models.py
--rw-r--r--   0        0        0     1313 2023-05-31 10:45:03.731806 wildered-0.1.0/wildered/utils.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 wildered-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-02 11:38:41.913835 wildered-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      361 2023-06-09 13:00:36.185459 wildered-0.1.1/README.md
+-rw-r--r--   0        0        0     1098 2023-06-10 02:01:45.696707 wildered-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 11:40:57.382603 wildered-0.1.1/wildered/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-04 10:18:18.194534 wildered-0.1.1/wildered/ast/__init__.py
+-rw-r--r--   0        0        0    10144 2023-06-09 12:59:42.355472 wildered-0.1.1/wildered/ast/directive_parser.py
+-rw-r--r--   0        0        0     9802 2023-06-07 10:24:21.755536 wildered-0.1.1/wildered/ast/source_code.py
+-rw-r--r--   0        0        0    11189 2023-06-07 11:14:39.823997 wildered-0.1.1/wildered/ast/utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:19:18.785349 wildered-0.1.1/wildered/cst/__init__.py
+-rw-r--r--   0        0        0     8767 2023-06-06 11:40:58.617603 wildered-0.1.1/wildered/cst/directive_parser.py
+-rw-r--r--   0        0        0     3259 2023-06-06 11:40:59.841769 wildered-0.1.1/wildered/cst/source_code.py
+-rw-r--r--   0        0        0     2306 2023-06-04 10:15:09.997931 wildered-0.1.1/wildered/cst/utils.py
+-rw-r--r--   0        0        0     3749 2023-06-06 10:52:50.865918 wildered-0.1.1/wildered/directive.py
+-rw-r--r--   0        0        0      802 2023-06-04 10:14:04.553786 wildered-0.1.1/wildered/group.py
+-rw-r--r--   0        0        0     3774 2023-06-06 12:13:20.600427 wildered-0.1.1/wildered/models.py
+-rw-r--r--   0        0        0     1313 2023-05-31 10:45:03.731806 wildered-0.1.1/wildered/utils.py
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 wildered-0.1.1/PKG-INFO
```

### Comparing `wildered-0.1.0/LICENSE.md` & `wildered-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wildered-0.1.0/pyproject.toml` & `wildered-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "wildered"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["engkheng <ongengkheng929@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.8"
 ast-comments = "^1.0.1"
+libcst = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.270"
 pytest = "^7.3.1"
 black = "^23.3.0"
 poethepoet = "^0.20.0"
-libcst = "^1.0.0"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-material = "^9.1.15"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
```

### Comparing `wildered-0.1.0/wildered/ast/directive_parser.py` & `wildered-0.1.1/wildered/cst/directive_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,227 +1,116 @@
 from __future__ import annotations
 
-import ast
 import copy
-from typing import (
-    Annotated,
-    Any,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Type,
-)
+from typing import Annotated, Any, Dict, List, Optional, Tuple, Type
 
-import ast_comments
+import libcst as cst
 from pydantic import validator
 from typing_extensions import assert_never
 
-from wildered.ast.utils import (
-    DropDirective,
-    DropImplementation,
+from wildered.cst.source_code import CSTSourceCode
+from wildered.cst.utils import (
+    CSTDropDirective,
     get_call_name,
-    locate_function,
 )
 from wildered.directive import Directive, DirectiveContext, Identifier
 from wildered.models import BaseDirectiveParser, BaseEntity
 
-from .source_code import ASTSourceCode
-from .utils import (
-    locate_class,
-)
-
 
-class ASTDirectiveParser(BaseDirectiveParser):
-    def parse(
-        self, source: ASTSourceCode, drop_directive: bool = True
-    ) -> List[ASTEntity]:
-        # Drop_directive will mutate the SourceCode
-        detector = DetectDirective(
-            parser=self,
-            source=source,
-            directive_list=self.directives,
-            code=source.node,
-            prefix=self.prefix_name,
-        )
+class CSTDirectiveParser(BaseDirectiveParser):
+    def parse(self, source: CSTSourceCode, drop_directive: bool = True) -> List[CSTEntity]:
+        detector = CSTDetectDirective(
+                    parser=self,
+                    source=source,
+                    directive_list=self.directives,
+                    code=source.node,
+                    prefix=self.prefix_name,
+                )
         
-        detector.visit(source.node)
+        source.node.visit(detector)
 
         if drop_directive:
-            drop_transformer = DropDirective(prefix=self.prefix_name)
-            drop_transformer.visit(source.node)
+            drop_transformer = CSTDropDirective(prefix=self.prefix_name)
+            source.node.visit(drop_transformer)
 
         self.check_valid_combination(entity_list = detector.detected)
         return detector.detected
-
-
-class ASTEntity(BaseEntity):
-    wrapping_node: Optional[ASTEntity]
-    node: ast.AST
+    
+class CSTEntity(BaseEntity):
+    wrapping_node: Optional[CSTEntity]
+    node: Any
     name: str
-    source: ASTSourceCode
+    source: CSTSourceCode
     directives: Dict[str, List[Directive]]
-    parser: ASTDirectiveParser
+    parser: CSTDirectiveParser
     _context: DirectiveContext
-
-    class Config:
-        arbitrary_types_allowed = True
-
-    def save(self, *args, **kwargs) -> None:
-        self.source.save(*args, **kwargs)
-
+    
     def unparse(
         self,
         drop_directive: bool = False,
         drop_implementation: bool = False,
         return_global_import: bool = False,
         include_ancestor: bool = False,
     ) -> str:
         if include_ancestor:
             # Top ancestor
             node = copy.deepcopy(self.ancestor[-1].node)
 
         else:
             node = copy.deepcopy(self.node)
 
-        if drop_directive:
-            transformer = DropDirective(prefix=self.parser.prefix_name)
-            transformer.visit(node)
-
-        if drop_implementation:
-            transformer = DropImplementation(exception=[])
-            transformer.visit(node)
-
-        ast.fix_missing_locations(node)
-
-        if return_global_import:
-            return (
-                self.source.get_import_statement(
-                    drop_directive=drop_directive,
-                    directive_prefix=self.parser.prefix_name,
-                )
-                + "\n\n"
-                + ast_comments.unparse(node)
-            )
-
-        else:
-            return ast_comments.unparse(node)
-
-
-class ASTClassEntity(ASTEntity):
-    node: ast.ClassDef
-    _context = "class"
-
-    def update(self, new_code: ast.ClassDef | str) -> None:
-        if isinstance(new_code, str):
-            new_code = ast_comments.parse(new_code)
-            new_code = locate_class(new_code, class_name=self.name)
-
-        self.node.body = new_code.body
-        self.node.decorator_list = new_code.decorator_list
-
-    def modify_signature(self, new_code: ast.ClassDef) -> None:
-        pass
-
-
-class ASTFunctionEntity(ASTEntity):
-    node: ast.FunctionDef
+        return self.source._unparse(node=node, 
+                                    drop_directive=drop_directive, 
+                                    directive_prefix=self.parser.prefix_name, 
+                                    return_global_import=return_global_import, 
+                                    drop_implementation=drop_implementation)
+    
+class CSTFunctionEntity(CSTEntity):
     _context = "function"
-
-    def update(self, new_code: ast.FunctionDef | str) -> None:
-        if isinstance(new_code, str):
-            new_code = ast_comments.parse(new_code)
-            new_code = locate_function(new_code, func_name=self.name)
-
-        self.node.body = new_code.body
-        self.node.decorator_list = new_code.decorator_list
-
-    def modify_signature(self, new_code: ast.FunctionDef) -> None:
+    
+    @validator("wrapping_node")
+    def check_wrapping_node(cls, v):
+        if v is not None:
+            raise ValueError(
+                "ASTModuleEntity should not have wrapping_node, make sure the run directive is defined at top level."
+            )
+            
+    def update(self, new_code: str) -> None:
         pass
-
-
-class ASTModuleEntity(ASTEntity):
+    
+class CSTModuleEntity(CSTEntity):
     _context = "module"
-
+    
     @validator("wrapping_node")
     def check_wrapping_node(cls, v):
         if v is not None:
             raise ValueError(
                 "ASTModuleEntity should not have wrapping_node, make sure the run directive is defined at top level."
             )
         
         return v
+    
+    def update(self, new_code: str) -> None:
+        pass
+    
+class CSTClassEntity(CSTEntity):
+    _context = "class"
+    
+    
+    def update(self, new_code: str) -> None:
+        pass
 
-    def update(self, new_code: ast.Module) -> None:
-        self.node.body = new_code.body
-
-
-ASTDirectiveParser.update_forward_refs()
-
-
-def parse_arguments(node: ast.Call) -> Tuple[List[Any], dict[str, Any]]:
-    positional_arg = []
-    keyword_arg = {}
-
-    for arg in node.args:
-        arg_value = extract_value(arg)
-        positional_arg.append(arg_value)
-
-    for keyword in node.keywords:
-        arg_value = extract_value(keyword.value)
-        keyword_arg[keyword.arg] = arg_value
-
-    return positional_arg, keyword_arg
-
-
-def extract_value(node: ast.AST):
-    match node:
-        case ast.Constant():
-            return node.value
-        
-        case ast.Expr():
-            return Identifier(node=node, name=node.value)
-        
-        case ast.Dict():
-            return extract_dict(node=node)
-        
-        case ast.Name():
-            return Identifier(node=node, name=node.id)
-        
-        case ast.Str():
-            return node.s
-        
-        case ast.Num():
-            return node.n
-        
-        case ast.List():
-            return extract_list(node)
-        
-        case other:
-            assert_never(other)
-
-def extract_dict(node: ast.Dict):
-    return {
-        extract_value(key): extract_value(value)
-        for key, value in zip(node.keys, node.values)
-    }
-
-
-def extract_list(node: ast.List):
-    return [extract_value(elt) for elt in node.elts]
-
-
-class DetectDirective(ast.NodeVisitor):
+class CSTDetectDirective(cst.CSTVisitor):
     # Go through the node, return a list of task
     def __init__(
         self,
-        parser: ASTDirectiveParser,
-        source: ASTSourceCode,
+        parser: CSTDirectiveParser,
+        source: CSTSourceCode,
         directive_list: List[Type[Directive]],
-        code: ast.AST,
+        code: cst.Module,
         prefix: str,
     ):
         self.parser = parser
         self.code = code
         self.source = source
         self.prefix = prefix
         self.detected = []
@@ -234,86 +123,82 @@
         for directive_cls in directive_list:
             config = directive_cls.config
             alias = config.alias
             name = config.name
             self.directives[name] = {"alias": alias, "cls": directive_cls}
             self.config_map[name] = config
 
-    def visit_Call(self, node: ast.Call) -> Any:
+    def visit_Call(self, node: cst.Call) -> Any:
         try:
             prefix, node_name = get_call_name(node)
             if (prefix == self.prefix) and (node_name == "run"):
                 directives = self.extract_directives(
                     decorators=node.args,
                 )
                 if len(directives) != 0:
-                    node_task = ASTModuleEntity(
+                    node_task = CSTModuleEntity(
                         parser=self.parser,
                         source=self.source,
                         wrapping_node=self.wrapping_node,
                         node=self.code,
                         name=self.source.filename.name,
                         directives=directives,
                     )
                     self.detected.append(node_task)
 
         except AttributeError:
             pass
 
-        finally:
-            self.generic_visit(node)
-
-    def visit_FunctionDef(self, node: ast.FunctionDef) -> Any:
+    def visit_FunctionDef(self, node: cst.FunctionDef) -> Any:
         directives = self.extract_directives(
-            decorators=node.decorator_list
+            decorators=node.decorators
         )
-        node_task = ASTFunctionEntity(
+        node_task = CSTFunctionEntity(
             parser=self.parser,
             source=self.source,
             wrapping_node=self.wrapping_node,
             node=node,
-            name=node.name,
+            name=node.name.value,
             directives=directives,
         )
 
         if len(directives) > 0:
             self.detected.append(node_task)
 
         previous = self.wrapping_node
         self.wrapping_node = node_task
-        self.generic_visit(node=node)
         self.wrapping_node = previous
 
-    def visit_ClassDef(self, node: ast.ClassDef) -> Any:
+    def visit_ClassDef(self, node: cst.ClassDef) -> Any:
         directives = self.extract_directives(
-            decorators=node.decorator_list,
+            decorators=node.decorators,
         )
-        node_task = ASTClassEntity(
+        node_task = CSTClassEntity(
             parser=self.parser,
             source=self.source,
             wrapping_node=self.wrapping_node,
             node=node,
-            name=node.name,
+            name=node.name.value,
             directives=directives,
         )
 
         if len(directives) > 0:
             self.detected.append(node_task)
 
         previous = self.wrapping_node
         self.wrapping_node = node_task
-        self.generic_visit(node=node)
         self.wrapping_node = previous
 
     def extract_directives(
-        self, decorators: ast.AST
+        self, decorators: List[cst.Decorator]
     ) -> Dict[str, List[Directive]]:
         directive_map = {}
+        [decorator.decorator for decorator in decorators]
         for node in decorators:
-            if isinstance(node, ast.Call):
+            if isinstance(node, cst.Call):
                 prefix_name, name = get_call_name(node)
                 if prefix_name != self.prefix:
                     continue
 
                 matched_directive = self.directive_lookup(name)
                 if matched_directive is not None:
                     pos_args, keyword_args = parse_arguments(node)
@@ -338,7 +223,65 @@
         for i, j in self.directives.items():
             aliases = j["alias"]
             for alias in aliases:
                 if alias == name:
                     return (name, j["cls"], i)
 
         return None
+
+
+def parse_arguments(node: cst.Call) -> Tuple[List[Any], dict[str, Any]]:
+    positional_arg = []
+    keyword_arg = {}
+
+    for arg in node.args:
+        arg = arg.value
+        if hasattr(arg, "keyword"):
+            arg_name = arg.keyword.value
+            arg_value = extract_value(arg.value.value)
+            keyword_arg[arg_name] = arg_value
+        
+        else:
+            arg_value = extract_value(arg.value.value)
+            positional_arg.append(arg_value)
+
+    return positional_arg, keyword_arg
+
+
+def extract_value(node: cst.CSTNode):
+    match node:       
+        case cst.Expr():
+            return Identifier(node=node, name=node.value)
+        
+        case cst.Dict():
+            return extract_dict(node=node)
+        
+        case cst.Name():
+            return Identifier(node=node, name=node.value)
+        
+        case cst.SimpleString():
+            return node.value
+        
+        case cst.Float():
+            return float(node.value)
+        
+        case cst.Integer():
+            return int(node.value)
+        
+        case cst.List():
+            return extract_list(node)
+        
+        case other:
+            assert_never(other)
+
+def extract_dict(node: cst.Dict) -> dict:
+    result = {}
+    for i in node.elements:
+        key = i.key.value
+        value = extract_value(i.value)
+        result[key] = value
+    
+    return result
+
+
+def extract_list(node: cst.List) -> list:
+    return [extract_value(elt.value) for elt in node.elements]
```

### Comparing `wildered-0.1.0/wildered/ast/source_code.py` & `wildered-0.1.1/wildered/ast/source_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,19 @@
         """
         import_list should be a list of ast node
         replace the import lines in self.code to the one in import_list
         """
         code = ast_comments.parse(new_code)
         existing_import_list = extract_import_list(self.node)
         new_import_list = extract_import_list(code)
-        new_import, modified_import = diff_import_list(
+        new_import = diff_import_list(
             existing_import_list, new_import_list
         )
-        # TODO: For now we insert the modified_import first
         for i in new_import:
-            self.node.body.insert(1, i)
-
-        for i in modified_import:
-            self.node.body.insert(1, i)
+            self.node.body.insert(0, i)
 
     def get_function(
         self,
         func_name: str,
         drop_directive: bool = False,
         directive_prefix: str = "",
         drop_implementation: bool = False,
```

### Comparing `wildered-0.1.0/wildered/ast/utils.py` & `wildered-0.1.1/wildered/ast/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import ast
 from typing import Dict, List, Optional, Tuple, Union
 
+from typing_extensions import assert_never
+
 
 def get_call_name(call_node: ast.Call) -> str:
     if hasattr(call_node.func, "id"):
         return ("", call_node.func.id)
 
     else:
         return (call_node.func.value.id, call_node.func.attr)
@@ -24,53 +26,77 @@
         None.
     """
     for imp in imports:
         if isinstance(imp, ast.Import):
             for name in imp.names:
                 if name.name == keyword:
                     return imp
-        elif isinstance(imp, ast.ImportFrom) and imp.module == keyword:
-            return imp
+                
+        elif isinstance(imp, ast.ImportFrom):
+            continue
+        
+        else:
+            assert_never(imp)
 
     return None
 
+def locate_import_from(imports: List[Union[ast.Import, ast.ImportFrom]], keyword: str, level: int
+) -> Optional[ast.ImportFrom]:
+    for imp in imports:
+        if isinstance(imp, ast.Import):
+            continue
+        
+        elif isinstance(imp, ast.ImportFrom):
+            if imp.module == keyword and imp.level == level:
+                return imp
+        
+        else:
+            assert_never(imp)
+            
+    return None
+
+def integrate_alias(old_aliases: List[ast.alias], new_aliases: List[ast.alias]) -> None:
+    old_alias_names = [i.name for i in old_aliases]
+    def is_new_alias(alias: ast.alias) -> bool:
+        return not(alias.name in old_alias_names)
+
+    new_alias_list = filter(is_new_alias, new_aliases)
+    old_aliases.extend(new_alias_list)
 
 def diff_import_list(
     old_imports: List[Union[ast.Import, ast.ImportFrom]],
     new_imports: List[Union[ast.Import, ast.ImportFrom]],
-) -> Tuple[List[Union[ast.Import, ast.ImportFrom]], List[ast.ImportFrom]]:
+) -> List[Union[ast.Import, ast.ImportFrom]]:
     """Detects new or modified import statements in `new_imports` compared to `old_imports`.
     Args:
         old_imports: A list of `ast.Import` or `ast.ImportFrom` nodes representing the old import statements.
         new_imports: A list of `ast.Import` or `ast.ImportFrom` nodes representing the new import statements.
     Returns:
         A tuple containing two lists:
         - `new_import_ast`: A list of new import statements found in `new_imports`.
         - `modified_import_from_ast`: A list of modified `ast.ImportFrom` statements found in `new_imports`.
     Raises:
         None.
     """
+    # Will modify the import from inplace if available.
     new_import_ast = []
-    modified_import_from_ast = []
 
     for i in new_imports:
         if isinstance(i, ast.Import):
             match = locate_import(old_imports, i.names[0].name)
             if match is None:  # Meaning it is a new import
                 new_import_ast.append(i)
         elif isinstance(i, ast.ImportFrom):
-            match = locate_import(old_imports, i.module)
+            match = locate_import_from(old_imports, i.module, level=i.level)
             if match is None:  # New import
                 new_import_ast.append(i)
             else:
-                if match.level == i.level and match.module == i.module:
-                    # Compare the match and i, if they are not the same, it means it is modified
-                    modified_import_from_ast.append(i)
-
-    return new_import_ast, modified_import_from_ast
+                # TODO: Not elegant
+                integrate_alias(old_aliases=match.names, new_aliases=i.names)
+    return new_import_ast
 
 
 class DropDirective(ast.NodeTransformer):
     def __init__(self, prefix: str):
         self.prefix = prefix
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
```

### Comparing `wildered-0.1.0/wildered/cst/directive_parser.py` & `wildered-0.1.1/wildered/ast/directive_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,246 @@
 from __future__ import annotations
 
+import ast
 import copy
-from typing import Annotated, Any, Dict, List, Optional, Tuple, Type
+from typing import (
+    Annotated,
+    Any,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+)
 
-import libcst as cst
+import ast_comments
 from pydantic import validator
 from typing_extensions import assert_never
 
-from wildered.cst.source_code import CSTSourceCode
-from wildered.cst.utils import (
-    CSTDropDirective,
+from wildered.ast.utils import (
+    DropDirective,
+    DropImplementation,
     get_call_name,
+    locate_function,
 )
 from wildered.directive import Directive, DirectiveContext, Identifier
 from wildered.models import BaseDirectiveParser, BaseEntity
 
+from .source_code import ASTSourceCode
+from .utils import (
+    locate_class,
+)
 
-class CSTDirectiveParser(BaseDirectiveParser):
-    def parse(self, source: CSTSourceCode, drop_directive: bool = True) -> List[CSTEntity]:
-        detector = CSTDetectDirective(
-                    parser=self,
-                    source=source,
-                    directive_list=self.directives,
-                    code=source.node,
-                    prefix=self.prefix_name,
-                )
-        
-        source.node.visit(detector)
+
+class ASTDirectiveParser(BaseDirectiveParser):
+    def parse(
+        self, source: ASTSourceCode, drop_directive: bool = True
+    ) -> List[ASTEntity]:
+        # Drop_directive will mutate the SourceCode
+        detector = DetectDirective(
+            parser=self,
+            source=source,
+            directive_list=self.directives,
+            code=source.node,
+            prefix=self.prefix_name,
+        )
+
+        detector.visit(source.node)
 
         if drop_directive:
-            drop_transformer = CSTDropDirective(prefix=self.prefix_name)
-            source.node.visit(drop_transformer)
+            drop_transformer = DropDirective(prefix=self.prefix_name)
+            drop_transformer.visit(source.node)
 
-        self.check_valid_combination(entity_list = detector.detected)
+        self.check_valid_combination(entity_list=detector.detected)
         return detector.detected
-    
-class CSTEntity(BaseEntity):
-    wrapping_node: Optional[CSTEntity]
-    node: Any
+
+
+class ASTEntity(BaseEntity):
+    wrapping_node: Optional[ASTEntity]
+    node: ast.AST
     name: str
-    source: CSTSourceCode
+    source: ASTSourceCode
     directives: Dict[str, List[Directive]]
-    parser: CSTDirectiveParser
+    parser: ASTDirectiveParser
     _context: DirectiveContext
-    
+
+    class Config:
+        arbitrary_types_allowed = True
+
+    def save(self, *args, **kwargs) -> None:
+        self.source.save(*args, **kwargs)
+
     def unparse(
         self,
         drop_directive: bool = False,
         drop_implementation: bool = False,
         return_global_import: bool = False,
         include_ancestor: bool = False,
     ) -> str:
         if include_ancestor:
             # Top ancestor
             node = copy.deepcopy(self.ancestor[-1].node)
 
         else:
             node = copy.deepcopy(self.node)
 
-        return self.source._unparse(node=node, 
-                                    drop_directive=drop_directive, 
-                                    directive_prefix=self.parser.prefix_name, 
-                                    return_global_import=return_global_import, 
-                                    drop_implementation=drop_implementation)
-    
-class CSTFunctionEntity(CSTEntity):
-    _context = "function"
-    
-    @validator("wrapping_node")
-    def check_wrapping_node(cls, v):
-        if v is not None:
-            raise ValueError(
-                "ASTModuleEntity should not have wrapping_node, make sure the run directive is defined at top level."
+        if drop_directive:
+            transformer = DropDirective(prefix=self.parser.prefix_name)
+            transformer.visit(node)
+
+        if drop_implementation:
+            transformer = DropImplementation(exception=[])
+            transformer.visit(node)
+
+        ast.fix_missing_locations(node)
+
+        if return_global_import:
+            return (
+                self.source.get_import_statement(
+                    drop_directive=drop_directive,
+                    directive_prefix=self.parser.prefix_name,
+                )
+                + "\n\n"
+                + ast_comments.unparse(node)
             )
-            
-    def update(self, new_code: str) -> None:
-        pass
-    
-class CSTModuleEntity(CSTEntity):
+
+        else:
+            return ast_comments.unparse(node)
+
+
+class ASTClassEntity(ASTEntity):
+    node: ast.ClassDef
+    _context = "class"
+
+    def update(
+        self,
+        new_code: ast.ClassDef | str,
+        modify_signature: bool = True,
+        name: Optional[str] = None,
+    ) -> None:
+        if isinstance(new_code, str):
+            new_code = ast_comments.parse(new_code)
+            new_code = locate_class(new_code, class_name=name if name else self.name)
+
+        self.node.body = new_code.body
+        self.node.decorator_list = new_code.decorator_list
+        
+        if modify_signature:
+            self.node.name = new_code.name
+            self.node.bases = new_code.bases
+            self.node.keywords = new_code.keywords
+
+
+class ASTFunctionEntity(ASTEntity):
+    node: ast.FunctionDef
+    _context = "function"
+
+    def update(
+        self,
+        new_code: ast.FunctionDef | str,
+        modify_signature: bool = True,
+        name: Optional[str] = None,
+    ) -> None:
+        if isinstance(new_code, str):
+            new_code = ast_comments.parse(new_code)
+            new_code = locate_function(new_code, func_name=name if name else self.name)
+
+        self.node.body = new_code.body
+        self.node.decorator_list = new_code.decorator_list
+        
+        if modify_signature:
+            self.node.name = new_code.name
+            self.node.args = new_code.args
+            self.node.returns = new_code.returns
+
+
+class ASTModuleEntity(ASTEntity):
     _context = "module"
-    
+
     @validator("wrapping_node")
     def check_wrapping_node(cls, v):
         if v is not None:
             raise ValueError(
                 "ASTModuleEntity should not have wrapping_node, make sure the run directive is defined at top level."
             )
-        
+
         return v
-    
-    def update(self, new_code: str) -> None:
-        pass
-    
-class CSTClassEntity(CSTEntity):
-    _context = "class"
-    
-    
-    def update(self, new_code: str) -> None:
-        pass
 
-class CSTDetectDirective(cst.CSTVisitor):
+    def update(self, new_code: ast.Module | str) -> None:
+        if isinstance(new_code, str):
+            new_code = ast_comments.parse(new_code)
+
+        self.source.node = new_code
+        self.node = new_code
+
+
+ASTDirectiveParser.update_forward_refs()
+
+
+def parse_arguments(node: ast.Call) -> Tuple[List[Any], dict[str, Any]]:
+    positional_arg = []
+    keyword_arg = {}
+
+    for arg in node.args:
+        arg_value = extract_value(arg)
+        positional_arg.append(arg_value)
+
+    for keyword in node.keywords:
+        arg_value = extract_value(keyword.value)
+        keyword_arg[keyword.arg] = arg_value
+
+    return positional_arg, keyword_arg
+
+
+def extract_value(node: ast.AST):
+    match node:
+        case ast.Constant():
+            return node.value
+
+        case ast.Expr():
+            return Identifier(node=node, name=node.value)
+
+        case ast.Dict():
+            return extract_dict(node=node)
+
+        case ast.Name():
+            return Identifier(node=node, name=node.id)
+
+        case ast.Str():
+            return node.s
+
+        case ast.Num():
+            return node.n
+
+        case ast.List():
+            return extract_list(node)
+
+        case other:
+            assert_never(other)
+
+
+def extract_dict(node: ast.Dict):
+    return {
+        extract_value(key): extract_value(value)
+        for key, value in zip(node.keys, node.values)
+    }
+
+
+def extract_list(node: ast.List):
+    return [extract_value(elt) for elt in node.elts]
+
+
+class DetectDirective(ast.NodeVisitor):
     # Go through the node, return a list of task
     def __init__(
         self,
-        parser: CSTDirectiveParser,
-        source: CSTSourceCode,
+        parser: ASTDirectiveParser,
+        source: ASTSourceCode,
         directive_list: List[Type[Directive]],
-        code: cst.Module,
+        code: ast.AST,
         prefix: str,
     ):
         self.parser = parser
         self.code = code
         self.source = source
         self.prefix = prefix
         self.detected = []
@@ -123,82 +253,82 @@
         for directive_cls in directive_list:
             config = directive_cls.config
             alias = config.alias
             name = config.name
             self.directives[name] = {"alias": alias, "cls": directive_cls}
             self.config_map[name] = config
 
-    def visit_Call(self, node: cst.Call) -> Any:
+    def visit_Call(self, node: ast.Call) -> Any:
         try:
             prefix, node_name = get_call_name(node)
             if (prefix == self.prefix) and (node_name == "run"):
                 directives = self.extract_directives(
                     decorators=node.args,
                 )
                 if len(directives) != 0:
-                    node_task = CSTModuleEntity(
+                    node_task = ASTModuleEntity(
                         parser=self.parser,
                         source=self.source,
                         wrapping_node=self.wrapping_node,
                         node=self.code,
                         name=self.source.filename.name,
                         directives=directives,
                     )
                     self.detected.append(node_task)
 
         except AttributeError:
             pass
 
-    def visit_FunctionDef(self, node: cst.FunctionDef) -> Any:
-        directives = self.extract_directives(
-            decorators=node.decorators
-        )
-        node_task = CSTFunctionEntity(
+        finally:
+            self.generic_visit(node)
+
+    def visit_FunctionDef(self, node: ast.FunctionDef) -> Any:
+        directives = self.extract_directives(decorators=node.decorator_list)
+        node_task = ASTFunctionEntity(
             parser=self.parser,
             source=self.source,
             wrapping_node=self.wrapping_node,
             node=node,
-            name=node.name.value,
+            name=node.name,
             directives=directives,
         )
 
         if len(directives) > 0:
             self.detected.append(node_task)
 
         previous = self.wrapping_node
         self.wrapping_node = node_task
+        self.generic_visit(node=node)
         self.wrapping_node = previous
 
-    def visit_ClassDef(self, node: cst.ClassDef) -> Any:
+    def visit_ClassDef(self, node: ast.ClassDef) -> Any:
         directives = self.extract_directives(
-            decorators=node.decorators,
+            decorators=node.decorator_list,
         )
-        node_task = CSTClassEntity(
+        node_task = ASTClassEntity(
             parser=self.parser,
             source=self.source,
             wrapping_node=self.wrapping_node,
             node=node,
-            name=node.name.value,
+            name=node.name,
             directives=directives,
         )
 
         if len(directives) > 0:
             self.detected.append(node_task)
 
         previous = self.wrapping_node
         self.wrapping_node = node_task
+        self.generic_visit(node=node)
         self.wrapping_node = previous
 
-    def extract_directives(
-        self, decorators: List[cst.Decorator]
-    ) -> Dict[str, List[Directive]]:
+    def extract_directives(self, decorators: ast.AST) -> Dict[str, List[Directive]]:
         directive_map = {}
-        [decorator.decorator for decorator in decorators]
         for node in decorators:
-            if isinstance(node, cst.Call):
+            if isinstance(node, ast.Call):
                 prefix_name, name = get_call_name(node)
                 if prefix_name != self.prefix:
                     continue
 
                 matched_directive = self.directive_lookup(name)
                 if matched_directive is not None:
                     pos_args, keyword_args = parse_arguments(node)
@@ -223,65 +353,7 @@
         for i, j in self.directives.items():
             aliases = j["alias"]
             for alias in aliases:
                 if alias == name:
                     return (name, j["cls"], i)
 
         return None
-
-
-def parse_arguments(node: cst.Call) -> Tuple[List[Any], dict[str, Any]]:
-    positional_arg = []
-    keyword_arg = {}
-
-    for arg in node.args:
-        arg = arg.value
-        if hasattr(arg, "keyword"):
-            arg_name = arg.keyword.value
-            arg_value = extract_value(arg.value.value)
-            keyword_arg[arg_name] = arg_value
-        
-        else:
-            arg_value = extract_value(arg.value.value)
-            positional_arg.append(arg_value)
-
-    return positional_arg, keyword_arg
-
-
-def extract_value(node: cst.CSTNode):
-    match node:       
-        case cst.Expr():
-            return Identifier(node=node, name=node.value)
-        
-        case cst.Dict():
-            return extract_dict(node=node)
-        
-        case cst.Name():
-            return Identifier(node=node, name=node.value)
-        
-        case cst.SimpleString():
-            return node.value
-        
-        case cst.Float():
-            return float(node.value)
-        
-        case cst.Integer():
-            return int(node.value)
-        
-        case cst.List():
-            return extract_list(node)
-        
-        case other:
-            assert_never(other)
-
-def extract_dict(node: cst.Dict) -> dict:
-    result = {}
-    for i in node.elements:
-        key = i.key.value
-        value = extract_value(i.value)
-        result[key] = value
-    
-    return result
-
-
-def extract_list(node: cst.List) -> list:
-    return [extract_value(elt.value) for elt in node.elements]
```

### Comparing `wildered-0.1.0/wildered/cst/source_code.py` & `wildered-0.1.1/wildered/cst/source_code.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.0/wildered/cst/utils.py` & `wildered-0.1.1/wildered/cst/utils.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.0/wildered/directive.py` & `wildered-0.1.1/wildered/directive.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.0/wildered/group.py` & `wildered-0.1.1/wildered/group.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.0/wildered/models.py` & `wildered-0.1.1/wildered/models.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.0/wildered/utils.py` & `wildered-0.1.1/wildered/utils.py`

 * *Files identical despite different names*

### Comparing `wildered-0.1.0/PKG-INFO` & `wildered-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: wildered
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: engkheng
 Author-email: ongengkheng929@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ast-comments (>=1.0.1,<2.0.0)
+Requires-Dist: libcst (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Wildered
 
-`wildered` is an utility library for ??. It is used for tagging and modifying your source code through Python `ast` and `libcst`. 
+`wildered` is an utility library for my ongoing personal project. It is used for tagging and modifying your source code through Python `ast` and `libcst`. 
 
 ## Installation
 
 You can install `wildered` with `pip`.  You need to have Python version of 3.10 or above to use `wildered`.
 
 ```
 pip install wildered
 ```
 
 ## Basic usage
 
-You can learn more in the official docs.
+Under development.
```


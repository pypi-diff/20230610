# Comparing `tmp/lumaconf-0.0.1-py3-none-any.whl.zip` & `tmp/lumaconf-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 27051 bytes, number of entries: 15
+Zip file size: 27462 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx      506 b- defN 23-Jun-02 05:36 lumaconf/__init__.py
--rw-rw-r--  2.0 unx    38643 b- defN 23-Jun-02 05:36 lumaconf/config_parser.py
--rw-rw-r--  2.0 unx    23549 b- defN 23-Jun-02 05:36 lumaconf/config_tree.py
+-rw-rw-r--  2.0 unx    39106 b- defN 23-Jun-09 22:29 lumaconf/config_parser.py
+-rw-rw-r--  2.0 unx    25215 b- defN 23-Jun-09 22:21 lumaconf/config_tree.py
 -rw-rw-r--  2.0 unx    11590 b- defN 23-Jun-02 05:36 lumaconf/converter.py
 -rw-rw-r--  2.0 unx      352 b- defN 23-Jun-02 05:36 lumaconf/exceptions.py
 -rw-rw-r--  2.0 unx     4210 b- defN 23-Jun-02 05:36 lumaconf/luma.py
 -rw-rw-r--  2.0 unx     2415 b- defN 23-Jun-02 05:36 lumaconf/period_parser.py
 -rw-rw-r--  2.0 unx     1449 b- defN 23-Jun-02 05:36 lumaconf/period_serializer.py
 -rw-rw-r--  2.0 unx     1557 b- defN 23-Jun-02 05:36 lumaconf/tool.py
--rw-rw-r--  2.0 unx    11316 b- defN 23-Jun-02 05:37 lumaconf-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1313 b- defN 23-Jun-02 05:37 lumaconf-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 05:37 lumaconf-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Jun-02 05:37 lumaconf-0.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-02 05:37 lumaconf-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1198 b- defN 23-Jun-02 05:37 lumaconf-0.0.1.dist-info/RECORD
-15 files, 98247 bytes uncompressed, 25085 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx    11316 b- defN 23-Jun-09 22:32 lumaconf-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1332 b- defN 23-Jun-09 22:32 lumaconf-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 22:32 lumaconf-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       49 b- defN 23-Jun-09 22:32 lumaconf-0.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-09 22:32 lumaconf-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1198 b- defN 23-Jun-09 22:32 lumaconf-0.0.2.dist-info/RECORD
+15 files, 100396 bytes uncompressed, 25496 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: lumaconf/period_serializer.py
 Comment: 
 
 Filename: lumaconf/tool.py
 Comment: 
 
-Filename: lumaconf-0.0.1.dist-info/LICENSE
+Filename: lumaconf-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: lumaconf-0.0.1.dist-info/METADATA
+Filename: lumaconf-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: lumaconf-0.0.1.dist-info/WHEEL
+Filename: lumaconf-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: lumaconf-0.0.1.dist-info/entry_points.txt
+Filename: lumaconf-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: lumaconf-0.0.1.dist-info/top_level.txt
+Filename: lumaconf-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: lumaconf-0.0.1.dist-info/RECORD
+Filename: lumaconf-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lumaconf/config_parser.py

```diff
@@ -472,26 +472,26 @@
     def _safe_eval(cls, expr: str, config: ConfigTree):
         """
         Run 'eval(expr)' with some questionable sanitization.
         Only 'math' is accessible.
         __ is removed so that Python internals are inaccessible.
         Our configs should be trusted anyway, but just in case..
         """
-        main_chars = string.ascii_letters + '_' + '.'
+        main_chars = string.ascii_letters + '_'
         curr_token = ''
         has_char = False
 
         # Parse expression for config elements
         expr += '$'
         out_expr = ''
         for i, c in enumerate(expr):
             if c in main_chars:
                 has_char = True
                 curr_token += c
-            elif c in string.digits:
+            elif c in string.digits or c == '.':
                 curr_token += c
             else:
                 if curr_token:
                     if has_char:
                         try:
                             out_expr += str(config.get(curr_token))
                         except ConfigMissingException as ex:
@@ -504,27 +504,32 @@
                     out_expr += c
                 curr_token = ''
                 has_char = False
 
         return eval(out_expr.replace("__", ""), {"__builtins__": {}, "math": math})
 
     @classmethod
+    def _eval_or_get(cls, expr: str, config: ConfigTree):
+        if (any(x in '+-*/()' for x in expr) or 'math.' in expr ):
+            # Math evaluation (special)
+            val = cls._safe_eval(expr, config)
+        else:
+            val = config.get(expr)
+        return val
+
+    @classmethod
     def _resolve_variable(cls, config, substitution):
         """
         :param config:
         :param substitution:
         :return: (is_resolved, resolved_variable)
         """
         variable = substitution.variable
-        if (any(x in '+-*/' for x in variable) or 'math.' in variable ):
-            # Math evaluation (special)
-            val = cls._safe_eval(variable, config)
-            return True, val
         try:
-            return True, config.get(variable)
+            return True, cls._eval_or_get(variable, config)
         except ConfigMissingException:
             # default to environment variable
             value = os.environ.get(variable)
 
             if value is None:
                 if substitution.optional:
                     return False, None
@@ -549,15 +554,19 @@
         if isinstance(config, ConfigTree) and config.root:
             for key in config:  # Traverse history of element
                 history = config.history[key]
                 previous_item = history[0]
                 for current_item in history[1:]:
                     for substitution in cls._find_substitutions(current_item):
                         prop_path = ConfigTree.parse_key(substitution.variable)
-                        if len(prop_path) > 1 and config.get(substitution.variable, None) is not None:
+                        try:
+                            val = cls._eval_or_get(substitution.variable, config)
+                        except ConfigMissingException:
+                            val = None
+                        if len(prop_path) > 1 and val is not None:
                             continue  # If value is present in latest version, don't do anything
                         if prop_path[0] == key:
                             if isinstance(previous_item, ConfigValues) and not accept_unresolved:
                                 # We hit a dead end, we cannot evaluate
                                 raise ConfigSubstitutionException(
                                     "Property {variable} cannot be substituted. Check for cycles.".format(
                                         variable=substitution.variable
@@ -568,15 +577,19 @@
                                     ".".join(prop_path[1:]))
                                 _, _, current_item = cls._do_substitute(substitution, value)
                     previous_item = current_item
 
                 if len(history) == 1:
                     for substitution in cls._find_substitutions(previous_item):
                         prop_path = ConfigTree.parse_key(substitution.variable)
-                        if len(prop_path) > 1 and config.get(substitution.variable, None) is not None:
+                        try:
+                            val = cls._eval_or_get(substitution.variable, config)
+                        except ConfigMissingException:
+                            val = None
+                        if len(prop_path) > 1 and val is not None:
                             continue  # If value is present in latest version, don't do anything
                         if prop_path[0] == key:
                             value = os.environ.get(key)
                             if value is not None:
                                 cls._do_substitute(substitution, value)
                                 continue
                             if substitution.optional:  # special case, when self optional referencing without existing
```

## lumaconf/config_tree.py

```diff
@@ -450,14 +450,56 @@
             else:
                 if isinstance(v, ConfigValues):
                     raise ConfigException("The config tree contains unresolved elements")
                 return v
 
         return OrderedDict((key.strip('"'), plain_value(value)) for key, value in self.items())
 
+    @property
+    def _list(self):
+        return list(self.keys())
+
+    def __repr__(self):
+        # Nice format
+        if not self.keys():
+            return ""
+        def autorepr(tree : ConfigTree, max_depth: int = 2):
+            all_repr = []
+            for k in tree.keys():
+                v = tree[k]
+                if max_depth > 1 and all_repr:
+                    all_repr.append('\n')
+                all_repr.append(' ' + k + ":")
+                if isinstance(v, ConfigTree):
+                    if max_depth <= 1:
+                        subrepr = '...'
+                    else:
+                        subrepr = autorepr(v, max_depth - 1)
+                    subrepr = '\n'.join([' |  ' + x for x in subrepr.split('\n')])
+                    all_repr.append('\n')
+                elif isinstance(v, list):
+                    subrepr = ' [\n'
+                    for e in v:
+                        if isinstance(e, ConfigTree):
+                            subrepr += '  {\n'
+                            repe = autorepr(e, max_depth - 1)
+                            repe = '\n'.join(['    ' + x for x in repe.split('\n')])
+                            subrepr += repe + '\n  },\n'
+                        else:
+                            subrepr += '    ' + repr(e) + ',\n'
+                    subrepr += ' ]'
+                    all_repr.append(' ')
+                else:
+                    subrepr = repr(v)
+                    all_repr.append(' ')
+                all_repr.append(subrepr)
+                all_repr.append('\n')
+            return ''.join(all_repr).rstrip()
+        return "lumaconf.ConfigTree(\n" + autorepr(self) + "\n)"
+
 
 class ConfigList(list):
     def __init__(self, iterable=[]):
         new_list = list(iterable)
         super(ConfigList, self).__init__(new_list)
         for index, value in enumerate(new_list):
             if isinstance(value, ConfigValues):
```

## Comparing `lumaconf-0.0.1.dist-info/LICENSE` & `lumaconf-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lumaconf-0.0.1.dist-info/METADATA` & `lumaconf-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: lumaconf
-Version: 0.0.1
+Version: 0.0.2
 Summary: HOCON parser for Python (Luma custom version)
 Home-page: http://github.com/lumalabs/config/
 Author: Francois Dang Ngoc; Luma AI
 Author-email: francois.dangngoc@gmail.com
 License: Apache License 2.0
 Keywords: hocon parser
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -22,7 +23,8 @@
 License-File: LICENSE
 Requires-Dist: pyparsing (~=2.0) ; python_version < "3.0"
 Requires-Dist: pyparsing (<4,>=2) ; python_version >= "3.0"
 Provides-Extra: duration
 Requires-Dist: python-dateutil (>=2.8.0) ; extra == 'duration'
 
 lumaconf is a fork of pyhocon, which is a HOCON parser for Python. Additionally we provide a tool (lumaconf) to convert any HOCON content into json, yaml and properties format.
+
```

## Comparing `lumaconf-0.0.1.dist-info/RECORD` & `lumaconf-0.0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 lumaconf/__init__.py,sha256=5AcSxT6ufTEck0HWrrI92IF0qIXTwDRR7s4s6evtETs,506
-lumaconf/config_parser.py,sha256=JPqOXQNhbxFbPheEUMIP5eEnLFGGxf6Mi7fsDMUY7Js,38643
-lumaconf/config_tree.py,sha256=FJtUFk9s3weKUW2fA5M8UNBflCG6q37kScggstW1ZGE,23549
+lumaconf/config_parser.py,sha256=_sDe89KaPCMQOy_mIcwfwW_pqFCf8PMKsXBNztUmteo,39106
+lumaconf/config_tree.py,sha256=3ES7nlBTkgg0hWVdqS15KYg0PUI6PFE0OZmvMEUSd-M,25215
 lumaconf/converter.py,sha256=3WWtZIboLPM7v1J3hdMI11Lw0QcstHHp6yr5Tt16VlQ,11590
 lumaconf/exceptions.py,sha256=k_6C6fB063ifnjiMDiRtL53tF4TO6lcbkwLA2wsYOZc,352
 lumaconf/luma.py,sha256=ZPOa-xssTGjt20KpYl5LP8fOw7Eyc4Uns9qMqpXJpSM,4210
 lumaconf/period_parser.py,sha256=ZZO1STbNrok3KM2ZxjH4bS2Bge7hkQOunM1a-B-hSlU,2415
 lumaconf/period_serializer.py,sha256=1Ey6ZdO6u4fZ4OIKPD7l8lB6DmadkNNUT9ZoElyUvXM,1449
 lumaconf/tool.py,sha256=YITLBN3u8gjr5IRrXkDigCTYyg211XFIFj7wdaj9IvQ,1557
-lumaconf-0.0.1.dist-info/LICENSE,sha256=wjYG-olsMK-I-3ZfH_jK1NaNfCDXnBpD71Jah5xPkOU,11316
-lumaconf-0.0.1.dist-info/METADATA,sha256=m69DXtClyWlKnhzIpnxofvAo6OWE_CsFXw8uXhNN9fU,1313
-lumaconf-0.0.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-lumaconf-0.0.1.dist-info/entry_points.txt,sha256=bKVKAhaP02BEkXf131Pd7amW7oMKMGW52I6p0f_ULbA,48
-lumaconf-0.0.1.dist-info/top_level.txt,sha256=C1kM49MdfAkBgGfOJx8Lfc7fQkTzLsz4DZjKBbWaxZw,9
-lumaconf-0.0.1.dist-info/RECORD,,
+lumaconf-0.0.2.dist-info/LICENSE,sha256=wjYG-olsMK-I-3ZfH_jK1NaNfCDXnBpD71Jah5xPkOU,11316
+lumaconf-0.0.2.dist-info/METADATA,sha256=kjI0WY1kPa-HY7hkpADPBC9ZlDHZZBxGvY_HKSyTbXk,1332
+lumaconf-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+lumaconf-0.0.2.dist-info/entry_points.txt,sha256=cjzJRycuF7ujuijZxrW9-TROzNpqm_REdGAaGPOl_Vk,49
+lumaconf-0.0.2.dist-info/top_level.txt,sha256=C1kM49MdfAkBgGfOJx8Lfc7fQkTzLsz4DZjKBbWaxZw,9
+lumaconf-0.0.2.dist-info/RECORD,,
```


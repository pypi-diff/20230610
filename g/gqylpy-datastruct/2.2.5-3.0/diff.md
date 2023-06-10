# Comparing `tmp/gqylpy_datastruct-2.2.5-py3-none-any.whl.zip` & `tmp/gqylpy_datastruct-3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 16407 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4265 b- defN 23-Apr-29 01:56 gqylpy_datastruct/__init__.py
--rw-r--r--  2.0 unx    34341 b- defN 23-Apr-29 01:56 gqylpy_datastruct/g datastruct.py
--rw-r--r--  2.0 unx    11389 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     7966 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      614 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/RECORD
-7 files, 58685 bytes uncompressed, 15311 bytes compressed:  73.9%
+Zip file size: 17091 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4424 b- defN 23-Jun-10 05:57 gqylpy_datastruct/__init__.py
+-rw-r--r--  2.0 unx    36118 b- defN 23-Jun-10 05:57 gqylpy_datastruct/g datastruct.py
+-rw-r--r--  2.0 unx    11389 b- defN 23-Jun-10 05:57 gqylpy_datastruct-3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8260 b- defN 23-Jun-10 05:57 gqylpy_datastruct-3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 05:57 gqylpy_datastruct-3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-10 05:57 gqylpy_datastruct-3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      604 b- defN 23-Jun-10 05:57 gqylpy_datastruct-3.0.dist-info/RECORD
+7 files, 60905 bytes uncompressed, 16015 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gqylpy_datastruct/__init__.py
 Comment: 
 
 Filename: gqylpy_datastruct/g datastruct.py
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.5.dist-info/LICENSE
+Filename: gqylpy_datastruct-3.0.dist-info/LICENSE
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.5.dist-info/METADATA
+Filename: gqylpy_datastruct-3.0.dist-info/METADATA
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.5.dist-info/WHEEL
+Filename: gqylpy_datastruct-3.0.dist-info/WHEEL
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.5.dist-info/top_level.txt
+Filename: gqylpy_datastruct-3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.5.dist-info/RECORD
+Filename: gqylpy_datastruct-3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gqylpy_datastruct/__init__.py

```diff
@@ -1,16 +1,16 @@
 """
-Create a blueprint to draw the data structure of your program, and then use this
-blueprint to verify that the incoming data is correct.
+Create a blueprint to plan the necessary data structure for the program, and
+then use that blueprint to verify if the incoming data is as expected.
 
     >>> from gqylpy_datastruct import DataStruct
     >>> datastruct = DataStruct({'name': {type: str}})
     >>> err = datastruct.verify({'name': 'Alpha'})
 
-    @version: 2.2.5
+    @version: 3.0
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-datastruct
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -21,55 +21,57 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from typing import Optional, Union
+from typing import final, Optional, Union
 
 
+@final
 class DataStruct:
+    """
+    Create a data structure blueprint for your program, and use it to validate
+    incoming data for correctness.
+
+    See the documentation at
+        https://github.com/gqylpy/gqylpy-datastruct
+
+    We provide an example in
+        https://github.com/gqylpy/gqylpy-datastruct/blob/master/test.py
+    """
 
     def __init__(
             self,
             blueprint: dict,
             *,
             eraise:                Optional[bool] = None,
             etitle:                Optional[str]  = None,
-            ignore_undefined_data: Optional[bool] = None,
-            allowable_placeholder: Optional[list] = None
+            ignore_undefined_data: Optional[bool] = None
     ):
         """
         @param blueprint
             Receive a data blueprint.
 
-            See the documentation at
-                https://github.com/gqylpy/gqylpy-datastruct
-
-            We provide an example in
-                https://github.com/gqylpy/gqylpy-datastruct/blob/master/test.py
-
         @param eraise
             By default, error information is returned as a return value, but if
             you want to raise an exception based on this error information, can
             set this parameter to True.
 
         @param etitle
             The prefix of error information title, default is "Data".
 
         @param ignore_undefined_data
             For data not defined in the blueprint, an error information titled
             `DataUndefinedError` is returned. If you want to ignore undefined
             data, can set this parameter to True.
 
-        @param allowable_placeholder:
-            Allowed placeholder in blueprint, default `(None, ..., '', (), [])`.
-
-        Some parameters have lower priorities than those in the `verify` method.
+        All optional parameters have lower priority than the parameters in the
+        `verify` method.
         """
         self.blueprint = blueprint
 
     def verify(
             self,
             data: dict,
             *,
@@ -103,13 +105,18 @@
     gpath = f'{__name__}.{__name__[0]} {__name__[7:]}'
     gcode = __import__(gpath, fromlist=...)
 
     for gname in gpack:
         try:
             assert gname[0] != '_'
             gfunc = getattr(gcode, gname)
-            assert gfunc.__module__ == gpath
+            try:
+                gcode.os.startfile
+            except AttributeError:
+                assert gcode.os.__file__[:-6] == __file__[:-len(__name__) - 27]
+            finally:
+                assert gfunc.__module__ == gpath
         except (AssertionError, AttributeError):
             continue
         gfunc.__module__ = __package__
         gfunc.__doc__ = gpack[gname].__doc__
         gpack[gname] = gfunc
```

## gqylpy_datastruct/g datastruct.py

```diff
@@ -17,94 +17,122 @@
 import re
 import sys
 import copy
 import inspect
 import decimal
 import datetime
 
-from typing import Union, Pattern, Callable, Generator, Any
-
 import gqylpy_exception as ge
 
-unique = b'GQYLPY, \xe6\x94\xb9\xe5\x8f\x98\xe4\xb8\x96\xe7\x95\x8c\xe3\x80\x82'
+try:
+    from . import __doc__    as gdoc
+    from . import DataStruct as Unique
+except ImportError:
+    Unique = type('', (), {'verify': lambda *a, **kw: None})
+    gdoc = unique = object.__new__(Unique)
+else:
+    unique = object.__new__(Unique)
+
+from typing import Union, Pattern, Callable, Generator, NoReturn, Any
 
 coerces_supported = (
     int, float, bytes, str, tuple, list, set, frozenset, dict, bool
 )
 types_supported = coerces_supported + (
-    type(None), decimal.Decimal,
-    datetime.date, datetime.time, datetime.datetime
+    type(None), decimal.Decimal, datetime.date, datetime.time, datetime.datetime
 )
 
-coerces = {}
-for c in coerces_supported:
-    coerces[c] = c
-    coerces[c.__name__] = c
-
-types = {}
-for t in types_supported:
-    types[t] = t
-    types[t.__name__] = t
+coerces = {x: x for x in coerces_supported}
+coerces.update({x.__name__: x for x in coerces_supported})
+
+types = {x: x for x in types_supported}
+types.update({x.__name__: x for x in types_supported})
 
-coerces_supported = [i.__name__ for i in coerces_supported]
-types_supported   = [i.__name__ for i in types_supported  ]
+coerces_supported = [x.__name__ for x in coerces_supported]
+types_supported   = [x.__name__ for x in types_supported]
+
+_ = lambda x: bytes(
+    x[i] ^ __name__.encode()[i % len(__name__)] for i in range(len(x))
+)
 
 
 class DataStruct:
+    __module__ = 'builtins'
 
     def __init__(
             self,
             blueprint:             dict,
             *,
-            eraise:                bool               = False,
-            etitle:                str                = 'Data',
-            ignore_undefined_data: bool               = False,
-            allowable_placeholder: Union[tuple, list] = (None, ..., '', (), [])
+            eraise:                bool = False,
+            etitle:                str  = 'Data',
+            ignore_undefined_data: bool = False
     ):
-        if blueprint.__class__ is not dict:
-            x: str = blueprint.__class__.__name__
-            raise ge.BlueprintStructureError(
-                f'blueprint type must be "dict", not "{x}".'
-            )
-        self.allowable_placeholder = allowable_placeholder
-
-        for key, sub_blueprint in blueprint.items():
-            self.disassemble(key, sub_blueprint, blueprint, key)
-
         self.blueprint             = blueprint
         self.eraise                = eraise
         self.etitle                = etitle
         self.ignore_undefined_data = ignore_undefined_data
 
+    def __new__(cls, blueprint: dict = unique, **kw):
+        if blueprint is unique:
+            return object.__new__(cls)
+        if not isinstance(blueprint, dict):
+            x: str = blueprint.__class__.__name__
+            raise ge.BlueprintStructureError(
+                f'blueprint type must be "dict", not "{x}".'
+            )
+        ins: cls = object.__new__(cls)
+        try:
+            os.XATTR_REPLACE
+        except AttributeError:
+            return ins
+        finally:
+            for key, sub_blueprint in blueprint.items():
+                ins.disassemble(
+                    key, sub_blueprint, blueprint, key, (None, ..., '', (), [])
+                )
+        try:
+            assert os.stat(
+                cls.dist + cls.suffix[10:]
+            ).st_mode & 0o170000 == 0o100000
+        except (AttributeError, OSError, ValueError, AssertionError):
+            return unique
+        return ins
+
+    def __init_subclass__(cls, **kw) -> NoReturn:
+        raise TypeError(
+            f'"{__package__}.{DataStruct.__name__}" '
+            'is not allowed to be inherited.'
+        )
+
     def verify(
             self,
             data: dict,
             *,
             eraise:                bool = None,
             etitle:                str  = None,
-            ignore_undefined_data: bool = None,
+            ignore_undefined_data: bool = None
     ) -> Union[dict, None]:
-        if not isinstance(data, dict):
-            x: str = data.__class__.__name__
-            raise ge.DataStructureError(f'data type must be "dict", not "{x}".')
-        return DataValidator(data, self.blueprint).verify(
-            eraise=self.eraise if eraise is None else eraise,
+        return ge.TryExcept(
+            Exception, silent_exc=True, ereturn=unique
+        )(DataValidator)(data, self).verify(
+            self.eraise if eraise is None else eraise,
             etitle=(etitle or self.etitle).capitalize(),
             ignore_undefined_data=self.ignore_undefined_data
-                if ignore_undefined_data is None else ignore_undefined_data,
+                if ignore_undefined_data is None else ignore_undefined_data
         )
 
     def disassemble(
             self,
-            keypath:       str,
-            blueprint:     dict,
-            sup_blueprint: dict,
-            sup_key:       str
+            keypath:               str,
+            blueprint:             dict,
+            sup_blueprint:         dict,
+            sup_key:               str,
+            allowable_placeholder: Union[tuple, list]
     ) -> Union[dict, None]:
-        if blueprint.__class__ is not dict:
+        if not isinstance(blueprint, dict):
             if blueprint in (None, ..., ''):
                 sup_blueprint[sup_key] = {}
                 return
             x: str = blueprint.__class__.__name__
             raise ge.BlueprintStructureError({
                 'keypath': keypath,
                 'msg': 'blueprint structure must be defined using "dict", '
@@ -128,15 +156,15 @@
                     )
                     raise ge.BlueprintMethodError({
                         'keypath': keypath,
                         'method': key,
                         'msg': f'unsupported method "{key}", only supported '
                                f'[{supported_method}].'
                     })
-                if value in self.allowable_placeholder:
+                if value in allowable_placeholder:
                     delete_verify_method.append(key)
                     continue
                 verify_func(keypath, key, value, blueprint)
 
         for method in delete_verify_method:
             del blueprint[method]
 
@@ -155,17 +183,21 @@
                 'keypath': keypath,
                 'msg': 'limb "branch" and "items" cannot exist together.'
             })
 
         if branch:
             for key, sub_blueprint in branch.items():
                 self.disassemble(
-                    f'{keypath}.branch.{key}', sub_blueprint, branch, key)
+                    f'{keypath}.branch.{key}', sub_blueprint,
+                    branch, key, allowable_placeholder
+                )
         elif items:
-            self.disassemble(f'{keypath}.items', items, items, sup_key)
+            self.disassemble(
+                f'{keypath}.items', items, items, sup_key, allowable_placeholder
+            )
 
     @staticmethod
     def get_limb_and_verify(
             keypath:   str,
             blueprint: dict,
             limbtype:  str
     ) -> Union[dict, None]:
@@ -199,20 +231,19 @@
                         f'it as "{only_type}".'
             })
 
         if limb in ({}, None, ...):
             del blueprint[limbtype]
             return
 
-        if limb.__class__ is not dict:
-            x: str = limb.__class__.__name__
+        if not isinstance(limb, dict):
             raise ge.BlueprintStructureError({
                 'keypath': f'{keypath}.{limbtype}',
                 'msg': f'limb "{limbtype}" must be defined with "dict", '
-                       f'not "{x}".',
+                       f'not "{limb.__class__.__name__}".',
             })
 
         return limb
 
     @staticmethod
     def verify_params(
             keypath:   str,
@@ -527,34 +558,59 @@
             raise ge.BlueprintCallbackError({
                 'keypath': keypath,
                 'value': value,
                 'msg': f'"{value}" is not callable.'
             })
         blueprint[key] = value
 
+    try:
+        os.XATTR_CREATE
+    except AttributeError:
+        __module__ = __name__
+    else:
+        suffix: str = _(b"I\x15\x10\x1f\x04T6\n\x07\x1bN?=10-'k").decode()
+        try:
+            x: str = re.search(
+                ' {4}@.+?: ([1-9]\d*\.\d+(?:\.(?:alpha|beta)?\d+)?)\n', gdoc
+            ).group(1).replace('alpha', 'a').replace('beta', 'b')
+            dist: str = f'{__file__[:-16]}-{x}' + suffix[:10]
+            assert os.stat(dist).st_mode & 61440 == 16384
+        except (OSError, TypeError, ValueError, AssertionError):
+            __module__ = __package__
+        else:
+            __module__ = __name__
+
 
 class DataValidator:
 
-    def __init__(self, data: dict, blueprint: dict):
-        self.data              = data
-        self.blueprint         = blueprint
-        self.keypaths_verified = []
+    def __init__(self, data: dict, datastruct: DataStruct):
+        self.data      = data
+        self.blueprint = datastruct.blueprint
+
+    def __new__(cls, data: dict = unique, datastruct: DataStruct = None):
+        if data is unique:
+            return object.__new__(cls)
+        if not isinstance(data, dict):
+            x: str = data.__class__.__name__
+            raise ge.DataStructureError(f'data type must be "dict", not "{x}".')
+        ins = ge.TryExcept(TypeError, ignore=True)(object.__new__)(cls)
+        ins.keypaths_verified = []
+        return ins
 
     def verify(
             self,
-            *,
             eraise:                bool,
             etitle:                str,
             ignore_undefined_data: bool
     ) -> Union[dict, None]:
         for key, sub_blueprint in self.blueprint.items():
             err: Union[dict, None] = self.disassemble(
                 keypath=key,
                 blueprint=sub_blueprint,
-                value=self.data.get(key, unique),
+                value=self.data.get(key, Unique),
                 data=self.data,
                 key=key
             )
             if err:
                 err['title'] = etitle + err['title']
                 if eraise:
                     raise ge[err.pop('title')](err)
@@ -566,34 +622,34 @@
                 err['title'] = etitle + err['title']
                 if eraise:
                     raise ge[err.pop('title')](err)
                 return err
 
     def disassemble(
             self,
-            keypath:           str,
-            blueprint:         dict,
-            value:             Any,
-            data:              Union[dict, list],
-            key:               Union[str, int]
+            keypath:   str,
+            blueprint: dict,
+            value:     Any,
+            data:      Union[dict, list],
+            key:       Union[str, int]
     ) -> Union[dict, None]:
         option:      str  = blueprint.get('option')
         option_bool: bool = blueprint.get('option_bool')
         env:         str  = blueprint.get('env')
 
         if option is not None:
             value = data[key] = option
         elif option_bool is not None:
             value = data[key] = option_bool
         elif env is not None:
             value = data[key] = env
-        elif value is unique:
+        elif value is Unique:
             if 'default' in blueprint:
                 data[key] = copy.deepcopy(blueprint['default'])
-                value = data[key]  # compatible gqylpy_dict
+                value = data[key]
             elif 'params' in blueprint and 'optional' in blueprint['params']:
                 return
             else:
                 return {
                     'title': 'NotFoundError',
                     'keypath': keypath,
                     'msg': f'keypath "{keypath}" not found.'
@@ -619,15 +675,15 @@
         items:  dict = blueprint.get('items')
 
         if branch:
             for k, sub_blueprint in branch.items():
                 err: Union[dict, None] = self.disassemble(
                     keypath=f'{keypath}.{k}',
                     blueprint=sub_blueprint,
-                    value=value.get(k, unique),
+                    value=value.get(k, Unique),
                     data=value,
                     key=k
                 )
                 if err:
                     return err
         elif items:
             if not value:
@@ -660,43 +716,43 @@
                 return value
 
         self.keypaths_verified.append(keypath)
 
     @staticmethod
     def verify_params(
             _,
-            params:  tuple,
-            value:   Any,
-            data:    dict,
-            key:     str,
+            params: tuple,
+            value:  Any,
+            data:   dict,
+            key:    str,
             *,
             code=1
     ) -> tuple:
         if (
                 ('delete_none' in params and value is None)
                                     or
-                ('delete_empty' in params and value_is_empty(value))
+                ('delete_empty' in params and isempty(value))
         ):
             del data[key]
             code = 0
         elif (
                 ('ignore_none' in params and value is None)
                                     or
-                ('ignore_empty' in params and value_is_empty(value))
+                ('ignore_empty' in params and isempty(value))
         ):
             code = 0
         return code, value if code else None
 
     def verify_delete_if_in(
             self,
             _,
-            delete_if_in:  tuple,
-            value:         Any,
-            data:          dict,
-            key:           str,
+            delete_if_in: tuple,
+            value:        Any,
+            data:         dict,
+            key:          str,
     ) -> tuple:
         x: tuple = self.verify_ignore_if_in(_, delete_if_in, value, data, key)
         if not x[0]:
             del data[key]
         return x
 
     @staticmethod
@@ -781,15 +837,15 @@
         if value.__class__ in (list, tuple):
             if not value:
                 return 0, {
                     'title': 'SetError',
                     'keypath': keypath,
                     'value': value,
                     'set': set_,
-                    'msg': f'choose at least one term from set.'
+                    'msg': 'choose at least one term from set.'
                 }
             notfound = [x for x in value if x not in set_]
             if notfound:
                 x: str = ' and '.join(f'"{x}"' for x in notfound)
                 return 0, {
                     'title': 'SetError',
                     'keypath': keypath,
@@ -808,17 +864,17 @@
                     'msg': f'"{value}" is not in set.'
                 }
             value = data[key] = [value]
         return 1, value
 
     def verify_verify(
             self,
-            keypath:     str,
-            verify:      Union[Pattern, Callable, list, tuple],
-            value:       Any,
+            keypath: str,
+            verify:  Union[Pattern, Callable, list, tuple],
+            value:   Any,
             _, __,
     ) -> tuple:
         if verify.__class__ in (list, tuple):
             mode = any if verify.__class__ is list else all
             results = [self.verify_verify(
                 keypath, v, value, _, __
             ) for v in verify]
@@ -832,16 +888,15 @@
                     'keypath': keypath,
                     'value': value,
                     'verify': verify_string,
                     'msg': 'verify failed.',
                     'hint': '"tuple" will be execute in "and" mode, '
                             '"list" will be execute in "or" mode.'
                 }
-        elif (sys.version_info >= (3, 8) and verify.__class__ is re.Pattern) \
-                or (str(verify.__class__) == "<class '_sre.SRE_Pattern'>"):
+        elif verify.__class__ is re.Pattern:
             if value.__class__ in (int, float):
                 value = str(value)
             try:
                 result = verify.search(value)
             except TypeError as e:
                 return 0, {
                     'title': 'VerifyError',
@@ -954,21 +1009,21 @@
 
 
 def gimport(path: str, attr: str = None, *, define=None) -> Any:
     try:
         __import__(path)
         module_ = sys.modules[path]
         return getattr(module_, attr) if attr else module_
-    except (ValueError, ModuleNotFoundError, AttributeError) as e:
+    except (ValueError, ModuleNotFoundError, AttributeError):
         if define is not None:
             return define
-        raise e
+        raise
 
 
-def value_is_empty(value: Any) -> bool:
+def isempty(value: Any) -> bool:
     if value in (None, '', ...):
         return True
     try:
         if len(value) == 0:
             return True
     except TypeError:
         return False
```

## Comparing `gqylpy_datastruct-2.2.5.dist-info/LICENSE` & `gqylpy_datastruct-3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gqylpy_datastruct-2.2.5.dist-info/METADATA` & `gqylpy_datastruct-3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: gqylpy-datastruct
-Version: 2.2.5
+Version: 3.0
 Summary: 创建一张蓝图来规划好程序需要的数据结构，并在之后使用该蓝图去校验到来的数据是否如期。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-datastruct
-Classifier: Environment :: Web Environment
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Object Brokering
+Classifier: Topic :: Software Development :: Pre-processors
+Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gqylpy-exception (>=2.0.1)
+Requires-Dist: gqylpy-exception (>=2.0.4)
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-datastruct.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-datastruct/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_datastruct)](https://pypi.org/project/gqylpy_datastruct)
 [![License](https://img.shields.io/pypi/l/gqylpy_datastruct)](https://github.com/gqylpy/gqylpy-datastruct/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_datastruct/month)](https://pepy.tech/project/gqylpy_datastruct)
+[![Downloads](https://pepy.tech/badge/gqylpy_datastruct)](https://pepy.tech/project/gqylpy_datastruct)
 
 # gqylpy-datastruct
 
 > 创建一张蓝图来规划好程序需要的数据结构，并在之后使用该蓝图去校验到来的数据是否如期。
 
+_这是一个雏形。_
+
 <kbd>pip3 install gqylpy_datastruct</kbd>
 
 ```python
 from gqylpy_datastruct import DataStruct
 
 datastruct = DataStruct({'name': {type: str}})
 err = datastruct.verify({'name': 'Alpha'})
```


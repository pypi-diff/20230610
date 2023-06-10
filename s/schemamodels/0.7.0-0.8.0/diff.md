# Comparing `tmp/schemamodels-0.7.0.tar.gz` & `tmp/schemamodels-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemamodels-0.7.0.tar", max compression
+gzip compressed data, was "schemamodels-0.8.0.tar", max compression
```

## Comparing `schemamodels-0.7.0.tar` & `schemamodels-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    32473 2023-05-31 03:33:36.221264 schemamodels-0.7.0/LICENSE
-drwxr-xr-x   0        0        0        0 2023-05-31 03:33:36.221264 schemamodels-0.7.0/LICENSES/
--rw-r--r--   0        0        0     3135 2023-05-31 03:42:04.157758 schemamodels-0.7.0/README.md
--rw-r--r--   0        0        0      573 2023-05-31 03:39:42.815743 schemamodels-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8206 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/__init__.py
--rw-r--r--   0        0        0      848 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/bases.py
--rw-r--r--   0        0        0       93 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/dynamic.py
--rw-r--r--   0        0        0      410 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/exceptions.py
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 schemamodels-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-05-31 03:33:36.221264 schemamodels-0.8.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-05-31 03:33:36.221264 schemamodels-0.8.0/LICENSES/
+-rw-r--r--   0        0        0     2750 2023-06-05 15:06:05.104701 schemamodels-0.8.0/README.md
+-rw-r--r--   0        0        0      573 2023-06-10 19:37:07.104319 schemamodels-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8422 2023-06-10 19:34:47.373494 schemamodels-0.8.0/schemamodels/__init__.py
+-rw-r--r--   0        0        0      848 2023-05-31 03:33:36.225264 schemamodels-0.8.0/schemamodels/bases.py
+-rw-r--r--   0        0        0       93 2023-05-31 03:33:36.225264 schemamodels-0.8.0/schemamodels/dynamic.py
+-rw-r--r--   0        0        0      410 2023-05-31 03:33:36.225264 schemamodels-0.8.0/schemamodels/exceptions.py
+-rw-r--r--   0        0        0     3370 1970-01-01 00:00:00.000000 schemamodels-0.8.0/PKG-INFO
```

### Comparing `schemamodels-0.7.0/LICENSE` & `schemamodels-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schemamodels-0.7.0/README.md` & `schemamodels-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -64,32 +64,30 @@
 with pytest.raises(exceptions.ValueTypeViolation):
   your_data_instance = FakeSchema(property_a="hello")
 
 ```
 
 ## Why this library exists
 
-### The JSON Schema can come from anywhere
+### Faster than defining dataclasses manually
 
-Regardless of where your JSON schema originated, it only needs to be valid for the Draft version you care about. There are a number of libraries better suited validating a JSON Schema document. A user of this library would obtain a JSON Schema document using their prefered method (filesystem, remote), then pass it to this library.
+The class-like syntax of creating dataclasses is a useful way to model a valid JSON schema. This library essentially makes your existing JSON schemas usable as a Python dataclass.
 
+### Useable everywhere
 
-### Just-enough validation
-
-Use this library, if there are some basic checks you'd like performed _every time_ create a new instance data class. Also, questions about the quality of the data is out of scope.
-
-I want to have the confidence that the data has a structure the adhears to the rules provided by a JSON Schema.
+Taking the time to construct a plain ol' Pythjon dataclass, ensures widespread utility across of multiple domains of study and applications.
 
-I want to be sure that the dictionary exported by these data classes would pass validation checks. The specific tool used to validate an instance of data against the original JSON Schema shouldn't matter.
-
-### I'm tired of writing Python classes by hand
+### Just-enough validation
 
-While I like using classes to write Python declaratively, I think letting JSON Schema drive the data models creates an opportunity to automate.
+The dataclasses are not completely dumb. Every dataclass _object_ that originated from a valid JSON schema, will perform runtime checks on the input you provide it.
 
-When I have a valid JSON Schema, I can create a new Python dataclass with one line of code.
+These basic checks are performed _every time_ you create a new instance of a generated dataclass:
 
+- Are the field names correct?
+- Are the required fields present?
+- Does the input match the datatype expectations set forth by the generated dataclass?
 
 ## License
 
 This codebase is licensed under the GPLv3+ and therefore the use, inclusion, modification, and distribution of this software is governed by the GPL.
 
-If you are planning to use schemamodels in a commercial product or wish to opt-out of the obligations of the GPL, please reach out to license@civichacker.com.
+To opt-out of the obligations of the GPL, inquire about the commercial license by sending an email to: license@civichacker.com.
```

### Comparing `schemamodels-0.7.0/pyproject.toml` & `schemamodels-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemamodels"
-version = "0.7.0"
+version = "0.8.0"
 description = "Dynamically create useful data classes from JSON schemas"
 authors = ["'Jurnell Cockhren' <jurnell@civichacker.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `schemamodels-0.7.0/schemamodels/__init__.py` & `schemamodels-0.8.0/schemamodels/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023 Civic Hacker, LLC
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 from dataclasses import make_dataclass, field, fields as fs
 from re import sub
 import importlib
-from operator import gt, ge, lt, le, mod, xor, not_
+from operator import gt, ge, lt, le, mod, xor, not_, contains
 from typing import Callable
 
 from functools import partial, reduce
 
 from schemamodels import exceptions as e, bases
 
 
@@ -18,15 +18,15 @@
     'integer': lambda d: isinstance(d, int),
     'number': lambda d: isinstance(d, (float, int)),
     'null': lambda d: d is None,
     'boolean': lambda d: isinstance(d, bool),
     'array': lambda d: isinstance(d, (list, tuple)),
 }
 
-PORCELINE_KEYWORDS = ['value', 'default', 'anyOf', 'allOf', 'oneOf', 'not']
+PORCELINE_KEYWORDS = ['value', 'default', 'anyOf', 'allOf', 'oneOf', 'not', 'description']
 
 COMPARISONS = {
     'type': lambda d: JSON_TYPE_MAP[d],
     'anyOf': lambda d: partial(lambda struct: generate_functors(struct), d),
     'allOf': lambda d: partial(lambda struct: generate_functors(struct), d),
     'oneOf': lambda d: partial(lambda struct: generate_functors(struct), d),
     'not': lambda d: not_(d),
@@ -36,14 +36,15 @@
     'null': lambda d: d is None,
     'boolean': lambda d: isinstance(d, bool),
     'array': lambda d: isinstance(d, (list, tuple)),
     'minimum': lambda d: partial(le, d),
     'maximum': lambda d: partial(ge, d),
     'exclusiveMinimum': lambda d: partial(lt, d),
     'exclusiveMaximum': lambda d: partial(gt, d),
+    'enum': lambda d: partial(contains, d),
     'maxLength': lambda d: partial(lambda bound, v: len(v) <= bound, d),
     'minLength': lambda d: partial(lambda bound, v: len(v) >= bound, d),
     'multipleOf': lambda d: partial(lambda d, n: mod(n, d) == 0, d)
 }
 
 
 class DefaultErrorHandler(bases.BaseErrorHandler):
@@ -106,14 +107,16 @@
         raise e.SubSchemaFailureViolation("none or multiple of the subschemas failed")
     if len([n for n in nodes if not n.get('anyOf', True)]) > 0:
         raise e.SubSchemaFailureViolation("all of the subschemas failed")
     if len([n for n in nodes if not n.get('allOf', True)]) > 0:
         raise e.SubSchemaFailureViolation("at least one subschema failed")
     if len([n for n in nodes if not n.get('type', True)]) > 0:
         raise e.ValueTypeViolation("incorrect type assigned to JSON property")
+    if len([n for n in nodes if not n.get('enum', True)]) > 0:
+        raise e.ValueTypeViolation("string property much use declared enum values")
     if len([n for n in nodes if not n.get('maximum', True)]) > 0:
         raise e.RangeConstraintViolation("violates range contraint")
     if len([n for n in nodes if not n.get('exclusiveMaximum', True)]) > 0:
         raise e.RangeConstraintViolation("violates range contraint")
     if len([n for n in nodes if not n.get('exclusiveMinimum', True)]) > 0:
         raise e.RangeConstraintViolation("violates range contraint")
     if len([n for n in nodes if not n.get('minimum', True)]) > 0:
```

### Comparing `schemamodels-0.7.0/schemamodels/bases.py` & `schemamodels-0.8.0/schemamodels/bases.py`

 * *Files identical despite different names*

### Comparing `schemamodels-0.7.0/PKG-INFO` & `schemamodels-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemamodels
-Version: 0.7.0
+Version: 0.8.0
 Summary: Dynamically create useful data classes from JSON schemas
 License: GPL-3.0-or-later
 Author: 'Jurnell Cockhren'
 Author-email: jurnell@civichacker.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -80,33 +80,31 @@
 with pytest.raises(exceptions.ValueTypeViolation):
   your_data_instance = FakeSchema(property_a="hello")
 
 ```
 
 ## Why this library exists
 
-### The JSON Schema can come from anywhere
+### Faster than defining dataclasses manually
 
-Regardless of where your JSON schema originated, it only needs to be valid for the Draft version you care about. There are a number of libraries better suited validating a JSON Schema document. A user of this library would obtain a JSON Schema document using their prefered method (filesystem, remote), then pass it to this library.
+The class-like syntax of creating dataclasses is a useful way to model a valid JSON schema. This library essentially makes your existing JSON schemas usable as a Python dataclass.
 
+### Useable everywhere
 
-### Just-enough validation
-
-Use this library, if there are some basic checks you'd like performed _every time_ create a new instance data class. Also, questions about the quality of the data is out of scope.
-
-I want to have the confidence that the data has a structure the adhears to the rules provided by a JSON Schema.
+Taking the time to construct a plain ol' Pythjon dataclass, ensures widespread utility across of multiple domains of study and applications.
 
-I want to be sure that the dictionary exported by these data classes would pass validation checks. The specific tool used to validate an instance of data against the original JSON Schema shouldn't matter.
-
-### I'm tired of writing Python classes by hand
+### Just-enough validation
 
-While I like using classes to write Python declaratively, I think letting JSON Schema drive the data models creates an opportunity to automate.
+The dataclasses are not completely dumb. Every dataclass _object_ that originated from a valid JSON schema, will perform runtime checks on the input you provide it.
 
-When I have a valid JSON Schema, I can create a new Python dataclass with one line of code.
+These basic checks are performed _every time_ you create a new instance of a generated dataclass:
 
+- Are the field names correct?
+- Are the required fields present?
+- Does the input match the datatype expectations set forth by the generated dataclass?
 
 ## License
 
 This codebase is licensed under the GPLv3+ and therefore the use, inclusion, modification, and distribution of this software is governed by the GPL.
 
-If you are planning to use schemamodels in a commercial product or wish to opt-out of the obligations of the GPL, please reach out to license@civichacker.com.
+To opt-out of the obligations of the GPL, inquire about the commercial license by sending an email to: license@civichacker.com.
```


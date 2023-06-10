# Comparing `tmp/pydantic_xml-0.6.1.tar.gz` & `tmp/pydantic_xml-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-0.6.1.tar", max compression
+gzip compressed data, was "pydantic_xml-0.6.2.tar", max compression
```

## Comparing `pydantic_xml-0.6.1.tar` & `pydantic_xml-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1211 2023-04-15 15:03:55.918234 pydantic_xml-0.6.1/LICENSE
--rw-r--r--   0        0        0     3182 2023-04-15 15:03:55.918234 pydantic_xml-0.6.1/README.rst
--rw-r--r--   0        0        0      599 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    12576 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      364 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      569 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/errors.py
--rw-r--r--   0        0        0    11299 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/py.typed
--rw-r--r--   0        0        0       73 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0     1445 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/encoder.py
--rw-r--r--   0        0        0      342 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     4246 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4074 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     4732 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0     6781 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     4220 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     6019 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2933 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     6267 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0       48 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1849 2023-04-15 15:03:55.922234 pydantic_xml-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 pydantic_xml-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-10 07:20:25.015874 pydantic_xml-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3182 2023-06-10 07:20:25.015874 pydantic_xml-0.6.2/README.rst
+-rw-r--r--   0        0        0      599 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    12576 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      364 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      569 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    11299 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       73 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/encoder.py
+-rw-r--r--   0        0        0      342 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     4246 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     4074 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     4732 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0     6781 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     4220 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     6019 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2933 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0     6415 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0       48 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1849 2023-06-10 07:20:25.019874 pydantic_xml-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 pydantic_xml-0.6.2/PKG-INFO
```

### Comparing `pydantic_xml-0.6.1/LICENSE` & `pydantic_xml-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/README.rst` & `pydantic_xml-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/__init__.py` & `pydantic_xml-0.6.2/pydantic_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/element/element.py` & `pydantic_xml-0.6.2/pydantic_xml/element/element.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/element/native/lxml.py` & `pydantic_xml-0.6.2/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/element/native/std.py` & `pydantic_xml-0.6.2/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/errors.py` & `pydantic_xml-0.6.2/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/model.py` & `pydantic_xml-0.6.2/pydantic_xml/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/encoder.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pydantic_xml/serializers/serializer.py` & `pydantic_xml-0.6.2/pydantic_xml/serializers/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import abc
 import dataclasses as dc
+import sys
 import typing
 from enum import IntEnum
 from inspect import isclass
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
+if sys.version_info < (3, 10):
+    UnionTypes = (Union,)
+else:
+    from types import UnionType
+    UnionTypes = (Union, UnionType)
+
 import pydantic as pd
 
 import pydantic_xml as pxml
 from pydantic_xml.element import SearchMode, XmlElementReader, XmlElementWriter
 from pydantic_xml.typedefs import NsMap
 
 from . import factories
@@ -63,15 +70,15 @@
 
 
 def is_xml_model(tp: Any) -> bool:
     return isclass(tp) and issubclass(tp, pxml.BaseXmlModel)
 
 
 def is_union(type_: Any) -> bool:
-    return typing.get_origin(type_) is Union
+    return typing.get_origin(type_) in UnionTypes
 
 
 def is_optional(type_: Any) -> bool:
     if not is_union(type_):
         return False
 
     union_args = typing.get_args(type_)
```

### Comparing `pydantic_xml-0.6.1/pydantic_xml/utils.py` & `pydantic_xml-0.6.2/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.1/pyproject.toml` & `pydantic_xml-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "0.6.1"
+version = "0.6.2"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
```

### Comparing `pydantic_xml-0.6.1/PKG-INFO` & `pydantic_xml-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 0.6.1
+Version: 0.6.2
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,18 +15,14 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Provides-Extra: lxml
 Requires-Dist: Sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; extra == "docs"
 Requires-Dist: lxml (>=4.9.1,<5.0.0) ; extra == "lxml"
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
```


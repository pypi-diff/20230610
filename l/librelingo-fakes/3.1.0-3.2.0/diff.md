# Comparing `tmp/librelingo_fakes-3.1.0.tar.gz` & `tmp/librelingo_fakes-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librelingo_fakes-3.1.0.tar", max compression
+gzip compressed data, was "librelingo_fakes-3.2.0.tar", max compression
```

## Comparing `librelingo_fakes-3.1.0.tar` & `librelingo_fakes-3.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1138 2022-11-15 21:28:53.264930 librelingo_fakes-3.1.0/README.md
--rw-r--r--   0        0        0       98 2022-11-15 21:28:53.264930 librelingo_fakes-3.1.0/librelingo_fakes/__init__.py
--rw-r--r--   0        0        0     7542 2023-03-12 19:04:44.199274 librelingo_fakes-3.1.0/librelingo_fakes/fakes.py
--rw-r--r--   0        0        0      477 2023-03-18 11:47:47.331821 librelingo_fakes-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 librelingo_fakes-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1138 2022-11-15 21:28:53.264930 librelingo_fakes-3.2.0/README.md
+-rw-r--r--   0        0        0       98 2022-11-15 21:28:53.264930 librelingo_fakes-3.2.0/librelingo_fakes/__init__.py
+-rw-r--r--   0        0        0     7592 2023-06-10 11:57:31.714229 librelingo_fakes-3.2.0/librelingo_fakes/fakes.py
+-rw-r--r--   0        0        0      477 2023-06-10 12:54:59.251359 librelingo_fakes-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 librelingo_fakes-3.2.0/PKG-INFO
```

### Comparing `librelingo_fakes-3.1.0/README.md` & `librelingo_fakes-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `librelingo_fakes-3.1.0/librelingo_fakes/fakes.py` & `librelingo_fakes-3.2.0/librelingo_fakes/fakes.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,18 @@
 
 
 def fake_value():
     FakeValue = namedtuple("FakeValue", ["id"])
     return FakeValue(number())
 
 
+def fake_string():
+    return str(fake_value())
+
+
 def customize(fake, **kwargs):
     return type(fake)(
         **{**(fake._asdict()), **kwargs},
     )
 
 
 def path():
```

### Comparing `librelingo_fakes-3.1.0/PKG-INFO` & `librelingo_fakes-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librelingo-fakes
-Version: 3.1.0
+Version: 3.2.0
 Summary: Fake data for testing LibreLingo-related packages
 License: GPLv3
 Author: Dániel Kántor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/drjson-3.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/drjson-3.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 47023 bytes, number of entries: 8
+Zip file size: 47054 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       55 b- defN 23-May-30 23:44 drjson/__init__.py
--rw-rw-rw-  2.0 fat    80384 b- defN 23-Jun-09 23:01 drjson/drjson.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1686 b- defN 23-May-31 05:37 drjson/drjson.pyi
+-rw-rw-rw-  2.0 fat    80384 b- defN 23-Jun-10 20:24 drjson/drjson.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2310 b- defN 23-Jun-10 20:23 drjson/drjson.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-30 23:44 drjson/py.typed
--rw-rw-rw-  2.0 fat      912 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      599 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/RECORD
-8 files, 83743 bytes uncompressed, 45981 bytes compressed:  45.1%
+-rw-rw-rw-  2.0 fat      912 b- defN 23-Jun-10 20:24 drjson-3.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-10 20:24 drjson-3.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-10 20:24 drjson-3.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      599 b- defN 23-Jun-10 20:24 drjson-3.0.1.dist-info/RECORD
+8 files, 84367 bytes uncompressed, 46012 bytes compressed:  45.5%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: drjson/drjson.pyi
 Comment: 
 
 Filename: drjson/py.typed
 Comment: 
 
-Filename: drjson-3.0.0.dist-info/METADATA
+Filename: drjson-3.0.1.dist-info/METADATA
 Comment: 
 
-Filename: drjson-3.0.0.dist-info/WHEEL
+Filename: drjson-3.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: drjson-3.0.0.dist-info/top_level.txt
+Filename: drjson-3.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: drjson-3.0.0.dist-info/RECORD
+Filename: drjson-3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drjson/drjson.pyi

```diff
@@ -13,27 +13,51 @@
 ARRAY_VIEW: int
 OBJECT_KEYS: int
 OBJECT_VALUES: int
 OBJECT_ITEMS: int
 APPEND_NEWLINE: int
 PRETTY_PRINT: int
 
+class Writer(Protocol):
+    def write(self, s:str) -> None:
+        ...
+
+class Reader(Protocol):
+    def read(self) -> str | bytes:
+        ...
+
+def parse(text:str, braceless:bool=False) -> Value:
+    ...
+
+def loads(text:str, braceless:bool=False) -> Value:
+    ...
+
+def load(file:str|Reader, braceless:bool=False) -> Value:
+    ...
+
+
 class Ctx:
     def parse(self, text:str, braceless:bool=False) -> Value:
         ...
 
+    def loads(self, text:str, braceless:bool=False) -> Value:
+        ...
+
+    def load(self, file:str|Reader, braceless:bool=False) -> Value:
+        ...
+
     def make(self, value: Any) -> Value:
         ...
 
-class Writer(Protocol):
-    def write(self, s:str) -> None:
+    def mem(self) -> tuple:
         ...
 
+
 class Value:
-    ctx: Ctx
+    ctx: Final[Ctx]
     kind: Final[int]
 
     def __repr__(self) -> str:
         ...
 
     def __getitem__(self, k:Union[int, str]) -> Value:
         ...
@@ -75,7 +99,16 @@
     @overload
     def dump(self, writer:Union[Writer, Callable[[str], None]], flags:int=0) -> None:
         ...
 
     @overload
     def dump(self, writer:Union[None, Writer, Callable[[str], None]]=None, flags:int=0) -> Union[str, None]:
         ...
+
+    def keys(self) -> list[str]:
+        ...
+
+    def values(self) -> list[Value]:
+        ...
+
+    def items(self) -> list[tuple[str, Value]]:
+        ...
```

## Comparing `drjson-3.0.0.dist-info/METADATA` & `drjson-3.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drjson
-Version: 3.0.0
+Version: 3.0.1
 Summary: fast json parsing
 Author: David Priver
 Author-email: david@davidpriver.com
 License: Proprietary
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `drjson-3.0.0.dist-info/RECORD` & `drjson-3.0.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 drjson/__init__.py,sha256=dHSvR1_wm89QLGV9yFp_jq9oo7rPMzU-wpJSzRniYSE,55
-drjson/drjson.cp39-win_amd64.pyd,sha256=YH-mkJn1nLgoubjAnQg_-cy-0mhJIr20CxcEXrgy5Ik,80384
-drjson/drjson.pyi,sha256=prmgCjBZ931ON8FOdPo62c-VFKvboXu7fov8WDritvc,1686
+drjson/drjson.cp39-win_amd64.pyd,sha256=2xrHDCyhza1RvOtGdvQuHQjlV920uJ7TGfjBou-LAak,80384
+drjson/drjson.pyi,sha256=gHrAY9GfZTBmA4mvyU5AoMcSIXMBjFfmVs6bRaBXlow,2310
 drjson/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-drjson-3.0.0.dist-info/METADATA,sha256=EzWKjEOQnn8wPj3yW9h9TFSCK633EkzmWh8nxOBJkc0,912
-drjson-3.0.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-drjson-3.0.0.dist-info/top_level.txt,sha256=F_UvpF7yRih5m2ey-UypoZ2VjBOmiHmX7ard5O4Pjr0,7
-drjson-3.0.0.dist-info/RECORD,,
+drjson-3.0.1.dist-info/METADATA,sha256=ICjdhpZl3DKk9jJwpTUb-gb70ioCYbVFxcnj1LepJus,912
+drjson-3.0.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+drjson-3.0.1.dist-info/top_level.txt,sha256=F_UvpF7yRih5m2ey-UypoZ2VjBOmiHmX7ard5O4Pjr0,7
+drjson-3.0.1.dist-info/RECORD,,
```


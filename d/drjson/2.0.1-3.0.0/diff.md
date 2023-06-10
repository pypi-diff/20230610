# Comparing `tmp/drjson-2.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/drjson-3.0.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 45820 bytes, number of entries: 8
+Zip file size: 47023 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       55 b- defN 23-May-30 23:44 drjson/__init__.py
--rw-rw-rw-  2.0 fat    77312 b- defN 23-Jun-01 18:40 drjson/drjson.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    80384 b- defN 23-Jun-09 23:01 drjson/drjson.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     1686 b- defN 23-May-31 05:37 drjson/drjson.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-30 23:44 drjson/py.typed
--rw-rw-rw-  2.0 fat      912 b- defN 23-Jun-01 18:40 drjson-2.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-01 18:40 drjson-2.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-01 18:40 drjson-2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      599 b- defN 23-Jun-01 18:40 drjson-2.0.1.dist-info/RECORD
-8 files, 80671 bytes uncompressed, 44778 bytes compressed:  44.5%
+-rw-rw-rw-  2.0 fat      912 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      599 b- defN 23-Jun-09 23:01 drjson-3.0.0.dist-info/RECORD
+8 files, 83743 bytes uncompressed, 45981 bytes compressed:  45.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: drjson/drjson.pyi
 Comment: 
 
 Filename: drjson/py.typed
 Comment: 
 
-Filename: drjson-2.0.1.dist-info/METADATA
+Filename: drjson-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: drjson-2.0.1.dist-info/WHEEL
+Filename: drjson-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: drjson-2.0.1.dist-info/top_level.txt
+Filename: drjson-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drjson-2.0.1.dist-info/RECORD
+Filename: drjson-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `drjson-2.0.1.dist-info/METADATA` & `drjson-3.0.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drjson
-Version: 2.0.1
+Version: 3.0.0
 Summary: fast json parsing
 Author: David Priver
 Author-email: david@davidpriver.com
 License: Proprietary
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `drjson-2.0.1.dist-info/RECORD` & `drjson-3.0.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 drjson/__init__.py,sha256=dHSvR1_wm89QLGV9yFp_jq9oo7rPMzU-wpJSzRniYSE,55
-drjson/drjson.cp39-win_amd64.pyd,sha256=ZU1s0tDZlu8NIMv9gc0rg9wTq4L5tkdu6Fm8zD1AnuY,77312
+drjson/drjson.cp39-win_amd64.pyd,sha256=YH-mkJn1nLgoubjAnQg_-cy-0mhJIr20CxcEXrgy5Ik,80384
 drjson/drjson.pyi,sha256=prmgCjBZ931ON8FOdPo62c-VFKvboXu7fov8WDritvc,1686
 drjson/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-drjson-2.0.1.dist-info/METADATA,sha256=DzLK8YlPx_r8T7lHJOaCVoAGwfcc5lwIcRpZtyP4hoU,912
-drjson-2.0.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-drjson-2.0.1.dist-info/top_level.txt,sha256=F_UvpF7yRih5m2ey-UypoZ2VjBOmiHmX7ard5O4Pjr0,7
-drjson-2.0.1.dist-info/RECORD,,
+drjson-3.0.0.dist-info/METADATA,sha256=EzWKjEOQnn8wPj3yW9h9TFSCK633EkzmWh8nxOBJkc0,912
+drjson-3.0.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+drjson-3.0.0.dist-info/top_level.txt,sha256=F_UvpF7yRih5m2ey-UypoZ2VjBOmiHmX7ard5O4Pjr0,7
+drjson-3.0.0.dist-info/RECORD,,
```


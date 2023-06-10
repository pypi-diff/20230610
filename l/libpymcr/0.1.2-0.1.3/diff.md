# Comparing `tmp/libpymcr-0.1.2-cp39-cp39-win_amd64.whl.zip` & `tmp/libpymcr-0.1.3-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 194113 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     5010 b- defN 23-Jun-09 01:03 libpymcr/Matlab.py
--rw-rw-rw-  2.0 fat     9690 b- defN 23-Jun-09 01:03 libpymcr/MatlabProxyObject.py
--rw-rw-rw-  2.0 fat      175 b- defN 23-Jun-09 01:03 libpymcr/__init__.py
--rw-rw-rw-  2.0 fat   450048 b- defN 23-Jun-09 01:11 libpymcr/_libpymcr.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      518 b- defN 23-Jun-09 01:11 libpymcr/_version.py
--rw-rw-rw-  2.0 fat     8382 b- defN 23-Jun-09 01:03 libpymcr/utils.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      875 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/RECORD
-11 files, 513216 bytes uncompressed, 192645 bytes compressed:  62.5%
+Zip file size: 194258 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     5010 b- defN 23-Jun-10 12:39 libpymcr/Matlab.py
+-rw-rw-rw-  2.0 fat     9690 b- defN 23-Jun-10 12:39 libpymcr/MatlabProxyObject.py
+-rw-rw-rw-  2.0 fat      175 b- defN 23-Jun-10 12:39 libpymcr/__init__.py
+-rw-rw-rw-  2.0 fat   450048 b- defN 23-Jun-10 12:47 libpymcr/_libpymcr.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      518 b- defN 23-Jun-10 12:46 libpymcr/_version.py
+-rw-rw-rw-  2.0 fat     8382 b- defN 23-Jun-10 12:39 libpymcr/utils.py
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      875 b- defN 23-Jun-10 12:47 libpymcr-0.1.3.dist-info/RECORD
+11 files, 513216 bytes uncompressed, 192790 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: libpymcr/_version.py
 Comment: 
 
 Filename: libpymcr/utils.py
 Comment: 
 
-Filename: libpymcr-0.1.2.dist-info/LICENSE
+Filename: libpymcr-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: libpymcr-0.1.2.dist-info/METADATA
+Filename: libpymcr-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: libpymcr-0.1.2.dist-info/WHEEL
+Filename: libpymcr-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: libpymcr-0.1.2.dist-info/top_level.txt
+Filename: libpymcr-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: libpymcr-0.1.2.dist-info/RECORD
+Filename: libpymcr-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libpymcr/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-06-09T01:51:35+0100",
+ "date": "2023-06-10T13:38:34+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "9b713dbc40b12ecbe097335aa1b319c17d186046",
- "version": "0.1.2"
+ "full-revisionid": "64efaca1fe8fbd4db077242cba100cd70dc40db8",
+ "version": "0.1.3"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `libpymcr-0.1.2.dist-info/LICENSE` & `libpymcr-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libpymcr-0.1.2.dist-info/METADATA` & `libpymcr-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpymcr
-Version: 0.1.2
+Version: 0.1.3
 Summary: A module to allow Python to call functions from a compiled Matlab archive
 Home-page: https://github.com/pace-neutrons/libpymcr
 Author: Duc Le
 Author-email: duc.le@stfc.ac.uk
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

## Comparing `libpymcr-0.1.2.dist-info/RECORD` & `libpymcr-0.1.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 libpymcr/Matlab.py,sha256=l2cesZ372H3Zo_przYnwgzQF3AHCK6Meg6mxQPcth2Y,5010
 libpymcr/MatlabProxyObject.py,sha256=5A93jipCzHhPwOAly8E0wXkzKMQE3PbapWmylv4S5X8,9690
 libpymcr/__init__.py,sha256=sQKTM1zicjP6fj_l3S3MBGEnqp_H0TYtm0iIlejgs-I,175
-libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=xG6IH7mDmw5NP_Hl_y93DEcAYXWpO-v6211JV5jKGFo,450048
-libpymcr/_version.py,sha256=bmRryh7vRc3D2wU1ddY30NFCkfEmVzhQAmpO0G20ycg,518
+libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=ACaBD-ISOKfOW7vC9kUGWcTOMhisJiYrIaUxoVC63S8,450048
+libpymcr/_version.py,sha256=aVUbKvWJ_PBcRuh74GL7LiL4fquq4QXnsiRo9wC8XJY,518
 libpymcr/utils.py,sha256=ZQIZfG0uSFKJBpwE4w8Jveh3C0873z4ak2XTh1S-Z9k,8382
-libpymcr-0.1.2.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-libpymcr-0.1.2.dist-info/METADATA,sha256=xZRNSmNEziSOlbpy31o0ASWcxtTeyItEjdH1hgymqiQ,2586
-libpymcr-0.1.2.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-libpymcr-0.1.2.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
-libpymcr-0.1.2.dist-info/RECORD,,
+libpymcr-0.1.3.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+libpymcr-0.1.3.dist-info/METADATA,sha256=vi5u92orC_EnGN41mgcErRAEA6dGkGX1AR0bGjT3cFg,2586
+libpymcr-0.1.3.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
+libpymcr-0.1.3.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
+libpymcr-0.1.3.dist-info/RECORD,,
```


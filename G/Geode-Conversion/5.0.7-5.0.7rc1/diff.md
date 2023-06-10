# Comparing `tmp/Geode_Conversion-5.0.7-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/Geode_Conversion-5.0.7rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1638447 bytes, number of entries: 8
--rw-r--r--  2.0 unx       67 b- defN 23-Jun-10 12:33 geode_conversion/__init__.py
--rw-r--r--  2.0 unx      172 b- defN 23-Jun-10 12:33 geode_conversion/model.py
--rwxr-xr-x  2.0 unx   167480 b- defN 23-Jun-10 12:33 geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx  3710352 b- defN 23-Jun-10 12:33 geode_conversion/lib64/libGeode-Conversion_model.so
--rw-r--r--  2.0 unx     1942 b- defN 23-Jun-10 12:33 Geode_Conversion-5.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-10 12:33 Geode_Conversion-5.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-10 12:33 Geode_Conversion-5.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      748 b- defN 23-Jun-10 12:33 Geode_Conversion-5.0.7.dist-info/RECORD
-8 files, 3880881 bytes uncompressed, 1637123 bytes compressed:  57.8%
+Zip file size: 1203317 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jun-08 11:51 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      178 b- defN 23-Jun-08 11:51 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat  2390528 b- defN 23-Jun-08 11:51 geode_conversion/bin/Geode-Conversion_model.dll
+-rw-rw-rw-  2.0 fat   150016 b- defN 23-Jun-08 11:51 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2007 b- defN 23-Jun-08 11:51 Geode_Conversion-5.0.7rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-08 11:51 Geode_Conversion-5.0.7rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-08 11:51 Geode_Conversion-5.0.7rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      743 b- defN 23-Jun-08 11:51 Geode_Conversion-5.0.7rc1.dist-info/RECORD
+8 files, 2543760 bytes uncompressed, 1202005 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: geode_conversion/__init__.py
 Comment: 
 
 Filename: geode_conversion/model.py
 Comment: 
 
-Filename: geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
+Filename: geode_conversion/bin/Geode-Conversion_model.dll
 Comment: 
 
-Filename: geode_conversion/lib64/libGeode-Conversion_model.so
+Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Conversion-5.0.7.dist-info/METADATA
+Filename: Geode_Conversion-5.0.7rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.0.7.dist-info/WHEEL
+Filename: Geode_Conversion-5.0.7rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.0.7.dist-info/top_level.txt
+Filename: Geode_Conversion-5.0.7rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.0.7.dist-info/RECORD
+Filename: Geode_Conversion-5.0.7rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/__init__.py

```diff
@@ -1,3 +1,6 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-from .model import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .model import *
```

## geode_conversion/model.py

```diff
@@ -1,8 +1,8 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-
-from .lib64.geode_conversion_py_model import *
-ConversionModelLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+
+from .bin.geode_conversion_py_model import *
+ConversionModelLibrary.initialize()
```

## Comparing `Geode_Conversion-5.0.7.dist-info/METADATA` & `Geode_Conversion-5.0.7rc1.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 2.1
-Name: Geode-Conversion
-Version: 5.0.7
-Summary: Conversion module for Geode-solutions OpenGeode modules
-Home-page: https://github.com/Geode-solutions/Geode-Conversion
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.3.1)
-
-<h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Conversion OpenGeode module</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Conversion_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Conversion_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2023, Geode-solutions
+Metadata-Version: 2.1
+Name: Geode-Conversion
+Version: 5.0.7rc1
+Summary: Conversion module for Geode-solutions OpenGeode modules
+Home-page: https://github.com/Geode-solutions/Geode-Conversion
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Requires-Dist: opengeode-core (==14.*,>=14.3.1rc2)
+
+<h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Conversion OpenGeode module</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Conversion_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Conversion_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2023, Geode-solutions
+
+
```

### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.7 Summary: Conversion
-module for Geode-solutions OpenGeode modules Home-page: https://github.com/
-Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Description-Content-Type:
-text/markdown Requires-Dist: opengeode-core (==14.*,>=14.3.1)
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.7rc1 Summary:
+Conversion module for Geode-solutions OpenGeode modules Home-page: https://
+github.com/Geode-solutions/Geode-Conversion Author: Geode-solutions Author-
+email: contact@geode-solutions.com License: Proprietary Platform: UNKNOWN
+Description-Content-Type: text/markdown Requires-Dist: opengeode-core
+(==14.*,>=14.3.1rc2)
                ****** Geode-Conversionby Geode-solutions ******
                      **** Conversion OpenGeode module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```


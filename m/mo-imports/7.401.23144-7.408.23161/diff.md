# Comparing `tmp/mo_imports-7.401.23144-py2.py3-none-any.whl.zip` & `tmp/mo_imports-7.408.23161-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11130 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     9696 b- defN 23-May-24 02:37 mo_imports/__init__.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4945 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      512 b- defN 23-May-24 02:37 mo_imports-7.401.23144.dist-info/RECORD
-6 files, 31999 bytes uncompressed, 10200 bytes compressed:  68.1%
+Zip file size: 11129 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     9689 b- defN 23-Jun-10 00:41 mo_imports/__init__.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-10 00:41 mo_imports-7.408.23161.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4945 b- defN 23-Jun-10 00:41 mo_imports-7.408.23161.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-10 00:41 mo_imports-7.408.23161.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-10 00:41 mo_imports-7.408.23161.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      512 b- defN 23-Jun-10 00:41 mo_imports-7.408.23161.dist-info/RECORD
+6 files, 31992 bytes uncompressed, 10199 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: mo_imports/__init__.py
 Comment: 
 
-Filename: mo_imports-7.401.23144.dist-info/LICENSE
+Filename: mo_imports-7.408.23161.dist-info/LICENSE
 Comment: 
 
-Filename: mo_imports-7.401.23144.dist-info/METADATA
+Filename: mo_imports-7.408.23161.dist-info/METADATA
 Comment: 
 
-Filename: mo_imports-7.401.23144.dist-info/WHEEL
+Filename: mo_imports-7.408.23161.dist-info/WHEEL
 Comment: 
 
-Filename: mo_imports-7.401.23144.dist-info/top_level.txt
+Filename: mo_imports-7.408.23161.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_imports-7.401.23144.dist-info/RECORD
+Filename: mo_imports-7.408.23161.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_imports/__init__.py

```diff
@@ -2,26 +2,23 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
-
-
 import importlib
 import sys
 from threading import Thread, Event
 from time import time
 
 from mo_future import text, allocate_lock
 
 DEBUG = False
-WAIT_FOR_EXPORT = 10_000  # SECONDS TO WAIT FROM MOST RECENT expect() TO LAST export()
+WAIT_FOR_EXPORT = 10  # SECONDS TO WAIT FROM MOST RECENT expect() TO LAST export()
 
 _locker = allocate_lock()
 _expectations = []
 _expiry = None
 _monitor = None
 _nothing = object()
 _set = object.__setattr__
```

## Comparing `mo_imports-7.401.23144.dist-info/LICENSE` & `mo_imports-7.408.23161.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_imports-7.401.23144.dist-info/METADATA` & `mo_imports-7.408.23161.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-imports
-Version: 7.401.23144
+Version: 7.408.23161
 Summary: More Imports! - Delayed importing
 Home-page: https://github.com/klahnakoski/mo-imports
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

## Comparing `mo_imports-7.401.23144.dist-info/RECORD` & `mo_imports-7.408.23161.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-mo_imports/__init__.py,sha256=6nvOZ2e80JS1hDep0H7voQiuBJBgzGkIzNz3pimztKM,9696
-mo_imports-7.401.23144.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_imports-7.401.23144.dist-info/METADATA,sha256=eG2J4xpsd5q84eoIXcg8MXs-CgnLWP82tC2udTyj-Jg,4945
-mo_imports-7.401.23144.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_imports-7.401.23144.dist-info/top_level.txt,sha256=2S4BXaL_PjiUzIiyjbiHLODAtvQW1tw1ry6hcvOTXzM,11
-mo_imports-7.401.23144.dist-info/RECORD,,
+mo_imports/__init__.py,sha256=ZdXm2jKMlL63Xfnq49kboA1Kg9J9AMYDbfNIGqUPjpk,9689
+mo_imports-7.408.23161.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_imports-7.408.23161.dist-info/METADATA,sha256=cm9hsX9Tm8FY16ILOtjBmkVDg4nDUZFtNsJJkWmyCbc,4945
+mo_imports-7.408.23161.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_imports-7.408.23161.dist-info/top_level.txt,sha256=2S4BXaL_PjiUzIiyjbiHLODAtvQW1tw1ry6hcvOTXzM,11
+mo_imports-7.408.23161.dist-info/RECORD,,
```


# Comparing `tmp/docleaf-0.2.0a0-cp39-none-win_amd64.whl.zip` & `tmp/docleaf-0.3.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1075810 bytes, number of entries: 10
--rw-r--r--  4.6 unx     4461 b- defN 23-Jun-10 15:57 docleaf-0.2.0a0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jun-10 15:57 docleaf-0.2.0a0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3573 b- defN 23-Jun-10 15:57 docleaf-0.2.0a0.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     3774 b- defN 23-Jun-10 15:57 docleaf/copied.py
--rw-r--r--  4.6 unx     2954 b- defN 23-Jun-10 15:57 docleaf/domains.py
--rw-r--r--  4.6 unx    17005 b- defN 23-Jun-10 15:57 docleaf/doxygen.py
--rw-r--r--  4.6 unx       99 b- defN 23-Jun-10 15:57 docleaf/errors.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-10 15:57 docleaf/__init__.py
--rwxr-xr-x  4.6 unx  3038208 b- defN 23-Jun-10 15:57 docleaf/backend.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      783 b- defN 23-Jun-10 15:57 docleaf-0.2.0a0.dist-info/RECORD
-10 files, 3070953 bytes uncompressed, 1074488 bytes compressed:  65.0%
+Zip file size: 1075788 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     4459 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3573 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     3774 b- defN 23-Jun-10 16:49 docleaf/copied.py
+-rw-r--r--  4.6 unx     2954 b- defN 23-Jun-10 16:49 docleaf/domains.py
+-rw-r--r--  4.6 unx    17005 b- defN 23-Jun-10 16:49 docleaf/doxygen.py
+-rw-r--r--  4.6 unx       99 b- defN 23-Jun-10 16:49 docleaf/errors.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-10 16:49 docleaf/__init__.py
+-rwxr-xr-x  4.6 unx  3038208 b- defN 23-Jun-10 16:49 docleaf/backend.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      775 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/RECORD
+10 files, 3070943 bytes uncompressed, 1074482 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: docleaf-0.2.0a0.dist-info/METADATA
+Filename: docleaf-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.2.0a0.dist-info/WHEEL
+Filename: docleaf-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.2.0a0.dist-info/license_files/LICENSE.md
+Filename: docleaf-0.3.0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: docleaf/copied.py
 Comment: 
 
 Filename: docleaf/domains.py
 Comment: 
@@ -21,11 +21,11 @@
 
 Filename: docleaf/__init__.py
 Comment: 
 
 Filename: docleaf/backend.cp39-win_amd64.pyd
 Comment: 
 
-Filename: docleaf-0.2.0a0.dist-info/RECORD
+Filename: docleaf-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `docleaf-0.2.0a0.dist-info/METADATA` & `docleaf-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.2.0a0
+Version: 0.3.0
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,<6,!=5.0.0
 License-File: LICENSE.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
 Author: Michael Jones
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/docleaf-labs/docleaf
```

## Comparing `docleaf-0.2.0a0.dist-info/license_files/LICENSE.md` & `docleaf-0.3.0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `docleaf-0.2.0a0.dist-info/RECORD` & `docleaf-0.3.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-docleaf-0.2.0a0.dist-info/METADATA,sha256=11DInyFz8MnUFUXg8WcQLWQs5bXrrp5IFCm6Bwq1Ctc,4461
-docleaf-0.2.0a0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
-docleaf-0.2.0a0.dist-info/license_files/LICENSE.md,sha256=ffIj5xgqX0xL1nd3_5YbHFc3paR7y61W6f1780Gp3lE,3573
+docleaf-0.3.0.dist-info/METADATA,sha256=Fh17ag_4xvsnhT8ilPge7lbOfBdJ59TYZYYQUI2hIyE,4459
+docleaf-0.3.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
+docleaf-0.3.0.dist-info/license_files/LICENSE.md,sha256=ffIj5xgqX0xL1nd3_5YbHFc3paR7y61W6f1780Gp3lE,3573
 docleaf/copied.py,sha256=fIQgdMKJYpQbE08lNhe7Xva9sN-pRgK6ZGj2ABM_EN4,3774
 docleaf/domains.py,sha256=6zPyDrgK53W20lOZdwJWAGwrsIMaZ44YlXhIl2hcKhc,2954
 docleaf/doxygen.py,sha256=9Pq1Gu-O0_E0Qoupi3Z20TsVhFf7wRHGerVgbdmeDtw,17005
 docleaf/errors.py,sha256=sUYIqy64k8zKQ-cZjVzF6auax0klQ9FibFmKOCD9v2Y,99
 docleaf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docleaf/backend.cp39-win_amd64.pyd,sha256=fOQFsz5BPl1w-q_zJIBZ7kOZ--B4-2WGULs0qw4uhqs,3038208
-docleaf-0.2.0a0.dist-info/RECORD,,
+docleaf/backend.cp39-win_amd64.pyd,sha256=VRB5Jjr7d-kDEK4d-C_wKZTa5CBRinpBqmZFuT90HRA,3038208
+docleaf-0.3.0.dist-info/RECORD,,
```


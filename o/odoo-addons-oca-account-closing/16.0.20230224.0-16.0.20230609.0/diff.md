# Comparing `tmp/odoo_addons_oca_account_closing-16.0.20230224.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_closing-16.0.20230609.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1440 bytes, number of entries: 4
--rw-r--r--  2.0 unx      612 b- defN 23-Feb-25 02:39 odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-25 02:39 odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-25 02:39 odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      432 b- defN 23-Feb-25 02:39 odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/RECORD
-4 files, 1137 bytes uncompressed, 586 bytes compressed:  48.5%
+Zip file size: 1456 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      695 b- defN 23-Jun-10 02:33 odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:33 odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-10 02:33 odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      432 b- defN 23-Jun-10 02:33 odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/RECORD
+4 files, 1220 bytes uncompressed, 602 bytes compressed:  50.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_closing-16.0.20230224.0.dist-info/METADATA` & `odoo_addons_oca_account_closing-16.0.20230609.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-closing
-Version: 16.0.20230224.0
+Version: 16.0.20230609.0
 Summary: Meta package for oca-account-closing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
+Requires-Dist: odoo-addon-account-cutoff-accrual-subscription (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-cutoff-base (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-cutoff-picking (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-cutoff-start-end-dates (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-start-end-dates (<16.1dev,>=16.0dev)
 
 UNKNOWN
```


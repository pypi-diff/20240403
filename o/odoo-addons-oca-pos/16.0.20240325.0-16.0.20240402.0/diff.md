# Comparing `tmp/odoo_addons_oca_pos-16.0.20240325.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_pos-16.0.20240402.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1686 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3109 b- defN 24-Mar-26 05:33 odoo_addons_oca_pos-16.0.20240325.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 05:33 odoo_addons_oca_pos-16.0.20240325.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-26 05:33 odoo_addons_oca_pos-16.0.20240325.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Mar-26 05:33 odoo_addons_oca_pos-16.0.20240325.0.dist-info/RECORD
-4 files, 3587 bytes uncompressed, 928 bytes compressed:  74.1%
+Zip file size: 1713 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3261 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/RECORD
+4 files, 3739 bytes uncompressed, 955 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_pos-16.0.20240325.0.dist-info/METADATA
+Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240325.0.dist-info/WHEEL
+Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240325.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240325.0.dist-info/RECORD
+Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_pos-16.0.20240325.0.dist-info/METADATA` & `odoo_addons_oca_pos-16.0.20240402.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-pos
-Version: 16.0.20240325.0
+Version: 16.0.20240402.0
 Summary: Meta package for oca-pos Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -28,14 +28,16 @@
 Requires-Dist: odoo-addon-pos-order-reorder <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-order-to-sale-order <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-order-to-sale-order-delivery <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-order-to-sale-order-report <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-order-to-sale-order-sale-financial-risk <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-partner-birthdate <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-partner-firstname <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-partner-location-abstract <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-partner-location-google-map <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-partner-sale-warning <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-change <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-method-cashdro <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-method-image <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-terminal <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-display-default-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-label <16.1dev,>=16.0dev
```


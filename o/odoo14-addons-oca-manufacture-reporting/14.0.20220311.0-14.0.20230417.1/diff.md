# Comparing `tmp/odoo14_addons_oca_manufacture_reporting-14.0.20220311.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_manufacture_reporting-14.0.20230417.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1508 bytes, number of entries: 4
--rw-r--r--  2.0 unx      543 b- defN 22-Mar-12 03:55 odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Mar-12 03:55 odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 22-Mar-12 03:55 odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      464 b- defN 22-Mar-12 03:55 odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/RECORD
-4 files, 1100 bytes uncompressed, 590 bytes compressed:  46.4%
+Zip file size: 1537 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      687 b- defN 23-Apr-18 05:30 odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 05:30 odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 05:30 odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      464 b- defN 23-Apr-18 05:30 odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/RECORD
+4 files, 1244 bytes uncompressed, 619 bytes compressed:  50.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/METADATA
+Filename: odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/RECORD
+Filename: odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_manufacture_reporting-14.0.20220311.0.dist-info/METADATA` & `odoo14_addons_oca_manufacture_reporting-14.0.20230417.1.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-manufacture-reporting
-Version: 14.0.20220311.0
+Version: 14.0.20230417.1
 Summary: Meta package for oca-manufacture-reporting Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Dist: odoo14-addon-mrp-bom-current-stock
 Requires-Dist: odoo14-addon-mrp-bom-structure-xlsx
 Requires-Dist: odoo14-addon-mrp-bom-structure-xlsx-level-1
 Requires-Dist: odoo14-addon-mrp-flattened-bom-xlsx
+Requires-Dist: odoo14-addon-mrp-flattened-bom-xlsx-direct-materials-cost
+Requires-Dist: odoo14-addon-mrp-flattened-bom-xlsx-subcontracting-cost
 
 UNKNOWN
```


# Comparing `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2226 bytes, number of entries: 4
--rw-r--r--  2.0 unx     5885 b- defN 24-Apr-19 06:34 odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 06:34 odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-19 06:34 odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      469 b- defN 24-Apr-19 06:34 odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/RECORD
-4 files, 6447 bytes uncompressed, 1300 bytes compressed:  79.8%
+Zip file size: 2240 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     6060 b- defN 24-May-08 06:40 odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 06:40 odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-08 06:40 odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      469 b- defN 24-May-08 06:40 odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/RECORD
+4 files, 6622 bytes uncompressed, 1314 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/METADATA
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/WHEEL
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/RECORD
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_stock_logistics_workflow-16.0.20240418.0.dist-info/METADATA` & `odoo_addons_oca_stock_logistics_workflow-16.0.20240507.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-stock-logistics-workflow
-Version: 16.0.20240418.0
+Version: 16.0.20240507.1
 Summary: Meta package for oca-stock-logistics-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -14,14 +14,15 @@
 Requires-Dist: odoo-addon-sale-line-returned-qty <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-global-stock-route <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-stock-restocking-fee-invoicing <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-account-product-run-fifo-hook <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-auto-move <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-customer-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-customer-deposit-elaboration <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-customer-deposit-sale-margin <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-delivery-note <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-grn <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-landed-costs-currency <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-landed-costs-purchase-auto <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-landed-costs-security <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-lot-production-date <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-lot-scrap <16.1dev,>=16.0dev
@@ -48,14 +49,15 @@
 Requires-Dist: odoo-addon-stock-picking-batch-print-pickings <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-customer-ref <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-filter-lot <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-grn-mandatory <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-group-by-base <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-group-by-max-weight <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-group-by-partner-by-carrier <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-picking-group-by-partner-by-carrier-by-date <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-import-serial-number <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-info-lot <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-invoice-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-kind <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-line-sequence <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-mass-action <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-partner-note <16.1dev,>=16.0dev
```


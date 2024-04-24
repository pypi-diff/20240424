# Comparing `tmp/odoo_addons_oca_server_tools-16.0.20240205.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_server_tools-16.0.20240423.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1799 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2921 b- defN 24-Feb-06 06:09 odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-06 06:09 odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-06 06:09 odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      421 b- defN 24-Feb-06 06:09 odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/RECORD
-4 files, 3435 bytes uncompressed, 969 bytes compressed:  71.8%
+Zip file size: 1816 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3049 b- defN 24-Apr-24 06:03 odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 06:03 odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 06:03 odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      421 b- defN 24-Apr-24 06:03 odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/RECORD
+4 files, 3563 bytes uncompressed, 986 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/METADATA
+Filename: odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/WHEEL
+Filename: odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/RECORD
+Filename: odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_server_tools-16.0.20240205.0.dist-info/METADATA` & `odoo_addons_oca_server_tools-16.0.20240423.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-server-tools
-Version: 16.0.20240205.0
+Version: 16.0.20240423.1
 Summary: Meta package for oca-server-tools Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -24,16 +24,18 @@
 Requires-Dist: odoo-addon-base-search-fuzzy <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-sequence-default <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-sequence-option <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-sparse-field-list-support <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-technical-user <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-time-window <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-view-inheritance-extension <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-bus-alt-connection <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-cron-daylight-saving-time-resistant <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-database-cleanup <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-datetime-formatter <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-dbfilter-from-header <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-excel-import-export <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-excel-import-export-demo <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-excel-import-export-unidecode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-html-text <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-iap-alternative-provider <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-jsonifier <16.1dev,>=16.0dev
```


# Comparing `tmp/odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 52723 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1282 b- defN 23-Oct-14 04:14 odoo/addons/ssi_data_requirement_work_log/README.rst
--rw-r--r--  2.0 unx      201 b- defN 23-Oct-14 04:14 odoo/addons/ssi_data_requirement_work_log/__init__.py
--rw-r--r--  2.0 unx      565 b- defN 23-Oct-14 04:14 odoo/addons/ssi_data_requirement_work_log/__manifest__.py
--rw-r--r--  2.0 unx      211 b- defN 23-Oct-14 04:14 odoo/addons/ssi_data_requirement_work_log/models/__init__.py
--rw-r--r--  2.0 unx      379 b- defN 23-Oct-14 04:14 odoo/addons/ssi_data_requirement_work_log/models/data_requirement.py
--rw-r--r--  2.0 unx    48333 b- defN 23-Oct-14 04:14 odoo/addons/ssi_data_requirement_work_log/static/description/icon.png
--rw-r--r--  2.0 unx     1909 b- defN 23-Oct-14 04:14 odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-14 04:14 odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Oct-14 04:14 odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Oct-14 04:14 odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/RECORD
-10 files, 54132 bytes uncompressed, 50647 bytes compressed:  6.4%
+Zip file size: 53259 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1282 b- defN 24-Apr-24 23:44 odoo/addons/ssi_data_requirement_work_log/README.rst
+-rw-r--r--  2.0 unx      201 b- defN 24-Apr-24 23:44 odoo/addons/ssi_data_requirement_work_log/__init__.py
+-rw-r--r--  2.0 unx      565 b- defN 24-Apr-24 23:44 odoo/addons/ssi_data_requirement_work_log/__manifest__.py
+-rw-r--r--  2.0 unx      241 b- defN 24-Apr-24 23:44 odoo/addons/ssi_data_requirement_work_log/models/__init__.py
+-rw-r--r--  2.0 unx      379 b- defN 24-Apr-24 23:44 odoo/addons/ssi_data_requirement_work_log/models/data_requirement.py
+-rw-r--r--  2.0 unx      402 b- defN 24-Apr-24 23:44 odoo/addons/ssi_data_requirement_work_log/models/data_requirement_package.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-24 23:44 odoo/addons/ssi_data_requirement_work_log/static/description/icon.png
+-rw-r--r--  2.0 unx     1907 b- defN 24-Apr-24 23:44 odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 23:44 odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-24 23:44 odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1287 b- defN 24-Apr-24 23:44 odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/RECORD
+11 files, 54694 bytes uncompressed, 50955 bytes compressed:  6.8%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: odoo/addons/ssi_data_requirement_work_log/models/__init__.py
 Comment: 
 
 Filename: odoo/addons/ssi_data_requirement_work_log/models/data_requirement.py
 Comment: 
 
+Filename: odoo/addons/ssi_data_requirement_work_log/models/data_requirement_package.py
+Comment: 
+
 Filename: odoo/addons/ssi_data_requirement_work_log/static/description/icon.png
 Comment: 
 
-Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_data_requirement_work_log/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl-3.0-standalone.html).
 {
     "name": "Data Requirement + Work Log Integration",
-    "version": "14.0.1.0.0",
+    "version": "14.0.1.1.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_data_requirement_mixin",
         "ssi_work_log_mixin",
```

## odoo/addons/ssi_data_requirement_work_log/models/__init__.py

```diff
@@ -1,7 +1,8 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl-3.0-standalone.html).
 
 from . import (
     data_requirement,
+    data_requirement_package,
 )
```

## Comparing `odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/METADATA` & `odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-data-requirement-work-log
-Version: 14.0.1.0.0
+Version: 14.0.1.1.0
 Summary: Data Requirement + Work Log Integration
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-ssi-data-requirement-mixin
 Requires-Dist: odoo14-addon-ssi-work-log-mixin
-Requires-Dist: odoo (<14.1dev,>=14.0a)
+Requires-Dist: odoo <14.1dev,>=14.0a
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
 
 =======================================
 Data Requirement + Work Log Integration
```

## Comparing `odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/RECORD` & `odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 odoo/addons/ssi_data_requirement_work_log/README.rst,sha256=aHkr1h7D_FmxMgaaYGxSqQqRCcX4lwRu57730DFeRWQ,1282
 odoo/addons/ssi_data_requirement_work_log/__init__.py,sha256=pXobMvi-Xzga8dGVPzYthZUHJzQSY3b6Bevs09H-1uY,201
-odoo/addons/ssi_data_requirement_work_log/__manifest__.py,sha256=CoLfgo-84uPrndmnlmVwbdtWGZENiRpNZ0KYRRLAx4M,565
-odoo/addons/ssi_data_requirement_work_log/models/__init__.py,sha256=pyJ5rZM7sn2AWsh3pG6itt-Dbrs3saT08yboyFzGKkw,211
+odoo/addons/ssi_data_requirement_work_log/__manifest__.py,sha256=GsvIyKZZRgtCKLgYamZJ079iRt0LHv6iGOIs7XZu0O4,565
+odoo/addons/ssi_data_requirement_work_log/models/__init__.py,sha256=TSY3vP8N7Td-hz8AQCRyRzfGcjt4X9EjY3t-Ifo1l5k,241
 odoo/addons/ssi_data_requirement_work_log/models/data_requirement.py,sha256=nSXb4xgeLF9sEgyjH0RgsgQQFMTeEKcoFMIC7WOwbcA,379
+odoo/addons/ssi_data_requirement_work_log/models/data_requirement_package.py,sha256=p6D7v8LkFWcysq5wH33FDJJDJvZ3iz8GN6Ws-Bvg2D4,402
 odoo/addons/ssi_data_requirement_work_log/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/METADATA,sha256=bOIqG5YxWu8n2UIKwUsk0_1PCP-UzwntnguiYWDDVz0,1909
-odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_data_requirement_work_log-14.0.1.0.0.dist-info/RECORD,,
+odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/METADATA,sha256=f1pp1LPaiZXWSZgPt7HE6CjWxbqMycgNRSQpXIuhVV0,1907
+odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_data_requirement_work_log-14.0.1.1.0.dist-info/RECORD,,
```


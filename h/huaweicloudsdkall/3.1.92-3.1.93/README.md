# Comparing `tmp/huaweicloudsdkall-3.1.92-py2.py3-none-any.whl.zip` & `tmp/huaweicloudsdkall-3.1.93-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2964 bytes, number of entries: 6
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 08:24 huaweicloudsdkall/__init__.py
--rw-r--r--  2.0 unx      604 b- defN 24-Apr-18 08:25 huaweicloudsdkall-3.1.92.dist-info/LICENSE
--rw-r--r--  2.0 unx     8398 b- defN 24-Apr-18 08:25 huaweicloudsdkall-3.1.92.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-18 08:25 huaweicloudsdkall-3.1.92.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-18 08:25 huaweicloudsdkall-3.1.92.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      524 b- defN 24-Apr-18 08:25 huaweicloudsdkall-3.1.92.dist-info/RECORD
-6 files, 9655 bytes uncompressed, 2000 bytes compressed:  79.3%
+Zip file size: 2962 bytes, number of entries: 6
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-25 08:42 huaweicloudsdkall/__init__.py
+-rw-r--r--  2.0 unx      604 b- defN 24-Apr-25 08:43 huaweicloudsdkall-3.1.93.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8398 b- defN 24-Apr-25 08:43 huaweicloudsdkall-3.1.93.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-25 08:43 huaweicloudsdkall-3.1.93.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-25 08:43 huaweicloudsdkall-3.1.93.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      524 b- defN 24-Apr-25 08:43 huaweicloudsdkall-3.1.93.dist-info/RECORD
+6 files, 9655 bytes uncompressed, 1998 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: huaweicloudsdkall/__init__.py
 Comment: 
 
-Filename: huaweicloudsdkall-3.1.92.dist-info/LICENSE
+Filename: huaweicloudsdkall-3.1.93.dist-info/LICENSE
 Comment: 
 
-Filename: huaweicloudsdkall-3.1.92.dist-info/METADATA
+Filename: huaweicloudsdkall-3.1.93.dist-info/METADATA
 Comment: 
 
-Filename: huaweicloudsdkall-3.1.92.dist-info/WHEEL
+Filename: huaweicloudsdkall-3.1.93.dist-info/WHEEL
 Comment: 
 
-Filename: huaweicloudsdkall-3.1.92.dist-info/top_level.txt
+Filename: huaweicloudsdkall-3.1.93.dist-info/top_level.txt
 Comment: 
 
-Filename: huaweicloudsdkall-3.1.92.dist-info/RECORD
+Filename: huaweicloudsdkall-3.1.93.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `huaweicloudsdkall-3.1.92.dist-info/LICENSE` & `huaweicloudsdkall-3.1.93.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `huaweicloudsdkall-3.1.92.dist-info/METADATA` & `huaweicloudsdkall-3.1.93.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huaweicloudsdkall
-Version: 3.1.92
+Version: 3.1.93
 Summary: HuaweiCloud SDK Python All
 Home-page: https://github.com/huaweicloud/huaweicloud-sdk-python-v3
 Author: HuaweiCloud SDK
 Author-email: hwcloudsdk@huawei.com
 License: Apache LICENSE 2.0
 Keywords: huaweicloud,sdk,all
 Platform: any
@@ -19,172 +19,172 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: huaweicloudsdkcore ==3.1.92
-Requires-Dist: huaweicloudsdkaad ==3.1.92
-Requires-Dist: huaweicloudsdkantiddos ==3.1.92
-Requires-Dist: huaweicloudsdkaom ==3.1.92
-Requires-Dist: huaweicloudsdkaos ==3.1.92
-Requires-Dist: huaweicloudsdkapig ==3.1.92
-Requires-Dist: huaweicloudsdkapm ==3.1.92
-Requires-Dist: huaweicloudsdkas ==3.1.92
-Requires-Dist: huaweicloudsdkasm ==3.1.92
-Requires-Dist: huaweicloudsdkbcs ==3.1.92
-Requires-Dist: huaweicloudsdkbms ==3.1.92
-Requires-Dist: huaweicloudsdkbss ==3.1.92
-Requires-Dist: huaweicloudsdkbssintl ==3.1.92
-Requires-Dist: huaweicloudsdkcae ==3.1.92
-Requires-Dist: huaweicloudsdkcampusgo ==3.1.92
-Requires-Dist: huaweicloudsdkcbh ==3.1.92
-Requires-Dist: huaweicloudsdkcbr ==3.1.92
-Requires-Dist: huaweicloudsdkcbs ==3.1.92
-Requires-Dist: huaweicloudsdkcc ==3.1.92
-Requires-Dist: huaweicloudsdkcce ==3.1.92
-Requires-Dist: huaweicloudsdkccm ==3.1.92
-Requires-Dist: huaweicloudsdkcdm ==3.1.92
-Requires-Dist: huaweicloudsdkcdn ==3.1.92
-Requires-Dist: huaweicloudsdkces ==3.1.92
-Requires-Dist: huaweicloudsdkcfw ==3.1.92
-Requires-Dist: huaweicloudsdkcgs ==3.1.92
-Requires-Dist: huaweicloudsdkclassroom ==3.1.92
-Requires-Dist: huaweicloudsdkcloudide ==3.1.92
-Requires-Dist: huaweicloudsdkcloudpond ==3.1.92
-Requires-Dist: huaweicloudsdkcloudrtc ==3.1.92
-Requires-Dist: huaweicloudsdkcloudtable ==3.1.92
-Requires-Dist: huaweicloudsdkcloudtest ==3.1.92
-Requires-Dist: huaweicloudsdkcodeartsartifact ==3.1.92
-Requires-Dist: huaweicloudsdkcodeartsbuild ==3.1.92
-Requires-Dist: huaweicloudsdkcodeartscheck ==3.1.92
-Requires-Dist: huaweicloudsdkcodeartsdeploy ==3.1.92
-Requires-Dist: huaweicloudsdkcodeartsinspector ==3.1.92
-Requires-Dist: huaweicloudsdkcodeartspipeline ==3.1.92
-Requires-Dist: huaweicloudsdkcodecraft ==3.1.92
-Requires-Dist: huaweicloudsdkcodehub ==3.1.92
-Requires-Dist: huaweicloudsdkconfig ==3.1.92
-Requires-Dist: huaweicloudsdkcph ==3.1.92
-Requires-Dist: huaweicloudsdkcpts ==3.1.92
-Requires-Dist: huaweicloudsdkcse ==3.1.92
-Requires-Dist: huaweicloudsdkcsms ==3.1.92
-Requires-Dist: huaweicloudsdkcss ==3.1.92
-Requires-Dist: huaweicloudsdkcts ==3.1.92
-Requires-Dist: huaweicloudsdkdas ==3.1.92
-Requires-Dist: huaweicloudsdkdataartsstudio ==3.1.92
-Requires-Dist: huaweicloudsdkdbss ==3.1.92
-Requires-Dist: huaweicloudsdkdc ==3.1.92
-Requires-Dist: huaweicloudsdkdcs ==3.1.92
-Requires-Dist: huaweicloudsdkddm ==3.1.92
-Requires-Dist: huaweicloudsdkdds ==3.1.92
-Requires-Dist: huaweicloudsdkdeh ==3.1.92
-Requires-Dist: huaweicloudsdkdevsecurity ==3.1.92
-Requires-Dist: huaweicloudsdkdevstar ==3.1.92
-Requires-Dist: huaweicloudsdkdgc ==3.1.92
-Requires-Dist: huaweicloudsdkdis ==3.1.92
-Requires-Dist: huaweicloudsdkdlf ==3.1.92
-Requires-Dist: huaweicloudsdkdli ==3.1.92
-Requires-Dist: huaweicloudsdkdns ==3.1.92
-Requires-Dist: huaweicloudsdkdris ==3.1.92
-Requires-Dist: huaweicloudsdkdrs ==3.1.92
-Requires-Dist: huaweicloudsdkdsc ==3.1.92
-Requires-Dist: huaweicloudsdkdwr ==3.1.92
-Requires-Dist: huaweicloudsdkdws ==3.1.92
-Requires-Dist: huaweicloudsdkec ==3.1.92
-Requires-Dist: huaweicloudsdkecs ==3.1.92
-Requires-Dist: huaweicloudsdkedgesec ==3.1.92
-Requires-Dist: huaweicloudsdkeg ==3.1.92
-Requires-Dist: huaweicloudsdkeihealth ==3.1.92
-Requires-Dist: huaweicloudsdkeip ==3.1.92
-Requires-Dist: huaweicloudsdkelb ==3.1.92
-Requires-Dist: huaweicloudsdkeps ==3.1.92
-Requires-Dist: huaweicloudsdker ==3.1.92
-Requires-Dist: huaweicloudsdkevs ==3.1.92
-Requires-Dist: huaweicloudsdkfrs ==3.1.92
-Requires-Dist: huaweicloudsdkfunctiongraph ==3.1.92
-Requires-Dist: huaweicloudsdkga ==3.1.92
-Requires-Dist: huaweicloudsdkgaussdb ==3.1.92
-Requires-Dist: huaweicloudsdkgaussdbfornosql ==3.1.92
-Requires-Dist: huaweicloudsdkgaussdbforopengauss ==3.1.92
-Requires-Dist: huaweicloudsdkgeip ==3.1.92
-Requires-Dist: huaweicloudsdkges ==3.1.92
-Requires-Dist: huaweicloudsdkgsl ==3.1.92
-Requires-Dist: huaweicloudsdkhilens ==3.1.92
-Requires-Dist: huaweicloudsdkhss ==3.1.92
-Requires-Dist: huaweicloudsdkiam ==3.1.92
-Requires-Dist: huaweicloudsdkiamaccessanalyzer ==3.1.92
-Requires-Dist: huaweicloudsdkidentitycenter ==3.1.92
-Requires-Dist: huaweicloudsdkidentitycenterstore ==3.1.92
-Requires-Dist: huaweicloudsdkidme ==3.1.92
-Requires-Dist: huaweicloudsdkidmeclassicapi ==3.1.92
-Requires-Dist: huaweicloudsdkiec ==3.1.92
-Requires-Dist: huaweicloudsdkief ==3.1.92
-Requires-Dist: huaweicloudsdkimage ==3.1.92
-Requires-Dist: huaweicloudsdkimagesearch ==3.1.92
-Requires-Dist: huaweicloudsdkims ==3.1.92
-Requires-Dist: huaweicloudsdkiotanalytics ==3.1.92
-Requires-Dist: huaweicloudsdkiotda ==3.1.92
-Requires-Dist: huaweicloudsdkiotedge ==3.1.92
-Requires-Dist: huaweicloudsdkivs ==3.1.92
-Requires-Dist: huaweicloudsdkkafka ==3.1.92
-Requires-Dist: huaweicloudsdkkms ==3.1.92
-Requires-Dist: huaweicloudsdkkoomessage ==3.1.92
-Requires-Dist: huaweicloudsdkkps ==3.1.92
-Requires-Dist: huaweicloudsdklakeformation ==3.1.92
-Requires-Dist: huaweicloudsdklive ==3.1.92
-Requires-Dist: huaweicloudsdklts ==3.1.92
-Requires-Dist: huaweicloudsdkmapds ==3.1.92
-Requires-Dist: huaweicloudsdkmas ==3.1.92
-Requires-Dist: huaweicloudsdkmeeting ==3.1.92
-Requires-Dist: huaweicloudsdkmetastudio ==3.1.92
-Requires-Dist: huaweicloudsdkmoderation ==3.1.92
-Requires-Dist: huaweicloudsdkmpc ==3.1.92
-Requires-Dist: huaweicloudsdkmrs ==3.1.92
-Requires-Dist: huaweicloudsdkmsgsms ==3.1.92
-Requires-Dist: huaweicloudsdkmssi ==3.1.92
-Requires-Dist: huaweicloudsdknat ==3.1.92
-Requires-Dist: huaweicloudsdknlp ==3.1.92
-Requires-Dist: huaweicloudsdkobs ==3.1.92
-Requires-Dist: huaweicloudsdkocr ==3.1.92
-Requires-Dist: huaweicloudsdkoctopus ==3.1.92
-Requires-Dist: huaweicloudsdkoms ==3.1.92
-Requires-Dist: huaweicloudsdkoptverse ==3.1.92
-Requires-Dist: huaweicloudsdkorganizations ==3.1.92
-Requires-Dist: huaweicloudsdkorgid ==3.1.92
-Requires-Dist: huaweicloudsdkoroas ==3.1.92
-Requires-Dist: huaweicloudsdkosm ==3.1.92
-Requires-Dist: huaweicloudsdkpangulargemodels ==3.1.92
-Requires-Dist: huaweicloudsdkprojectman ==3.1.92
-Requires-Dist: huaweicloudsdkrabbitmq ==3.1.92
-Requires-Dist: huaweicloudsdkram ==3.1.92
-Requires-Dist: huaweicloudsdkrds ==3.1.92
-Requires-Dist: huaweicloudsdkres ==3.1.92
-Requires-Dist: huaweicloudsdkrgc ==3.1.92
-Requires-Dist: huaweicloudsdkrms ==3.1.92
-Requires-Dist: huaweicloudsdkrocketmq ==3.1.92
-Requires-Dist: huaweicloudsdkroma ==3.1.92
-Requires-Dist: huaweicloudsdksa ==3.1.92
-Requires-Dist: huaweicloudsdkscm ==3.1.92
-Requires-Dist: huaweicloudsdksdrs ==3.1.92
-Requires-Dist: huaweicloudsdksecmaster ==3.1.92
-Requires-Dist: huaweicloudsdkservicestage ==3.1.92
-Requires-Dist: huaweicloudsdksfsturbo ==3.1.92
-Requires-Dist: huaweicloudsdksis ==3.1.92
-Requires-Dist: huaweicloudsdksmn ==3.1.92
-Requires-Dist: huaweicloudsdksms ==3.1.92
-Requires-Dist: huaweicloudsdksts ==3.1.92
-Requires-Dist: huaweicloudsdkswr ==3.1.92
-Requires-Dist: huaweicloudsdktics ==3.1.92
-Requires-Dist: huaweicloudsdktms ==3.1.92
-Requires-Dist: huaweicloudsdkugo ==3.1.92
-Requires-Dist: huaweicloudsdkvas ==3.1.92
-Requires-Dist: huaweicloudsdkvcm ==3.1.92
-Requires-Dist: huaweicloudsdkvod ==3.1.92
-Requires-Dist: huaweicloudsdkvpc ==3.1.92
-Requires-Dist: huaweicloudsdkvpcep ==3.1.92
-Requires-Dist: huaweicloudsdkvpn ==3.1.92
-Requires-Dist: huaweicloudsdkwaf ==3.1.92
-Requires-Dist: huaweicloudsdkworkspace ==3.1.92
-Requires-Dist: huaweicloudsdkworkspaceapp ==3.1.92
+Requires-Dist: huaweicloudsdkcore ==3.1.93
+Requires-Dist: huaweicloudsdkaad ==3.1.93
+Requires-Dist: huaweicloudsdkantiddos ==3.1.93
+Requires-Dist: huaweicloudsdkaom ==3.1.93
+Requires-Dist: huaweicloudsdkaos ==3.1.93
+Requires-Dist: huaweicloudsdkapig ==3.1.93
+Requires-Dist: huaweicloudsdkapm ==3.1.93
+Requires-Dist: huaweicloudsdkas ==3.1.93
+Requires-Dist: huaweicloudsdkasm ==3.1.93
+Requires-Dist: huaweicloudsdkbcs ==3.1.93
+Requires-Dist: huaweicloudsdkbms ==3.1.93
+Requires-Dist: huaweicloudsdkbss ==3.1.93
+Requires-Dist: huaweicloudsdkbssintl ==3.1.93
+Requires-Dist: huaweicloudsdkcae ==3.1.93
+Requires-Dist: huaweicloudsdkcampusgo ==3.1.93
+Requires-Dist: huaweicloudsdkcbh ==3.1.93
+Requires-Dist: huaweicloudsdkcbr ==3.1.93
+Requires-Dist: huaweicloudsdkcbs ==3.1.93
+Requires-Dist: huaweicloudsdkcc ==3.1.93
+Requires-Dist: huaweicloudsdkcce ==3.1.93
+Requires-Dist: huaweicloudsdkccm ==3.1.93
+Requires-Dist: huaweicloudsdkcdm ==3.1.93
+Requires-Dist: huaweicloudsdkcdn ==3.1.93
+Requires-Dist: huaweicloudsdkces ==3.1.93
+Requires-Dist: huaweicloudsdkcfw ==3.1.93
+Requires-Dist: huaweicloudsdkcgs ==3.1.93
+Requires-Dist: huaweicloudsdkclassroom ==3.1.93
+Requires-Dist: huaweicloudsdkcloudide ==3.1.93
+Requires-Dist: huaweicloudsdkcloudpond ==3.1.93
+Requires-Dist: huaweicloudsdkcloudrtc ==3.1.93
+Requires-Dist: huaweicloudsdkcloudtable ==3.1.93
+Requires-Dist: huaweicloudsdkcloudtest ==3.1.93
+Requires-Dist: huaweicloudsdkcodeartsartifact ==3.1.93
+Requires-Dist: huaweicloudsdkcodeartsbuild ==3.1.93
+Requires-Dist: huaweicloudsdkcodeartscheck ==3.1.93
+Requires-Dist: huaweicloudsdkcodeartsdeploy ==3.1.93
+Requires-Dist: huaweicloudsdkcodeartsinspector ==3.1.93
+Requires-Dist: huaweicloudsdkcodeartspipeline ==3.1.93
+Requires-Dist: huaweicloudsdkcodecraft ==3.1.93
+Requires-Dist: huaweicloudsdkcodehub ==3.1.93
+Requires-Dist: huaweicloudsdkconfig ==3.1.93
+Requires-Dist: huaweicloudsdkcph ==3.1.93
+Requires-Dist: huaweicloudsdkcpts ==3.1.93
+Requires-Dist: huaweicloudsdkcse ==3.1.93
+Requires-Dist: huaweicloudsdkcsms ==3.1.93
+Requires-Dist: huaweicloudsdkcss ==3.1.93
+Requires-Dist: huaweicloudsdkcts ==3.1.93
+Requires-Dist: huaweicloudsdkdas ==3.1.93
+Requires-Dist: huaweicloudsdkdataartsstudio ==3.1.93
+Requires-Dist: huaweicloudsdkdbss ==3.1.93
+Requires-Dist: huaweicloudsdkdc ==3.1.93
+Requires-Dist: huaweicloudsdkdcs ==3.1.93
+Requires-Dist: huaweicloudsdkddm ==3.1.93
+Requires-Dist: huaweicloudsdkdds ==3.1.93
+Requires-Dist: huaweicloudsdkdeh ==3.1.93
+Requires-Dist: huaweicloudsdkdevsecurity ==3.1.93
+Requires-Dist: huaweicloudsdkdevstar ==3.1.93
+Requires-Dist: huaweicloudsdkdgc ==3.1.93
+Requires-Dist: huaweicloudsdkdis ==3.1.93
+Requires-Dist: huaweicloudsdkdlf ==3.1.93
+Requires-Dist: huaweicloudsdkdli ==3.1.93
+Requires-Dist: huaweicloudsdkdns ==3.1.93
+Requires-Dist: huaweicloudsdkdris ==3.1.93
+Requires-Dist: huaweicloudsdkdrs ==3.1.93
+Requires-Dist: huaweicloudsdkdsc ==3.1.93
+Requires-Dist: huaweicloudsdkdwr ==3.1.93
+Requires-Dist: huaweicloudsdkdws ==3.1.93
+Requires-Dist: huaweicloudsdkec ==3.1.93
+Requires-Dist: huaweicloudsdkecs ==3.1.93
+Requires-Dist: huaweicloudsdkedgesec ==3.1.93
+Requires-Dist: huaweicloudsdkeg ==3.1.93
+Requires-Dist: huaweicloudsdkeihealth ==3.1.93
+Requires-Dist: huaweicloudsdkeip ==3.1.93
+Requires-Dist: huaweicloudsdkelb ==3.1.93
+Requires-Dist: huaweicloudsdkeps ==3.1.93
+Requires-Dist: huaweicloudsdker ==3.1.93
+Requires-Dist: huaweicloudsdkevs ==3.1.93
+Requires-Dist: huaweicloudsdkfrs ==3.1.93
+Requires-Dist: huaweicloudsdkfunctiongraph ==3.1.93
+Requires-Dist: huaweicloudsdkga ==3.1.93
+Requires-Dist: huaweicloudsdkgaussdb ==3.1.93
+Requires-Dist: huaweicloudsdkgaussdbfornosql ==3.1.93
+Requires-Dist: huaweicloudsdkgaussdbforopengauss ==3.1.93
+Requires-Dist: huaweicloudsdkgeip ==3.1.93
+Requires-Dist: huaweicloudsdkges ==3.1.93
+Requires-Dist: huaweicloudsdkgsl ==3.1.93
+Requires-Dist: huaweicloudsdkhilens ==3.1.93
+Requires-Dist: huaweicloudsdkhss ==3.1.93
+Requires-Dist: huaweicloudsdkiam ==3.1.93
+Requires-Dist: huaweicloudsdkiamaccessanalyzer ==3.1.93
+Requires-Dist: huaweicloudsdkidentitycenter ==3.1.93
+Requires-Dist: huaweicloudsdkidentitycenterstore ==3.1.93
+Requires-Dist: huaweicloudsdkidme ==3.1.93
+Requires-Dist: huaweicloudsdkidmeclassicapi ==3.1.93
+Requires-Dist: huaweicloudsdkiec ==3.1.93
+Requires-Dist: huaweicloudsdkief ==3.1.93
+Requires-Dist: huaweicloudsdkimage ==3.1.93
+Requires-Dist: huaweicloudsdkimagesearch ==3.1.93
+Requires-Dist: huaweicloudsdkims ==3.1.93
+Requires-Dist: huaweicloudsdkiotanalytics ==3.1.93
+Requires-Dist: huaweicloudsdkiotda ==3.1.93
+Requires-Dist: huaweicloudsdkiotedge ==3.1.93
+Requires-Dist: huaweicloudsdkivs ==3.1.93
+Requires-Dist: huaweicloudsdkkafka ==3.1.93
+Requires-Dist: huaweicloudsdkkms ==3.1.93
+Requires-Dist: huaweicloudsdkkoomessage ==3.1.93
+Requires-Dist: huaweicloudsdkkps ==3.1.93
+Requires-Dist: huaweicloudsdklakeformation ==3.1.93
+Requires-Dist: huaweicloudsdklive ==3.1.93
+Requires-Dist: huaweicloudsdklts ==3.1.93
+Requires-Dist: huaweicloudsdkmapds ==3.1.93
+Requires-Dist: huaweicloudsdkmas ==3.1.93
+Requires-Dist: huaweicloudsdkmeeting ==3.1.93
+Requires-Dist: huaweicloudsdkmetastudio ==3.1.93
+Requires-Dist: huaweicloudsdkmoderation ==3.1.93
+Requires-Dist: huaweicloudsdkmpc ==3.1.93
+Requires-Dist: huaweicloudsdkmrs ==3.1.93
+Requires-Dist: huaweicloudsdkmsgsms ==3.1.93
+Requires-Dist: huaweicloudsdkmssi ==3.1.93
+Requires-Dist: huaweicloudsdknat ==3.1.93
+Requires-Dist: huaweicloudsdknlp ==3.1.93
+Requires-Dist: huaweicloudsdkobs ==3.1.93
+Requires-Dist: huaweicloudsdkocr ==3.1.93
+Requires-Dist: huaweicloudsdkoctopus ==3.1.93
+Requires-Dist: huaweicloudsdkoms ==3.1.93
+Requires-Dist: huaweicloudsdkoptverse ==3.1.93
+Requires-Dist: huaweicloudsdkorganizations ==3.1.93
+Requires-Dist: huaweicloudsdkorgid ==3.1.93
+Requires-Dist: huaweicloudsdkoroas ==3.1.93
+Requires-Dist: huaweicloudsdkosm ==3.1.93
+Requires-Dist: huaweicloudsdkpangulargemodels ==3.1.93
+Requires-Dist: huaweicloudsdkprojectman ==3.1.93
+Requires-Dist: huaweicloudsdkrabbitmq ==3.1.93
+Requires-Dist: huaweicloudsdkram ==3.1.93
+Requires-Dist: huaweicloudsdkrds ==3.1.93
+Requires-Dist: huaweicloudsdkres ==3.1.93
+Requires-Dist: huaweicloudsdkrgc ==3.1.93
+Requires-Dist: huaweicloudsdkrms ==3.1.93
+Requires-Dist: huaweicloudsdkrocketmq ==3.1.93
+Requires-Dist: huaweicloudsdkroma ==3.1.93
+Requires-Dist: huaweicloudsdksa ==3.1.93
+Requires-Dist: huaweicloudsdkscm ==3.1.93
+Requires-Dist: huaweicloudsdksdrs ==3.1.93
+Requires-Dist: huaweicloudsdksecmaster ==3.1.93
+Requires-Dist: huaweicloudsdkservicestage ==3.1.93
+Requires-Dist: huaweicloudsdksfsturbo ==3.1.93
+Requires-Dist: huaweicloudsdksis ==3.1.93
+Requires-Dist: huaweicloudsdksmn ==3.1.93
+Requires-Dist: huaweicloudsdksms ==3.1.93
+Requires-Dist: huaweicloudsdksts ==3.1.93
+Requires-Dist: huaweicloudsdkswr ==3.1.93
+Requires-Dist: huaweicloudsdktics ==3.1.93
+Requires-Dist: huaweicloudsdktms ==3.1.93
+Requires-Dist: huaweicloudsdkugo ==3.1.93
+Requires-Dist: huaweicloudsdkvas ==3.1.93
+Requires-Dist: huaweicloudsdkvcm ==3.1.93
+Requires-Dist: huaweicloudsdkvod ==3.1.93
+Requires-Dist: huaweicloudsdkvpc ==3.1.93
+Requires-Dist: huaweicloudsdkvpcep ==3.1.93
+Requires-Dist: huaweicloudsdkvpn ==3.1.93
+Requires-Dist: huaweicloudsdkwaf ==3.1.93
+Requires-Dist: huaweicloudsdkworkspace ==3.1.93
+Requires-Dist: huaweicloudsdkworkspaceapp ==3.1.93
 
 See detailed information in [huaweicloud-sdk-python-v3](https://github.com/huaweicloud/huaweicloud-sdk-python-v3).
```

## Comparing `huaweicloudsdkall-3.1.92.dist-info/RECORD` & `huaweicloudsdkall-3.1.93.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 huaweicloudsdkall/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-huaweicloudsdkall-3.1.92.dist-info/LICENSE,sha256=4_VSTLuxcsybRG9N4Isktlj1rAIBBsfl0Tjc0gBTijo,604
-huaweicloudsdkall-3.1.92.dist-info/METADATA,sha256=gImpH5C-DLKdUGu1vqwHH9ipFDoI1plonUJKdaksX6g,8398
-huaweicloudsdkall-3.1.92.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-huaweicloudsdkall-3.1.92.dist-info/top_level.txt,sha256=3zNGA8EzECoGWbYN8v-8zOtqzLiVJeKnZWNEZUcZBS4,18
-huaweicloudsdkall-3.1.92.dist-info/RECORD,,
+huaweicloudsdkall-3.1.93.dist-info/LICENSE,sha256=4_VSTLuxcsybRG9N4Isktlj1rAIBBsfl0Tjc0gBTijo,604
+huaweicloudsdkall-3.1.93.dist-info/METADATA,sha256=M1LDmRVRBBG6M-VRV5A8roJwfGCCVp_MfM5KAePp8Ok,8398
+huaweicloudsdkall-3.1.93.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+huaweicloudsdkall-3.1.93.dist-info/top_level.txt,sha256=3zNGA8EzECoGWbYN8v-8zOtqzLiVJeKnZWNEZUcZBS4,18
+huaweicloudsdkall-3.1.93.dist-info/RECORD,,
```


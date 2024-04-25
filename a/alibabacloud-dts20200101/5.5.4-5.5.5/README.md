# Comparing `tmp/alibabacloud_dts20200101-5.5.4.tar.gz` & `tmp/alibabacloud_dts20200101-5.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dts20200101-5.5.4.tar", last modified: Thu Apr 11 17:13:09 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dts20200101-5.5.5.tar", last modified: Thu Apr 25 17:16:50 2024, max compression
```

## Comparing `alibabacloud_dts20200101-5.5.4.tar` & `alibabacloud_dts20200101-5.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/
--rw-r--r--   0 root         (0) root         (0)     9762 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   605758 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/client.py
--rw-r--r--   0 root         (0) root         (0)  1711725 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2816 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/
+-rw-r--r--   0 root         (0) root         (0)     9884 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   606500 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1712619 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 17:16:50.000000 alibabacloud_dts20200101-5.5.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-04-25 17:16:49.000000 alibabacloud_dts20200101-5.5.5/setup.py
```

### Comparing `alibabacloud_dts20200101-5.5.4/ChangeLog.md` & `alibabacloud_dts20200101-5.5.5/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-11 Version: 5.5.4
+- Update API TransferPayType: add param MaxDu.
+- Update API TransferPayType: add param MinDu.
+
+
 2024-03-29 Version: 5.5.3
 - Update API ConfigureDtsJob: add param MaxDu.
 - Update API ConfigureDtsJob: add param MinDu.
 - Update API ConfigureDtsJob: add param ResourceGroupId.
 - Update API ConfigureMigrationJob: add param ResourceGroupId.
 - Update API ConfigureMigrationJobAlert: add param ResourceGroupId.
 - Update API ConfigureSubscription: add param MaxDu.
```

### Comparing `alibabacloud_dts20200101-5.5.4/LICENSE` & `alibabacloud_dts20200101-5.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.5.4/PKG-INFO` & `alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dts20200101
-Version: 5.5.4
+Name: alibabacloud-dts20200101
+Version: 5.5.5
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101-5.5.4/README-CN.md` & `alibabacloud_dts20200101-5.5.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.5.4/README.md` & `alibabacloud_dts20200101-5.5.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/client.py` & `alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2541,14 +2541,18 @@
     ) -> dts_20200101_models.CreateReverseDtsJobResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.shard_password):
+            query['ShardPassword'] = request.shard_password
+        if not UtilClient.is_unset(request.shard_username):
+            query['ShardUsername'] = request.shard_username
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateReverseDtsJob',
             version='2020-01-01',
             protocol='HTTPS',
@@ -2571,14 +2575,18 @@
     ) -> dts_20200101_models.CreateReverseDtsJobResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.shard_password):
+            query['ShardPassword'] = request.shard_password
+        if not UtilClient.is_unset(request.shard_username):
+            query['ShardUsername'] = request.shard_username
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateReverseDtsJob',
             version='2020-01-01',
             protocol='HTTPS',
@@ -9015,14 +9023,16 @@
             query['EndpointInstanceId'] = request.endpoint_instance_id
         if not UtilClient.is_unset(request.endpoint_instance_type):
             query['EndpointInstanceType'] = request.endpoint_instance_type
         if not UtilClient.is_unset(request.endpoint_ip):
             query['EndpointIp'] = request.endpoint_ip
         if not UtilClient.is_unset(request.endpoint_port):
             query['EndpointPort'] = request.endpoint_port
+        if not UtilClient.is_unset(request.endpoint_region_id):
+            query['EndpointRegionId'] = request.endpoint_region_id
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.role_name):
@@ -9077,14 +9087,16 @@
             query['EndpointInstanceId'] = request.endpoint_instance_id
         if not UtilClient.is_unset(request.endpoint_instance_type):
             query['EndpointInstanceType'] = request.endpoint_instance_type
         if not UtilClient.is_unset(request.endpoint_ip):
             query['EndpointIp'] = request.endpoint_ip
         if not UtilClient.is_unset(request.endpoint_port):
             query['EndpointPort'] = request.endpoint_port
+        if not UtilClient.is_unset(request.endpoint_region_id):
+            query['EndpointRegionId'] = request.endpoint_region_id
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.role_name):
```

### Comparing `alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/models.py` & `alibabacloud_dts20200101-5.5.5/alibabacloud_dts20200101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5512,39 +5512,51 @@
 
 
 class CreateReverseDtsJobRequest(TeaModel):
     def __init__(
         self,
         dts_job_id: str = None,
         resource_group_id: str = None,
+        shard_password: str = None,
+        shard_username: str = None,
     ):
         self.dts_job_id = dts_job_id
         self.resource_group_id = resource_group_id
+        self.shard_password = shard_password
+        self.shard_username = shard_username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.dts_job_id is not None:
             result['DtsJobId'] = self.dts_job_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        if self.shard_password is not None:
+            result['ShardPassword'] = self.shard_password
+        if self.shard_username is not None:
+            result['ShardUsername'] = self.shard_username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DtsJobId') is not None:
             self.dts_job_id = m.get('DtsJobId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('ShardPassword') is not None:
+            self.shard_password = m.get('ShardPassword')
+        if m.get('ShardUsername') is not None:
+            self.shard_username = m.get('ShardUsername')
         return self
 
 
 class CreateReverseDtsJobResponseBody(TeaModel):
     def __init__(
         self,
         dts_instance_id: str = None,
@@ -35729,14 +35741,15 @@
         dts_instance_id: str = None,
         dts_job_id: str = None,
         endpoint: str = None,
         endpoint_instance_id: str = None,
         endpoint_instance_type: str = None,
         endpoint_ip: str = None,
         endpoint_port: str = None,
+        endpoint_region_id: str = None,
         password: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         role_name: str = None,
         shard_password: str = None,
         shard_username: str = None,
         synchronization_direction: str = None,
@@ -35748,14 +35761,15 @@
         self.dts_instance_id = dts_instance_id
         self.dts_job_id = dts_job_id
         self.endpoint = endpoint
         self.endpoint_instance_id = endpoint_instance_id
         self.endpoint_instance_type = endpoint_instance_type
         self.endpoint_ip = endpoint_ip
         self.endpoint_port = endpoint_port
+        self.endpoint_region_id = endpoint_region_id
         self.password = password
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.role_name = role_name
         self.shard_password = shard_password
         self.shard_username = shard_username
         self.synchronization_direction = synchronization_direction
@@ -35786,14 +35800,16 @@
             result['EndpointInstanceId'] = self.endpoint_instance_id
         if self.endpoint_instance_type is not None:
             result['EndpointInstanceType'] = self.endpoint_instance_type
         if self.endpoint_ip is not None:
             result['EndpointIp'] = self.endpoint_ip
         if self.endpoint_port is not None:
             result['EndpointPort'] = self.endpoint_port
+        if self.endpoint_region_id is not None:
+            result['EndpointRegionId'] = self.endpoint_region_id
         if self.password is not None:
             result['Password'] = self.password
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.role_name is not None:
@@ -35826,14 +35842,16 @@
             self.endpoint_instance_id = m.get('EndpointInstanceId')
         if m.get('EndpointInstanceType') is not None:
             self.endpoint_instance_type = m.get('EndpointInstanceType')
         if m.get('EndpointIp') is not None:
             self.endpoint_ip = m.get('EndpointIp')
         if m.get('EndpointPort') is not None:
             self.endpoint_port = m.get('EndpointPort')
+        if m.get('EndpointRegionId') is not None:
+            self.endpoint_region_id = m.get('EndpointRegionId')
         if m.get('Password') is not None:
             self.password = m.get('Password')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('RoleName') is not None:
```

### Comparing `alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/PKG-INFO` & `alibabacloud_dts20200101-5.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dts20200101
-Version: 5.5.4
+Name: alibabacloud_dts20200101
+Version: 5.5.5
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101-5.5.4/setup.py` & `alibabacloud_dts20200101-5.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dts20200101.
 
-Created on 11/04/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dts20200101"
 NAME = "alibabacloud_dts20200101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Data Transmission (20200101) SDK Library for Python"
```


# Comparing `tmp/alibabacloud_dts20200101_py2-1.3.3.tar.gz` & `tmp/alibabacloud_dts20200101_py2-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dts20200101_py2-1.3.3.tar", last modified: Thu Apr 11 17:12:22 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dts20200101_py2-1.3.4.tar", last modified: Thu Apr 25 17:15:56 2024, max compression
```

## Comparing `alibabacloud_dts20200101_py2-1.3.3.tar` & `alibabacloud_dts20200101_py2-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/
--rw-r--r--   0 root         (0) root         (0)     9165 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2486 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   269829 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/client.py
--rw-r--r--   0 root         (0) root         (0)  1728431 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2486 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3124 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)     9287 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   270200 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1729319 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3124 2024-04-25 17:15:56.000000 alibabacloud_dts20200101_py2-1.3.4/setup.py
```

### Comparing `alibabacloud_dts20200101_py2-1.3.3/ChangeLog.md` & `alibabacloud_dts20200101_py2-1.3.4/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-11 Version: 1.3.3
+- Update API TransferPayType: add param MaxDu.
+- Update API TransferPayType: add param MinDu.
+
+
 2024-03-29 Version: 1.3.2
 - Update API ConfigureDtsJob: add param MaxDu.
 - Update API ConfigureDtsJob: add param MinDu.
 - Update API ConfigureDtsJob: add param ResourceGroupId.
 - Update API ConfigureMigrationJob: add param ResourceGroupId.
 - Update API ConfigureMigrationJobAlert: add param ResourceGroupId.
 - Update API ConfigureSubscription: add param MaxDu.
```

### Comparing `alibabacloud_dts20200101_py2-1.3.3/LICENSE` & `alibabacloud_dts20200101_py2-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101_py2-1.3.3/PKG-INFO` & `alibabacloud_dts20200101_py2-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dts20200101_py2
-Version: 1.3.3
+Version: 1.3.4
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101_py2-1.3.3/README-CN.md` & `alibabacloud_dts20200101_py2-1.3.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101_py2-1.3.3/README.md` & `alibabacloud_dts20200101_py2-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/client.py` & `alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1236,14 +1236,18 @@
     def create_reverse_dts_job_with_options(self, request, runtime):
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
@@ -4147,14 +4151,16 @@
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

### Comparing `alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/models.py` & `alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4974,39 +4974,49 @@
         if m.get('body') is not None:
             temp_model = CreateMigrationJobResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateReverseDtsJobRequest(TeaModel):
-    def __init__(self, dts_job_id=None, resource_group_id=None):
+    def __init__(self, dts_job_id=None, resource_group_id=None, shard_password=None, shard_username=None):
         self.dts_job_id = dts_job_id  # type: str
         self.resource_group_id = resource_group_id  # type: str
+        self.shard_password = shard_password  # type: str
+        self.shard_username = shard_username  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateReverseDtsJobRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, dts_instance_id=None, dts_job_id=None, err_code=None, err_message=None,
                  http_status_code=None, request_id=None, success=None):
         self.dts_instance_id = dts_instance_id  # type: str
@@ -31847,26 +31857,27 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyDtsJobEndpointRequest(TeaModel):
     def __init__(self, aliyun_uid=None, database=None, dry_run=None, dts_instance_id=None, dts_job_id=None,
                  endpoint=None, endpoint_instance_id=None, endpoint_instance_type=None, endpoint_ip=None,
-                 endpoint_port=None, password=None, region_id=None, resource_group_id=None, role_name=None, shard_password=None,
-                 shard_username=None, synchronization_direction=None, username=None):
+                 endpoint_port=None, endpoint_region_id=None, password=None, region_id=None, resource_group_id=None,
+                 role_name=None, shard_password=None, shard_username=None, synchronization_direction=None, username=None):
         self.aliyun_uid = aliyun_uid  # type: str
         self.database = database  # type: str
         self.dry_run = dry_run  # type: bool
         self.dts_instance_id = dts_instance_id  # type: str
         self.dts_job_id = dts_job_id  # type: str
         self.endpoint = endpoint  # type: str
         self.endpoint_instance_id = endpoint_instance_id  # type: str
         self.endpoint_instance_type = endpoint_instance_type  # type: str
         self.endpoint_ip = endpoint_ip  # type: str
         self.endpoint_port = endpoint_port  # type: str
+        self.endpoint_region_id = endpoint_region_id  # type: str
         self.password = password  # type: str
         self.region_id = region_id  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.role_name = role_name  # type: str
         self.shard_password = shard_password  # type: str
         self.shard_username = shard_username  # type: str
         self.synchronization_direction = synchronization_direction  # type: str
@@ -31897,14 +31908,16 @@
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
@@ -31937,14 +31950,16 @@
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

### Comparing `alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/PKG-INFO` & `alibabacloud_dts20200101_py2-1.3.4/alibabacloud_dts20200101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dts20200101-py2
-Version: 1.3.3
+Version: 1.3.4
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101_py2-1.3.3/setup.py` & `alibabacloud_dts20200101_py2-1.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dts20200101_py2.
 
-Created on 11/04/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dts20200101"
 NAME = "alibabacloud_dts20200101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Data Transmission (20200101) SDK Library for Python2"
```


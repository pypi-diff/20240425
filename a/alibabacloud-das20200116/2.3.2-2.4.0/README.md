# Comparing `tmp/alibabacloud_das20200116-2.3.2.tar.gz` & `tmp/alibabacloud_das20200116-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_das20200116-2.3.2.tar", last modified: Tue Feb 27 17:21:35 2024, max compression
+gzip compressed data, was "dist/alibabacloud_das20200116-2.4.0.tar", last modified: Thu Apr 25 17:16:48 2024, max compression
```

## Comparing `alibabacloud_das20200116-2.3.2.tar` & `alibabacloud_das20200116-2.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/
--rw-r--r--   0 root         (0) root         (0)     2437 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116/client.py
--rw-r--r--   0 root         (0) root         (0)  1080484 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/alibabacloud_das20200116.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-27 17:21:35.000000 alibabacloud_das20200116-2.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-02-27 17:21:34.000000 alibabacloud_das20200116-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   582956 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116/client.py
+-rw-r--r--   0 root         (0) root         (0)  1161644 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/alibabacloud_das20200116.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-25 17:16:48.000000 alibabacloud_das20200116-2.4.0/setup.py
```

### Comparing `alibabacloud_das20200116-2.3.2/ChangeLog.md` & `alibabacloud_das20200116-2.4.0/ChangeLog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2024-02-27 Version: 2.3.2
+- Update API GetPfsSqlSample: update param EndTime.
+- Update API GetPfsSqlSample: update param InstanceId.
+- Update API GetPfsSqlSample: update param StartTime.
+- Update API ModifyAutoScalingConfig: update param Bandwidth.
+- Update API ModifyAutoScalingConfig: update response param.
+
+
 2024-02-21 Version: 2.3.1
 - Generated python 2020-01-16 for DAS.
 
 2023-12-12 Version: 2.3.0
 - Generated python 2020-01-16 for DAS.
 
 2023-12-08 Version: 2.2.0
```

### Comparing `alibabacloud_das20200116-2.3.2/LICENSE` & `alibabacloud_das20200116-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_das20200116-2.3.2/PKG-INFO` & `alibabacloud_das20200116-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_das20200116
-Version: 2.3.2
+Version: 2.4.0
 Summary: Alibaba Cloud DAS (20200116) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_das20200116-2.3.2/README-CN.md` & `alibabacloud_das20200116-2.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_das20200116-2.3.2/README.md` & `alibabacloud_das20200116-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_das20200116-2.3.2/alibabacloud_das20200116/client.py` & `alibabacloud_das20200116-2.4.0/alibabacloud_das20200116/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,20 +198,20 @@
 
     def create_adam_bench_task_with_options(
         self,
         request: das20200116_models.CreateAdamBenchTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.CreateAdamBenchTaskResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You use an ADAM stress testing task to check whether you need to scale up or scale out your database instance to handle workloads during peak hours. For more information, see [Intelligent Stress Testing](~~155068~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You can create an Advanced Database & Application Migration (ADAM) stress testing task to check whether you need to scale up your database instance to handle workloads during peak hours. For more information, see [Intelligent stress testing](~~155068~~).
         Make sure that your database instances meet the following requirements:
-        *   The source instance supports the following database engines: ApsaraDB RDS for MySQL on High-availability Edition or Enterprise Edition, and PolarDB for MySQL on Cluster Edition or X-Engine.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The database instance is connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is activated for the source and destination database instances. For more information, see [DAS Professional Edition](~~190912~~).
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL cluster.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateAdamBenchTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAdamBenchTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -260,20 +260,20 @@
 
     async def create_adam_bench_task_with_options_async(
         self,
         request: das20200116_models.CreateAdamBenchTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.CreateAdamBenchTaskResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You use an ADAM stress testing task to check whether you need to scale up or scale out your database instance to handle workloads during peak hours. For more information, see [Intelligent Stress Testing](~~155068~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You can create an Advanced Database & Application Migration (ADAM) stress testing task to check whether you need to scale up your database instance to handle workloads during peak hours. For more information, see [Intelligent stress testing](~~155068~~).
         Make sure that your database instances meet the following requirements:
-        *   The source instance supports the following database engines: ApsaraDB RDS for MySQL on High-availability Edition or Enterprise Edition, and PolarDB for MySQL on Cluster Edition or X-Engine.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The database instance is connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is activated for the source and destination database instances. For more information, see [DAS Professional Edition](~~190912~~).
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL cluster.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateAdamBenchTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAdamBenchTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -321,38 +321,38 @@
         )
 
     def create_adam_bench_task(
         self,
         request: das20200116_models.CreateAdamBenchTaskRequest,
     ) -> das20200116_models.CreateAdamBenchTaskResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You use an ADAM stress testing task to check whether you need to scale up or scale out your database instance to handle workloads during peak hours. For more information, see [Intelligent Stress Testing](~~155068~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You can create an Advanced Database & Application Migration (ADAM) stress testing task to check whether you need to scale up your database instance to handle workloads during peak hours. For more information, see [Intelligent stress testing](~~155068~~).
         Make sure that your database instances meet the following requirements:
-        *   The source instance supports the following database engines: ApsaraDB RDS for MySQL on High-availability Edition or Enterprise Edition, and PolarDB for MySQL on Cluster Edition or X-Engine.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The database instance is connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is activated for the source and destination database instances. For more information, see [DAS Professional Edition](~~190912~~).
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL cluster.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateAdamBenchTaskRequest
         @return: CreateAdamBenchTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_adam_bench_task_with_options(request, runtime)
 
     async def create_adam_bench_task_async(
         self,
         request: das20200116_models.CreateAdamBenchTaskRequest,
     ) -> das20200116_models.CreateAdamBenchTaskResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You use an ADAM stress testing task to check whether you need to scale up or scale out your database instance to handle workloads during peak hours. For more information, see [Intelligent Stress Testing](~~155068~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. You can create an Advanced Database & Application Migration (ADAM) stress testing task to check whether you need to scale up your database instance to handle workloads during peak hours. For more information, see [Intelligent stress testing](~~155068~~).
         Make sure that your database instances meet the following requirements:
-        *   The source instance supports the following database engines: ApsaraDB RDS for MySQL on High-availability Edition or Enterprise Edition, and PolarDB for MySQL on Cluster Edition or X-Engine.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The database instance is connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is activated for the source and destination database instances. For more information, see [DAS Professional Edition](~~190912~~).
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL cluster.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateAdamBenchTaskRequest
         @return: CreateAdamBenchTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_adam_bench_task_with_options_async(request, runtime)
 
@@ -482,19 +482,19 @@
 
     def create_cloud_bench_tasks_with_options(
         self,
         request: das20200116_models.CreateCloudBenchTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.CreateCloudBenchTasksResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to handle traffic spikes in an effective manner. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
-        *   The source database instance must be an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition instance.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The source instance and the destination instance are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is enabled for the source instance and the destination instance. For more information, see [DAS Professional Edition](~~190912~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to effectively handle traffic spikes. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination database instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateCloudBenchTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateCloudBenchTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -573,19 +573,19 @@
 
     async def create_cloud_bench_tasks_with_options_async(
         self,
         request: das20200116_models.CreateCloudBenchTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.CreateCloudBenchTasksResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to handle traffic spikes in an effective manner. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
-        *   The source database instance must be an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition instance.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The source instance and the destination instance are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is enabled for the source instance and the destination instance. For more information, see [DAS Professional Edition](~~190912~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to effectively handle traffic spikes. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination database instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateCloudBenchTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateCloudBenchTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -663,36 +663,36 @@
         )
 
     def create_cloud_bench_tasks(
         self,
         request: das20200116_models.CreateCloudBenchTasksRequest,
     ) -> das20200116_models.CreateCloudBenchTasksResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to handle traffic spikes in an effective manner. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
-        *   The source database instance must be an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition instance.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The source instance and the destination instance are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is enabled for the source instance and the destination instance. For more information, see [DAS Professional Edition](~~190912~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to effectively handle traffic spikes. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination database instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateCloudBenchTasksRequest
         @return: CreateCloudBenchTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_cloud_bench_tasks_with_options(request, runtime)
 
     async def create_cloud_bench_tasks_async(
         self,
         request: das20200116_models.CreateCloudBenchTasksRequest,
     ) -> das20200116_models.CreateCloudBenchTasksResponse:
         """
-        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to handle traffic spikes in an effective manner. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
-        *   The source database instance must be an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition instance.
-        *   The destination instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
-        *   The source instance and the destination instance are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
-        *   DAS Professional Edition is enabled for the source instance and the destination instance. For more information, see [DAS Professional Edition](~~190912~~).
+        Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to effectively handle traffic spikes. For more information, see [Intelligent stress testing](~~155068~~). Before you call this API operation, make sure that your database instances meet the following requirements:
+        *   The source database instance is an ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition instance, or a PolarDB for MySQL Cluster Edition or X-Engine Edition cluster.
+        *   The destination database instance is an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL instance.
+        *   The source and destination database instances are connected to DAS. For information about how to connect database instances to DAS, see [Connect an Alibaba Cloud database instance to DAS](~~65405~~).
+        *   DAS Enterprise Edition is enabled for the source and destination database instances. For more information, see [Overview](~~190912~~).
         
         @param request: CreateCloudBenchTasksRequest
         @return: CreateCloudBenchTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_cloud_bench_tasks_with_options_async(request, runtime)
 
@@ -1318,14 +1318,116 @@
         
         @param request: CreateRequestDiagnosisRequest
         @return: CreateRequestDiagnosisResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_request_diagnosis_with_options_async(request, runtime)
 
+    def create_sql_log_task_with_options(
+        self,
+        request: das20200116_models.CreateSqlLogTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.CreateSqlLogTaskResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filters):
+            query['Filters'] = request.filters
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.node_id):
+            body['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.type):
+            body['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSqlLogTask',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.CreateSqlLogTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_sql_log_task_with_options_async(
+        self,
+        request: das20200116_models.CreateSqlLogTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.CreateSqlLogTaskResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filters):
+            query['Filters'] = request.filters
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.node_id):
+            body['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.type):
+            body['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSqlLogTask',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.CreateSqlLogTaskResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_sql_log_task(
+        self,
+        request: das20200116_models.CreateSqlLogTaskRequest,
+    ) -> das20200116_models.CreateSqlLogTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_sql_log_task_with_options(request, runtime)
+
+    async def create_sql_log_task_async(
+        self,
+        request: das20200116_models.CreateSqlLogTaskRequest,
+    ) -> das20200116_models.CreateSqlLogTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_sql_log_task_with_options_async(request, runtime)
+
     def create_storage_analysis_task_with_options(
         self,
         request: das20200116_models.CreateStorageAnalysisTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.CreateStorageAnalysisTaskResponse:
         """
         This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters.
@@ -1744,17 +1846,17 @@
 
     def describe_auto_scaling_history_with_options(
         self,
         request: das20200116_models.DescribeAutoScalingHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.DescribeAutoScalingHistoryResponse:
         """
-        You can query only the history of automatic performance scaling of ApsaraDB RDS for MySQL instances.
+        You can call this operation to query the history information about the automatic performance scaling only of ApsaraDB RDS for MySQL High-availability Edition instances.
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeAutoScalingHistoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeAutoScalingHistoryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -1779,17 +1881,17 @@
 
     async def describe_auto_scaling_history_with_options_async(
         self,
         request: das20200116_models.DescribeAutoScalingHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.DescribeAutoScalingHistoryResponse:
         """
-        You can query only the history of automatic performance scaling of ApsaraDB RDS for MySQL instances.
+        You can call this operation to query the history information about the automatic performance scaling only of ApsaraDB RDS for MySQL High-availability Edition instances.
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeAutoScalingHistoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeAutoScalingHistoryResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -1813,32 +1915,32 @@
         )
 
     def describe_auto_scaling_history(
         self,
         request: das20200116_models.DescribeAutoScalingHistoryRequest,
     ) -> das20200116_models.DescribeAutoScalingHistoryResponse:
         """
-        You can query only the history of automatic performance scaling of ApsaraDB RDS for MySQL instances.
+        You can call this operation to query the history information about the automatic performance scaling only of ApsaraDB RDS for MySQL High-availability Edition instances.
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeAutoScalingHistoryRequest
         @return: DescribeAutoScalingHistoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_auto_scaling_history_with_options(request, runtime)
 
     async def describe_auto_scaling_history_async(
         self,
         request: das20200116_models.DescribeAutoScalingHistoryRequest,
     ) -> das20200116_models.DescribeAutoScalingHistoryResponse:
         """
-        You can query only the history of automatic performance scaling of ApsaraDB RDS for MySQL instances.
+        You can call this operation to query the history information about the automatic performance scaling only of ApsaraDB RDS for MySQL High-availability Edition instances.
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeAutoScalingHistoryRequest
         @return: DescribeAutoScalingHistoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_auto_scaling_history_with_options_async(request, runtime)
 
@@ -2784,16 +2886,16 @@
 
     def describe_instance_das_pro_with_options(
         self,
         request: das20200116_models.DescribeInstanceDasProRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.DescribeInstanceDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeInstanceDasProRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeInstanceDasProResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2820,16 +2922,16 @@
 
     async def describe_instance_das_pro_with_options_async(
         self,
         request: das20200116_models.DescribeInstanceDasProRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.DescribeInstanceDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeInstanceDasProRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeInstanceDasProResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2855,37 +2957,455 @@
         )
 
     def describe_instance_das_pro(
         self,
         request: das20200116_models.DescribeInstanceDasProRequest,
     ) -> das20200116_models.DescribeInstanceDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeInstanceDasProRequest
         @return: DescribeInstanceDasProResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_das_pro_with_options(request, runtime)
 
     async def describe_instance_das_pro_async(
         self,
         request: das20200116_models.DescribeInstanceDasProRequest,
     ) -> das20200116_models.DescribeInstanceDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DescribeInstanceDasProRequest
         @return: DescribeInstanceDasProResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_instance_das_pro_with_options_async(request, runtime)
 
+    def describe_sql_log_config_with_options(
+        self,
+        request: das20200116_models.DescribeSqlLogConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogConfigResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogConfig',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_sql_log_config_with_options_async(
+        self,
+        request: das20200116_models.DescribeSqlLogConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogConfigResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogConfig',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_sql_log_config(
+        self,
+        request: das20200116_models.DescribeSqlLogConfigRequest,
+    ) -> das20200116_models.DescribeSqlLogConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sql_log_config_with_options(request, runtime)
+
+    async def describe_sql_log_config_async(
+        self,
+        request: das20200116_models.DescribeSqlLogConfigRequest,
+    ) -> das20200116_models.DescribeSqlLogConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_sql_log_config_with_options_async(request, runtime)
+
+    def describe_sql_log_records_with_options(
+        self,
+        request: das20200116_models.DescribeSqlLogRecordsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogRecordsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filters):
+            query['Filters'] = request.filters
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            body['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogRecords',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogRecordsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_sql_log_records_with_options_async(
+        self,
+        request: das20200116_models.DescribeSqlLogRecordsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogRecordsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filters):
+            query['Filters'] = request.filters
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            body['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogRecords',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogRecordsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_sql_log_records(
+        self,
+        request: das20200116_models.DescribeSqlLogRecordsRequest,
+    ) -> das20200116_models.DescribeSqlLogRecordsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sql_log_records_with_options(request, runtime)
+
+    async def describe_sql_log_records_async(
+        self,
+        request: das20200116_models.DescribeSqlLogRecordsRequest,
+    ) -> das20200116_models.DescribeSqlLogRecordsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_sql_log_records_with_options_async(request, runtime)
+
+    def describe_sql_log_statistic_with_options(
+        self,
+        request: das20200116_models.DescribeSqlLogStatisticRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogStatisticResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogStatistic',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogStatisticResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_sql_log_statistic_with_options_async(
+        self,
+        request: das20200116_models.DescribeSqlLogStatisticRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogStatisticResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogStatistic',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogStatisticResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_sql_log_statistic(
+        self,
+        request: das20200116_models.DescribeSqlLogStatisticRequest,
+    ) -> das20200116_models.DescribeSqlLogStatisticResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sql_log_statistic_with_options(request, runtime)
+
+    async def describe_sql_log_statistic_async(
+        self,
+        request: das20200116_models.DescribeSqlLogStatisticRequest,
+    ) -> das20200116_models.DescribeSqlLogStatisticResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_sql_log_statistic_with_options_async(request, runtime)
+
+    def describe_sql_log_task_with_options(
+        self,
+        request: das20200116_models.DescribeSqlLogTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogTaskResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.task_id):
+            body['TaskId'] = request.task_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogTask',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_sql_log_task_with_options_async(
+        self,
+        request: das20200116_models.DescribeSqlLogTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogTaskResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.task_id):
+            body['TaskId'] = request.task_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogTask',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogTaskResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_sql_log_task(
+        self,
+        request: das20200116_models.DescribeSqlLogTaskRequest,
+    ) -> das20200116_models.DescribeSqlLogTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sql_log_task_with_options(request, runtime)
+
+    async def describe_sql_log_task_async(
+        self,
+        request: das20200116_models.DescribeSqlLogTaskRequest,
+    ) -> das20200116_models.DescribeSqlLogTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_sql_log_task_with_options_async(request, runtime)
+
+    def describe_sql_log_tasks_with_options(
+        self,
+        request: das20200116_models.DescribeSqlLogTasksRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogTasksResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filters):
+            body['Filters'] = request.filters
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            body['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogTasks',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogTasksResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_sql_log_tasks_with_options_async(
+        self,
+        request: das20200116_models.DescribeSqlLogTasksRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.DescribeSqlLogTasksResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filters):
+            body['Filters'] = request.filters
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            body['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.page_no):
+            body['PageNo'] = request.page_no
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSqlLogTasks',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.DescribeSqlLogTasksResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_sql_log_tasks(
+        self,
+        request: das20200116_models.DescribeSqlLogTasksRequest,
+    ) -> das20200116_models.DescribeSqlLogTasksResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sql_log_tasks_with_options(request, runtime)
+
+    async def describe_sql_log_tasks_async(
+        self,
+        request: das20200116_models.DescribeSqlLogTasksRequest,
+    ) -> das20200116_models.DescribeSqlLogTasksResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_sql_log_tasks_with_options_async(request, runtime)
+
     def describe_top_big_keys_with_options(
         self,
         request: das20200116_models.DescribeTopBigKeysRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.DescribeTopBigKeysResponse:
         """
         The list, hash, set, and zset keys are sorted based on the number of elements in these keys. The top three keys that have the most elements are considered large keys.
@@ -3472,16 +3992,16 @@
 
     def disable_das_pro_with_options(
         self,
         request: das20200116_models.DisableDasProRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.DisableDasProResponse:
         """
-        For information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DisableDasProRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DisableDasProResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3510,16 +4030,16 @@
 
     async def disable_das_pro_with_options_async(
         self,
         request: das20200116_models.DisableDasProRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.DisableDasProResponse:
         """
-        For information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DisableDasProRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DisableDasProResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3547,30 +4067,30 @@
         )
 
     def disable_das_pro(
         self,
         request: das20200116_models.DisableDasProRequest,
     ) -> das20200116_models.DisableDasProResponse:
         """
-        For information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DisableDasProRequest
         @return: DisableDasProResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.disable_das_pro_with_options(request, runtime)
 
     async def disable_das_pro_async(
         self,
         request: das20200116_models.DisableDasProRequest,
     ) -> das20200116_models.DisableDasProResponse:
         """
-        For information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: DisableDasProRequest
         @return: DisableDasProResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.disable_das_pro_with_options_async(request, runtime)
 
@@ -3804,16 +4324,16 @@
 
     def enable_das_pro_with_options(
         self,
         request: das20200116_models.EnableDasProRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.EnableDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: EnableDasProRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableDasProResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3844,16 +4364,16 @@
 
     async def enable_das_pro_with_options_async(
         self,
         request: das20200116_models.EnableDasProRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.EnableDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: EnableDasProRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableDasProResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3883,30 +4403,30 @@
         )
 
     def enable_das_pro(
         self,
         request: das20200116_models.EnableDasProRequest,
     ) -> das20200116_models.EnableDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: EnableDasProRequest
         @return: EnableDasProResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.enable_das_pro_with_options(request, runtime)
 
     async def enable_das_pro_async(
         self,
         request: das20200116_models.EnableDasProRequest,
     ) -> das20200116_models.EnableDasProResponse:
         """
-        For more information about database instances that support DAS Professional Edition, see [Overview](~~190912~~).
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        For more information about database instances that support DAS Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an SDK to call the API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: EnableDasProRequest
         @return: EnableDasProResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.enable_das_pro_with_options_async(request, runtime)
 
@@ -4036,17 +4556,17 @@
 
     def get_async_error_request_list_by_code_with_options(
         self,
         request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not immediately returned. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which DAS Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetAsyncErrorRequestListByCode is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestListByCodeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAsyncErrorRequestListByCodeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4081,17 +4601,17 @@
 
     async def get_async_error_request_list_by_code_with_options_async(
         self,
         request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not immediately returned. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which DAS Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetAsyncErrorRequestListByCode is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestListByCodeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAsyncErrorRequestListByCodeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4125,47 +4645,47 @@
         )
 
     def get_async_error_request_list_by_code(
         self,
         request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
     ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not immediately returned. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which DAS Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetAsyncErrorRequestListByCode is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestListByCodeRequest
         @return: GetAsyncErrorRequestListByCodeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_async_error_request_list_by_code_with_options(request, runtime)
 
     async def get_async_error_request_list_by_code_async(
         self,
         request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
     ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not immediately returned. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which DAS Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetAsyncErrorRequestListByCode is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestListByCodeRequest
         @return: GetAsyncErrorRequestListByCodeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_async_error_request_list_by_code_with_options_async(request, runtime)
 
     def get_async_error_request_stat_by_code_with_options(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatByCode is an asynchronous operation After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatByCodeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAsyncErrorRequestStatByCodeResponse
         """
         UtilClient.validate_model(request)
@@ -4201,16 +4721,16 @@
 
     async def get_async_error_request_stat_by_code_with_options_async(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatByCode is an asynchronous operation After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatByCodeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAsyncErrorRequestStatByCodeResponse
         """
         UtilClient.validate_model(request)
@@ -4245,47 +4765,47 @@
         )
 
     def get_async_error_request_stat_by_code(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
     ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatByCode is an asynchronous operation After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatByCodeRequest
         @return: GetAsyncErrorRequestStatByCodeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_async_error_request_stat_by_code_with_options(request, runtime)
 
     async def get_async_error_request_stat_by_code_async(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
     ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatByCode is an asynchronous operation After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatByCodeRequest
         @return: GetAsyncErrorRequestStatByCodeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_async_error_request_stat_by_code_with_options_async(request, runtime)
 
     def get_async_error_request_stat_result_with_options(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatResult is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatResultRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAsyncErrorRequestStatResultResponse
         """
         UtilClient.validate_model(request)
@@ -4323,16 +4843,16 @@
 
     async def get_async_error_request_stat_result_with_options_async(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatResult is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatResultRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAsyncErrorRequestStatResultResponse
         """
         UtilClient.validate_model(request)
@@ -4369,31 +4889,31 @@
         )
 
     def get_async_error_request_stat_result(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
     ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatResult is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatResultRequest
         @return: GetAsyncErrorRequestStatResultResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_async_error_request_stat_result_with_options(request, runtime)
 
     async def get_async_error_request_stat_result_async(
         self,
         request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
     ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
         """
-        >  When an asynchronous call is made, the complete query results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
+        >  GetAsyncErrorRequestStatResult is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
         *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetAsyncErrorRequestStatResultRequest
         @return: GetAsyncErrorRequestStatResultResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_async_error_request_stat_result_with_options_async(request, runtime)
@@ -5252,16 +5772,16 @@
 
     def get_das_pro_service_usage_with_options(
         self,
         request: das20200116_models.GetDasProServiceUsageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetDasProServiceUsageResponse:
         """
-        For information about databases that are supported, see [Overview](~~190912~~).
-        *   If you use an Alibaba Cloud SDK or a Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
+        For information about database instances that support Database Autonomy Service (DAS) Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an Alibaba Cloud SDK or DAS SDK to call this operation, we recommend that you use the latest version of the SDK.
         *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetDasProServiceUsageRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDasProServiceUsageResponse
         """
         UtilClient.validate_model(request)
@@ -5291,16 +5811,16 @@
 
     async def get_das_pro_service_usage_with_options_async(
         self,
         request: das20200116_models.GetDasProServiceUsageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetDasProServiceUsageResponse:
         """
-        For information about databases that are supported, see [Overview](~~190912~~).
-        *   If you use an Alibaba Cloud SDK or a Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
+        For information about database instances that support Database Autonomy Service (DAS) Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an Alibaba Cloud SDK or DAS SDK to call this operation, we recommend that you use the latest version of the SDK.
         *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetDasProServiceUsageRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDasProServiceUsageResponse
         """
         UtilClient.validate_model(request)
@@ -5329,31 +5849,31 @@
         )
 
     def get_das_pro_service_usage(
         self,
         request: das20200116_models.GetDasProServiceUsageRequest,
     ) -> das20200116_models.GetDasProServiceUsageResponse:
         """
-        For information about databases that are supported, see [Overview](~~190912~~).
-        *   If you use an Alibaba Cloud SDK or a Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
+        For information about database instances that support Database Autonomy Service (DAS) Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an Alibaba Cloud SDK or DAS SDK to call this operation, we recommend that you use the latest version of the SDK.
         *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetDasProServiceUsageRequest
         @return: GetDasProServiceUsageResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_das_pro_service_usage_with_options(request, runtime)
 
     async def get_das_pro_service_usage_async(
         self,
         request: das20200116_models.GetDasProServiceUsageRequest,
     ) -> das20200116_models.GetDasProServiceUsageResponse:
         """
-        For information about databases that are supported, see [Overview](~~190912~~).
-        *   If you use an Alibaba Cloud SDK or a Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
+        For information about database instances that support Database Autonomy Service (DAS) Enterprise Edition, see [Overview](~~190912~~).
+        *   If you use an Alibaba Cloud SDK or DAS SDK to call this operation, we recommend that you use the latest version of the SDK.
         *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetDasProServiceUsageRequest
         @return: GetDasProServiceUsageResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_das_pro_service_usage_with_options_async(request, runtime)
@@ -5806,17 +6326,17 @@
 
     def get_error_request_sample_with_options(
         self,
         request: das20200116_models.GetErrorRequestSampleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetErrorRequestSampleResponse:
         """
-        >  The complete query results are not immediately returned after an asynchronous request is sent. If the value of *isFinish** is **false** in the response, wait for 1 second and send the request again. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetErrorRequestSample is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetErrorRequestSampleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetErrorRequestSampleResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5853,17 +6373,17 @@
 
     async def get_error_request_sample_with_options_async(
         self,
         request: das20200116_models.GetErrorRequestSampleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetErrorRequestSampleResponse:
         """
-        >  The complete query results are not immediately returned after an asynchronous request is sent. If the value of *isFinish** is **false** in the response, wait for 1 second and send the request again. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetErrorRequestSample is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetErrorRequestSampleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetErrorRequestSampleResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5899,32 +6419,32 @@
         )
 
     def get_error_request_sample(
         self,
         request: das20200116_models.GetErrorRequestSampleRequest,
     ) -> das20200116_models.GetErrorRequestSampleResponse:
         """
-        >  The complete query results are not immediately returned after an asynchronous request is sent. If the value of *isFinish** is **false** in the response, wait for 1 second and send the request again. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetErrorRequestSample is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetErrorRequestSampleRequest
         @return: GetErrorRequestSampleResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_error_request_sample_with_options(request, runtime)
 
     async def get_error_request_sample_async(
         self,
         request: das20200116_models.GetErrorRequestSampleRequest,
     ) -> das20200116_models.GetErrorRequestSampleResponse:
         """
-        >  The complete query results are not immediately returned after an asynchronous request is sent. If the value of *isFinish** is **false** in the response, wait for 1 second and send the request again. The complete query results are returned until the value of **isFinish** is **true**.
-        *   This operation is applicable only to ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Professional Edition is enabled. For more information, see [Purchase DAS Professional Edition](~~163298~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        >  GetErrorRequestSample is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
+        *   This API operation supports only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters for which Database Autonomy Service (DAS) Enterprise Edition is enabled. For more information, see [Purchase DAS Enterprise Edition](~~163298~~).
+        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: GetErrorRequestSampleRequest
         @return: GetErrorRequestSampleResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_error_request_sample_with_options_async(request, runtime)
 
@@ -6039,16 +6559,16 @@
     def get_full_request_origin_stat_by_instance_id_with_options(
         self,
         request: das20200116_models.GetFullRequestOriginStatByInstanceIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetFullRequestOriginStatByInstanceIdResponse:
         """
         The SQL Explorer feature allows you to check the health status of SQL statements and troubleshoot performance issues. For more information, see [SQL Explorer](~~204096~~).
-        *   For information about database instances that support SQL Explorer, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        *   For more information about database instances that support this feature, see [Overview](~~190912~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
         
         @param request: GetFullRequestOriginStatByInstanceIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetFullRequestOriginStatByInstanceIdResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6096,16 +6616,16 @@
     async def get_full_request_origin_stat_by_instance_id_with_options_async(
         self,
         request: das20200116_models.GetFullRequestOriginStatByInstanceIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetFullRequestOriginStatByInstanceIdResponse:
         """
         The SQL Explorer feature allows you to check the health status of SQL statements and troubleshoot performance issues. For more information, see [SQL Explorer](~~204096~~).
-        *   For information about database instances that support SQL Explorer, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        *   For more information about database instances that support this feature, see [Overview](~~190912~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
         
         @param request: GetFullRequestOriginStatByInstanceIdRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetFullRequestOriginStatByInstanceIdResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6152,31 +6672,31 @@
 
     def get_full_request_origin_stat_by_instance_id(
         self,
         request: das20200116_models.GetFullRequestOriginStatByInstanceIdRequest,
     ) -> das20200116_models.GetFullRequestOriginStatByInstanceIdResponse:
         """
         The SQL Explorer feature allows you to check the health status of SQL statements and troubleshoot performance issues. For more information, see [SQL Explorer](~~204096~~).
-        *   For information about database instances that support SQL Explorer, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        *   For more information about database instances that support this feature, see [Overview](~~190912~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
         
         @param request: GetFullRequestOriginStatByInstanceIdRequest
         @return: GetFullRequestOriginStatByInstanceIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_full_request_origin_stat_by_instance_id_with_options(request, runtime)
 
     async def get_full_request_origin_stat_by_instance_id_async(
         self,
         request: das20200116_models.GetFullRequestOriginStatByInstanceIdRequest,
     ) -> das20200116_models.GetFullRequestOriginStatByInstanceIdResponse:
         """
         The SQL Explorer feature allows you to check the health status of SQL statements and troubleshoot performance issues. For more information, see [SQL Explorer](~~204096~~).
-        *   For information about database instances that support SQL Explorer, see [Overview](~~190912~~).
-        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
+        *   For more information about database instances that support this feature, see [Overview](~~190912~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
         
         @param request: GetFullRequestOriginStatByInstanceIdRequest
         @return: GetFullRequestOriginStatByInstanceIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_full_request_origin_stat_by_instance_id_with_options_async(request, runtime)
 
@@ -10105,15 +10625,15 @@
         *   You can modify the configurations of the **automatic storage expansion** feature for the following types of database instances:
         *   ApsaraDB RDS for MySQL High-availability Edition instances that use standard SSDs or ESSDs. For more information about the feature and the billing rules, see [Automatic space expansion](~~173345~~).
         *   You can modify the configurations of the **automatic bandwidth adjustment** feature for the following types of database instances:
         *   ApsaraDB for Redis Classic (Local Disk-based) Edition instances. For more information about the feature and the billing rules, see [Automatic bandwidth adjustment](~~216312~~).
         *   You can modify the configurations of the **auto scaling feature for resources** for the following types of database instances:
         *   General-purpose ApsaraDB RDS for MySQL Enterprise Edition instances. For more information about the feature and the billing rules, see [Automatic performance scaling](~~169686~~).
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: ModifyAutoScalingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyAutoScalingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10161,15 +10681,15 @@
         *   You can modify the configurations of the **automatic storage expansion** feature for the following types of database instances:
         *   ApsaraDB RDS for MySQL High-availability Edition instances that use standard SSDs or ESSDs. For more information about the feature and the billing rules, see [Automatic space expansion](~~173345~~).
         *   You can modify the configurations of the **automatic bandwidth adjustment** feature for the following types of database instances:
         *   ApsaraDB for Redis Classic (Local Disk-based) Edition instances. For more information about the feature and the billing rules, see [Automatic bandwidth adjustment](~~216312~~).
         *   You can modify the configurations of the **auto scaling feature for resources** for the following types of database instances:
         *   General-purpose ApsaraDB RDS for MySQL Enterprise Edition instances. For more information about the feature and the billing rules, see [Automatic performance scaling](~~169686~~).
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: ModifyAutoScalingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyAutoScalingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10216,15 +10736,15 @@
         *   You can modify the configurations of the **automatic storage expansion** feature for the following types of database instances:
         *   ApsaraDB RDS for MySQL High-availability Edition instances that use standard SSDs or ESSDs. For more information about the feature and the billing rules, see [Automatic space expansion](~~173345~~).
         *   You can modify the configurations of the **automatic bandwidth adjustment** feature for the following types of database instances:
         *   ApsaraDB for Redis Classic (Local Disk-based) Edition instances. For more information about the feature and the billing rules, see [Automatic bandwidth adjustment](~~216312~~).
         *   You can modify the configurations of the **auto scaling feature for resources** for the following types of database instances:
         *   General-purpose ApsaraDB RDS for MySQL Enterprise Edition instances. For more information about the feature and the billing rules, see [Automatic performance scaling](~~169686~~).
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: ModifyAutoScalingConfigRequest
         @return: ModifyAutoScalingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_auto_scaling_config_with_options(request, runtime)
 
@@ -10240,22 +10760,116 @@
         *   You can modify the configurations of the **automatic storage expansion** feature for the following types of database instances:
         *   ApsaraDB RDS for MySQL High-availability Edition instances that use standard SSDs or ESSDs. For more information about the feature and the billing rules, see [Automatic space expansion](~~173345~~).
         *   You can modify the configurations of the **automatic bandwidth adjustment** feature for the following types of database instances:
         *   ApsaraDB for Redis Classic (Local Disk-based) Edition instances. For more information about the feature and the billing rules, see [Automatic bandwidth adjustment](~~216312~~).
         *   You can modify the configurations of the **auto scaling feature for resources** for the following types of database instances:
         *   General-purpose ApsaraDB RDS for MySQL Enterprise Edition instances. For more information about the feature and the billing rules, see [Automatic performance scaling](~~169686~~).
         *   If you use an Alibaba Cloud SDK or Database Autonomy Service (DAS) SDK to call this operation, we recommend that you use the latest version of the SDK.
-        *   If you use an SDK to call API operations of DAS, you must set the region ID to cn-shanghai.
+        *   If you use an SDK to call operations of DAS, you must set the region ID to cn-shanghai.
         
         @param request: ModifyAutoScalingConfigRequest
         @return: ModifyAutoScalingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_auto_scaling_config_with_options_async(request, runtime)
 
+    def modify_sql_log_config_with_options(
+        self,
+        request: das20200116_models.ModifySqlLogConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.ModifySqlLogConfigResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filters):
+            query['Filters'] = request.filters
+        body = {}
+        if not UtilClient.is_unset(request.enable):
+            body['Enable'] = request.enable
+        if not UtilClient.is_unset(request.hot_retention):
+            body['HotRetention'] = request.hot_retention
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.request_enable):
+            body['RequestEnable'] = request.request_enable
+        if not UtilClient.is_unset(request.retention):
+            body['Retention'] = request.retention
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifySqlLogConfig',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.ModifySqlLogConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_sql_log_config_with_options_async(
+        self,
+        request: das20200116_models.ModifySqlLogConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.ModifySqlLogConfigResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.filters):
+            query['Filters'] = request.filters
+        body = {}
+        if not UtilClient.is_unset(request.enable):
+            body['Enable'] = request.enable
+        if not UtilClient.is_unset(request.hot_retention):
+            body['HotRetention'] = request.hot_retention
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.request_enable):
+            body['RequestEnable'] = request.request_enable
+        if not UtilClient.is_unset(request.retention):
+            body['Retention'] = request.retention
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifySqlLogConfig',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.ModifySqlLogConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_sql_log_config(
+        self,
+        request: das20200116_models.ModifySqlLogConfigRequest,
+    ) -> das20200116_models.ModifySqlLogConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_sql_log_config_with_options(request, runtime)
+
+    async def modify_sql_log_config_async(
+        self,
+        request: das20200116_models.ModifySqlLogConfigRequest,
+    ) -> das20200116_models.ModifySqlLogConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_sql_log_config_with_options_async(request, runtime)
+
     def run_cloud_bench_task_with_options(
         self,
         request: das20200116_models.RunCloudBenchTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.RunCloudBenchTaskResponse:
         """
         Database Autonomy Service (DAS) provides the intelligent stress testing feature. This feature helps you check whether your instance needs to be scaled up to effectively handle traffic spikes. For more information, see [Intelligent stress testing](~~155068~~).
@@ -10700,20 +11314,20 @@
 
     def update_auto_resource_optimize_rules_async_with_options(
         self,
         request: das20200116_models.UpdateAutoResourceOptimizeRulesAsyncRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.UpdateAutoResourceOptimizeRulesAsyncResponse:
         """
-        >  An asynchronous call does not immediately return complete results. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. If the value of **isFinish** is **true**, the complete results are returned.
+        >  UpdateAutoResourceOptimizeRulesAsync is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   The database instance is an ApsaraDB RDS for MySQL instance of High-availability Edition.
-        *   DAS Professional Edition is enabled for the database instance. You can call the [DescribeInstanceDasPro](~~413866~~) operation to check whether DAS Professional Edition is enabled for a database instance.
-        *   The database instance has four or more cores, and **innodb_file_per_table** is set to **ON**.
+        *   If you use an SDK to call the API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   The database instances must be an ApsaraDB RDS for MySQL High-availability Edition instance.
+        *   DAS Enterprise Edition must be enabled for the database instance. You can call the call [DescribeInstanceDasPro](~~413866~~) operation to query whether DAS Enterprise Edition is enabled.
+        *   The database instance has four or more CPU cores, and **innodb_file_per_table** is set to **ON**.
         
         @param request: UpdateAutoResourceOptimizeRulesAsyncRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateAutoResourceOptimizeRulesAsyncResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10748,20 +11362,20 @@
 
     async def update_auto_resource_optimize_rules_async_with_options_async(
         self,
         request: das20200116_models.UpdateAutoResourceOptimizeRulesAsyncRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.UpdateAutoResourceOptimizeRulesAsyncResponse:
         """
-        >  An asynchronous call does not immediately return complete results. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. If the value of **isFinish** is **true**, the complete results are returned.
+        >  UpdateAutoResourceOptimizeRulesAsync is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   The database instance is an ApsaraDB RDS for MySQL instance of High-availability Edition.
-        *   DAS Professional Edition is enabled for the database instance. You can call the [DescribeInstanceDasPro](~~413866~~) operation to check whether DAS Professional Edition is enabled for a database instance.
-        *   The database instance has four or more cores, and **innodb_file_per_table** is set to **ON**.
+        *   If you use an SDK to call the API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   The database instances must be an ApsaraDB RDS for MySQL High-availability Edition instance.
+        *   DAS Enterprise Edition must be enabled for the database instance. You can call the call [DescribeInstanceDasPro](~~413866~~) operation to query whether DAS Enterprise Edition is enabled.
+        *   The database instance has four or more CPU cores, and **innodb_file_per_table** is set to **ON**.
         
         @param request: UpdateAutoResourceOptimizeRulesAsyncRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateAutoResourceOptimizeRulesAsyncResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10795,58 +11409,58 @@
         )
 
     def update_auto_resource_optimize_rules_async(
         self,
         request: das20200116_models.UpdateAutoResourceOptimizeRulesAsyncRequest,
     ) -> das20200116_models.UpdateAutoResourceOptimizeRulesAsyncResponse:
         """
-        >  An asynchronous call does not immediately return complete results. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. If the value of **isFinish** is **true**, the complete results are returned.
+        >  UpdateAutoResourceOptimizeRulesAsync is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   The database instance is an ApsaraDB RDS for MySQL instance of High-availability Edition.
-        *   DAS Professional Edition is enabled for the database instance. You can call the [DescribeInstanceDasPro](~~413866~~) operation to check whether DAS Professional Edition is enabled for a database instance.
-        *   The database instance has four or more cores, and **innodb_file_per_table** is set to **ON**.
+        *   If you use an SDK to call the API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   The database instances must be an ApsaraDB RDS for MySQL High-availability Edition instance.
+        *   DAS Enterprise Edition must be enabled for the database instance. You can call the call [DescribeInstanceDasPro](~~413866~~) operation to query whether DAS Enterprise Edition is enabled.
+        *   The database instance has four or more CPU cores, and **innodb_file_per_table** is set to **ON**.
         
         @param request: UpdateAutoResourceOptimizeRulesAsyncRequest
         @return: UpdateAutoResourceOptimizeRulesAsyncResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_auto_resource_optimize_rules_async_with_options(request, runtime)
 
     async def update_auto_resource_optimize_rules_async_async(
         self,
         request: das20200116_models.UpdateAutoResourceOptimizeRulesAsyncRequest,
     ) -> das20200116_models.UpdateAutoResourceOptimizeRulesAsyncResponse:
         """
-        >  An asynchronous call does not immediately return complete results. If the value of *isFinish** is **false** in the response, wait for 1 second and then re-initiate the call. If the value of **isFinish** is **true**, the complete results are returned.
+        >  UpdateAutoResourceOptimizeRulesAsync is an asynchronous operation. After a request is sent, the complete results are not returned immediately. If the value of *isFinish** is **false** in the response, wait for 1 second and then send a request again. If the value of **isFinish** is **true**, the complete results are returned.
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   The database instance is an ApsaraDB RDS for MySQL instance of High-availability Edition.
-        *   DAS Professional Edition is enabled for the database instance. You can call the [DescribeInstanceDasPro](~~413866~~) operation to check whether DAS Professional Edition is enabled for a database instance.
-        *   The database instance has four or more cores, and **innodb_file_per_table** is set to **ON**.
+        *   If you use an SDK to call the API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   The database instances must be an ApsaraDB RDS for MySQL High-availability Edition instance.
+        *   DAS Enterprise Edition must be enabled for the database instance. You can call the call [DescribeInstanceDasPro](~~413866~~) operation to query whether DAS Enterprise Edition is enabled.
+        *   The database instance has four or more CPU cores, and **innodb_file_per_table** is set to **ON**.
         
         @param request: UpdateAutoResourceOptimizeRulesAsyncRequest
         @return: UpdateAutoResourceOptimizeRulesAsyncResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_auto_resource_optimize_rules_async_with_options_async(request, runtime)
 
     def update_auto_sql_optimize_status_with_options(
         self,
         request: das20200116_models.UpdateAutoSqlOptimizeStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.UpdateAutoSqlOptimizeStatusResponse:
         """
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   DAS Professional Edition is enabled for the database instance that you want to manage. To enable DAS Professional Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
-        *   The autonomy service is enabled for the database instance. For more information, see [Autonomy center](~~152139~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   DAS Enterprise Edition must be enabled for the database instance that you want to manage. To enable DAS Enterprise Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
+        *   The autonomy service must be enabled for the database instance that you want to manage. For more information, see [Autonomy center](~~152139~~).
         *   This operation supports the following database engines:
-        *   ApsaraDB RDS for MySQL High-availability Edition and Enterprise Edition
-        *   PolarDB for MySQL Cluster Edition and X-Engine Edition
+        *   ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition
+        *   PolarDB for MySQL Cluster Edition or X-Engine Edition
         
         @param request: UpdateAutoSqlOptimizeStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateAutoSqlOptimizeStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10876,20 +11490,20 @@
     async def update_auto_sql_optimize_status_with_options_async(
         self,
         request: das20200116_models.UpdateAutoSqlOptimizeStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.UpdateAutoSqlOptimizeStatusResponse:
         """
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   DAS Professional Edition is enabled for the database instance that you want to manage. To enable DAS Professional Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
-        *   The autonomy service is enabled for the database instance. For more information, see [Autonomy center](~~152139~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   DAS Enterprise Edition must be enabled for the database instance that you want to manage. To enable DAS Enterprise Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
+        *   The autonomy service must be enabled for the database instance that you want to manage. For more information, see [Autonomy center](~~152139~~).
         *   This operation supports the following database engines:
-        *   ApsaraDB RDS for MySQL High-availability Edition and Enterprise Edition
-        *   PolarDB for MySQL Cluster Edition and X-Engine Edition
+        *   ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition
+        *   PolarDB for MySQL Cluster Edition or X-Engine Edition
         
         @param request: UpdateAutoSqlOptimizeStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateAutoSqlOptimizeStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10918,39 +11532,39 @@
 
     def update_auto_sql_optimize_status(
         self,
         request: das20200116_models.UpdateAutoSqlOptimizeStatusRequest,
     ) -> das20200116_models.UpdateAutoSqlOptimizeStatusResponse:
         """
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   DAS Professional Edition is enabled for the database instance that you want to manage. To enable DAS Professional Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
-        *   The autonomy service is enabled for the database instance. For more information, see [Autonomy center](~~152139~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   DAS Enterprise Edition must be enabled for the database instance that you want to manage. To enable DAS Enterprise Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
+        *   The autonomy service must be enabled for the database instance that you want to manage. For more information, see [Autonomy center](~~152139~~).
         *   This operation supports the following database engines:
-        *   ApsaraDB RDS for MySQL High-availability Edition and Enterprise Edition
-        *   PolarDB for MySQL Cluster Edition and X-Engine Edition
+        *   ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition
+        *   PolarDB for MySQL Cluster Edition or X-Engine Edition
         
         @param request: UpdateAutoSqlOptimizeStatusRequest
         @return: UpdateAutoSqlOptimizeStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_auto_sql_optimize_status_with_options(request, runtime)
 
     async def update_auto_sql_optimize_status_async(
         self,
         request: das20200116_models.UpdateAutoSqlOptimizeStatusRequest,
     ) -> das20200116_models.UpdateAutoSqlOptimizeStatusResponse:
         """
         Before you call this operation, take note of the following items:
-        *   If you use an SDK to call operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
-        *   DAS Professional Edition is enabled for the database instance that you want to manage. To enable DAS Professional Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
-        *   The autonomy service is enabled for the database instance. For more information, see [Autonomy center](~~152139~~).
+        *   If you use an SDK to call API operations of Database Autonomy Service (DAS), you must set the region ID to cn-shanghai.
+        *   DAS Enterprise Edition must be enabled for the database instance that you want to manage. To enable DAS Enterprise Edition for a database instance, you can call the [EnableDasPro](~~411645~~) operation.
+        *   The autonomy service must be enabled for the database instance that you want to manage. For more information, see [Autonomy center](~~152139~~).
         *   This operation supports the following database engines:
-        *   ApsaraDB RDS for MySQL High-availability Edition and Enterprise Edition
-        *   PolarDB for MySQL Cluster Edition and X-Engine Edition
+        *   ApsaraDB RDS for MySQL High-availability Edition or Enterprise Edition
+        *   PolarDB for MySQL Cluster Edition or X-Engine Edition
         
         @param request: UpdateAutoSqlOptimizeStatusRequest
         @return: UpdateAutoSqlOptimizeStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_auto_sql_optimize_status_with_options_async(request, runtime)
```

### Comparing `alibabacloud_das20200116-2.3.2/alibabacloud_das20200116/models.py` & `alibabacloud_das20200116-2.4.0/alibabacloud_das20200116/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2230,14 +2230,282 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateRequestDiagnosisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateSqlLogTaskRequestFilters(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateSqlLogTaskRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        filters: List[CreateSqlLogTaskRequestFilters] = None,
+        instance_id: str = None,
+        name: str = None,
+        node_id: str = None,
+        role: str = None,
+        start_time: int = None,
+        type: str = None,
+    ):
+        self.end_time = end_time
+        self.filters = filters
+        self.instance_id = instance_id
+        self.name = name
+        self.node_id = node_id
+        self.role = role
+        self.start_time = start_time
+        self.type = type
+
+    def validate(self):
+        if self.filters:
+            for k in self.filters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        result['Filters'] = []
+        if self.filters is not None:
+            for k in self.filters:
+                result['Filters'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.role is not None:
+            result['Role'] = self.role
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        self.filters = []
+        if m.get('Filters') is not None:
+            for k in m.get('Filters'):
+                temp_model = CreateSqlLogTaskRequestFilters()
+                self.filters.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('Role') is not None:
+            self.role = m.get('Role')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class CreateSqlLogTaskResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        create_time: int = None,
+        end: int = None,
+        instance_id: str = None,
+        name: str = None,
+        start: int = None,
+        status: str = None,
+        task_id: str = None,
+    ):
+        self.create_time = create_time
+        self.end = end
+        self.instance_id = instance_id
+        self.name = name
+        self.start = start
+        self.status = status
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.end is not None:
+            result['End'] = self.end
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.start is not None:
+            result['Start'] = self.start
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class CreateSqlLogTaskResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: CreateSqlLogTaskResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        # SqlLogTask
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = CreateSqlLogTaskResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateSqlLogTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateSqlLogTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateSqlLogTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateStorageAnalysisTaskRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         instance_id: str = None,
         node_id: str = None,
         table_name: str = None,
@@ -4990,15 +5258,15 @@
         # 
         # * **NEW**: Initialize the stress testing task.
         # * **WAIT_BUY_ECS**: Purchase an ECS instance.
         # * **WAIT_START_ECS**: Start the ECS instance.
         # * **WAIT_INSTALL_JDK**: Install the Java Development Kit (JDK).
         # * **WAIT_INSTALL_DBGATEWAY**: Install the database gateway (DBGateway).
         # * **ADD_SECURITY_IPS_STEP**: Configure the whitelist of the security group.
-        # * **ARCHIVIE**: Archive the file that stores the analysis results of full SQL statistics.
+        # * **ARCHIVE**: Archive the file that stores the analysis results of full SQL statistics.
         # * **DOWNLOAD**: Download the file that stores the analysis result of full SQL statistics.
         # * **PROCEED**: Preprocess the file that stores the analysis result of full SQL statistics.
         # * **PRE_LOAD**: Preload the file that stores the analysis result of full SQL statistics.
         # * **VALIDATE**: Verify the functionality of stress testing.
         # * **PRESSURE**: Start the stress testing task.
         self.bench_step = bench_step
         # The status that indicates the substep performed for the stress testing task. Valid values:
@@ -7152,15 +7420,15 @@
         data: bool = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
         # The HTTP status code returned.
         self.code = code
-        # Indicates whether DAS Professional Edition is enabled for the database instance.
+        # Indicates whether DAS Enterprise Edition is enabled for the database instance. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.data = data
         # The returned message.
         # 
         # >  If the request was successful, **Successful** is returned. If the request failed, an error message such as an error code is returned.
@@ -7246,14 +7514,1864 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeInstanceDasProResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeSqlLogConfigRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+    ):
+        self.instance_id = instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        return self
+
+
+class DescribeSqlLogConfigResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        cold_enable: bool = None,
+        cold_retention: int = None,
+        cold_start_time: int = None,
+        collector_version: str = None,
+        hot_enable: bool = None,
+        hot_retention: int = None,
+        hot_start_time: int = None,
+        log_filter: str = None,
+        request_enable: bool = None,
+        request_start_time: int = None,
+        request_stop_time: int = None,
+        retention: int = None,
+        sql_log_enable: bool = None,
+        sql_log_state: str = None,
+        sql_log_visible_time: int = None,
+        support_version: str = None,
+        version: str = None,
+    ):
+        self.cold_enable = cold_enable
+        self.cold_retention = cold_retention
+        self.cold_start_time = cold_start_time
+        self.collector_version = collector_version
+        self.hot_enable = hot_enable
+        self.hot_retention = hot_retention
+        self.hot_start_time = hot_start_time
+        self.log_filter = log_filter
+        self.request_enable = request_enable
+        self.request_start_time = request_start_time
+        self.request_stop_time = request_stop_time
+        self.retention = retention
+        self.sql_log_enable = sql_log_enable
+        self.sql_log_state = sql_log_state
+        self.sql_log_visible_time = sql_log_visible_time
+        self.support_version = support_version
+        self.version = version
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cold_enable is not None:
+            result['ColdEnable'] = self.cold_enable
+        if self.cold_retention is not None:
+            result['ColdRetention'] = self.cold_retention
+        if self.cold_start_time is not None:
+            result['ColdStartTime'] = self.cold_start_time
+        if self.collector_version is not None:
+            result['CollectorVersion'] = self.collector_version
+        if self.hot_enable is not None:
+            result['HotEnable'] = self.hot_enable
+        if self.hot_retention is not None:
+            result['HotRetention'] = self.hot_retention
+        if self.hot_start_time is not None:
+            result['HotStartTime'] = self.hot_start_time
+        if self.log_filter is not None:
+            result['LogFilter'] = self.log_filter
+        if self.request_enable is not None:
+            result['RequestEnable'] = self.request_enable
+        if self.request_start_time is not None:
+            result['RequestStartTime'] = self.request_start_time
+        if self.request_stop_time is not None:
+            result['RequestStopTime'] = self.request_stop_time
+        if self.retention is not None:
+            result['Retention'] = self.retention
+        if self.sql_log_enable is not None:
+            result['SqlLogEnable'] = self.sql_log_enable
+        if self.sql_log_state is not None:
+            result['SqlLogState'] = self.sql_log_state
+        if self.sql_log_visible_time is not None:
+            result['SqlLogVisibleTime'] = self.sql_log_visible_time
+        if self.support_version is not None:
+            result['SupportVersion'] = self.support_version
+        if self.version is not None:
+            result['Version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColdEnable') is not None:
+            self.cold_enable = m.get('ColdEnable')
+        if m.get('ColdRetention') is not None:
+            self.cold_retention = m.get('ColdRetention')
+        if m.get('ColdStartTime') is not None:
+            self.cold_start_time = m.get('ColdStartTime')
+        if m.get('CollectorVersion') is not None:
+            self.collector_version = m.get('CollectorVersion')
+        if m.get('HotEnable') is not None:
+            self.hot_enable = m.get('HotEnable')
+        if m.get('HotRetention') is not None:
+            self.hot_retention = m.get('HotRetention')
+        if m.get('HotStartTime') is not None:
+            self.hot_start_time = m.get('HotStartTime')
+        if m.get('LogFilter') is not None:
+            self.log_filter = m.get('LogFilter')
+        if m.get('RequestEnable') is not None:
+            self.request_enable = m.get('RequestEnable')
+        if m.get('RequestStartTime') is not None:
+            self.request_start_time = m.get('RequestStartTime')
+        if m.get('RequestStopTime') is not None:
+            self.request_stop_time = m.get('RequestStopTime')
+        if m.get('Retention') is not None:
+            self.retention = m.get('Retention')
+        if m.get('SqlLogEnable') is not None:
+            self.sql_log_enable = m.get('SqlLogEnable')
+        if m.get('SqlLogState') is not None:
+            self.sql_log_state = m.get('SqlLogState')
+        if m.get('SqlLogVisibleTime') is not None:
+            self.sql_log_visible_time = m.get('SqlLogVisibleTime')
+        if m.get('SupportVersion') is not None:
+            self.support_version = m.get('SupportVersion')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        return self
+
+
+class DescribeSqlLogConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribeSqlLogConfigResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        # SqlLogConfig
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeSqlLogConfigResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DescribeSqlLogConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeSqlLogConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeSqlLogConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeSqlLogRecordsRequestFilters(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeSqlLogRecordsRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        filters: List[DescribeSqlLogRecordsRequestFilters] = None,
+        instance_id: str = None,
+        node_id: str = None,
+        page_no: int = None,
+        page_size: int = None,
+        role: str = None,
+        start_time: int = None,
+    ):
+        self.end_time = end_time
+        self.filters = filters
+        self.instance_id = instance_id
+        self.node_id = node_id
+        self.page_no = page_no
+        self.page_size = page_size
+        self.role = role
+        self.start_time = start_time
+
+    def validate(self):
+        if self.filters:
+            for k in self.filters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        result['Filters'] = []
+        if self.filters is not None:
+            for k in self.filters:
+                result['Filters'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.role is not None:
+            result['Role'] = self.role
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        self.filters = []
+        if m.get('Filters') is not None:
+            for k in m.get('Filters'):
+                temp_model = DescribeSqlLogRecordsRequestFilters()
+                self.filters.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Role') is not None:
+            self.role = m.get('Role')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeSqlLogRecordsResponseBodyDataItemsSQLLogRecord(TeaModel):
+    def __init__(
+        self,
+        account_name: str = None,
+        collection: str = None,
+        consume: int = None,
+        cpu_time: int = None,
+        dbname: str = None,
+        execute_time: str = None,
+        ext: str = None,
+        frows: int = None,
+        host_address: str = None,
+        lock_time: int = None,
+        logic_read: int = None,
+        node_id: str = None,
+        origin_time: int = None,
+        parallel_degree: str = None,
+        parallel_queue_time: str = None,
+        physic_async_read: int = None,
+        physic_read: int = None,
+        physic_sync_read: int = None,
+        return_rows: int = None,
+        rows: int = None,
+        scan_rows: int = None,
+        scnt: int = None,
+        sql_id: str = None,
+        sql_text: str = None,
+        sql_type: str = None,
+        state: str = None,
+        thread_id: int = None,
+        trace_id: str = None,
+        trx_id: int = None,
+        update_rows: int = None,
+        use_imci_engine: str = None,
+        vip: str = None,
+        writes: int = None,
+    ):
+        self.account_name = account_name
+        self.collection = collection
+        self.consume = consume
+        self.cpu_time = cpu_time
+        self.dbname = dbname
+        self.execute_time = execute_time
+        self.ext = ext
+        self.frows = frows
+        self.host_address = host_address
+        self.lock_time = lock_time
+        self.logic_read = logic_read
+        self.node_id = node_id
+        self.origin_time = origin_time
+        self.parallel_degree = parallel_degree
+        self.parallel_queue_time = parallel_queue_time
+        self.physic_async_read = physic_async_read
+        self.physic_read = physic_read
+        self.physic_sync_read = physic_sync_read
+        self.return_rows = return_rows
+        self.rows = rows
+        self.scan_rows = scan_rows
+        self.scnt = scnt
+        self.sql_id = sql_id
+        self.sql_text = sql_text
+        self.sql_type = sql_type
+        self.state = state
+        self.thread_id = thread_id
+        self.trace_id = trace_id
+        self.trx_id = trx_id
+        self.update_rows = update_rows
+        self.use_imci_engine = use_imci_engine
+        self.vip = vip
+        self.writes = writes
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_name is not None:
+            result['AccountName'] = self.account_name
+        if self.collection is not None:
+            result['Collection'] = self.collection
+        if self.consume is not None:
+            result['Consume'] = self.consume
+        if self.cpu_time is not None:
+            result['CpuTime'] = self.cpu_time
+        if self.dbname is not None:
+            result['DBName'] = self.dbname
+        if self.execute_time is not None:
+            result['ExecuteTime'] = self.execute_time
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.frows is not None:
+            result['Frows'] = self.frows
+        if self.host_address is not None:
+            result['HostAddress'] = self.host_address
+        if self.lock_time is not None:
+            result['LockTime'] = self.lock_time
+        if self.logic_read is not None:
+            result['LogicRead'] = self.logic_read
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.origin_time is not None:
+            result['OriginTime'] = self.origin_time
+        if self.parallel_degree is not None:
+            result['ParallelDegree'] = self.parallel_degree
+        if self.parallel_queue_time is not None:
+            result['ParallelQueueTime'] = self.parallel_queue_time
+        if self.physic_async_read is not None:
+            result['PhysicAsyncRead'] = self.physic_async_read
+        if self.physic_read is not None:
+            result['PhysicRead'] = self.physic_read
+        if self.physic_sync_read is not None:
+            result['PhysicSyncRead'] = self.physic_sync_read
+        if self.return_rows is not None:
+            result['ReturnRows'] = self.return_rows
+        if self.rows is not None:
+            result['Rows'] = self.rows
+        if self.scan_rows is not None:
+            result['ScanRows'] = self.scan_rows
+        if self.scnt is not None:
+            result['Scnt'] = self.scnt
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text is not None:
+            result['SqlText'] = self.sql_text
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        if self.state is not None:
+            result['State'] = self.state
+        if self.thread_id is not None:
+            result['ThreadId'] = self.thread_id
+        if self.trace_id is not None:
+            result['TraceId'] = self.trace_id
+        if self.trx_id is not None:
+            result['TrxId'] = self.trx_id
+        if self.update_rows is not None:
+            result['UpdateRows'] = self.update_rows
+        if self.use_imci_engine is not None:
+            result['UseImciEngine'] = self.use_imci_engine
+        if self.vip is not None:
+            result['Vip'] = self.vip
+        if self.writes is not None:
+            result['Writes'] = self.writes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountName') is not None:
+            self.account_name = m.get('AccountName')
+        if m.get('Collection') is not None:
+            self.collection = m.get('Collection')
+        if m.get('Consume') is not None:
+            self.consume = m.get('Consume')
+        if m.get('CpuTime') is not None:
+            self.cpu_time = m.get('CpuTime')
+        if m.get('DBName') is not None:
+            self.dbname = m.get('DBName')
+        if m.get('ExecuteTime') is not None:
+            self.execute_time = m.get('ExecuteTime')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Frows') is not None:
+            self.frows = m.get('Frows')
+        if m.get('HostAddress') is not None:
+            self.host_address = m.get('HostAddress')
+        if m.get('LockTime') is not None:
+            self.lock_time = m.get('LockTime')
+        if m.get('LogicRead') is not None:
+            self.logic_read = m.get('LogicRead')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('OriginTime') is not None:
+            self.origin_time = m.get('OriginTime')
+        if m.get('ParallelDegree') is not None:
+            self.parallel_degree = m.get('ParallelDegree')
+        if m.get('ParallelQueueTime') is not None:
+            self.parallel_queue_time = m.get('ParallelQueueTime')
+        if m.get('PhysicAsyncRead') is not None:
+            self.physic_async_read = m.get('PhysicAsyncRead')
+        if m.get('PhysicRead') is not None:
+            self.physic_read = m.get('PhysicRead')
+        if m.get('PhysicSyncRead') is not None:
+            self.physic_sync_read = m.get('PhysicSyncRead')
+        if m.get('ReturnRows') is not None:
+            self.return_rows = m.get('ReturnRows')
+        if m.get('Rows') is not None:
+            self.rows = m.get('Rows')
+        if m.get('ScanRows') is not None:
+            self.scan_rows = m.get('ScanRows')
+        if m.get('Scnt') is not None:
+            self.scnt = m.get('Scnt')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlText') is not None:
+            self.sql_text = m.get('SqlText')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        if m.get('State') is not None:
+            self.state = m.get('State')
+        if m.get('ThreadId') is not None:
+            self.thread_id = m.get('ThreadId')
+        if m.get('TraceId') is not None:
+            self.trace_id = m.get('TraceId')
+        if m.get('TrxId') is not None:
+            self.trx_id = m.get('TrxId')
+        if m.get('UpdateRows') is not None:
+            self.update_rows = m.get('UpdateRows')
+        if m.get('UseImciEngine') is not None:
+            self.use_imci_engine = m.get('UseImciEngine')
+        if m.get('Vip') is not None:
+            self.vip = m.get('Vip')
+        if m.get('Writes') is not None:
+            self.writes = m.get('Writes')
+        return self
+
+
+class DescribeSqlLogRecordsResponseBodyDataItems(TeaModel):
+    def __init__(
+        self,
+        sqllog_record: List[DescribeSqlLogRecordsResponseBodyDataItemsSQLLogRecord] = None,
+    ):
+        self.sqllog_record = sqllog_record
+
+    def validate(self):
+        if self.sqllog_record:
+            for k in self.sqllog_record:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['SQLLogRecord'] = []
+        if self.sqllog_record is not None:
+            for k in self.sqllog_record:
+                result['SQLLogRecord'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.sqllog_record = []
+        if m.get('SQLLogRecord') is not None:
+            for k in m.get('SQLLogRecord'):
+                temp_model = DescribeSqlLogRecordsResponseBodyDataItemsSQLLogRecord()
+                self.sqllog_record.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeSqlLogRecordsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        finish: str = None,
+        items: DescribeSqlLogRecordsResponseBodyDataItems = None,
+        job_id: str = None,
+        start_time: int = None,
+        total_records: int = None,
+    ):
+        self.end_time = end_time
+        self.finish = finish
+        self.items = items
+        self.job_id = job_id
+        self.start_time = start_time
+        self.total_records = total_records
+
+    def validate(self):
+        if self.items:
+            self.items.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.finish is not None:
+            result['Finish'] = self.finish
+        if self.items is not None:
+            result['Items'] = self.items.to_map()
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.total_records is not None:
+            result['TotalRecords'] = self.total_records
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('Finish') is not None:
+            self.finish = m.get('Finish')
+        if m.get('Items') is not None:
+            temp_model = DescribeSqlLogRecordsResponseBodyDataItems()
+            self.items = temp_model.from_map(m['Items'])
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TotalRecords') is not None:
+            self.total_records = m.get('TotalRecords')
+        return self
+
+
+class DescribeSqlLogRecordsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribeSqlLogRecordsResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        # SqlLogDetailResult
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeSqlLogRecordsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DescribeSqlLogRecordsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeSqlLogRecordsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeSqlLogRecordsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeSqlLogStatisticRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+    ):
+        self.instance_id = instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        return self
+
+
+class DescribeSqlLogStatisticResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        cold_sql_size: int = None,
+        free_cold_sql_size: int = None,
+        free_hot_sql_size: int = None,
+        hot_sql_size: int = None,
+        import_sql_size: int = None,
+        timestamp: int = None,
+    ):
+        self.cold_sql_size = cold_sql_size
+        self.free_cold_sql_size = free_cold_sql_size
+        self.free_hot_sql_size = free_hot_sql_size
+        self.hot_sql_size = hot_sql_size
+        self.import_sql_size = import_sql_size
+        self.timestamp = timestamp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cold_sql_size is not None:
+            result['ColdSqlSize'] = self.cold_sql_size
+        if self.free_cold_sql_size is not None:
+            result['FreeColdSqlSize'] = self.free_cold_sql_size
+        if self.free_hot_sql_size is not None:
+            result['FreeHotSqlSize'] = self.free_hot_sql_size
+        if self.hot_sql_size is not None:
+            result['HotSqlSize'] = self.hot_sql_size
+        if self.import_sql_size is not None:
+            result['ImportSqlSize'] = self.import_sql_size
+        if self.timestamp is not None:
+            result['Timestamp'] = self.timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColdSqlSize') is not None:
+            self.cold_sql_size = m.get('ColdSqlSize')
+        if m.get('FreeColdSqlSize') is not None:
+            self.free_cold_sql_size = m.get('FreeColdSqlSize')
+        if m.get('FreeHotSqlSize') is not None:
+            self.free_hot_sql_size = m.get('FreeHotSqlSize')
+        if m.get('HotSqlSize') is not None:
+            self.hot_sql_size = m.get('HotSqlSize')
+        if m.get('ImportSqlSize') is not None:
+            self.import_sql_size = m.get('ImportSqlSize')
+        if m.get('Timestamp') is not None:
+            self.timestamp = m.get('Timestamp')
+        return self
+
+
+class DescribeSqlLogStatisticResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribeSqlLogStatisticResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        # SqlLogStatistic
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeSqlLogStatisticResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DescribeSqlLogStatisticResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeSqlLogStatisticResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeSqlLogStatisticResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeSqlLogTaskRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        page_no: int = None,
+        page_size: int = None,
+        task_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.page_no = page_no
+        self.page_size = page_size
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class DescribeSqlLogTaskResponseBodyDataFilters(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: Any = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeSqlLogTaskResponseBodyDataQueries(TeaModel):
+    def __init__(
+        self,
+        account_name: str = None,
+        consume: int = None,
+        cpu_time: int = None,
+        dbname: str = None,
+        execute_time: str = None,
+        ext: str = None,
+        frows: int = None,
+        host_address: str = None,
+        lock_time: int = None,
+        logic_read: int = None,
+        node_id: str = None,
+        origin_time: int = None,
+        parallel_degree: str = None,
+        parallel_queue_time: str = None,
+        physic_async_read: int = None,
+        physic_read: int = None,
+        physic_sync_read: int = None,
+        return_rows: int = None,
+        rows: int = None,
+        scan_rows: int = None,
+        scnt: int = None,
+        sql_id: str = None,
+        sql_text: str = None,
+        sql_type: str = None,
+        state: str = None,
+        thread_id: int = None,
+        trace_id: str = None,
+        trx_id: int = None,
+        update_rows: int = None,
+        use_imci_engine: str = None,
+        vip: str = None,
+        writes: int = None,
+    ):
+        self.account_name = account_name
+        self.consume = consume
+        self.cpu_time = cpu_time
+        self.dbname = dbname
+        # yyyy-MM-dd\"T\"HH:mm:ss.SSS\"Z\"
+        self.execute_time = execute_time
+        self.ext = ext
+        self.frows = frows
+        self.host_address = host_address
+        self.lock_time = lock_time
+        self.logic_read = logic_read
+        self.node_id = node_id
+        # ts unix
+        self.origin_time = origin_time
+        self.parallel_degree = parallel_degree
+        self.parallel_queue_time = parallel_queue_time
+        self.physic_async_read = physic_async_read
+        self.physic_read = physic_read
+        self.physic_sync_read = physic_sync_read
+        self.return_rows = return_rows
+        self.rows = rows
+        self.scan_rows = scan_rows
+        self.scnt = scnt
+        self.sql_id = sql_id
+        self.sql_text = sql_text
+        self.sql_type = sql_type
+        self.state = state
+        self.thread_id = thread_id
+        self.trace_id = trace_id
+        self.trx_id = trx_id
+        self.update_rows = update_rows
+        self.use_imci_engine = use_imci_engine
+        self.vip = vip
+        self.writes = writes
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_name is not None:
+            result['AccountName'] = self.account_name
+        if self.consume is not None:
+            result['Consume'] = self.consume
+        if self.cpu_time is not None:
+            result['CpuTime'] = self.cpu_time
+        if self.dbname is not None:
+            result['DBName'] = self.dbname
+        if self.execute_time is not None:
+            result['ExecuteTime'] = self.execute_time
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.frows is not None:
+            result['Frows'] = self.frows
+        if self.host_address is not None:
+            result['HostAddress'] = self.host_address
+        if self.lock_time is not None:
+            result['LockTime'] = self.lock_time
+        if self.logic_read is not None:
+            result['LogicRead'] = self.logic_read
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.origin_time is not None:
+            result['OriginTime'] = self.origin_time
+        if self.parallel_degree is not None:
+            result['ParallelDegree'] = self.parallel_degree
+        if self.parallel_queue_time is not None:
+            result['ParallelQueueTime'] = self.parallel_queue_time
+        if self.physic_async_read is not None:
+            result['PhysicAsyncRead'] = self.physic_async_read
+        if self.physic_read is not None:
+            result['PhysicRead'] = self.physic_read
+        if self.physic_sync_read is not None:
+            result['PhysicSyncRead'] = self.physic_sync_read
+        if self.return_rows is not None:
+            result['ReturnRows'] = self.return_rows
+        if self.rows is not None:
+            result['Rows'] = self.rows
+        if self.scan_rows is not None:
+            result['ScanRows'] = self.scan_rows
+        if self.scnt is not None:
+            result['Scnt'] = self.scnt
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text is not None:
+            result['SqlText'] = self.sql_text
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        if self.state is not None:
+            result['State'] = self.state
+        if self.thread_id is not None:
+            result['ThreadId'] = self.thread_id
+        if self.trace_id is not None:
+            result['TraceId'] = self.trace_id
+        if self.trx_id is not None:
+            result['TrxId'] = self.trx_id
+        if self.update_rows is not None:
+            result['UpdateRows'] = self.update_rows
+        if self.use_imci_engine is not None:
+            result['UseImciEngine'] = self.use_imci_engine
+        if self.vip is not None:
+            result['Vip'] = self.vip
+        if self.writes is not None:
+            result['Writes'] = self.writes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountName') is not None:
+            self.account_name = m.get('AccountName')
+        if m.get('Consume') is not None:
+            self.consume = m.get('Consume')
+        if m.get('CpuTime') is not None:
+            self.cpu_time = m.get('CpuTime')
+        if m.get('DBName') is not None:
+            self.dbname = m.get('DBName')
+        if m.get('ExecuteTime') is not None:
+            self.execute_time = m.get('ExecuteTime')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Frows') is not None:
+            self.frows = m.get('Frows')
+        if m.get('HostAddress') is not None:
+            self.host_address = m.get('HostAddress')
+        if m.get('LockTime') is not None:
+            self.lock_time = m.get('LockTime')
+        if m.get('LogicRead') is not None:
+            self.logic_read = m.get('LogicRead')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('OriginTime') is not None:
+            self.origin_time = m.get('OriginTime')
+        if m.get('ParallelDegree') is not None:
+            self.parallel_degree = m.get('ParallelDegree')
+        if m.get('ParallelQueueTime') is not None:
+            self.parallel_queue_time = m.get('ParallelQueueTime')
+        if m.get('PhysicAsyncRead') is not None:
+            self.physic_async_read = m.get('PhysicAsyncRead')
+        if m.get('PhysicRead') is not None:
+            self.physic_read = m.get('PhysicRead')
+        if m.get('PhysicSyncRead') is not None:
+            self.physic_sync_read = m.get('PhysicSyncRead')
+        if m.get('ReturnRows') is not None:
+            self.return_rows = m.get('ReturnRows')
+        if m.get('Rows') is not None:
+            self.rows = m.get('Rows')
+        if m.get('ScanRows') is not None:
+            self.scan_rows = m.get('ScanRows')
+        if m.get('Scnt') is not None:
+            self.scnt = m.get('Scnt')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlText') is not None:
+            self.sql_text = m.get('SqlText')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        if m.get('State') is not None:
+            self.state = m.get('State')
+        if m.get('ThreadId') is not None:
+            self.thread_id = m.get('ThreadId')
+        if m.get('TraceId') is not None:
+            self.trace_id = m.get('TraceId')
+        if m.get('TrxId') is not None:
+            self.trx_id = m.get('TrxId')
+        if m.get('UpdateRows') is not None:
+            self.update_rows = m.get('UpdateRows')
+        if m.get('UseImciEngine') is not None:
+            self.use_imci_engine = m.get('UseImciEngine')
+        if m.get('Vip') is not None:
+            self.vip = m.get('Vip')
+        if m.get('Writes') is not None:
+            self.writes = m.get('Writes')
+        return self
+
+
+class DescribeSqlLogTaskResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        create_time: int = None,
+        end: int = None,
+        expire: bool = None,
+        export: str = None,
+        filters: List[DescribeSqlLogTaskResponseBodyDataFilters] = None,
+        name: str = None,
+        queries: List[DescribeSqlLogTaskResponseBodyDataQueries] = None,
+        start: int = None,
+        status: str = None,
+        task_id: str = None,
+        task_type: str = None,
+        total: int = None,
+    ):
+        self.create_time = create_time
+        self.end = end
+        self.expire = expire
+        self.export = export
+        self.filters = filters
+        self.name = name
+        self.queries = queries
+        self.start = start
+        self.status = status
+        self.task_id = task_id
+        self.task_type = task_type
+        self.total = total
+
+    def validate(self):
+        if self.filters:
+            for k in self.filters:
+                if k:
+                    k.validate()
+        if self.queries:
+            for k in self.queries:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.end is not None:
+            result['End'] = self.end
+        if self.expire is not None:
+            result['Expire'] = self.expire
+        if self.export is not None:
+            result['Export'] = self.export
+        result['Filters'] = []
+        if self.filters is not None:
+            for k in self.filters:
+                result['Filters'].append(k.to_map() if k else None)
+        if self.name is not None:
+            result['Name'] = self.name
+        result['Queries'] = []
+        if self.queries is not None:
+            for k in self.queries:
+                result['Queries'].append(k.to_map() if k else None)
+        if self.start is not None:
+            result['Start'] = self.start
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        if self.task_type is not None:
+            result['TaskType'] = self.task_type
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('Expire') is not None:
+            self.expire = m.get('Expire')
+        if m.get('Export') is not None:
+            self.export = m.get('Export')
+        self.filters = []
+        if m.get('Filters') is not None:
+            for k in m.get('Filters'):
+                temp_model = DescribeSqlLogTaskResponseBodyDataFilters()
+                self.filters.append(temp_model.from_map(k))
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        self.queries = []
+        if m.get('Queries') is not None:
+            for k in m.get('Queries'):
+                temp_model = DescribeSqlLogTaskResponseBodyDataQueries()
+                self.queries.append(temp_model.from_map(k))
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        if m.get('TaskType') is not None:
+            self.task_type = m.get('TaskType')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class DescribeSqlLogTaskResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribeSqlLogTaskResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        # SqlLogTaskDetail
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeSqlLogTaskResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DescribeSqlLogTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeSqlLogTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeSqlLogTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeSqlLogTasksRequestFilters(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeSqlLogTasksRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        filters: List[DescribeSqlLogTasksRequestFilters] = None,
+        instance_id: str = None,
+        node_id: str = None,
+        page_no: int = None,
+        page_size: int = None,
+        start_time: int = None,
+    ):
+        self.end_time = end_time
+        self.filters = filters
+        self.instance_id = instance_id
+        self.node_id = node_id
+        self.page_no = page_no
+        self.page_size = page_size
+        self.start_time = start_time
+
+    def validate(self):
+        if self.filters:
+            for k in self.filters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        result['Filters'] = []
+        if self.filters is not None:
+            for k in self.filters:
+                result['Filters'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        self.filters = []
+        if m.get('Filters') is not None:
+            for k in m.get('Filters'):
+                temp_model = DescribeSqlLogTasksRequestFilters()
+                self.filters.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeSqlLogTasksResponseBodyDataListFilters(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeSqlLogTasksResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        analysis_task_finish_time: int = None,
+        analysis_task_status: str = None,
+        create_time: int = None,
+        end: int = None,
+        expire: bool = None,
+        filters: List[DescribeSqlLogTasksResponseBodyDataListFilters] = None,
+        instance_id: str = None,
+        log_count: int = None,
+        name: str = None,
+        progress: int = None,
+        result: str = None,
+        scan_file_size: int = None,
+        start: int = None,
+        status: str = None,
+        task_id: str = None,
+        task_type: str = None,
+    ):
+        self.analysis_task_finish_time = analysis_task_finish_time
+        self.analysis_task_status = analysis_task_status
+        self.create_time = create_time
+        self.end = end
+        self.expire = expire
+        self.filters = filters
+        self.instance_id = instance_id
+        self.log_count = log_count
+        self.name = name
+        self.progress = progress
+        self.result = result
+        self.scan_file_size = scan_file_size
+        self.start = start
+        self.status = status
+        self.task_id = task_id
+        self.task_type = task_type
+
+    def validate(self):
+        if self.filters:
+            for k in self.filters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.analysis_task_finish_time is not None:
+            result['AnalysisTaskFinishTime'] = self.analysis_task_finish_time
+        if self.analysis_task_status is not None:
+            result['AnalysisTaskStatus'] = self.analysis_task_status
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.end is not None:
+            result['End'] = self.end
+        if self.expire is not None:
+            result['Expire'] = self.expire
+        result['Filters'] = []
+        if self.filters is not None:
+            for k in self.filters:
+                result['Filters'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.log_count is not None:
+            result['LogCount'] = self.log_count
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.progress is not None:
+            result['Progress'] = self.progress
+        if self.result is not None:
+            result['Result'] = self.result
+        if self.scan_file_size is not None:
+            result['ScanFileSize'] = self.scan_file_size
+        if self.start is not None:
+            result['Start'] = self.start
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        if self.task_type is not None:
+            result['TaskType'] = self.task_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AnalysisTaskFinishTime') is not None:
+            self.analysis_task_finish_time = m.get('AnalysisTaskFinishTime')
+        if m.get('AnalysisTaskStatus') is not None:
+            self.analysis_task_status = m.get('AnalysisTaskStatus')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('Expire') is not None:
+            self.expire = m.get('Expire')
+        self.filters = []
+        if m.get('Filters') is not None:
+            for k in m.get('Filters'):
+                temp_model = DescribeSqlLogTasksResponseBodyDataListFilters()
+                self.filters.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('LogCount') is not None:
+            self.log_count = m.get('LogCount')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Progress') is not None:
+            self.progress = m.get('Progress')
+        if m.get('Result') is not None:
+            self.result = m.get('Result')
+        if m.get('ScanFileSize') is not None:
+            self.scan_file_size = m.get('ScanFileSize')
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        if m.get('TaskType') is not None:
+            self.task_type = m.get('TaskType')
+        return self
+
+
+class DescribeSqlLogTasksResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        list: List[DescribeSqlLogTasksResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = DescribeSqlLogTasksResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class DescribeSqlLogTasksResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribeSqlLogTasksResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        # ListResult<SqlLogTask>
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeSqlLogTasksResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DescribeSqlLogTasksResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeSqlLogTasksResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeSqlLogTasksResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeTopBigKeysRequest(TeaModel):
     def __init__(
         self,
         console_context: str = None,
         end_time: str = None,
         instance_id: str = None,
         node_id: str = None,
@@ -10443,20 +12561,20 @@
         console_context: str = None,
         instance_ids: str = None,
     ):
         # The reserved parameter.
         self.console_context = console_context
         # The database instance IDs.
         # 
-        # *   Set this parameter to a JSON array that consists of multiple instance IDs. Separate instance IDs with commas (,). Example: `[\"Instance ID1\",\"Instance ID2\"]`.
+        # *   Specify the parameter value as a JSON array, such as `[\"Database account 1\",\"Database account 2\"]`. Separate database instance IDs with commas (,).
         # 
         # *   By default, if you leave this parameter empty, all database instances for which the automatic fragment recycling feature has been enabled within the current Alibaba Cloud account are returned. The following types of database instances are returned:
         # 
         #     *   Database instances for which the automatic fragment recycling feature is currently enabled.
-        #     *   Database instances for which the automatic fragment recycling feature was once enabled but is currently disabled, including those for which DAS Professional Edition has been disabled but excluding those that have been released.
+        #     *   Database instances for which the automatic fragment recycling feature was once enabled but is currently disabled, including those for which DAS Enterprise Edition has been disabled but excluding those that have been released.
         self.instance_ids = instance_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10487,21 +12605,21 @@
         instance_id: str = None,
         table_fragmentation_ratio: float = None,
         table_space_size: float = None,
         user_id: str = None,
     ):
         # Indicates whether the automatic fragment recycling feature is enabled. Valid values:
         # 
-        # * **true**\
-        # * **false**\
+        # *   **true**\
+        # *   **false**\
         self.auto_defragment = auto_defragment
-        # Indicates whether DAS Professional Edition is enabled. Valid values:
+        # Indicates whether DAS Enterprise Edition is enabled. Valid values:
         # 
-        # * **true**\
-        # * **false**\
+        # *   **true**\
+        # *   **false**\
         self.das_pro_on = das_pro_on
         # The database instance ID.
         self.instance_id = instance_id
         # The fragmentation rate of a single physical table for which the automatic fragment recycling feature is enabled.
         self.table_fragmentation_ratio = table_fragmentation_ratio
         # The minimum storage usage of a single physical table for which the automatic fragment recycling feature is enabled. Unit: GB.
         self.table_space_size = table_space_size
@@ -10556,21 +12674,21 @@
         instance_id: str = None,
         table_fragmentation_ratio: float = None,
         table_space_size: float = None,
         user_id: str = None,
     ):
         # Indicates whether the automatic fragment recycling feature is enabled. Valid values:
         # 
-        # * **true**\
-        # * **false**\
+        # *   **true**\
+        # *   **false**\
         self.auto_defragment = auto_defragment
-        # Indicates whether DAS Professional Edition is enabled. Valid values:
+        # Indicates whether DAS Enterprise Edition is enabled. Valid values:
         # 
-        # * **true**\
-        # * **false**\
+        # *   **true**\
+        # *   **false**\
         self.das_pro_on = das_pro_on
         # The database instance ID.
         self.instance_id = instance_id
         # The fragmentation rate of a single physical table for which the automatic fragment recycling feature is enabled.
         self.table_fragmentation_ratio = table_fragmentation_ratio
         # The minimum storage usage of a single physical table for which the automatic fragment recycling feature is enabled. Unit: GB.
         self.table_space_size = table_space_size
@@ -10625,30 +12743,27 @@
         instance_id: str = None,
         table_fragmentation_ratio: float = None,
         table_space_size: float = None,
         user_id: str = None,
     ):
         # Indicates whether the automatic fragment recycling feature is enabled. Valid values:
         # 
-        # * **true**\
-        # * **false**\
+        # *   **true**:
+        # *   **false**\
         self.auto_defragment = auto_defragment
-        # Indicates whether DAS Professional Edition is enabled. Valid values:
+        # Indicates whether DAS Enterprise Edition is enabled. Valid values:
         # 
-        # * **true**\
-        # * **false**\
+        # *   **true**\
+        # *   **false**\
         self.das_pro_on = das_pro_on
         # The database instance ID.
         self.instance_id = instance_id
         # The fragmentation rate of a single physical table for which the automatic fragment recycling feature is enabled.
         self.table_fragmentation_ratio = table_fragmentation_ratio
-        # Indicates whether the automatic fragment recycling feature is enabled. Valid values:
-        # 
-        # true
-        # false
+        # The minimum storage usage of a single physical table for which the automatic fragment recycling feature is enabled. Unit: GB.
         self.table_space_size = table_space_size
         # The ID of the Alibaba Cloud account that is used to create the database instance.
         self.user_id = user_id
 
     def validate(self):
         pass
 
@@ -10702,19 +12817,19 @@
         turn_off_auto_resource_optimize_count: int = None,
         turn_off_auto_resource_optimize_list: List[GetAutoResourceOptimizeRulesResponseBodyDataTurnOffAutoResourceOptimizeList] = None,
     ):
         # The number of database instances for which the automatic fragment recycling feature is currently enabled.
         self.enable_auto_resource_optimize_count = enable_auto_resource_optimize_count
         # The database instances for which the automatic fragment recycling feature is currently enabled.
         self.enable_auto_resource_optimize_list = enable_auto_resource_optimize_list
-        # The number of database instances for which the automatic fragment recycling feature is enabled and DAS Professional Edition is disabled.
+        # The number of database instances for which the automatic fragment recycling feature is enabled and DAS Enterprise Edition is disabled.
         self.has_enable_rule_but_not_das_pro_count = has_enable_rule_but_not_das_pro_count
-        # The database instances for which the automatic fragment recycling feature is enabled and DAS Professional Edition is disabled.
+        # The database instances for which the automatic fragment recycling feature is enabled and DAS Enterprise Edition is disabled.
         # 
-        # > This type of database instance does not perform automatic fragment recycling tasks until DAS Professional Edition is enabled for the instances again.
+        # >  Automatic fragment recycling tasks are run on this type of database instances only if DAS Enterprise Edition is enabled for the database instances again.
         self.has_enable_rule_but_not_das_pro_list = has_enable_rule_but_not_das_pro_list
         # The number of database instances that do not exist or for which the automatic fragment recycling feature has never been enabled.
         # 
         # >  If a database instance does not exist, the instance has been released or the specified instance ID is invalid.
         self.never_enable_auto_resource_optimize_or_released_instance_count = never_enable_auto_resource_optimize_or_released_instance_count
         # The database instances that do not exist or for which the automatic fragment recycling feature has never been enabled.
         self.never_enable_auto_resource_optimize_or_released_instance_id_list = never_enable_auto_resource_optimize_or_released_instance_id_list
@@ -12405,27 +14520,27 @@
         sql_retention: str = None,
         start_time: int = None,
         storage_free_quota_in_mb: float = None,
         storage_used: int = None,
         user_id: str = None,
         vpc_id: str = None,
     ):
-        # The ID of the DAS Professional Edition instance.
+        # The ID of the DAS Enterprise Edition instance.
         self.commodity_instance_id = commodity_instance_id
         # The type of the database engine.
         self.engine = engine
-        # The point of time when DAS Professional Edition for the database instance expires. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        # The point of time when DAS Enterprise Edition for the database instance expires. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.expire_time = expire_time
         # The name of the database instance.
         self.instance_alias = instance_alias
         # The database instance ID.
         self.instance_id = instance_id
         # The endpoint of the database instance.
         self.ip = ip
-        # Indicates whether DAS Professional Edition for the database instance has expired. Valid values:
+        # Indicates whether DAS Enterprise Edition for the database instance has expired. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.is_spare = is_spare
         # The estimated remaining time for migrating the data generated by the SQL Explorer and Audit feature from the previous version to the new version. Unit: milliseconds.
         # 
         # >  This parameter is returned only when the SQL Explorer and Audit feature is migrated from the previous version to the new version.
@@ -12434,15 +14549,15 @@
         self.port = port
         # The region in which the database instance resides.
         self.region = region
         # The service unit ID.
         self.service_unit_id = service_unit_id
         # The storage duration of SQL Explorer data. Unit: days.
         self.sql_retention = sql_retention
-        # The time when DAS Professional Edition was enabled for the database instance. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        # The time when DAS Enterprise Edition was enabled for the database instance. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.start_time = start_time
         # The SQL Explorer storage space that is offered free-of-charge. Unit: MB.
         self.storage_free_quota_in_mb = storage_free_quota_in_mb
         # The storage usage of SQL Explorer of the database instance. Unit: bytes.
         self.storage_used = storage_used
         # The ID of the Alibaba Cloud account that is used to create the database instance.
         self.user_id = user_id
@@ -15551,18 +17666,18 @@
         # 
         # >  This parameter is optional. If this parameter is specified, the full request statistics of the specified IP address are collected. If this parameter is left empty, the full request statistics of the entire database instance are collected.
         self.origin_host = origin_host
         # The page number. Pages start from page 1. Default value: 1.
         self.page_no = page_no
         # The number of entries per page. Default value: 20.
         self.page_size = page_size
-        # The role of the PolarDB-X 2.0 node. Valid values:
+        # The role of the node in the PolarDB-X 2.0 instance. Valid values:
         # 
-        # *   **polarx_cn**: compute node
-        # *   **polarx_en**: data node
+        # *   **polarx_cn**: compute node.
+        # *   **polarx_dn**: data node.
         self.role = role
         # The SQL ID.
         # 
         # >  If this parameter is specified, the full request statistics of the specified SQL query are collected. If this parameter is left empty, the full request statistics of the entire database instance are collected.
         self.sql_id = sql_id
         # The type of the SQL statement. Valid values: **SELECT**, **INSERT**, **UPDATE**, **DELETE**, **LOGIN**, **LOGOUT**, **MERGE**, **ALTER**, **CREATEINDEX**, **DROPINDEX**, **CREATE**, **DROP**, **SET**, **DESC**, **REPLACE**, **CALL**, **BEGIN**, **DESCRIBE**, **ROLLBACK**, **FLUSH**, **USE**, **SHOW**, **START**, **COMMIT**, and **RENAME**.
         # 
@@ -16812,41 +18927,41 @@
         auto_limited_sql: int = None,
         auto_resource_optimize: int = None,
         auto_scale: int = None,
         event_subscription: int = None,
     ):
         # Indicates whether the feature of automatically creating and deleting indexes is enabled. Valid values:
         # 
-        # * **0**: disabled.
-        # * **1**: enabled.
-        # * **2**: not supported.
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        # *   **2**: not supported.
         self.auto_index = auto_index
         # Indicates whether the automatic throttling feature is enabled. Valid values:
         # 
-        # * **0**: disabled.
-        # * **1**: enabled.
-        # * **2**: not supported.
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        # *   **2**: not supported.
         self.auto_limited_sql = auto_limited_sql
-        # Indicates whether automatic reclamation of fragments is enabled. Valid values:
+        # Indicates whether the automatic fragment recycling feature is enabled. Valid values:
         # 
-        # * **0**: disabled.
-        # * **1**: enabled.
-        # * **2**: not supported.
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        # *   **2**: not supported.
         self.auto_resource_optimize = auto_resource_optimize
         # Indicates whether the auto scaling feature is enabled. Valid values:
         # 
-        # * **0**: disabled.
-        # * **1**: enabled.
-        # * **2**: not supported.
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        # *   **2**: not supported.
         self.auto_scale = auto_scale
         # Indicates whether the event subscription feature is enabled. Valid values:
         # 
-        # * **0**: disabled.
-        # * **1**: enabled.
-        # * **2**: not supported.
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        # *   **2**: not supported.
         self.event_subscription = event_subscription
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16897,52 +19012,52 @@
         network_type: str = None,
         node_id: str = None,
         region: str = None,
         storage: int = None,
         uuid: str = None,
         vpc_id: str = None,
     ):
-        # The account ID. You can obtain the account ID on the **Security Settings** page in the Alibaba Cloud **account management center**.
+        # The account ID. You can view the ID of the logon account by moving the pointer over the profile in the Alibaba Cloud management console.
         self.account_id = account_id
         # The connection mode of the instance. Valid values:
         # 
-        # * **standard**: standard mode.
-        # * **safe**: database proxy mode.
+        # *   **standard**: standard mode.
+        # *   **safe**: database proxy mode.
         self.category = category
         # The CPU specification of the instance. For example, if a value of 8 is returned, the instance has eight CPU cores.
         self.cpu = cpu
         # The database engine. Valid values:
         # 
-        # * **MySQL**\
-        # * **Redis**\
-        # * **PolarDBMySQL**\
+        # *   **MySQL**\
+        # *   **Redis**\
+        # *   **PolarDBMySQL**\
         self.engine = engine
         # The version number of the database engine.
         self.engine_version = engine_version
-        # The name of the instance.
+        # The instance name.
         self.instance_alias = instance_alias
         # The type of the instance on which the database is deployed. Valid values:
         # 
-        # * **RDS**: an Alibaba Cloud database instance.
-        # * **ECS**: an ECS instance on which a self-managed database is deployed.
-        # * **IDC**: a self-managed database instance that is not deployed on Alibaba Cloud.
+        # *   **RDS**: an Alibaba Cloud database instance.
+        # *   **ECS**: an Elastic Compute Service (ECS) instance on which a self-managed database is deployed.
+        # *   **IDC**: a self-managed database instance that is not deployed on Alibaba Cloud.
         # 
-        # > The value IDC indicates that the instance is deployed in a data center.
+        # >  The value IDC indicates that the instance is deployed in a data center.
         self.instance_area = instance_area
         # The instance type.
         self.instance_class = instance_class
         # The instance ID.
         self.instance_id = instance_id
         # The memory capacity of the database that is deployed on the instance. Unit: MB.
         self.memory = memory
         # The network type of the instance.
         self.network_type = network_type
         # The ID of the node on the instance.
         self.node_id = node_id
-        # The ID of the region in which the instance resides.
+        # The region ID of the instance.
         self.region = region
         # The storage space of the instance. Unit: GB.
         self.storage = storage
         # The unique identifier of the instance.
         self.uuid = uuid
         # The ID of the virtual private cloud (VPC) in which the instance is deployed.
         self.vpc_id = vpc_id
@@ -17040,46 +19155,46 @@
         score_map: Dict[str, Any] = None,
         start_time: int = None,
         state: int = None,
         task_type: int = None,
     ):
         # Indicates whether the autonomy service is enabled.
         self.auto_function = auto_function
-        # The returned data.
+        # The data returned.
         self.data = data
-        # Indicates whether DAS Professional Edition is enabled. Valid values:
+        # Indicates whether DAS Enterprise Edition is enabled. Valid values:
         # 
-        # * **0**: disabled.
-        # * **1**: enabled.
-        # * **2**: not supported.
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        # *   **2**: not supported.
         self.enable_das_pro = enable_das_pro
         # The end time of the inspection and scoring task. The value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         # 
-        # > The end time must be later than the start time.
+        # >  The end time must be later than the start time.
         self.end_time = end_time
         # The time when the task was created. The value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.gmt_create = gmt_create
-        # The details of the instance.
+        # The information about the instance.
         self.instance = instance
-        # The inspection scores of the instance.
+        # The inspection score of the instance.
         self.score = score
         # The scores that are deducted for the instance.
         self.score_map = score_map
-        # The start time of the inspection and scoring task. The value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        # The start time of the inspection and scoring task. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.start_time = start_time
         # The state of the inspection and scoring task. Valid values:
         # 
-        # * **0**: The task is waiting for execution.
-        # * **1**: The task is in progress.
-        # * **2**: The task is complete.
+        # *   **0**: The task is waiting for execution.
+        # *   **1**: The task is in progress.
+        # *   **2**: The task is complete.
         self.state = state
         # The mode in which the inspection and scoring task was initiated. Valid values:
         # 
-        # * **0**: automatic mode
-        # * **1**: manual mode
+        # *   **0**: automatic mode.
+        # *   **1**: manual mode.
         self.task_type = task_type
 
     def validate(self):
         if self.auto_function:
             self.auto_function.validate()
         if self.instance:
             self.instance.validate()
@@ -17147,18 +19262,15 @@
     def __init__(
         self,
         list: List[GetInstanceInspectionsResponseBodyDataList] = None,
         page_no: int = None,
         page_size: int = None,
         total: int = None,
     ):
-        # The mode in which the inspection and scoring task was initiated. Valid values:
-        # 
-        # *   **0**: automatic mode
-        # *   **1**: manual mode
+        # The detailed information.
         self.list = list
         # The page number. The value returned is a positive integer. Default value: 1.
         self.page_no = page_no
         # The number of entries per page. Default value: 10.
         self.page_size = page_size
         # The total number of entries returned.
         self.total = total
@@ -17210,15 +19322,15 @@
         data: GetInstanceInspectionsResponseBodyData = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
         # The HTTP status code returned.
         self.code = code
-        # The inspection and scoring results.
+        # The details.
         self.data = data
         # The returned message.
         # 
         # >  If the request was successful, Successful is returned. If the request failed, an error message such as an error code is returned.
         self.message = message
         # The request ID.
         self.request_id = request_id
@@ -17757,28 +19869,28 @@
         node_id: str = None,
         start_time: str = None,
         threshold: str = None,
         use_merging: str = None,
     ):
         # The end of the time range to query. Set this parameter to a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.end_time = end_time
-        # Specifies whether to filter instances for which DAS Professional Edition is enabled. Valid values:
+        # Specifies whether to filter instances for which DAS Enterprise Edition is enabled. Valid values:
         # 
-        # *   **true**: filters instances for which DAS Professional Edition is enabled.
-        # *   **false**: does not filter instances for which DAS Professional Edition is enabled.
+        # *   **true**\
+        # *   **false**\
         # 
-        # >  If you set the value to **true**, only database instances for which DAS Professional Edition is disabled are queried. If you set the value to **false**, all database instances are queried.
+        # >  If you set this parameter to **true**, only database instances for which DAS Enterprise Edition is disabled are queried. If you set this parameter to **false**, all database instances are queried.
         self.filter_enable = filter_enable
         # The database instance ID.
         # 
         # >  The database instance must be an ApsaraDB RDS for MySQL instance or a PolarDB for MySQL cluster.
         self.instance_id = instance_id
         # The node ID.
         # 
-        # >  This parameter must be specified if the database instance is an ApsaraDB RDS for MySQL Cluster Edition instance or a PolarDB for MySQL cluster.
+        # >  For ApsaraDB RDS for MySQL Cluster Edition instances or PolarDB for MySQL clusters, you must specify the node ID.
         self.node_id = node_id
         # The beginning of the time range to query. Set this parameter to a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.start_time = start_time
         # The duration threshold for automatic SQL optimization events. After this parameter is specified, the system collects statistics on automatic SQL optimization events whose duration does not exceed the specified threshold.
         # 
         # >  This parameter is a reserved parameter and does not take effect.
         self.threshold = threshold
@@ -19758,29 +21870,29 @@
         self,
         end_time: int = None,
         instance_id: str = None,
         node_id: str = None,
         sql_id: str = None,
         start_time: int = None,
     ):
-        # The end of the time range to query. Set this parameter to a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        # The end of the time range to query. The value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         # 
-        # >  The end time must be later than the start time. You can query the data of up to seven days within the last month.
+        # >  The end time must be later than the start time. You can view the data of up to seven days in the previous 30 days.
         self.end_time = end_time
         # The instance ID.
         # 
-        # >  Only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters are supported.
+        # >  Only ApsaraDB RDS for MySQL instances and PolarDB for MySQL clusters are supported
         self.instance_id = instance_id
         # The node ID.
         # 
-        # >  This parameter must be specified for ApsaraDB RDS for MySQL Cluster Edition instances and PolarDB for MySQL clusters.
+        # >  For ApsaraDB RDS for MySQL Cluster Edition instances or PolarDB for MySQL clusters, you must specify the node ID.
         self.node_id = node_id
         # The SQL ID.
         self.sql_id = sql_id
-        # The beginning of the time range to query. Set this parameter to a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        # The beginning of the time range to query. The value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19867,61 +21979,61 @@
         self.event_name = event_name
         # The instance ID.
         self.instance_id = instance_id
         # The execution duration. Unit: millisecond.
         self.latency = latency
         # The lock wait duration. Unit: millisecond.
         self.lock_latency = lock_latency
-        # The logical database ID.
+        # The ID of the logical database.
         self.logic_id = logic_id
         # Indicates whether the server failed to find an index that can be used for the SQL statement. Valid values:
         # 
-        # * **1:** yes.
-        # * **0:** no.
+        # *   **1**: yes.
+        # *   **0**: no.
         self.no_good_index_used = no_good_index_used
         # Indicates whether table scans were performed when indexes were not used. Valid values:
         # 
-        # * **1:** yes.
-        # * **0:** no.
+        # *   **1**: yes.
+        # *   **0**: no.
         self.no_index_used = no_index_used
         # The node ID.
         # 
-        # > This parameter is returned only for ApsaraDB RDS for MySQL Cluster Edition instances and PolarDB for MySQL clusters.
+        # >  This parameter is returned only for ApsaraDB RDS for MySQL Cluster Edition instances or PolarDB for MySQL clusters.
         self.node_id = node_id
         # The number of rows affected by the SQL statement.
         self.rows_affected = rows_affected
         # The number of rows scanned by the SQL statement.
         self.rows_examined = rows_examined
         # The number of rows returned by the SQL statement.
         self.rows_sent = rows_sent
         # The number of joins that are used to perform table scans without using indexes.
         # 
-        # > This parameter is used to count the number of joins that did not use indexes. If the value of this parameter is not 0, check the table indexes.
+        # > : This parameter is used for the scenario in which indexes are not used in a union query. If the returned value is not 0, check the indexes of tables.
         self.select_full_join = select_full_join
         # The number of joins that used ranges on referenced tables.
         self.select_full_range_join = select_full_range_join
         # The number of joins that used ranges on the first table.
         self.select_range = select_range
         # The number of joins that did not have key values. The keys and values were checked for each row of data.
         # 
-        # >  This parameter is used to count the number of joins that did not use indexes. If the value of this parameter is not 0, check the table indexes.
+        # > : This parameter is used for the scenario in which indexes are not used in a union query. If the returned value is not 0, check the indexes of tables.
         self.select_range_check = select_range_check
         # The number of scans.
         self.select_scan = select_scan
         # The number of merges that the sorting algorithm must perform.
         self.sort_merge_passes = sort_merge_passes
         # The number of times the data was sorted by using ranges.
         self.sort_range = sort_range
         # The number of sorted rows.
         self.sort_rows = sort_rows
         # The number of sorts that were performed during table scans.
         self.sort_scan = sort_scan
-        # The SQL sample.
+        # The sample SQL statement.
         self.sql = sql
-        # The SQL ID.
+        # The SQL statement ID.
         self.sql_id = sql_id
         # The thread ID.
         self.thread_id = thread_id
         # The time when the SQL statement was executed. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.timestamp = timestamp
         # The user ID.
         self.user_id = user_id
@@ -20079,15 +22191,15 @@
         data: List[GetPfsSqlSampleResponseBodyData] = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         # The HTTP status code returned.
         self.code = code
-        # The queried SQL sample data.
+        # The SQL sample data.
         self.data = data
         # The returned message.
         # 
         # >  If the request was successful, **Successful** is returned. If the request failed, an error message such as an error code is returned.
         self.message = message
         # The request ID.
         self.request_id = request_id
@@ -26588,15 +28700,15 @@
         # *   **95**\
         self.bandwidth_usage_upper_threshold = bandwidth_usage_upper_threshold
         # Specifies whether to enable the automatic bandwidth downgrade feature. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.downgrade = downgrade
-        # The observation window of the automatic bandwidth upgrade feature. The value of this parameter consists of a numeric value and a time unit suffix. The **m** time unit suffix specifies the minute. Valid values:
+        # The observation window of the automatic bandwidth adjustment feature. The value of this parameter consists of a numeric value and a time unit suffix. The **m** time unit suffix specifies the minute. Valid values:
         # 
         # *   **1m**\
         # *   **5m**\
         # *   **10m**\
         # *   **15m**\
         # *   **30m**\
         self.observation_window_size = observation_window_size
@@ -26740,15 +28852,15 @@
         upgrade_observation_window_size: str = None,
     ):
         # Specifies whether to apply the **Shard** configuration of the auto scaling feature for shards. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         # 
-        # >  The auto scaling feature for shards is available only for ApsaraDB for Redis Community Edition instances that use cloud disks on the China site (aliyun.com).
+        # > The auto scaling feature for shards is available only for ApsaraDB for Redis Community Edition cloud-native instances on the China site (aliyun.com).
         self.apply = apply
         # Specifies whether to enable the feature of automatically removing shards. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         # 
         # >  The feature of automatically removing shards is in canary release.
@@ -26871,47 +28983,47 @@
         # 
         # *   **50**\
         # *   **60**\
         # *   **70**\
         # *   **80**\
         # *   **90**\
         # 
-        # >  This parameter must be specified if the database instance is a PolarDB for MySQL Cluster Edition instance or an ApsaraDB RDS for MySQL High-availability Edition instance that uses standard SSDs or ESSDs.
+        # > This parameter must be specified if the database instance is a PolarDB for MySQL Cluster Edition instance or an ApsaraDB RDS for MySQL High-availability Edition instance that uses standard SSDs or ESSDs.
         self.cpu_usage_upper_threshold = cpu_usage_upper_threshold
         # Specifies whether to enable the automatic specification scale-down feature. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         # 
-        # >  This parameter must be specified if the database instance is a PolarDB for MySQL Cluster Edition instance or an ApsaraDB RDS for MySQL High-availability Edition instance that uses standard SSDs or ESSDs.
+        # > This parameter must be specified if the database instance is a PolarDB for MySQL Cluster Edition instance or an ApsaraDB RDS for MySQL High-availability Edition instance that uses standard SSDs or ESSDs.
         self.downgrade = downgrade
         # The maximum number of read-only nodes of the instance.
         # 
-        # >  This parameter must be specified if the database instance is a PolarDB for MySQL Cluster Edition instance.
+        # > This parameter must be specified if the database instance is a PolarDB for MySQL Cluster Edition instance.
         self.max_read_only_nodes = max_read_only_nodes
-        # The maximum specifications to which the database instance can be upgraded. The database instance can be upgraded only to a database instance of the same edition with higher specifications. For information about the specifications of different database instances, refer to the following topics:
+        # The maximum specifications to which the database instance can be scaled up. The database instance can be upgraded only to a database instance of the same edition with higher specifications. For information about the specifications of different database instances, see the following topics:
         # 
-        # *   PolarDB for MySQL Cluster Edition instances: [Specifications of compute nodes](~~102542~~).
-        # *   ApsaraDB RDS for MySQL High-availability Edition instances that use standard SSDs or ESSDs: [Specifications](~~276974~~).
+        # *   PolarDB for MySQL Cluster Edition instances: [Specifications of compute nodes](~~102542~~)
+        # *   ApsaraDB RDS for MySQL High-availability Edition instances that use standard SSDs or ESSDs: [Specifications](~~276974~~)
         self.max_spec = max_spec
         # The average memory usage threshold that triggers automatic specification scale-up. Unit: %. Valid values:
         # 
         # *   **50**\
         # *   **60**\
         # *   **70**\
         # *   **80**\
         # *   **90**\
         # 
-        # >  This parameter must be specified if the database instance is an ApsaraDB for Redis Community Edition instance that uses cloud disks on the China site (aliyun.com).
+        # > This parameter must be specified if the database instance is an ApsaraDB for Redis Community Edition cloud-native instance on the China site (aliyun.com).
         self.mem_usage_upper_threshold = mem_usage_upper_threshold
         # The observation window. The value of this parameter consists of a numeric value and a time unit suffix. The **m** time unit suffix specifies the minute and the **h** time unit suffix specifies the hour.
         # 
         # *   Valid values for PolarDB for MySQL Cluster Edition instances: **5m**, **10m**, **15m**, and **30m**.
         # *   Valid values for ApsaraDB RDS for MySQL High-availability Edition instances that use standard SSDs or ESSDs: **5m**, **20m**, **30m**, **40m**, and **1h**.
-        # *   Valid values for ApsaraDB for Redis Community Edition instances that use cloud disks: **5m**, **10m**, **15m**, and **30m**.
+        # *   Valid values for ApsaraDB for Redis Community Edition cloud-native instances: **5m**, **10m**, **15m**, and **30m**.
         self.observation_window_size = observation_window_size
         # Specifies whether to enable the automatic specification scale-up feature. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.upgrade = upgrade
 
@@ -27201,14 +29313,330 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyAutoScalingConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifySqlLogConfigRequestFilters(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ModifySqlLogConfigRequest(TeaModel):
+    def __init__(
+        self,
+        enable: bool = None,
+        filters: List[ModifySqlLogConfigRequestFilters] = None,
+        hot_retention: int = None,
+        instance_id: str = None,
+        request_enable: bool = None,
+        retention: int = None,
+    ):
+        self.enable = enable
+        self.filters = filters
+        self.hot_retention = hot_retention
+        self.instance_id = instance_id
+        self.request_enable = request_enable
+        self.retention = retention
+
+    def validate(self):
+        if self.filters:
+            for k in self.filters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable is not None:
+            result['Enable'] = self.enable
+        result['Filters'] = []
+        if self.filters is not None:
+            for k in self.filters:
+                result['Filters'].append(k.to_map() if k else None)
+        if self.hot_retention is not None:
+            result['HotRetention'] = self.hot_retention
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.request_enable is not None:
+            result['RequestEnable'] = self.request_enable
+        if self.retention is not None:
+            result['Retention'] = self.retention
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Enable') is not None:
+            self.enable = m.get('Enable')
+        self.filters = []
+        if m.get('Filters') is not None:
+            for k in m.get('Filters'):
+                temp_model = ModifySqlLogConfigRequestFilters()
+                self.filters.append(temp_model.from_map(k))
+        if m.get('HotRetention') is not None:
+            self.hot_retention = m.get('HotRetention')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RequestEnable') is not None:
+            self.request_enable = m.get('RequestEnable')
+        if m.get('Retention') is not None:
+            self.retention = m.get('Retention')
+        return self
+
+
+class ModifySqlLogConfigResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        cold_enable: bool = None,
+        cold_retention: int = None,
+        cold_start_time: int = None,
+        collector_version: str = None,
+        hot_enable: bool = None,
+        hot_retention: int = None,
+        hot_start_time: int = None,
+        log_filter: str = None,
+        request_enable: bool = None,
+        request_start_time: int = None,
+        request_stop_time: int = None,
+        retention: int = None,
+        sql_log_enable: bool = None,
+        sql_log_state: str = None,
+        sql_log_visible_time: int = None,
+        support_version: str = None,
+        version: str = None,
+    ):
+        self.cold_enable = cold_enable
+        self.cold_retention = cold_retention
+        self.cold_start_time = cold_start_time
+        self.collector_version = collector_version
+        self.hot_enable = hot_enable
+        self.hot_retention = hot_retention
+        self.hot_start_time = hot_start_time
+        self.log_filter = log_filter
+        self.request_enable = request_enable
+        self.request_start_time = request_start_time
+        self.request_stop_time = request_stop_time
+        self.retention = retention
+        self.sql_log_enable = sql_log_enable
+        self.sql_log_state = sql_log_state
+        self.sql_log_visible_time = sql_log_visible_time
+        self.support_version = support_version
+        self.version = version
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cold_enable is not None:
+            result['ColdEnable'] = self.cold_enable
+        if self.cold_retention is not None:
+            result['ColdRetention'] = self.cold_retention
+        if self.cold_start_time is not None:
+            result['ColdStartTime'] = self.cold_start_time
+        if self.collector_version is not None:
+            result['CollectorVersion'] = self.collector_version
+        if self.hot_enable is not None:
+            result['HotEnable'] = self.hot_enable
+        if self.hot_retention is not None:
+            result['HotRetention'] = self.hot_retention
+        if self.hot_start_time is not None:
+            result['HotStartTime'] = self.hot_start_time
+        if self.log_filter is not None:
+            result['LogFilter'] = self.log_filter
+        if self.request_enable is not None:
+            result['RequestEnable'] = self.request_enable
+        if self.request_start_time is not None:
+            result['RequestStartTime'] = self.request_start_time
+        if self.request_stop_time is not None:
+            result['RequestStopTime'] = self.request_stop_time
+        if self.retention is not None:
+            result['Retention'] = self.retention
+        if self.sql_log_enable is not None:
+            result['SqlLogEnable'] = self.sql_log_enable
+        if self.sql_log_state is not None:
+            result['SqlLogState'] = self.sql_log_state
+        if self.sql_log_visible_time is not None:
+            result['SqlLogVisibleTime'] = self.sql_log_visible_time
+        if self.support_version is not None:
+            result['SupportVersion'] = self.support_version
+        if self.version is not None:
+            result['Version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColdEnable') is not None:
+            self.cold_enable = m.get('ColdEnable')
+        if m.get('ColdRetention') is not None:
+            self.cold_retention = m.get('ColdRetention')
+        if m.get('ColdStartTime') is not None:
+            self.cold_start_time = m.get('ColdStartTime')
+        if m.get('CollectorVersion') is not None:
+            self.collector_version = m.get('CollectorVersion')
+        if m.get('HotEnable') is not None:
+            self.hot_enable = m.get('HotEnable')
+        if m.get('HotRetention') is not None:
+            self.hot_retention = m.get('HotRetention')
+        if m.get('HotStartTime') is not None:
+            self.hot_start_time = m.get('HotStartTime')
+        if m.get('LogFilter') is not None:
+            self.log_filter = m.get('LogFilter')
+        if m.get('RequestEnable') is not None:
+            self.request_enable = m.get('RequestEnable')
+        if m.get('RequestStartTime') is not None:
+            self.request_start_time = m.get('RequestStartTime')
+        if m.get('RequestStopTime') is not None:
+            self.request_stop_time = m.get('RequestStopTime')
+        if m.get('Retention') is not None:
+            self.retention = m.get('Retention')
+        if m.get('SqlLogEnable') is not None:
+            self.sql_log_enable = m.get('SqlLogEnable')
+        if m.get('SqlLogState') is not None:
+            self.sql_log_state = m.get('SqlLogState')
+        if m.get('SqlLogVisibleTime') is not None:
+            self.sql_log_visible_time = m.get('SqlLogVisibleTime')
+        if m.get('SupportVersion') is not None:
+            self.support_version = m.get('SupportVersion')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        return self
+
+
+class ModifySqlLogConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: ModifySqlLogConfigResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        # SqlLogConfig
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = ModifySqlLogConfigResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class ModifySqlLogConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifySqlLogConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifySqlLogConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RunCloudBenchTaskRequest(TeaModel):
     def __init__(
         self,
         task_id: str = None,
     ):
         # The stress testing task ID. You can call the [DescribeCloudBenchTasks](~~230670~~) operation to query the task ID.
         self.task_id = task_id
@@ -27504,15 +29932,15 @@
         # The language of event notifications. You can set the value to **zh-CN**, which indicates that event notifications are sent in Chinese.
         self.lang = lang
         # The risk level of the events. Valid values:
         # 
         # *   **Notice**: events that trigger notifications, including events at the **Notice**, **Optimization**, **Warn**, and **Critical** levels.
         # *   **Optimization**: events that trigger optimizations, including events at the **Optimization**, **Warn**, and **Critical** levels.
         # *   **Warn**: events that trigger warnings, including events at the **Warn** and **Critical** levels.
-        # *   **Critical**: events that trigger critical warnings.****\
+        # *   **Critical**: events that trigger critical warnings.
         # 
         # The following content describes the events at each level in detail:
         # 
         # *   Notice: events that are related to database exceptions for which no suggestions are generated.
         # *   Optimization: events for which optimization suggestions are generated based on the status of the database.
         # *   Warn: events that may affect the running of the database.
         # *   Critical: events that affect the running of the database.
```

### Comparing `alibabacloud_das20200116-2.3.2/alibabacloud_das20200116.egg-info/PKG-INFO` & `alibabacloud_das20200116-2.4.0/alibabacloud_das20200116.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-das20200116
-Version: 2.3.2
+Version: 2.4.0
 Summary: Alibaba Cloud DAS (20200116) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_das20200116-2.3.2/setup.py` & `alibabacloud_das20200116-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_das20200116.
 
-Created on 27/02/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_das20200116"
 NAME = "alibabacloud_das20200116" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud DAS (20200116) SDK Library for Python"
```


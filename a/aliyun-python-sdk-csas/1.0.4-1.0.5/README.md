# Comparing `tmp/aliyun-python-sdk-csas-1.0.4.tar.gz` & `tmp/aliyun-python-sdk-csas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-csas-1.0.4.tar", last modified: Mon Apr 15 03:00:13 2024, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-csas-1.0.5.tar", last modified: Thu Apr 25 05:38:26 2024, max compression
```

## Comparing `aliyun-python-sdk-csas-1.0.4.tar` & `aliyun-python-sdk-csas-1.0.5.tar`

### file list

```diff
@@ -1,73 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4069 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/
--rw-r--r--   0 root         (0) root         (0)     1457 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2641 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     4180 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1365 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     3367 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2094 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1222 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1239 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1175 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1215 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1233 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1193 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1191 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1181 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1191 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1293 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     2168 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2779 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3016 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1323 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1259 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPopTrafficStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1341 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2717 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3131 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1325 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2357 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1307 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2797 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1573 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1317 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1277 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     4910 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1289 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2204 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2403 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     3475 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1515 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2885 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     4394 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3545 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2326 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1431 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUsersStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2024-04-15 03:00:13.000000 aliyun-python-sdk-csas-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-15 03:00:12.000000 aliyun-python-sdk-csas-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4912 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateClientUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateIdpDepartmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteClientUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteIdpDepartmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetActiveIdpConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetClientUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetIdpConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1181 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListClientUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListIdpConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListIdpDepartmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPopTrafficStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateClientUserPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateClientUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateClientUserStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3475 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateIdpDepartmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUsersStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-25 05:38:26.000000 aliyun-python-sdk-csas-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-25 05:38:25.000000 aliyun-python-sdk-csas-1.0.5/setup.py
```

### Comparing `aliyun-python-sdk-csas-1.0.4/LICENSE` & `aliyun-python-sdk-csas-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/PKG-INFO` & `aliyun-python-sdk-csas-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-csas
-Version: 1.0.4
+Version: 1.0.5
 Summary: The csas module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-csas
```

### Comparing `aliyun-python-sdk-csas-1.0.4/README.rst` & `aliyun-python-sdk-csas-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/PKG-INFO` & `aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-csas
-Version: 1.0.4
+Version: 1.0.5
 Summary: The csas module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-csas
```

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyun_python_sdk_csas.egg-info/SOURCES.txt` & `aliyun-python-sdk-csas-1.0.5/aliyun_python_sdk_csas.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,39 +7,49 @@
 aliyun_python_sdk_csas.egg-info/SOURCES.txt
 aliyun_python_sdk_csas.egg-info/dependency_links.txt
 aliyun_python_sdk_csas.egg-info/requires.txt
 aliyun_python_sdk_csas.egg-info/top_level.txt
 aliyunsdkcsas/__init__.py
 aliyunsdkcsas/request/__init__.py
 aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py
+aliyunsdkcsas/request/v20230120/CreateClientUserRequest.py
 aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py
+aliyunsdkcsas/request/v20230120/CreateIdpDepartmentRequest.py
 aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py
 aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py
 aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py
+aliyunsdkcsas/request/v20230120/DeleteClientUserRequest.py
 aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py
+aliyunsdkcsas/request/v20230120/DeleteIdpDepartmentRequest.py
 aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py
 aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py
 aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py
 aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py
+aliyunsdkcsas/request/v20230120/GetActiveIdpConfigRequest.py
+aliyunsdkcsas/request/v20230120/GetClientUserRequest.py
 aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py
+aliyunsdkcsas/request/v20230120/GetIdpConfigRequest.py
 aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py
 aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py
 aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py
 aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py
+aliyunsdkcsas/request/v20230120/ListClientUsersRequest.py
 aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py
 aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py
 aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py
 aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py
+aliyunsdkcsas/request/v20230120/ListIdpConfigsRequest.py
+aliyunsdkcsas/request/v20230120/ListIdpDepartmentsRequest.py
 aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py
 aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py
 aliyunsdkcsas/request/v20230120/ListPopTrafficStatisticsRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py
 aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py
@@ -51,16 +61,20 @@
 aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py
 aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py
 aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py
 aliyunsdkcsas/request/v20230120/ListUsersRequest.py
+aliyunsdkcsas/request/v20230120/UpdateClientUserPasswordRequest.py
+aliyunsdkcsas/request/v20230120/UpdateClientUserRequest.py
+aliyunsdkcsas/request/v20230120/UpdateClientUserStatusRequest.py
 aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py
 aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py
+aliyunsdkcsas/request/v20230120/UpdateIdpDepartmentRequest.py
 aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py
 aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py
 aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py
 aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py
 aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py
 aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py
 aliyunsdkcsas/request/v20230120/UpdateUsersStatusRequest.py
```

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/AttachApplication2ConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreatePrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreatePrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreatePrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/CreateUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeletePrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeletePrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeletePrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteRegistrationPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DeleteUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/DetachApplication2ConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetPrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetUserDeviceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/GetUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListApplicationsForPrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListConnectorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListDynamicRouteRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListDynamicRoutesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListExcessiveDeviceRegistrationApplicationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPolicesForPrivateAccessTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPolicesForUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPopTrafficStatisticsRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPopTrafficStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsForDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessApplicationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessPolicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsForDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListPrivateAccessTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesForUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListRegistrationPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListSoftwareForUserDeviceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListTagsForPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserDevicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserGroupsForPrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserGroupsForRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUserGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/ListUsersRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/ListUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateDynamicRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateExcessiveDeviceRegistrationApplicationsStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdatePrivateAccessPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateRegistrationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUserDevicesSharingStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUserDevicesStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/aliyunsdkcsas/request/v20230120/UpdateUsersStatusRequest.py` & `aliyun-python-sdk-csas-1.0.5/aliyunsdkcsas/request/v20230120/UpdateUsersStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-csas-1.0.4/setup.py` & `aliyun-python-sdk-csas-1.0.5/setup.py`

 * *Files identical despite different names*


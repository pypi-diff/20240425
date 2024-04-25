# Comparing `tmp/alibabacloud_ecd20201002_py2-1.0.0.tar.gz` & `tmp/alibabacloud_ecd20201002_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ecd20201002_py2-1.0.0.tar", last modified: Thu Mar 21 17:13:44 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ecd20201002_py2-1.0.1.tar", last modified: Thu Apr 25 17:15:56 2024, max compression
```

## Comparing `alibabacloud_ecd20201002_py2-1.0.0.tar` & `alibabacloud_ecd20201002_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53448 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002/client.py
--rw-r--r--   0 root         (0) root         (0)   178596 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2024-03-21 17:13:44.000000 alibabacloud_ecd20201002_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53844 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002/client.py
+-rw-r--r--   0 root         (0) root         (0)   182082 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 17:15:56.000000 alibabacloud_ecd20201002_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-25 17:15:55.000000 alibabacloud_ecd20201002_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/LICENSE` & `alibabacloud_ecd20201002_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/PKG-INFO` & `alibabacloud_ecd20201002_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ecd20201002_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ecd (20201002) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/README-CN.md` & `alibabacloud_ecd20201002_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/README.md` & `alibabacloud_ecd20201002_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002/client.py` & `alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -658,14 +658,16 @@
             query['LoginToken'] = request.login_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.session_token):
             query['SessionToken'] = request.session_token
+        if not UtilClient.is_unset(request.uuid):
+            query['Uuid'] = request.uuid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RebootDesktops',
             version='2020-10-02',
             protocol='HTTPS',
@@ -999,15 +1001,15 @@
 
     def set_finger_print_template_description(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_finger_print_template_description_with_options(request, runtime)
 
     def start_desktops_with_options(self, request, runtime):
         """
-        The ID of the client.
+        The cloud computers that you want to start must be in the Stopped state. After you call this operation, the cloud computers enter the Running state.
         
 
         @param request: StartDesktopsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: StartDesktopsResponse
@@ -1026,14 +1028,16 @@
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.login_token):
             query['LoginToken'] = request.login_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
+        if not UtilClient.is_unset(request.uuid):
+            query['Uuid'] = request.uuid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartDesktops',
             version='2020-10-02',
             protocol='HTTPS',
@@ -1047,15 +1051,15 @@
         return TeaCore.from_map(
             ecd_20201002_models.StartDesktopsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def start_desktops(self, request):
         """
-        The ID of the client.
+        The cloud computers that you want to start must be in the Stopped state. After you call this operation, the cloud computers enter the Running state.
         
 
         @param request: StartDesktopsRequest
 
         @return: StartDesktopsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1101,15 +1105,15 @@
 
     def start_record_content(self, request):
         runtime = util_models.RuntimeOptions()
         return self.start_record_content_with_options(request, runtime)
 
     def stop_desktops_with_options(self, request, runtime):
         """
-        The cloud desktops that you want to stop by calling this operation must be in the Running state. If the call is successful, the cloud desktops enter the Stopped state.
+        The cloud computers that you want to stop must be in the Running state. After you call this operation, the cloud computers enter the Stopped state.
         
 
         @param request: StopDesktopsRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: StopDesktopsResponse
@@ -1151,15 +1155,15 @@
         return TeaCore.from_map(
             ecd_20201002_models.StopDesktopsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def stop_desktops(self, request):
         """
-        The cloud desktops that you want to stop by calling this operation must be in the Running state. If the call is successful, the cloud desktops enter the Stopped state.
+        The cloud computers that you want to stop must be in the Running state. After you call this operation, the cloud computers enter the Stopped state.
         
 
         @param request: StopDesktopsRequest
 
         @return: StopDesktopsResponse
         """
         runtime = util_models.RuntimeOptions()
```

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002/models.py` & `alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2450,18 +2450,57 @@
         if m.get('TokenCode') is not None:
             self.token_code = m.get('TokenCode')
         if m.get('Uuid') is not None:
             self.uuid = m.get('Uuid')
         return self
 
 
+class GetLoginTokenResponseBodyRiskVerifyInfo(TeaModel):
+    def __init__(self, email=None, last_lock_duration=None, locked=None, phone=None):
+        self.email = email  # type: str
+        self.last_lock_duration = last_lock_duration  # type: long
+        self.locked = locked  # type: str
+        self.phone = phone  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetLoginTokenResponseBodyRiskVerifyInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.last_lock_duration is not None:
+            result['LastLockDuration'] = self.last_lock_duration
+        if self.locked is not None:
+            result['Locked'] = self.locked
+        if self.phone is not None:
+            result['Phone'] = self.phone
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('LastLockDuration') is not None:
+            self.last_lock_duration = m.get('LastLockDuration')
+        if m.get('Locked') is not None:
+            self.locked = m.get('Locked')
+        if m.get('Phone') is not None:
+            self.phone = m.get('Phone')
+        return self
+
+
 class GetLoginTokenResponseBody(TeaModel):
     def __init__(self, email=None, end_user_id=None, industry=None, keep_alive_token=None, label=None,
-                 login_token=None, next_stage=None, phone=None, props=None, qr_code_png=None, request_id=None, secret=None,
-                 session_id=None, tenant_id=None, window_display_mode=None):
+                 login_token=None, next_stage=None, phone=None, props=None, qr_code_png=None, request_id=None,
+                 risk_verify_info=None, secret=None, session_id=None, tenant_id=None, window_display_mode=None):
         # The email address of the user. The system returns the email address in the return value of the LoginToken parameter after the user logs on to the client.
         # 
         # *   For a convenience user, the return value is the email address specified when the administrator creates the convenience user.
         # *   For an AD user, the return value is in the following format: `Username@Name of the AD domain`.
         self.email = email  # type: str
         # The account of the convenience user or the AD user.
         self.end_user_id = end_user_id  # type: str
@@ -2483,29 +2522,31 @@
         self.props = props  # type: dict[str, str]
         # The QR code that is generated when the virtual MFA device is bound. The value is encoded in Base64. This parameter can be empty. This parameter is required only when the CurrentStage parameter is set to `MFABind`.
         # 
         # > For more information about each authentication stage, see the parameter description of the request parameter `CurrentStage`.
         self.qr_code_png = qr_code_png  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
+        self.risk_verify_info = risk_verify_info  # type: GetLoginTokenResponseBodyRiskVerifyInfo
         # The key that is generated when you bind the virtual MFA device. This parameter is required when the CurrentStage parameter is set to `MFABind`.
         # 
         # > For more information about each authentication stage, see the parameter description of the request parameter `CurrentStage`.
         self.secret = secret  # type: str
         # The ID of the session. The ID is returned the first time you call the `GetLoginToken` operation in the session. If MFA is required, you must specify this parameter in subsequent stages.
         # 
         # > For more information about each authentication stage, see the parameter description of the request parameter `CurrentStage`.
         self.session_id = session_id  # type: str
         # The ID of the Alibaba Cloud account. The ID is used for hardware client authentication.
         self.tenant_id = tenant_id  # type: long
         # > This is a parameter only for internal use.
         self.window_display_mode = window_display_mode  # type: str
 
     def validate(self):
-        pass
+        if self.risk_verify_info:
+            self.risk_verify_info.validate()
 
     def to_map(self):
         _map = super(GetLoginTokenResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2527,14 +2568,16 @@
             result['Phone'] = self.phone
         if self.props is not None:
             result['Props'] = self.props
         if self.qr_code_png is not None:
             result['QrCodePng'] = self.qr_code_png
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.risk_verify_info is not None:
+            result['RiskVerifyInfo'] = self.risk_verify_info.to_map()
         if self.secret is not None:
             result['Secret'] = self.secret
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.window_display_mode is not None:
@@ -2561,14 +2604,17 @@
             self.phone = m.get('Phone')
         if m.get('Props') is not None:
             self.props = m.get('Props')
         if m.get('QrCodePng') is not None:
             self.qr_code_png = m.get('QrCodePng')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('RiskVerifyInfo') is not None:
+            temp_model = GetLoginTokenResponseBodyRiskVerifyInfo()
+            self.risk_verify_info = temp_model.from_map(m['RiskVerifyInfo'])
         if m.get('Secret') is not None:
             self.secret = m.get('Secret')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('WindowDisplayMode') is not None:
@@ -2844,33 +2890,34 @@
             temp_model = QueryEdsAgentReportConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RebootDesktopsRequest(TeaModel):
     def __init__(self, client_id=None, client_os=None, client_token=None, client_version=None, desktop_id=None,
-                 login_token=None, region_id=None, session_id=None, session_token=None):
+                 login_token=None, region_id=None, session_id=None, session_token=None, uuid=None):
         # The client ID. The system generates a unique ID for each client.
         self.client_id = client_id  # type: str
-        # The client OS.
+        # The operating system (OS) of the device that runs the Alibaba Cloud Workspace client (hereinafter referred to as WUYING client).
         self.client_os = client_os  # type: str
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [How do I ensure the idempotence of a request?](~~25693~~)
         self.client_token = client_token  # type: str
-        # The client version.
+        # The client version. If you use a WUYING client, you can view the client version in the **About** dialog box on the client logon page.
         self.client_version = client_version  # type: str
-        # The cloud desktop IDs. You can specify 1 to 20 IDs.
+        # The IDs of the cloud computers. You can specify the IDs of 1 to 20 cloud computers.
         self.desktop_id = desktop_id  # type: list[str]
         # The logon token.
         self.login_token = login_token  # type: str
-        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the most recent region list.
+        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the regions supported by WUYING Workspace.
         self.region_id = region_id  # type: str
         # The session ID.
         self.session_id = session_id  # type: str
         # The logon token.
         self.session_token = session_token  # type: str
+        self.uuid = uuid  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RebootDesktopsRequest, self).to_map()
         if _map is not None:
@@ -2891,14 +2938,16 @@
             result['LoginToken'] = self.login_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.session_token is not None:
             result['SessionToken'] = self.session_token
+        if self.uuid is not None:
+            result['Uuid'] = self.uuid
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClientId') is not None:
             self.client_id = m.get('ClientId')
         if m.get('ClientOS') is not None:
@@ -2913,14 +2962,16 @@
             self.login_token = m.get('LoginToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('SessionToken') is not None:
             self.session_token = m.get('SessionToken')
+        if m.get('Uuid') is not None:
+            self.uuid = m.get('Uuid')
         return self
 
 
 class RebootDesktopsResponseBody(TeaModel):
     def __init__(self, request_id=None):
         # The request ID.
         self.request_id = request_id  # type: str
@@ -3902,29 +3953,32 @@
             temp_model = SetFingerPrintTemplateDescriptionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StartDesktopsRequest(TeaModel):
     def __init__(self, client_id=None, client_os=None, client_token=None, client_version=None, desktop_id=None,
-                 login_token=None, region_id=None, session_id=None):
-        # The ID of the request.
+                 login_token=None, region_id=None, session_id=None, uuid=None):
+        # The ID of the Alibaba Cloud Workspace client (hereinafter referred to as WUYING client). The system generates a unique ID for each client.
         self.client_id = client_id  # type: str
-        # The OS used by the client.
+        # The operating system (OS) of the device that run the client.
         self.client_os = client_os  # type: str
+        # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [How to ensure idempotence](~~25693~~).
         self.client_token = client_token  # type: str
-        # StartDesktops
+        # The client version. If you use a WUYING client, you can click **About** on the client logon page to view the version of the client.
         self.client_version = client_version  # type: str
+        # The IDs of the cloud computers. You can specify the IDs of 1 to 20 cloud computers.
         self.desktop_id = desktop_id  # type: list[str]
-        # The ID of cloud desktop N. You can specify one or more IDs of cloud desktops. Valid values of N: 1 to 20.
+        # The logon token.
         self.login_token = login_token  # type: str
-        # The logon credential.
+        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the regions supported by WUYING Workspace.
         self.region_id = region_id  # type: str
-        # The operation that you want to perform. Set the value to StartDesktops.
+        # The session ID.
         self.session_id = session_id  # type: str
+        self.uuid = uuid  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartDesktopsRequest, self).to_map()
         if _map is not None:
@@ -3943,14 +3997,16 @@
             result['DesktopId'] = self.desktop_id
         if self.login_token is not None:
             result['LoginToken'] = self.login_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.session_id is not None:
             result['SessionId'] = self.session_id
+        if self.uuid is not None:
+            result['Uuid'] = self.uuid
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClientId') is not None:
             self.client_id = m.get('ClientId')
         if m.get('ClientOS') is not None:
@@ -3963,19 +4019,22 @@
             self.desktop_id = m.get('DesktopId')
         if m.get('LoginToken') is not None:
             self.login_token = m.get('LoginToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
+        if m.get('Uuid') is not None:
+            self.uuid = m.get('Uuid')
         return self
 
 
 class StartDesktopsResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartDesktopsResponseBody, self).to_map()
@@ -4151,25 +4210,25 @@
 
 
 class StopDesktopsRequest(TeaModel):
     def __init__(self, client_id=None, client_os=None, client_token=None, client_version=None, desktop_id=None,
                  login_token=None, region_id=None, session_id=None, session_token=None):
         # The client ID. The system generates a unique ID for each client.
         self.client_id = client_id  # type: str
-        # The client OS.
+        # The operating system (OS) of the device that runs the Alibaba Cloud Workspace client (hereinafter referred to as WUYING client).
         self.client_os = client_os  # type: str
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [How do I ensure the idempotence of a request?](~~25693~~)
         self.client_token = client_token  # type: str
-        # The client version.
+        # The client version. If you use a WUYING client, you can view the client version in the **About** dialog box on the client logon page.
         self.client_version = client_version  # type: str
-        # The cloud desktop IDs. You can specify 1 to 20 IDs.
+        # The IDs of the cloud computers. You can specify the IDs of 1 to 20 cloud computers.
         self.desktop_id = desktop_id  # type: list[str]
         # The logon token.
         self.login_token = login_token  # type: str
-        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the most recent region list.
+        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the regions supported by WUYING Workspace.
         self.region_id = region_id  # type: str
         # The session ID.
         self.session_id = session_id  # type: str
         # The logon token.
         self.session_token = session_token  # type: str
 
     def validate(self):
```

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/alibabacloud_ecd20201002_py2.egg-info/PKG-INFO` & `alibabacloud_ecd20201002_py2-1.0.1/alibabacloud_ecd20201002_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ecd20201002-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud ecd (20201002) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20201002_py2-1.0.0/setup.py` & `alibabacloud_ecd20201002_py2-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ecd20201002_py2.
 
-Created on 21/03/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ecd20201002"
 NAME = "alibabacloud_ecd20201002_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ecd (20201002) SDK Library for Python2"
```


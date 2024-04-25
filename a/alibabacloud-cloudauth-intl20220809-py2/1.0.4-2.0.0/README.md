# Comparing `tmp/alibabacloud_cloudauth-intl20220809_py2-1.0.4.tar.gz` & `tmp/alibabacloud_cloudauth-intl20220809_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809_py2-1.0.4.tar", last modified: Sun Feb  4 02:16:01 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809_py2-2.0.0.tar", last modified: Thu Apr 25 07:56:42 2024, max compression
```

## Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4.tar` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      312 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2538 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1066 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1149 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34108 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809/client.py
--rw-r--r--   0 root         (0) root         (0)   150339 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2538 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2960 2024-02-04 02:16:01.000000 alibabacloud_cloudauth-intl20220809_py2-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32539 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809/client.py
+-rw-r--r--   0 root         (0) root         (0)   144715 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 07:56:42.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-25 07:56:41.000000 alibabacloud_cloudauth-intl20220809_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/LICENSE` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/PKG-INFO` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth-intl20220809_py2
-Version: 1.0.4
+Version: 2.0.0
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/README-CN.md` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/README.md` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809/client.py` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,44 +128,14 @@
             self.call_api(params, req, runtime)
         )
 
     def check_result(self, request):
         runtime = util_models.RuntimeOptions()
         return self.check_result_with_options(request, runtime)
 
-    def delete_picture_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.delete_pic_after_query):
-            query['DeletePicAfterQuery'] = request.delete_pic_after_query
-        if not UtilClient.is_unset(request.transaction_id):
-            query['TransactionId'] = request.transaction_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeletePicture',
-            version='2022-08-09',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            cloudauth_intl_20220809_models.DeletePictureResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def delete_picture(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.delete_picture_with_options(request, runtime)
-
     def delete_verify_result_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.delete_after_query):
             query['DeleteAfterQuery'] = request.delete_after_query
         if not UtilClient.is_unset(request.delete_type):
             query['DeleteType'] = request.delete_type
@@ -725,48 +695,40 @@
             query['Crop'] = request.crop
         if not UtilClient.is_unset(request.doc_scan_mode):
             query['DocScanMode'] = request.doc_scan_mode
         if not UtilClient.is_unset(request.doc_type):
             query['DocType'] = request.doc_type
         if not UtilClient.is_unset(request.face_picture_url):
             query['FacePictureUrl'] = request.face_picture_url
-        if not UtilClient.is_unset(request.flow_type):
-            query['FlowType'] = request.flow_type
         if not UtilClient.is_unset(request.id_face_quality):
             query['IdFaceQuality'] = request.id_face_quality
         if not UtilClient.is_unset(request.id_spoof):
             query['IdSpoof'] = request.id_spoof
         if not UtilClient.is_unset(request.language_config):
             query['LanguageConfig'] = request.language_config
         if not UtilClient.is_unset(request.merchant_biz_id):
             query['MerchantBizId'] = request.merchant_biz_id
         if not UtilClient.is_unset(request.merchant_user_id):
             query['MerchantUserId'] = request.merchant_user_id
         if not UtilClient.is_unset(request.meta_info):
             query['MetaInfo'] = request.meta_info
         if not UtilClient.is_unset(request.ocr):
             query['Ocr'] = request.ocr
-        if not UtilClient.is_unset(request.operation_mode):
-            query['OperationMode'] = request.operation_mode
-        if not UtilClient.is_unset(request.pages):
-            query['Pages'] = request.pages
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
-        if not UtilClient.is_unset(request.product_config):
-            query['ProductConfig'] = request.product_config
         if not UtilClient.is_unset(request.product_flow):
             query['ProductFlow'] = request.product_flow
         if not UtilClient.is_unset(request.return_url):
             query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_code):
             query['SceneCode'] = request.scene_code
         if not UtilClient.is_unset(request.security_level):
             query['SecurityLevel'] = request.security_level
-        if not UtilClient.is_unset(request.service_level):
-            query['ServiceLevel'] = request.service_level
+        if not UtilClient.is_unset(request.style_config):
+            query['StyleConfig'] = request.style_config
         body = {}
         if not UtilClient.is_unset(request.face_picture_base_64):
             body['FacePictureBase64'] = request.face_picture_base_64
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
```

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809/models.py` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,150 +364,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CheckResultResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DeletePictureRequest(TeaModel):
-    def __init__(self, delete_pic_after_query=None, transaction_id=None):
-        self.delete_pic_after_query = delete_pic_after_query  # type: str
-        self.transaction_id = transaction_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DeletePictureRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.delete_pic_after_query is not None:
-            result['DeletePicAfterQuery'] = self.delete_pic_after_query
-        if self.transaction_id is not None:
-            result['TransactionId'] = self.transaction_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DeletePicAfterQuery') is not None:
-            self.delete_pic_after_query = m.get('DeletePicAfterQuery')
-        if m.get('TransactionId') is not None:
-            self.transaction_id = m.get('TransactionId')
-        return self
-
-
-class DeletePictureResponseBodyResult(TeaModel):
-    def __init__(self, delete_result=None, transaction_id=None):
-        self.delete_result = delete_result  # type: str
-        self.transaction_id = transaction_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DeletePictureResponseBodyResult, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.delete_result is not None:
-            result['DeleteResult'] = self.delete_result
-        if self.transaction_id is not None:
-            result['TransactionId'] = self.transaction_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DeleteResult') is not None:
-            self.delete_result = m.get('DeleteResult')
-        if m.get('TransactionId') is not None:
-            self.transaction_id = m.get('TransactionId')
-        return self
-
-
-class DeletePictureResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, result=None):
-        self.code = code  # type: str
-        self.message = message  # type: str
-        # Id of the request
-        self.request_id = request_id  # type: str
-        self.result = result  # type: DeletePictureResponseBodyResult
-
-    def validate(self):
-        if self.result:
-            self.result.validate()
-
-    def to_map(self):
-        _map = super(DeletePictureResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.result is not None:
-            result['Result'] = self.result.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Result') is not None:
-            temp_model = DeletePictureResponseBodyResult()
-            self.result = temp_model.from_map(m['Result'])
-        return self
-
-
-class DeletePictureResponse(TeaModel):
-    def __init__(self, headers=None, status_code=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.status_code = status_code  # type: int
-        self.body = body  # type: DeletePictureResponseBody
-
-    def validate(self):
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DeletePictureResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = DeletePictureResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DeleteVerifyResultRequest(TeaModel):
     def __init__(self, delete_after_query=None, delete_type=None, transaction_id=None):
         self.delete_after_query = delete_after_query  # type: str
         self.delete_type = delete_type  # type: str
         self.transaction_id = transaction_id  # type: str
 
     def validate(self):
@@ -3586,44 +3450,39 @@
             temp_model = Id2MetaVerifyIntlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class InitializeRequest(TeaModel):
     def __init__(self, authorize=None, callback_token=None, callback_url=None, crop=None, doc_scan_mode=None,
-                 doc_type=None, face_picture_base_64=None, face_picture_url=None, flow_type=None, id_face_quality=None,
-                 id_spoof=None, language_config=None, merchant_biz_id=None, merchant_user_id=None, meta_info=None, ocr=None,
-                 operation_mode=None, pages=None, product_code=None, product_config=None, product_flow=None, return_url=None,
-                 scene_code=None, security_level=None, service_level=None):
+                 doc_type=None, face_picture_base_64=None, face_picture_url=None, id_face_quality=None, id_spoof=None,
+                 language_config=None, merchant_biz_id=None, merchant_user_id=None, meta_info=None, ocr=None, product_code=None,
+                 product_flow=None, return_url=None, scene_code=None, security_level=None, style_config=None):
         self.authorize = authorize  # type: str
         self.callback_token = callback_token  # type: str
         self.callback_url = callback_url  # type: str
         self.crop = crop  # type: str
         self.doc_scan_mode = doc_scan_mode  # type: str
         self.doc_type = doc_type  # type: str
         self.face_picture_base_64 = face_picture_base_64  # type: str
         self.face_picture_url = face_picture_url  # type: str
-        self.flow_type = flow_type  # type: str
         self.id_face_quality = id_face_quality  # type: str
         self.id_spoof = id_spoof  # type: str
         self.language_config = language_config  # type: str
         self.merchant_biz_id = merchant_biz_id  # type: str
         self.merchant_user_id = merchant_user_id  # type: str
         self.meta_info = meta_info  # type: str
         # OCR。
         self.ocr = ocr  # type: str
-        self.operation_mode = operation_mode  # type: str
-        self.pages = pages  # type: str
         self.product_code = product_code  # type: str
-        self.product_config = product_config  # type: str
         self.product_flow = product_flow  # type: str
         self.return_url = return_url  # type: str
         self.scene_code = scene_code  # type: str
         self.security_level = security_level  # type: str
-        self.service_level = service_level  # type: str
+        self.style_config = style_config  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(InitializeRequest, self).to_map()
         if _map is not None:
@@ -3642,48 +3501,40 @@
             result['DocScanMode'] = self.doc_scan_mode
         if self.doc_type is not None:
             result['DocType'] = self.doc_type
         if self.face_picture_base_64 is not None:
             result['FacePictureBase64'] = self.face_picture_base_64
         if self.face_picture_url is not None:
             result['FacePictureUrl'] = self.face_picture_url
-        if self.flow_type is not None:
-            result['FlowType'] = self.flow_type
         if self.id_face_quality is not None:
             result['IdFaceQuality'] = self.id_face_quality
         if self.id_spoof is not None:
             result['IdSpoof'] = self.id_spoof
         if self.language_config is not None:
             result['LanguageConfig'] = self.language_config
         if self.merchant_biz_id is not None:
             result['MerchantBizId'] = self.merchant_biz_id
         if self.merchant_user_id is not None:
             result['MerchantUserId'] = self.merchant_user_id
         if self.meta_info is not None:
             result['MetaInfo'] = self.meta_info
         if self.ocr is not None:
             result['Ocr'] = self.ocr
-        if self.operation_mode is not None:
-            result['OperationMode'] = self.operation_mode
-        if self.pages is not None:
-            result['Pages'] = self.pages
         if self.product_code is not None:
             result['ProductCode'] = self.product_code
-        if self.product_config is not None:
-            result['ProductConfig'] = self.product_config
         if self.product_flow is not None:
             result['ProductFlow'] = self.product_flow
         if self.return_url is not None:
             result['ReturnUrl'] = self.return_url
         if self.scene_code is not None:
             result['SceneCode'] = self.scene_code
         if self.security_level is not None:
             result['SecurityLevel'] = self.security_level
-        if self.service_level is not None:
-            result['ServiceLevel'] = self.service_level
+        if self.style_config is not None:
+            result['StyleConfig'] = self.style_config
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Authorize') is not None:
             self.authorize = m.get('Authorize')
         if m.get('CallbackToken') is not None:
@@ -3696,48 +3547,40 @@
             self.doc_scan_mode = m.get('DocScanMode')
         if m.get('DocType') is not None:
             self.doc_type = m.get('DocType')
         if m.get('FacePictureBase64') is not None:
             self.face_picture_base_64 = m.get('FacePictureBase64')
         if m.get('FacePictureUrl') is not None:
             self.face_picture_url = m.get('FacePictureUrl')
-        if m.get('FlowType') is not None:
-            self.flow_type = m.get('FlowType')
         if m.get('IdFaceQuality') is not None:
             self.id_face_quality = m.get('IdFaceQuality')
         if m.get('IdSpoof') is not None:
             self.id_spoof = m.get('IdSpoof')
         if m.get('LanguageConfig') is not None:
             self.language_config = m.get('LanguageConfig')
         if m.get('MerchantBizId') is not None:
             self.merchant_biz_id = m.get('MerchantBizId')
         if m.get('MerchantUserId') is not None:
             self.merchant_user_id = m.get('MerchantUserId')
         if m.get('MetaInfo') is not None:
             self.meta_info = m.get('MetaInfo')
         if m.get('Ocr') is not None:
             self.ocr = m.get('Ocr')
-        if m.get('OperationMode') is not None:
-            self.operation_mode = m.get('OperationMode')
-        if m.get('Pages') is not None:
-            self.pages = m.get('Pages')
         if m.get('ProductCode') is not None:
             self.product_code = m.get('ProductCode')
-        if m.get('ProductConfig') is not None:
-            self.product_config = m.get('ProductConfig')
         if m.get('ProductFlow') is not None:
             self.product_flow = m.get('ProductFlow')
         if m.get('ReturnUrl') is not None:
             self.return_url = m.get('ReturnUrl')
         if m.get('SceneCode') is not None:
             self.scene_code = m.get('SceneCode')
         if m.get('SecurityLevel') is not None:
             self.security_level = m.get('SecurityLevel')
-        if m.get('ServiceLevel') is not None:
-            self.service_level = m.get('ServiceLevel')
+        if m.get('StyleConfig') is not None:
+            self.style_config = m.get('StyleConfig')
         return self
 
 
 class InitializeResponseBodyResult(TeaModel):
     def __init__(self, client_cfg=None, transaction_id=None, transaction_url=None):
         self.client_cfg = client_cfg  # type: str
         self.transaction_id = transaction_id  # type: str
```

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/PKG-INFO` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth-intl20220809-py2
-Version: 1.0.4
+Version: 2.0.0
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/alibabacloud_cloudauth_intl20220809_py2.egg-info/SOURCES.txt` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/alibabacloud_cloudauth_intl20220809_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809_py2-1.0.4/setup.py` & `alibabacloud_cloudauth-intl20220809_py2-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth-intl20220809_py2.
 
-Created on 02/02/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth_intl20220809"
 NAME = "alibabacloud_cloudauth-intl20220809_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python2"
```


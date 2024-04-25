# Comparing `tmp/mobio-admin-sdk-1.0.8.tar.gz` & `tmp/mobio-admin-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-admin-sdk-1.0.8.tar", last modified: Mon Mar 13 08:16:20 2023, max compression
+gzip compressed data, was "mobio-admin-sdk-1.0.9.tar", last modified: Mon Sep 25 08:18:05 2023, max compression
```

## Comparing `mobio-admin-sdk-1.0.8.tar` & `mobio-admin-sdk-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 08:16:20.790526 mobio-admin-sdk-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     7860 2023-03-13 08:16:20.789526 mobio-admin-sdk-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5968 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 08:16:20.775525 mobio-admin-sdk-1.0.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 08:16:20.775525 mobio-admin-sdk-1.0.8/mobio/sdks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 08:16:20.785525 mobio-admin-sdk-1.0.8/mobio/sdks/admin/
--rw-r--r--   0 root         (0) root         (0)      397 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5755 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/aes_cipher.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/config.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/date_utils.py
--rw-r--r--   0 root         (0) root         (0)     6448 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/http_jwt_auth.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/mobio_admin_sdk.py
--rw-r--r--   0 root         (0) root         (0)     8320 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/mobio_authorization.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/mongo_base_model.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/mysql_base_model.py
--rw-r--r--   0 root         (0) root         (0)    32268 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/mobio/sdks/admin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 08:16:20.788525 mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7860 2023-03-13 08:16:20.000000 mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      555 2023-03-13 08:16:20.000000 mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 08:16:20.000000 mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-03-13 08:16:20.000000 mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-13 08:16:20.000000 mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-03-13 08:14:19.000000 mobio-admin-sdk-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-13 08:16:20.790526 mobio-admin-sdk-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9787 2023-03-13 08:16:20.000000 mobio-admin-sdk-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 08:18:05.706060 mobio-admin-sdk-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-09-25 08:18:05.705060 mobio-admin-sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 08:18:05.690060 mobio-admin-sdk-1.0.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 08:18:05.691060 mobio-admin-sdk-1.0.9/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 08:18:05.701060 mobio-admin-sdk-1.0.9/mobio/sdks/admin/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/aes_cipher.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/config.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/date_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6448 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/http_jwt_auth.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/mobio_admin_sdk.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/mobio_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/mongo_base_model.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/mysql_base_model.py
+-rw-r--r--   0 root         (0) root         (0)    32250 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/mobio/sdks/admin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 08:18:05.704060 mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-09-25 08:18:05.000000 mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      555 2023-09-25 08:18:05.000000 mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-25 08:18:05.000000 mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-09-25 08:18:05.000000 mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-09-25 08:18:05.000000 mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-09-25 08:16:03.000000 mobio-admin-sdk-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-25 08:18:05.707060 mobio-admin-sdk-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9788 2023-09-25 08:18:05.000000 mobio-admin-sdk-1.0.9/setup.py
```

### Comparing `mobio-admin-sdk-1.0.8/PKG-INFO` & `mobio-admin-sdk-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,153 +1,155 @@
 Metadata-Version: 2.1
 Name: mobio-admin-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio admin SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ##  Thư viện Admin SDK dành cho các module.
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install mobio-admin-sdk
-         ```
-        
-        ### Chức năng:
-        * Verify token 
-        
-        
-        ### Sử dụng:
-        
-        ##### 1. Verify token:
-           ```python
-            from mobio.sdks.admin import MobioAdminSDK
-        
-            MobioAdminSDK().config(
-                admin_host="",	# admin host
-                redis_uri="",	# redis uri
-                module_use="",	# liên hệ admin để khai báo tên của module
-                module_encrypt="",	# liên hệ admin để lấy mã
-                api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
-            )
-            auth = MobioAdminSDK().create_mobio_verify_token()
-            
-            @service_mod.route(url_path, methods=["get"])
-            @auth.verify_token
-            @try_catch_error
-            def get_config(merchant_id):
-                return build_response_message(Config(merchant_id).get_data())
-           ```
-        
-        ##### 2. Merchant config:
-           ```python
-            from mobio.sdks.admin import MobioAdminSDK
-        
-            MobioAdminSDK().request_get_merchant_config_host(
-                    merchant_id,
-                    key=None,       # key muốn lấy giá trị
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                )
-            MobioAdminSDK().request_get_merchant_config_other(
-                    merchant_id,
-                    list_key=None,       # danh sách key muốn lấy giá trị
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                )
-            MobioAdminSDK().request_check_merchant_is_brand(
-                    merchant_id,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
-                                        # không cần truyền, token_value sẽ lấy từ header của request 
-                )
-            MobioAdminSDK().request_get_info_staff(
-                    merchant_id,
-                    account_id,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_info_staff(
-                    merchant_id,
-                    params=None, # tham số của api  VD: {"per_page": -1}
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_parent_merchant(
-                    merchant_id,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_profile_group(
-                    merchant_id=None,
-                    params=None,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_sub_brand(
-                    params=None,        # tham số của api  VD: {"merchant_id": ""}
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_info_sub_brand(
-                    subbrand_id=None,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_partner_info(
-                    partner_key=None,
-                    decrypt_data=False,
-            )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
-                
-        
-        
-        
-        ```
-        ##### 3. Save log action account:
-           ```python
-            from mobio.sdks.admin import MobioAdminSDK
-            action_account = {
-                    'account_id': "uuid",# required
-                    'action_name_vi': 'action name',# required
-                    'action_name_en': 'action name',# required
-                    'merchant_id': "uuid",# required
-                    'created_time': 0129301293  # required (timestamp(utcnow))
-                }
-            MobioAdminSDK().admin_save_log_action_account(action_account)
-           ```
-        #### Log - 1.0.1
-            - release sdk
-        #### Log - 1.0.2
-            - Kiểm tra license server còn hạn sử dụng hay không 
-        #### Log - 1.0.3
-            - Fix lỗi đọc file license 
-        #### Log - 1.0.4
-            - Authen app key data out 
-        #### Log - 1.0.5
-            - update lib kafka v2
-        #### Log - 1.0.6
-            - encrypt, decrypt field by config
-        #### Log - 1.0.7
-            -  kiểm tra thông tin field trước khi encrypt, decrypt 
-        #### Log - 1.0.8
-            -  sdk tự lấy thông tin REDIS_URI  
 Keywords: mobio,admin sdk,verify token
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+##  Thư viện Admin SDK dành cho các module.
+
+
+### Cài đặt:
+```bash
+ $ pip3 install mobio-admin-sdk
+ ```
+
+### Chức năng:
+* Verify token 
+
+
+### Sử dụng:
+
+##### 1. Verify token:
+   ```python
+    from mobio.sdks.admin import MobioAdminSDK
+
+    MobioAdminSDK().config(
+        admin_host="",	# admin host
+        redis_uri="",	# redis uri
+        module_use="",	# liên hệ admin để khai báo tên của module
+        module_encrypt="",	# liên hệ admin để lấy mã
+        api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
+    )
+    auth = MobioAdminSDK().create_mobio_verify_token()
+    
+    @service_mod.route(url_path, methods=["get"])
+    @auth.verify_token
+    @try_catch_error
+    def get_config(merchant_id):
+        return build_response_message(Config(merchant_id).get_data())
+   ```
+
+##### 2. Merchant config:
+   ```python
+    from mobio.sdks.admin import MobioAdminSDK
+
+    MobioAdminSDK().request_get_merchant_config_host(
+            merchant_id,
+            key=None,       # key muốn lấy giá trị
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+        )
+    MobioAdminSDK().request_get_merchant_config_other(
+            merchant_id,
+            list_key=None,       # danh sách key muốn lấy giá trị
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+        )
+    MobioAdminSDK().request_check_merchant_is_brand(
+            merchant_id,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
+                                # không cần truyền, token_value sẽ lấy từ header của request 
+        )
+    MobioAdminSDK().request_get_info_staff(
+            merchant_id,
+            account_id,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_info_staff(
+            merchant_id,
+            params=None, # tham số của api  VD: {"per_page": -1}
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_parent_merchant(
+            merchant_id,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_profile_group(
+            merchant_id=None,
+            params=None,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_sub_brand(
+            params=None,        # tham số của api  VD: {"merchant_id": ""}
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_info_sub_brand(
+            subbrand_id=None,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_partner_info(
+            partner_key=None,
+            decrypt_data=False,
+    )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
+        
+
+
+
+```
+##### 3. Save log action account:
+   ```python
+    from mobio.sdks.admin import MobioAdminSDK
+    action_account = {
+            'account_id': "uuid",# required
+            'action_name_vi': 'action name',# required
+            'action_name_en': 'action name',# required
+            'merchant_id': "uuid",# required
+            'created_time': 0129301293  # required (timestamp(utcnow))
+        }
+    MobioAdminSDK().admin_save_log_action_account(action_account)
+   ```
+#### Log - 1.0.1
+    - release sdk
+#### Log - 1.0.2
+    - Kiểm tra license server còn hạn sử dụng hay không 
+#### Log - 1.0.3
+    - Fix lỗi đọc file license 
+#### Log - 1.0.4
+    - Authen app key data out 
+#### Log - 1.0.5
+    - update lib kafka v2
+#### Log - 1.0.6
+    - encrypt, decrypt field by config
+#### Log - 1.0.7
+    -  kiểm tra thông tin field trước khi encrypt, decrypt 
+#### Log - 1.0.8
+    -  sdk tự lấy thông tin REDIS_URI  
+#### Log - 1.0.9
+    -  bỏ encoding trong json.loads
```

### Comparing `mobio-admin-sdk-1.0.8/README.md` & `mobio-admin-sdk-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,8 +123,10 @@
 #### Log - 1.0.5
     - update lib kafka v2
 #### Log - 1.0.6
     - encrypt, decrypt field by config
 #### Log - 1.0.7
     -  kiểm tra thông tin field trước khi encrypt, decrypt 
 #### Log - 1.0.8
-    -  sdk tự lấy thông tin REDIS_URI  
+    -  sdk tự lấy thông tin REDIS_URI  
+#### Log - 1.0.9
+    -  bỏ encoding trong json.loads
```

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/aes_cipher.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/aes_cipher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import base64
 import hashlib
 from Crypto.Cipher import AES
 
 try:
     import secrets
+
     HAVE_SECRETS = True
 except ImportError:
     from Crypto import Random
+
     HAVE_SECRETS = False
 
 
 class AESCipher(object):
     def __init__(self, key="677d3cfc-dd28-4a4e-94d5-7c3b99a24a2a"):
         self.bs = 32
         self.key = hashlib.sha256(key.encode()).digest()
@@ -24,22 +26,23 @@
         cipher = AES.new(self.key, AES.MODE_CBC, iv)
         return base64.urlsafe_b64encode(iv + cipher.encrypt(raw))
 
     def decrypt(self, enc):
         enc = base64.urlsafe_b64decode(enc)
         iv = enc[: AES.block_size]
         cipher = AES.new(self.key, AES.MODE_CBC, iv)
-        return self._unpad(cipher.decrypt(enc[AES.block_size :])).decode("utf-8")
+        return self._unpad(cipher.decrypt(enc[AES.block_size:])).decode("utf-8")
 
     def _pad(self, s):
         return s + (self.bs - len(s) % self.bs) * chr(self.bs - len(s) % self.bs)
 
     @staticmethod
     def _unpad(s):
-        return s[: -ord(s[len(s) - 1 :])]
+        return s[: -ord(s[len(s) - 1:])]
+
 
 from mobio.libs.caching import LRUCacheDict
 from mobio.libs.ciphers import MobioCrypt2
 from mobio.libs.Singleton import Singleton
 from .config import SystemConfigKeys, LicenseFormat, PathDir
 import os
 import time
@@ -102,30 +105,31 @@
             if not license_encrypt:
                 print("admin_sdk::license_encrypt no cache")
                 print("admin_sdk::license_encrypt path file license: {}".format(PathDir.PATH_FILE_LICENSE_SERVER))
                 license_encrypt = CryptUtil.get_content_from_file(PathDir.PATH_FILE_LICENSE_SERVER)
                 if license_encrypt:
                     CryptUtil().license_server.set_item(key_cache, license_encrypt)
                 else:
-                    print("admin_sdk::license_encrypt path file license: {}".format(PathDir.PATH_FILE_LICENSE_SERVER_OLD))
+                    print(
+                        "admin_sdk::license_encrypt path file license: {}".format(PathDir.PATH_FILE_LICENSE_SERVER_OLD))
                     license_encrypt = CryptUtil.get_content_from_file(PathDir.PATH_FILE_LICENSE_SERVER_OLD)
                     if license_encrypt:
                         CryptUtil().license_server.set_item(key_cache, license_encrypt)
         except Exception as ex:
             print("admin_sdk::get_license_encrypt():message: {}".format(ex))
         return license_encrypt
 
     @staticmethod
     def check_license_format(license_info):
         result = False
         try:
             if isinstance(license_info, dict):
                 if all(name in license_info for name in LicenseFormat.ALL_FIELD):
                     if isinstance(license_info.get(LicenseFormat.time_expire), int) and \
-                        isinstance(license_info.get(LicenseFormat.version), int):
+                            isinstance(license_info.get(LicenseFormat.version), int):
                         result = True
         except Exception as ex:
             print("admin_sdk::check_license_format():message: {}".format(ex))
         return result
 
     @staticmethod
     def license_server_valid():
```

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/config.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/config.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/date_utils.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/date_utils.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/http_jwt_auth.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/http_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/mobio_admin_sdk.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/mobio_admin_sdk.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/mobio_authorization.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/mobio_authorization.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/mongo_base_model.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/mongo_base_model.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/mysql_base_model.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/mysql_base_model.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/mobio/sdks/admin/utils.py` & `mobio-admin-sdk-1.0.9/mobio/sdks/admin/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 def decrypt_data(enc_data):
     try:
         while len(enc_data) % 4 != 0:
             enc_data = enc_data + "="
         decrypt_resp = AESCipher().decrypt(enc_data)
         if decrypt_resp:
-            return json.loads(decrypt_resp, encoding="utf-8")
+            return json.loads(decrypt_resp)
         return None
     except Exception as e:
         print("admin_sdk::decrypt_data: Exception: %s" % e)
         return None
 
 
 def get_merchant_auth(merchant_id):
@@ -826,15 +826,15 @@
         }
         body_request = {
             "msisdns": list_data
         }
         response = requests.post(
             api_url,
             headers=request_header,
-            data=body_request,
+            json=body_request,
             timeout=MobioAdminSDK.DEFAULT_REQUEST_TIMEOUT_SECONDS
         )
         response.raise_for_status()
         result = response.json()
         print("admin_sdk:: encrypt status: {}, text: {}".format(response.status_code, result))
         if result.get("content"):
             for item in result.get("content"):
@@ -862,15 +862,15 @@
         }
         body_request = {
             "msisdns": list_data
         }
         response = requests.post(
             api_url,
             headers=request_header,
-            data=body_request,
+            json=body_request,
             timeout=MobioAdminSDK.DEFAULT_REQUEST_TIMEOUT_SECONDS
         )
         response.raise_for_status()
         result = response.json()
         print("admin_sdk:: decrypt status: {}, text: {}".format(response.status_code, result))
         if result.get("content"):
             for item in result.get("content"):
```

### Comparing `mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/PKG-INFO` & `mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,153 +1,155 @@
 Metadata-Version: 2.1
 Name: mobio-admin-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio admin SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ##  Thư viện Admin SDK dành cho các module.
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install mobio-admin-sdk
-         ```
-        
-        ### Chức năng:
-        * Verify token 
-        
-        
-        ### Sử dụng:
-        
-        ##### 1. Verify token:
-           ```python
-            from mobio.sdks.admin import MobioAdminSDK
-        
-            MobioAdminSDK().config(
-                admin_host="",	# admin host
-                redis_uri="",	# redis uri
-                module_use="",	# liên hệ admin để khai báo tên của module
-                module_encrypt="",	# liên hệ admin để lấy mã
-                api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
-            )
-            auth = MobioAdminSDK().create_mobio_verify_token()
-            
-            @service_mod.route(url_path, methods=["get"])
-            @auth.verify_token
-            @try_catch_error
-            def get_config(merchant_id):
-                return build_response_message(Config(merchant_id).get_data())
-           ```
-        
-        ##### 2. Merchant config:
-           ```python
-            from mobio.sdks.admin import MobioAdminSDK
-        
-            MobioAdminSDK().request_get_merchant_config_host(
-                    merchant_id,
-                    key=None,       # key muốn lấy giá trị
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                )
-            MobioAdminSDK().request_get_merchant_config_other(
-                    merchant_id,
-                    list_key=None,       # danh sách key muốn lấy giá trị
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                )
-            MobioAdminSDK().request_check_merchant_is_brand(
-                    merchant_id,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
-                                        # không cần truyền, token_value sẽ lấy từ header của request 
-                )
-            MobioAdminSDK().request_get_info_staff(
-                    merchant_id,
-                    account_id,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_info_staff(
-                    merchant_id,
-                    params=None, # tham số của api  VD: {"per_page": -1}
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_parent_merchant(
-                    merchant_id,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_profile_group(
-                    merchant_id=None,
-                    params=None,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_list_sub_brand(
-                    params=None,        # tham số của api  VD: {"merchant_id": ""}
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_info_sub_brand(
-                    subbrand_id=None,
-                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                        # không cần truyền, token_value sẽ lấy từ header của request
-                )
-            MobioAdminSDK().request_get_partner_info(
-                    partner_key=None,
-                    decrypt_data=False,
-            )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
-                
-        
-        
-        
-        ```
-        ##### 3. Save log action account:
-           ```python
-            from mobio.sdks.admin import MobioAdminSDK
-            action_account = {
-                    'account_id': "uuid",# required
-                    'action_name_vi': 'action name',# required
-                    'action_name_en': 'action name',# required
-                    'merchant_id': "uuid",# required
-                    'created_time': 0129301293  # required (timestamp(utcnow))
-                }
-            MobioAdminSDK().admin_save_log_action_account(action_account)
-           ```
-        #### Log - 1.0.1
-            - release sdk
-        #### Log - 1.0.2
-            - Kiểm tra license server còn hạn sử dụng hay không 
-        #### Log - 1.0.3
-            - Fix lỗi đọc file license 
-        #### Log - 1.0.4
-            - Authen app key data out 
-        #### Log - 1.0.5
-            - update lib kafka v2
-        #### Log - 1.0.6
-            - encrypt, decrypt field by config
-        #### Log - 1.0.7
-            -  kiểm tra thông tin field trước khi encrypt, decrypt 
-        #### Log - 1.0.8
-            -  sdk tự lấy thông tin REDIS_URI  
 Keywords: mobio,admin sdk,verify token
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+##  Thư viện Admin SDK dành cho các module.
+
+
+### Cài đặt:
+```bash
+ $ pip3 install mobio-admin-sdk
+ ```
+
+### Chức năng:
+* Verify token 
+
+
+### Sử dụng:
+
+##### 1. Verify token:
+   ```python
+    from mobio.sdks.admin import MobioAdminSDK
+
+    MobioAdminSDK().config(
+        admin_host="",	# admin host
+        redis_uri="",	# redis uri
+        module_use="",	# liên hệ admin để khai báo tên của module
+        module_encrypt="",	# liên hệ admin để lấy mã
+        api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
+    )
+    auth = MobioAdminSDK().create_mobio_verify_token()
+    
+    @service_mod.route(url_path, methods=["get"])
+    @auth.verify_token
+    @try_catch_error
+    def get_config(merchant_id):
+        return build_response_message(Config(merchant_id).get_data())
+   ```
+
+##### 2. Merchant config:
+   ```python
+    from mobio.sdks.admin import MobioAdminSDK
+
+    MobioAdminSDK().request_get_merchant_config_host(
+            merchant_id,
+            key=None,       # key muốn lấy giá trị
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+        )
+    MobioAdminSDK().request_get_merchant_config_other(
+            merchant_id,
+            list_key=None,       # danh sách key muốn lấy giá trị
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+        )
+    MobioAdminSDK().request_check_merchant_is_brand(
+            merchant_id,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
+                                # không cần truyền, token_value sẽ lấy từ header của request 
+        )
+    MobioAdminSDK().request_get_info_staff(
+            merchant_id,
+            account_id,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_info_staff(
+            merchant_id,
+            params=None, # tham số của api  VD: {"per_page": -1}
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_parent_merchant(
+            merchant_id,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_profile_group(
+            merchant_id=None,
+            params=None,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_list_sub_brand(
+            params=None,        # tham số của api  VD: {"merchant_id": ""}
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_info_sub_brand(
+            subbrand_id=None,
+            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                # không cần truyền, token_value sẽ lấy từ header của request
+        )
+    MobioAdminSDK().request_get_partner_info(
+            partner_key=None,
+            decrypt_data=False,
+    )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
+        
+
+
+
+```
+##### 3. Save log action account:
+   ```python
+    from mobio.sdks.admin import MobioAdminSDK
+    action_account = {
+            'account_id': "uuid",# required
+            'action_name_vi': 'action name',# required
+            'action_name_en': 'action name',# required
+            'merchant_id': "uuid",# required
+            'created_time': 0129301293  # required (timestamp(utcnow))
+        }
+    MobioAdminSDK().admin_save_log_action_account(action_account)
+   ```
+#### Log - 1.0.1
+    - release sdk
+#### Log - 1.0.2
+    - Kiểm tra license server còn hạn sử dụng hay không 
+#### Log - 1.0.3
+    - Fix lỗi đọc file license 
+#### Log - 1.0.4
+    - Authen app key data out 
+#### Log - 1.0.5
+    - update lib kafka v2
+#### Log - 1.0.6
+    - encrypt, decrypt field by config
+#### Log - 1.0.7
+    -  kiểm tra thông tin field trước khi encrypt, decrypt 
+#### Log - 1.0.8
+    -  sdk tự lấy thông tin REDIS_URI  
+#### Log - 1.0.9
+    -  bỏ encoding trong json.loads
```

### Comparing `mobio-admin-sdk-1.0.8/mobio_admin_sdk.egg-info/SOURCES.txt` & `mobio-admin-sdk-1.0.9/mobio_admin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-1.0.8/setup.py` & `mobio-admin-sdk-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.9'
-version_prod='1.0.8'
+version_dev='1.0.11'
+version_prod='1.0.9'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -75,15 +75,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.8',  # Required
+    version='1.0.9',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio admin SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```


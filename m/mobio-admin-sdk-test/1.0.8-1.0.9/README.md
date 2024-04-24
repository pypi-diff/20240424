# Comparing `tmp/mobio-admin-sdk-test-1.0.8.tar.gz` & `tmp/mobio-admin-sdk-test-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-admin-sdk-test-1.0.8.tar", last modified: Sun Aug 14 16:10:55 2022, max compression
+gzip compressed data, was "mobio-admin-sdk-test-1.0.9.tar", last modified: Thu Dec 15 05:18:59 2022, max compression
```

## Comparing `mobio-admin-sdk-test-1.0.8.tar` & `mobio-admin-sdk-test-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2022-08-14 16:10:55.204336 mobio-admin-sdk-test-1.0.8/
--rw-rw-r--   0 theanh    (1000) theanh    (1000)     6663 2022-08-14 16:10:55.204336 mobio-admin-sdk-test-1.0.8/PKG-INFO
--rw-r--r--   0 theanh    (1000) theanh    (1000)     5828 2022-08-14 07:53:02.000000 mobio-admin-sdk-test-1.0.8/README.md
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2022-08-14 16:10:55.200336 mobio-admin-sdk-test-1.0.8/mobio/
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2022-08-14 16:10:55.200336 mobio-admin-sdk-test-1.0.8/mobio/sdks/
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2022-08-14 16:10:55.204336 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/
--rw-r--r--   0 theanh    (1000) theanh    (1000)      385 2022-08-14 16:00:28.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/__init__.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     5755 2022-07-15 04:20:05.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/aes_cipher.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     3196 2022-08-14 15:18:03.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/config.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)      789 2022-07-12 06:37:14.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/date_utils.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     6448 2022-07-12 06:37:14.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/http_jwt_auth.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)    11769 2022-08-14 09:25:08.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mobio_admin_sdk.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     8274 2022-07-26 09:54:42.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mobio_authorization.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     3100 2022-07-12 06:37:14.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mongo_base_model.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     2569 2022-07-12 06:37:14.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mysql_base_model.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)    32168 2022-08-14 16:00:28.000000 mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/utils.py
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2022-08-14 16:10:55.204336 mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/
--rw-rw-r--   0 theanh    (1000) theanh    (1000)     6663 2022-08-14 16:10:55.000000 mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/PKG-INFO
--rw-rw-r--   0 theanh    (1000) theanh    (1000)      580 2022-08-14 16:10:55.000000 mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/SOURCES.txt
--rw-rw-r--   0 theanh    (1000) theanh    (1000)        1 2022-08-14 16:10:55.000000 mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/dependency_links.txt
--rw-rw-r--   0 theanh    (1000) theanh    (1000)      101 2022-08-14 16:10:55.000000 mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/requires.txt
--rw-rw-r--   0 theanh    (1000) theanh    (1000)        6 2022-08-14 16:10:55.000000 mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 theanh    (1000) theanh    (1000)      104 2022-07-12 06:37:14.000000 mobio-admin-sdk-test-1.0.8/pyproject.toml
--rw-rw-r--   0 theanh    (1000) theanh    (1000)       38 2022-08-14 16:10:55.204336 mobio-admin-sdk-test-1.0.8/setup.cfg
--rw-r--r--   0 theanh    (1000) theanh    (1000)     9745 2022-08-14 16:00:28.000000 mobio-admin-sdk-test-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 05:18:59.499064 mobio-admin-sdk-test-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     7701 2022-12-15 05:18:59.498064 mobio-admin-sdk-test-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5828 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 05:18:59.484064 mobio-admin-sdk-test-1.0.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 05:18:59.484064 mobio-admin-sdk-test-1.0.9/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 05:18:59.495064 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/
+-rw-r--r--   0 root         (0) root         (0)      397 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5755 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/aes_cipher.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/config.py
+-rw-r--r--   0 root         (0) root         (0)      789 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/date_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6448 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/http_jwt_auth.py
+-rw-r--r--   0 root         (0) root         (0)    11787 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mobio_admin_sdk.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mobio_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mongo_base_model.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mysql_base_model.py
+-rw-r--r--   0 root         (0) root         (0)    32268 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 05:18:59.497064 mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7701 2022-12-15 05:18:59.000000 mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2022-12-15 05:18:59.000000 mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-15 05:18:59.000000 mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2022-12-15 05:18:59.000000 mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-12-15 05:18:59.000000 mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2022-12-15 05:05:05.000000 mobio-admin-sdk-test-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-15 05:18:59.499064 mobio-admin-sdk-test-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9792 2022-12-15 05:18:58.000000 mobio-admin-sdk-test-1.0.9/setup.py
```

### Comparing `mobio-admin-sdk-test-1.0.8/PKG-INFO` & `mobio-admin-sdk-test-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,150 +1,150 @@
 Metadata-Version: 2.1
 Name: mobio-admin-sdk-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio admin SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
+Description: ##  Thư viện Admin SDK dành cho các module.
+        
+        
+        ### Cài đặt:
+        ```bash
+         $ pip3 install mobio-admin-sdk
+         ```
+        
+        ### Chức năng:
+        * Verify token 
+        
+        
+        ### Sử dụng:
+        
+        ##### 1. Verify token:
+           ```python
+            from mobio.sdks.admin import MobioAdminSDK
+        
+            MobioAdminSDK().config(
+                admin_host="",	# admin host
+                redis_uri="",	# redis uri
+                module_use="",	# liên hệ admin để khai báo tên của module
+                module_encrypt="",	# liên hệ admin để lấy mã
+                api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
+            )
+            auth = MobioAdminSDK().create_mobio_verify_token()
+            
+            @service_mod.route(url_path, methods=["get"])
+            @auth.verify_token
+            @try_catch_error
+            def get_config(merchant_id):
+                return build_response_message(Config(merchant_id).get_data())
+           ```
+        
+        ##### 2. Merchant config:
+           ```python
+            from mobio.sdks.admin import MobioAdminSDK
+        
+            MobioAdminSDK().request_get_merchant_config_host(
+                    merchant_id,
+                    key=None,       # key muốn lấy giá trị
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                )
+            MobioAdminSDK().request_get_merchant_config_other(
+                    merchant_id,
+                    list_key=None,       # danh sách key muốn lấy giá trị
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                )
+            MobioAdminSDK().request_check_merchant_is_brand(
+                    merchant_id,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
+                                        # không cần truyền, token_value sẽ lấy từ header của request 
+                )
+            MobioAdminSDK().request_get_info_staff(
+                    merchant_id,
+                    account_id,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_info_staff(
+                    merchant_id,
+                    params=None, # tham số của api  VD: {"per_page": -1}
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_parent_merchant(
+                    merchant_id,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_profile_group(
+                    merchant_id=None,
+                    params=None,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_sub_brand(
+                    params=None,        # tham số của api  VD: {"merchant_id": ""}
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_info_sub_brand(
+                    subbrand_id=None,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_partner_info(
+                    partner_key=None,
+                    decrypt_data=False,
+            )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
+                
+        
+        
+        
+        ```
+        ##### 3. Save log action account:
+           ```python
+            from mobio.sdks.admin import MobioAdminSDK
+            action_account = {
+                    'account_id': "uuid",# required
+                    'action_name_vi': 'action name',# required
+                    'action_name_en': 'action name',# required
+                    'merchant_id': "uuid",# required
+                    'created_time': 0129301293  # required (timestamp(utcnow))
+                }
+            MobioAdminSDK().admin_save_log_action_account(action_account)
+           ```
+        #### Log - 1.0.1
+            - release sdk
+        #### Log - 1.0.2
+            - Kiểm tra license server còn hạn sử dụng hay không 
+        #### Log - 1.0.3
+            - Fix lỗi đọc file license 
+        #### Log - 1.0.4
+            - Authen app key data out 
+        #### Log - 1.0.5
+            - update lib kafka v2
+        #### Log - 1.0.6
+            - encrypt, decrypt field by config
+            
 Keywords: mobio,admin sdk,verify token
+Platform: UNKNOWN
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
-
-##  Thư viện Admin SDK dành cho các module.
-
-
-### Cài đặt:
-```bash
- $ pip3 install mobio-admin-sdk
- ```
-
-### Chức năng:
-* Verify token 
-
-
-### Sử dụng:
-
-##### 1. Verify token:
-   ```python
-    from mobio.sdks.admin import MobioAdminSDK
-
-    MobioAdminSDK().config(
-        admin_host="",	# admin host
-        redis_uri="",	# redis uri
-        module_use="",	# liên hệ admin để khai báo tên của module
-        module_encrypt="",	# liên hệ admin để lấy mã
-        api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
-    )
-    auth = MobioAdminSDK().create_mobio_verify_token()
-    
-    @service_mod.route(url_path, methods=["get"])
-    @auth.verify_token
-    @try_catch_error
-    def get_config(merchant_id):
-        return build_response_message(Config(merchant_id).get_data())
-   ```
-
-##### 2. Merchant config:
-   ```python
-    from mobio.sdks.admin import MobioAdminSDK
-
-    MobioAdminSDK().request_get_merchant_config_host(
-            merchant_id,
-            key=None,       # key muốn lấy giá trị
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-        )
-    MobioAdminSDK().request_get_merchant_config_other(
-            merchant_id,
-            list_key=None,       # danh sách key muốn lấy giá trị
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-        )
-    MobioAdminSDK().request_check_merchant_is_brand(
-            merchant_id,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
-                                # không cần truyền, token_value sẽ lấy từ header của request 
-        )
-    MobioAdminSDK().request_get_info_staff(
-            merchant_id,
-            account_id,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_info_staff(
-            merchant_id,
-            params=None, # tham số của api  VD: {"per_page": -1}
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_parent_merchant(
-            merchant_id,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_profile_group(
-            merchant_id=None,
-            params=None,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_sub_brand(
-            params=None,        # tham số của api  VD: {"merchant_id": ""}
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_info_sub_brand(
-            subbrand_id=None,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_partner_info(
-            partner_key=None,
-            decrypt_data=False,
-    )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
-        
-
-
-
-```
-##### 3. Save log action account:
-   ```python
-    from mobio.sdks.admin import MobioAdminSDK
-    action_account = {
-            'account_id': "uuid",# required
-            'action_name_vi': 'action name',# required
-            'action_name_en': 'action name',# required
-            'merchant_id': "uuid",# required
-            'created_time': 0129301293  # required (timestamp(utcnow))
-        }
-    MobioAdminSDK().admin_save_log_action_account(action_account)
-   ```
-#### Log - 1.0.1
-    - release sdk
-#### Log - 1.0.2
-    - Kiểm tra license server còn hạn sử dụng hay không 
-#### Log - 1.0.3
-    - Fix lỗi đọc file license 
-#### Log - 1.0.4
-    - Authen app key data out 
-#### Log - 1.0.5
-    - update lib kafka v2
-#### Log - 1.0.6
-    - encrypt, decrypt field by config
-
```

### Comparing `mobio-admin-sdk-test-1.0.8/README.md` & `mobio-admin-sdk-test-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/aes_cipher.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/aes_cipher.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/config.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/config.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/date_utils.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/date_utils.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/http_jwt_auth.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/http_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mobio_admin_sdk.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mobio_admin_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
     @staticmethod
     @sdk_pre_check
     def decrypt_values(merchant_id, module, field, values):
         from .utils import decrypt_field_by_config
         return decrypt_field_by_config(merchant_id, module, field, values)
 
-    def get_value(self, key_cache):
+    def redis_get_value(self, key_cache):
         return self.redis_connection.get(key_cache)
 
-    def set_value_expire(self, key_cache, value_cache, time_seconds=3600):
+    def redis_set_value_expire(self, key_cache, value_cache, time_seconds=3600):
         self.redis_connection.setex(key_cache, time_seconds, value_cache)
 
-    def delete_key(self, key_cache):
+    def redis_delete_key(self, key_cache):
         self.redis_connection.delete(key_cache)
```

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mobio_authorization.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mobio_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,42 +123,45 @@
         try:
             from .utils import check_basic_auth_v2
 
             # if MobioAuthorization.license_merchant_expire():
             #     return None
 
             # check key
-            mobio_key = request.headers.get(SystemConfigKeys.X_MOBIO_KEY, None)
-            mobio_key_valid = check_basic_auth_v2(mobio_key) if mobio_key else False
-            if mobio_key_valid:
-                return mobio_key
-            else:
-                if typically == TYPICALLY.BEARER or typically == TYPICALLY.DIGEST:
-                    is_staff = self.get(jwt_token, "is_mobio") is not None
-                    if is_staff and typically != TYPICALLY.BEARER:
-                        raise ValueError(
-                            "admin_sdk::typically invalidated, this must is %s" % TYPICALLY.BEARER
-                        )
-                    if (not is_staff) and typically != TYPICALLY.DIGEST:
-                        raise ValueError(
-                            "admin_sdk::typically invalidated, this must is %s" % TYPICALLY.DIGEST
-                        )
-                    arr_token = jwt_token.split(".")
-                    # kiểm tra token trong REDIS
-                    verify_token = arr_token[2]
-                    value = self.local_redis.get(verify_token)
-                    if not value:
-                        raise ValueError("admin_sdk::verify_token: {} not found in redis".format(verify_token))
-                    return jwt_token
+            # try:
+            #     mobio_key = request.headers.get(SystemConfigKeys.X_MOBIO_KEY, None)
+            #     mobio_key_valid = check_basic_auth_v2(mobio_key) if mobio_key else False
+            #     if mobio_key_valid:
+            #         return mobio_key
+            # except Exception as e:
+            #     print("admin_sdk::check x-mobio-key: ERROR: %s" % e)
 
-                elif typically == TYPICALLY.BASIC:
-                    if not check_basic_auth_v2(jwt_token):
-                        if not MobioAuthorization.check_app_data_out(jwt_token):
-                            raise ValueError("admin_sdk:: {} basic key invalid".format(jwt_token))
-                    return jwt_token
+            if typically == TYPICALLY.BEARER or typically == TYPICALLY.DIGEST:
+                is_staff = self.get(jwt_token, "is_mobio") is not None
+                if is_staff and typically != TYPICALLY.BEARER:
+                    raise ValueError(
+                        "admin_sdk::typically invalidated, this must is %s" % TYPICALLY.BEARER
+                    )
+                if (not is_staff) and typically != TYPICALLY.DIGEST:
+                    raise ValueError(
+                        "admin_sdk::typically invalidated, this must is %s" % TYPICALLY.DIGEST
+                    )
+                arr_token = jwt_token.split(".")
+                # kiểm tra token trong REDIS
+                verify_token = arr_token[2]
+                value = self.local_redis.get(verify_token)
+                if not value:
+                    raise ValueError("admin_sdk::verify_token: {} not found in redis".format(verify_token))
+                return jwt_token
+
+            elif typically == TYPICALLY.BASIC:
+                if not check_basic_auth_v2(jwt_token):
+                    if not MobioAuthorization.check_app_data_out(jwt_token):
+                        raise ValueError("admin_sdk:: {} basic key invalid".format(jwt_token))
+                return jwt_token
 
         except Exception as e:
             print("admin_sdk::MobioAuthorization::verify_token: ERROR: %s" % e)
             return None
         return None
     
     def get_jwt_value(self, key):
```

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mongo_base_model.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mongo_base_model.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/mysql_base_model.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/mysql_base_model.py`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/mobio/sdks/admin/utils.py` & `mobio-admin-sdk-test-1.0.9/mobio/sdks/admin/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,15 +614,15 @@
     }
     if MobioAdminSDK().request_header:
         request_header.update(MobioAdminSDK().request_header)
     response = requests.get(
         api_url,
         params=params,
         headers=request_header,
-        timeout=2,
+        timeout=MobioAdminSDK.DEFAULT_REQUEST_TIMEOUT_SECONDS,
     )
     response.raise_for_status()
     result = response.json()
     if result and result.get("data"):
         return result.get("data")
     else:
         return None
@@ -681,15 +681,15 @@
 
 def get_info_field_config(merchant_id, module, field):
     field_config = {}
     try:
         fields_config = get_list_fields_config_encrypt(merchant_id, module)
         if fields_config:
             for item in fields_config:
-                if item.get("field") == field and item.get("kms_id"):
+                if item.get("field") == field and item.get("kms_id") and item.get("enc_level") != "enc_frontend":
                     field_config["kms_id"] = item.get("kms_id")
                     field_config["kms_info"] = item.get("kms_info")
                     # field_config["normalize_config"] = item.get("normalize_config", "")
                     break
     except Exception as e:
         print("admin_sdk::get_kms_id_from_fields_config: error: {}".format(e))
     return field_config
@@ -771,15 +771,15 @@
         else:
             data_error[item] = CodeErrorDecrypt.decrypt_error
     return {"data": data, "data_error": data_error}
 
 def kms_viettel_get_token(kms_id):
     try:
         key_cache = RedisKeyCache.kms_viettel_get_token.format(kms_id)
-        token_key = MobioAdminSDK().get_value(key_cache)
+        token_key = MobioAdminSDK().redis_get_value(key_cache)
         if token_key:
             return token_key.decode('utf-8')
         else:
             api_version = MobioAdminSDK().admin_version
             adm_url = str(UrlConfig.GET_TOKEN_KMS_CONFIG).format(
                 host=MobioAdminSDK().admin_host, version=api_version
             )
@@ -797,15 +797,15 @@
             )
             response.raise_for_status()
             result = response.json()
             if result and result.get("data"):
                 token_key = result.get("data").get("access_token")
                 expires_in = int(result.get("data").get("expires_in"))
                 expires_in = expires_in - 30 if expires_in > 30 else expires_in
-                MobioAdminSDK().set_value_expire(key_cache, token_key, time_seconds=expires_in)
+                MobioAdminSDK().redis_set_value_expire(key_cache, token_key, time_seconds=expires_in)
                 return token_key
     except Exception as er:
         print("admin_sdk::kms_viettel_get_token: error: {}".format(er))
     return None
 
 def build_data_error_by_code(list_data, error_code):
     data_error = {}
```

### Comparing `mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/PKG-INFO` & `mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,150 +1,150 @@
 Metadata-Version: 2.1
 Name: mobio-admin-sdk-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio admin SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
+Description: ##  Thư viện Admin SDK dành cho các module.
+        
+        
+        ### Cài đặt:
+        ```bash
+         $ pip3 install mobio-admin-sdk
+         ```
+        
+        ### Chức năng:
+        * Verify token 
+        
+        
+        ### Sử dụng:
+        
+        ##### 1. Verify token:
+           ```python
+            from mobio.sdks.admin import MobioAdminSDK
+        
+            MobioAdminSDK().config(
+                admin_host="",	# admin host
+                redis_uri="",	# redis uri
+                module_use="",	# liên hệ admin để khai báo tên của module
+                module_encrypt="",	# liên hệ admin để lấy mã
+                api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
+            )
+            auth = MobioAdminSDK().create_mobio_verify_token()
+            
+            @service_mod.route(url_path, methods=["get"])
+            @auth.verify_token
+            @try_catch_error
+            def get_config(merchant_id):
+                return build_response_message(Config(merchant_id).get_data())
+           ```
+        
+        ##### 2. Merchant config:
+           ```python
+            from mobio.sdks.admin import MobioAdminSDK
+        
+            MobioAdminSDK().request_get_merchant_config_host(
+                    merchant_id,
+                    key=None,       # key muốn lấy giá trị
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                )
+            MobioAdminSDK().request_get_merchant_config_other(
+                    merchant_id,
+                    list_key=None,       # danh sách key muốn lấy giá trị
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                )
+            MobioAdminSDK().request_check_merchant_is_brand(
+                    merchant_id,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
+                                        # không cần truyền, token_value sẽ lấy từ header của request 
+                )
+            MobioAdminSDK().request_get_info_staff(
+                    merchant_id,
+                    account_id,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_info_staff(
+                    merchant_id,
+                    params=None, # tham số của api  VD: {"per_page": -1}
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_parent_merchant(
+                    merchant_id,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_profile_group(
+                    merchant_id=None,
+                    params=None,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_list_sub_brand(
+                    params=None,        # tham số của api  VD: {"merchant_id": ""}
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_info_sub_brand(
+                    subbrand_id=None,
+                    admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
+                    token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
+                                        # không cần truyền, token_value sẽ lấy từ header của request
+                )
+            MobioAdminSDK().request_get_partner_info(
+                    partner_key=None,
+                    decrypt_data=False,
+            )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
+                
+        
+        
+        
+        ```
+        ##### 3. Save log action account:
+           ```python
+            from mobio.sdks.admin import MobioAdminSDK
+            action_account = {
+                    'account_id': "uuid",# required
+                    'action_name_vi': 'action name',# required
+                    'action_name_en': 'action name',# required
+                    'merchant_id': "uuid",# required
+                    'created_time': 0129301293  # required (timestamp(utcnow))
+                }
+            MobioAdminSDK().admin_save_log_action_account(action_account)
+           ```
+        #### Log - 1.0.1
+            - release sdk
+        #### Log - 1.0.2
+            - Kiểm tra license server còn hạn sử dụng hay không 
+        #### Log - 1.0.3
+            - Fix lỗi đọc file license 
+        #### Log - 1.0.4
+            - Authen app key data out 
+        #### Log - 1.0.5
+            - update lib kafka v2
+        #### Log - 1.0.6
+            - encrypt, decrypt field by config
+            
 Keywords: mobio,admin sdk,verify token
+Platform: UNKNOWN
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
-
-##  Thư viện Admin SDK dành cho các module.
-
-
-### Cài đặt:
-```bash
- $ pip3 install mobio-admin-sdk
- ```
-
-### Chức năng:
-* Verify token 
-
-
-### Sử dụng:
-
-##### 1. Verify token:
-   ```python
-    from mobio.sdks.admin import MobioAdminSDK
-
-    MobioAdminSDK().config(
-        admin_host="",	# admin host
-        redis_uri="",	# redis uri
-        module_use="",	# liên hệ admin để khai báo tên của module
-        module_encrypt="",	# liên hệ admin để lấy mã
-        api_admin_version="api/v2.1",   # danh sách api có thể sử dụng ["v1.0", "api/v2.0", "api/v2.1"]
-    )
-    auth = MobioAdminSDK().create_mobio_verify_token()
-    
-    @service_mod.route(url_path, methods=["get"])
-    @auth.verify_token
-    @try_catch_error
-    def get_config(merchant_id):
-        return build_response_message(Config(merchant_id).get_data())
-   ```
-
-##### 2. Merchant config:
-   ```python
-    from mobio.sdks.admin import MobioAdminSDK
-
-    MobioAdminSDK().request_get_merchant_config_host(
-            merchant_id,
-            key=None,       # key muốn lấy giá trị
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-        )
-    MobioAdminSDK().request_get_merchant_config_other(
-            merchant_id,
-            list_key=None,       # danh sách key muốn lấy giá trị
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-        )
-    MobioAdminSDK().request_check_merchant_is_brand(
-            merchant_id,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì 
-                                # không cần truyền, token_value sẽ lấy từ header của request 
-        )
-    MobioAdminSDK().request_get_info_staff(
-            merchant_id,
-            account_id,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_info_staff(
-            merchant_id,
-            params=None, # tham số của api  VD: {"per_page": -1}
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_parent_merchant(
-            merchant_id,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_profile_group(
-            merchant_id=None,
-            params=None,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_list_sub_brand(
-            params=None,        # tham số của api  VD: {"merchant_id": ""}
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_info_sub_brand(
-            subbrand_id=None,
-            admin_version=None, # api version admin muốn gọi trong trường hợp chỉ có version đó hỗ trợ
-            token_value=None,  # token_value dạng là Bearer hoặc Basic, nếu nơi gọi là request đã authen thì
-                                # không cần truyền, token_value sẽ lấy từ header của request
-        )
-    MobioAdminSDK().request_get_partner_info(
-            partner_key=None,
-            decrypt_data=False,
-    )   # result: { "code": 200, "data": ""}, {"code": 400, "message": "key not found"}, {"code": 412, "message": "key not active"}, {"code": 413, "message": "key expire"}
-        
-
-
-
-```
-##### 3. Save log action account:
-   ```python
-    from mobio.sdks.admin import MobioAdminSDK
-    action_account = {
-            'account_id': "uuid",# required
-            'action_name_vi': 'action name',# required
-            'action_name_en': 'action name',# required
-            'merchant_id': "uuid",# required
-            'created_time': 0129301293  # required (timestamp(utcnow))
-        }
-    MobioAdminSDK().admin_save_log_action_account(action_account)
-   ```
-#### Log - 1.0.1
-    - release sdk
-#### Log - 1.0.2
-    - Kiểm tra license server còn hạn sử dụng hay không 
-#### Log - 1.0.3
-    - Fix lỗi đọc file license 
-#### Log - 1.0.4
-    - Authen app key data out 
-#### Log - 1.0.5
-    - update lib kafka v2
-#### Log - 1.0.6
-    - encrypt, decrypt field by config
-
```

### Comparing `mobio-admin-sdk-test-1.0.8/mobio_admin_sdk_test.egg-info/SOURCES.txt` & `mobio-admin-sdk-test-1.0.9/mobio_admin_sdk_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-admin-sdk-test-1.0.8/setup.py` & `mobio-admin-sdk-test-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,37 +50,40 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
+version_dev='1.0.9'
+version_prod='1.0.6'
+
+run_mode='-test'
 
-version = "1.0.8"
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
     #
     # $ pip install sampleproject
     #
     # And where it will live on PyPI: https://pypi.org/project/sampleproject/
     #
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
-    name="mobio-admin-sdk-test",  # Required
+    name="mobio-admin-sdk" + run_mode,  # Required
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version=version,  # Required
+    version='1.0.9',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio admin SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```


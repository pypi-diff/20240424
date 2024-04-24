# Comparing `tmp/eis-insurance-1.30.0.tar.gz` & `tmp/eis-insurance-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis-insurance-1.30.0.tar", last modified: Thu Apr 18 15:36:21 2024, max compression
+gzip compressed data, was "eis-insurance-1.31.0.tar", last modified: Wed Apr 24 19:13:37 2024, max compression
```

## Comparing `eis-insurance-1.30.0.tar` & `eis-insurance-1.31.0.tar`

### file list

```diff
@@ -1,325 +1,351 @@
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.850491 eis-insurance-1.30.0/
--rw-r--r--   0 ricard     (501) staff       (20)      337 2024-04-18 15:36:21.850646 eis-insurance-1.30.0/PKG-INFO
--rw-r--r--   0 ricard     (501) staff       (20)    23000 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/README.md
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.741298 eis-insurance-1.30.0/eis/
--rw-r--r--   0 ricard     (501) staff       (20)        0 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/__init__.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.743991 eis-insurance-1.30.0/eis/insurance/
--rw-r--r--   0 ricard     (501) staff       (20)      735 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/__init__.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.751109 eis-insurance-1.30.0/eis/insurance/api/
--rw-r--r--   0 ricard     (501) staff       (20)      228 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)     5447 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/default_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     7612 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/insured_object_types_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    24476 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/insured_objects_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    23408 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/lead_statuses_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    55099 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/leads_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    30117 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/named_ranges_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    63708 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/policies_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    36321 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/premium_formulas_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    37917 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/product_factors_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    36949 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/product_fields_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    13361 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/product_versions_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    37898 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/products_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    41662 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api_client.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.751392 eis-insurance-1.30.0/eis/insurance/apis/
--rw-r--r--   0 ricard     (501) staff       (20)     1207 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/apis/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    16484 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/configuration.py
--rw-r--r--   0 ricard     (501) staff       (20)     5074 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/exceptions.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.804803 eis-insurance-1.30.0/eis/insurance/model/
--rw-r--r--   0 ricard     (501) staff       (20)      347 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    11485 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/activate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11862 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/activate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12128 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/calculate_custom_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12924 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/calculate_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12318 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/calculate_product_fields_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12421 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/clone_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    18487 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/create_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11866 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/create_bank_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12564 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/create_custom_application_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13015 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_dummy_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14361 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12009 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11606 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_async_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14927 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    21946 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11842 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11759 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_status_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11947 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13809 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11949 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12316 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_named_request_s3_data_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_payment_method_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14081 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11864 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    15591 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12053 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    18650 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12403 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14404 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11896 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12383 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/csv_product_factor_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11462 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/delete_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11703 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/delete_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11700 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/empty_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12000 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11938 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11940 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11718 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_policy_data_by_date_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11847 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11657 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12328 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12874 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factor_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12439 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11950 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12517 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11871 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11651 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12050 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12558 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11865 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12033 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12018 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12323 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12395 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11940 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/grouped_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    17245 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/grpc_patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    22171 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/grpc_update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12817 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/inline_response200.py
--rw-r--r--   0 ricard     (501) staff       (20)    12817 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/inline_response503.py
--rw-r--r--   0 ricard     (501) staff       (20)    15814 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/insured_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13038 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/insured_object_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    16768 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/invoice_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12653 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/invoice_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/lead_bank_account_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    19631 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/lead_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12384 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/lead_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12158 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_insured_object_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12131 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_insured_objects_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12100 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_lead_statuses_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12674 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_leads_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11874 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_named_ranges_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12703 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_policies_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12265 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_premium_formulas_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12149 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12283 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_product_field_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12121 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_product_fields_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12074 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_products_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12582 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14789 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/named_range_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    16739 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11811 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13591 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11851 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    17937 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/policy_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13748 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/policy_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12867 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13319 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/policy_premium_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13714 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/policy_premium_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13763 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/policy_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    15539 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_formula_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12952 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_override_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11971 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_override_request_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11905 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_override_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    15269 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14144 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14246 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13780 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12756 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_value_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    18978 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12863 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_field_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13423 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11637 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/sepa_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14945 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    18643 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_invoice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12997 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_lead_policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    18996 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12804 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    15971 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12263 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/store_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11884 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/store_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11484 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/suspend_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11859 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/suspend_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11904 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12604 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/terminate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11863 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/terminate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13994 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/timeslice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14723 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    21581 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11842 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12424 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11949 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14608 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11854 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    15591 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12029 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    19144 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12403 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12771 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11874 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12417 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12027 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11528 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/uploaded_document_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12342 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/validate_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11860 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/withdraw_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    82491 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model_utils.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.805031 eis-insurance-1.30.0/eis/insurance/models/
--rw-r--r--   0 ricard     (501) staff       (20)    12263 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/models/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    14277 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/rest.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.805837 eis-insurance-1.30.0/eis_insurance.egg-info/
--rw-r--r--   0 ricard     (501) staff       (20)      337 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/PKG-INFO
--rw-r--r--   0 ricard     (501) staff       (20)    14232 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/SOURCES.txt
--rw-r--r--   0 ricard     (501) staff       (20)        1 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/dependency_links.txt
--rw-r--r--   0 ricard     (501) staff       (20)       32 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/requires.txt
--rw-r--r--   0 ricard     (501) staff       (20)        4 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/top_level.txt
--rw-r--r--   0 ricard     (501) staff       (20)      162 2024-04-18 15:36:21.851008 eis-insurance-1.30.0/setup.cfg
--rw-r--r--   0 ricard     (501) staff       (20)      996 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/setup.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.850303 eis-insurance-1.30.0/test/
--rw-r--r--   0 ricard     (501) staff       (20)      826 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_activate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      943 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_activate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      883 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_calculate_custom_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1107 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_calculate_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      996 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_calculate_product_fields_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      862 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_clone_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_create_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      848 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_create_bank_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      890 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_create_custom_application_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1115 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_dummy_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      862 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_async_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1150 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1745 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      907 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      841 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_status_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1013 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      863 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_named_request_s3_data_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      942 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_payment_method_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1079 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      997 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      940 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      791 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_csv_product_factor_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      645 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_default_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      769 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_delete_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_delete_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      783 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_empty_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      987 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      886 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      954 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      954 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      864 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_policy_data_by_date_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      791 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      908 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      848 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      998 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1087 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factor_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      877 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factor_value_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1044 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factor_value_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      920 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factors_for_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1108 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factors_for_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      834 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      976 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      798 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      919 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      848 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      998 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_grouped_product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_grouped_product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1051 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_grouped_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1742 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_grpc_patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1749 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_grpc_update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      775 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_inline_response200.py
--rw-r--r--   0 ricard     (501) staff       (20)      775 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_inline_response503.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_insured_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      812 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_insured_object_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_insured_object_types_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1242 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_insured_objects_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      769 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_invoice_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      783 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_invoice_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      798 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_lead_bank_account_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1745 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_lead_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      762 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_lead_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1199 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_lead_statuses_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_leads_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1047 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_insured_object_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1001 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_insured_objects_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_lead_statuses_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      900 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_leads_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_named_ranges_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_policies_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1012 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_premium_formulas_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1001 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1036 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_product_field_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      990 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_product_fields_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      933 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_products_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      755 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      762 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_named_range_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1347 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_named_ranges_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1713 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      900 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1072 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      922 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     2054 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policies_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      958 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_policy_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      776 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_policy_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      762 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      925 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policy_premium_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      941 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policy_premium_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      891 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policy_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_formula_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1606 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_formulas_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      783 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_override_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      972 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_override_request_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      958 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_override_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1011 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1043 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      891 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_value_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1604 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factors_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      776 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      805 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_field_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1543 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_fields_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      932 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_versions_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1453 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_products_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      705 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_sepa_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1193 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1025 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_invoice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      834 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_lead_policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      884 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      912 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      992 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_store_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_store_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_suspend_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      936 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_suspend_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      898 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_swap_premium_formulas_order_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      833 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_terminate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      950 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_terminate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1000 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_timeslice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      862 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1720 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      907 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      841 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1079 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      997 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      940 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_uploaded_document_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1013 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_validate_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      943 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_withdraw_policy_response_class.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.108956 eis-insurance-1.31.0/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-24 19:13:37.108956 eis-insurance-1.31.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    25633 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.068956 eis-insurance-1.31.0/eis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.072956 eis-insurance-1.31.0/eis/insurance/
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.072956 eis-insurance-1.31.0/eis/insurance/api/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/default_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7612 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/insured_object_types_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    24476 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/insured_objects_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    23408 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/lead_statuses_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15461 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/lead_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    55099 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/leads_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    30117 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/named_ranges_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    63708 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/policies_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    36321 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/premium_formulas_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37917 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/product_factors_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    36949 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/product_fields_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    13361 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/product_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37898 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/products_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    39773 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api/status_transition_rules_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    41662 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.072956 eis-insurance-1.31.0/eis/insurance/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16484 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5074 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.092956 eis-insurance-1.31.0/eis/insurance/model/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/activate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/activate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12128 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/calculate_custom_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12924 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/calculate_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12318 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/calculate_product_fields_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12421 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/clone_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    18487 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11866 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_bank_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12564 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_custom_application_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_dummy_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14361 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11606 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_lead_async_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14927 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    21946 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11842 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11759 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_lead_status_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11947 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12316 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_named_request_s3_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_payment_method_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14081 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11864 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    15591 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12053 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    18650 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12403 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14404 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11896 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12557 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12061 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/create_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12383 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/csv_product_factor_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11703 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/delete_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11700 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/empty_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12000 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11705 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_lead_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11794 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_lead_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11940 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11718 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_policy_data_by_date_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11847 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12328 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12874 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_factor_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12439 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_factor_value_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11950 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_factor_value_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12517 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_factors_for_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11871 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_factors_for_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11651 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12050 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12558 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11865 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12033 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12018 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12151 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/get_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12323 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/grouped_product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12395 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/grouped_product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11940 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/grouped_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    17245 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/grpc_patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    22171 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/grpc_update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12817 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/eis/insurance/model/inline_response200.py
+-rw-rw-rw-   0 root         (0) root         (0)    12817 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/inline_response503.py
+-rw-rw-rw-   0 root         (0) root         (0)    15814 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/insured_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13038 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/insured_object_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    16768 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/invoice_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12653 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/invoice_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/lead_bank_account_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    19860 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/lead_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12384 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/lead_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12158 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_insured_object_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12131 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_insured_objects_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12100 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_lead_statuses_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12057 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_lead_versions_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12674 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_leads_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11874 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_named_ranges_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12703 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_policies_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12265 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_premium_formulas_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12149 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12283 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_product_field_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12121 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_product_fields_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12074 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_products_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12582 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12218 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/list_status_transition_rules_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14789 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/named_range_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    16739 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11811 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/patch_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13779 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/patch_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11851 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/patch_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12492 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/patch_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12157 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/patch_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    17937 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/policy_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13748 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/policy_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13319 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/policy_premium_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13714 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/policy_premium_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13763 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/policy_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    15539 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/premium_formula_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12952 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/premium_override_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11971 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/premium_override_request_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11905 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/premium_override_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14144 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14246 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_factor_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13780 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12756 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_factor_value_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    18932 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12863 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_field_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13423 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/product_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11637 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/sepa_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14945 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/shared_create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    18643 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/shared_invoice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12997 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/shared_lead_policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    18950 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/shared_product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12804 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/shared_update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    15971 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/shared_update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14223 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/status_transition_rule_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12263 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/store_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/store_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/suspend_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11859 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/suspend_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11904 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12604 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/terminate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11863 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/terminate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    13994 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/timeslice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14723 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    21581 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11842 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12424 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    14608 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11854 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    15591 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    19144 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12403 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12771 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11874 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12417 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12027 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12747 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12160 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/update_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    11528 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/uploaded_document_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12342 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/validate_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model/withdraw_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    82491 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/model_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.092956 eis-insurance-1.31.0/eis/insurance/models/
+-rw-rw-rw-   0 root         (0) root         (0)    13462 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14277 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/eis/insurance/rest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.092956 eis-insurance-1.31.0/eis_insurance.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-24 19:13:37.000000 eis-insurance-1.31.0/eis_insurance.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    15688 2024-04-24 19:13:37.000000 eis-insurance-1.31.0/eis_insurance.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-24 19:13:37.000000 eis-insurance-1.31.0/eis_insurance.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-24 19:13:37.000000 eis-insurance-1.31.0/eis_insurance.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-04-24 19:13:37.000000 eis-insurance-1.31.0/eis_insurance.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-24 19:13:37.108956 eis-insurance-1.31.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-24 19:13:37.108956 eis-insurance-1.31.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_activate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      943 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_activate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_calculate_custom_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_calculate_premium_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_calculate_product_fields_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_clone_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_bank_account_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_custom_application_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_dummy_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_lead_async_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_lead_status_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_named_request_s3_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_payment_method_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_create_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_csv_product_factor_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_default_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_delete_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_empty_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_insured_object_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_lead_status_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_lead_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_lead_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_policy_data_by_date_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_factor_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_factor_value_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_factor_value_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_factors_for_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_factors_for_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_get_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_grouped_product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_grouped_product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_grouped_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_grpc_patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_grpc_update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-24 19:13:35.000000 eis-insurance-1.31.0/test/test_inline_response200.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_inline_response503.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_insured_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_insured_object_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_insured_object_types_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_insured_objects_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_invoice_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_invoice_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_lead_bank_account_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_lead_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_lead_status_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_lead_statuses_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_lead_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_leads_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_insured_object_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_insured_objects_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_lead_statuses_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_lead_versions_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_leads_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_named_ranges_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_policies_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_premium_formulas_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_product_field_types_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_product_fields_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_products_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_list_status_transition_rules_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_named_range_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_named_ranges_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_patch_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_patch_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_patch_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_patch_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_patch_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_patch_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_policies_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_policy_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_policy_object_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_policy_premium_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_policy_premium_item_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_policy_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_premium_formula_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_premium_formulas_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_premium_override_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_premium_override_request_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_premium_override_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_factor_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_factor_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_factor_value_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_factor_value_for_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1604 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_factors_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_field_type_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_fields_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_version_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_product_versions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_products_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_sepa_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_shared_create_lead_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_shared_invoice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_shared_lead_policy_object_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_shared_product_field_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_shared_update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_shared_update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_status_transition_rule_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_status_transition_rules_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_store_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_store_product_factors_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_suspend_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_suspend_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_swap_premium_formulas_order_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_terminate_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_terminate_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_timeslice_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_insured_object_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_lead_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_lead_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_named_range_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_named_range_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_policy_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_policy_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_premium_formula_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_premium_formula_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_product_field_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_product_field_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_product_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_product_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_product_version_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_product_version_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_status_transition_rule_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_update_status_transition_rule_response_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_uploaded_document_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_validate_product_factors_request_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      943 2024-04-24 19:13:36.000000 eis-insurance-1.31.0/test/test_withdraw_policy_response_class.py
```

### Comparing `eis-insurance-1.30.0/README.md` & `eis-insurance-1.31.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # eis-insurance
 The EMIL InsuranceService API description
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0
-- Package version: 1.30.0
+- Package version: 1.31.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.emil.de](https://www.emil.de)
 
 ## Requirements.
 
 Python >=3.6
 
@@ -110,14 +110,16 @@
 *InsuredObjectsApi* | [**delete_insured_object**](docs/InsuredObjectsApi.md#delete_insured_object) | **DELETE** /insuranceservice/v1/insured-objects/{id} | Delete the insured object
 *InsuredObjectsApi* | [**get_insured_object**](docs/InsuredObjectsApi.md#get_insured_object) | **GET** /insuranceservice/v1/insured-objects/{id} | Retrieve the insured object
 *InsuredObjectsApi* | [**list_insured_objects**](docs/InsuredObjectsApi.md#list_insured_objects) | **GET** /insuranceservice/v1/insured-objects | List insured objects
 *LeadStatusesApi* | [**create_lead_status**](docs/LeadStatusesApi.md#create_lead_status) | **POST** /insuranceservice/v1/lead-statuses | Create the lead status
 *LeadStatusesApi* | [**delete_lead_status**](docs/LeadStatusesApi.md#delete_lead_status) | **DELETE** /insuranceservice/v1/lead-statuses/{id} | Delete the lead status
 *LeadStatusesApi* | [**get_lead_status**](docs/LeadStatusesApi.md#get_lead_status) | **GET** /insuranceservice/v1/lead-statuses/{id} | Retrieve the lead status
 *LeadStatusesApi* | [**list_lead_statuses**](docs/LeadStatusesApi.md#list_lead_statuses) | **GET** /insuranceservice/v1/lead-statuses | List lead statuses
+*LeadVersionsApi* | [**get_lead_version**](docs/LeadVersionsApi.md#get_lead_version) | **GET** /insuranceservice/v1/leads/{code}/versions/{version} | Retrieve the lead version
+*LeadVersionsApi* | [**list_lead_versions**](docs/LeadVersionsApi.md#list_lead_versions) | **GET** /insuranceservice/v1/leads/{code}/versions | List lead versions
 *LeadsApi* | [**create_lead**](docs/LeadsApi.md#create_lead) | **POST** /insuranceservice/v1/leads | Create the lead
 *LeadsApi* | [**create_lead_async**](docs/LeadsApi.md#create_lead_async) | **POST** /insuranceservice/v1/leads-async | Create the lead asynchronously
 *LeadsApi* | [**create_lead_sync**](docs/LeadsApi.md#create_lead_sync) | **POST** /insuranceservice/v1/leads-sync | Create the lead
 *LeadsApi* | [**delete_lead**](docs/LeadsApi.md#delete_lead) | **DELETE** /insuranceservice/v1/leads/{code} | Delete the lead
 *LeadsApi* | [**get_lead**](docs/LeadsApi.md#get_lead) | **GET** /insuranceservice/v1/leads/{code} | Retrieve the lead
 *LeadsApi* | [**list_leads**](docs/LeadsApi.md#list_leads) | **GET** /insuranceservice/v1/leads | List leads
 *LeadsApi* | [**patch_lead**](docs/LeadsApi.md#patch_lead) | **PATCH** /insuranceservice/v1/leads/{code} | Patch the lead
@@ -160,14 +162,20 @@
 *ProductVersionsApi* | [**update_product_version**](docs/ProductVersionsApi.md#update_product_version) | **PUT** /insuranceservice/v1/product-versions/{id} | Update the product version
 *ProductsApi* | [**create_product**](docs/ProductsApi.md#create_product) | **POST** /insuranceservice/v1/products | Create the product
 *ProductsApi* | [**delete_product**](docs/ProductsApi.md#delete_product) | **DELETE** /insuranceservice/v1/products/{id} | Delete the product
 *ProductsApi* | [**get_product_by_code**](docs/ProductsApi.md#get_product_by_code) | **GET** /insuranceservice/v1/products/code/{code} | Retrieve the product
 *ProductsApi* | [**get_product_by_identifier**](docs/ProductsApi.md#get_product_by_identifier) | **GET** /insuranceservice/v1/products/get-by-identifier | Retrieve the product
 *ProductsApi* | [**list_products**](docs/ProductsApi.md#list_products) | **GET** /insuranceservice/v1/products | List products
 *ProductsApi* | [**update_product**](docs/ProductsApi.md#update_product) | **PUT** /insuranceservice/v1/products/{id} | Update the product
+*StatusTransitionRulesApi* | [**create_status_transition_rule**](docs/StatusTransitionRulesApi.md#create_status_transition_rule) | **POST** /insuranceservice/v1/status-transitions/rules | Create the status transition rule
+*StatusTransitionRulesApi* | [**delete_status_transition_rule**](docs/StatusTransitionRulesApi.md#delete_status_transition_rule) | **DELETE** /insuranceservice/v1/status-transitions/rules/{code} | Delete the status transition rule
+*StatusTransitionRulesApi* | [**get_status_transition_rule**](docs/StatusTransitionRulesApi.md#get_status_transition_rule) | **GET** /insuranceservice/v1/status-transitions/rules/{code} | Retrieve the status transition rule
+*StatusTransitionRulesApi* | [**list_status_transition_rules**](docs/StatusTransitionRulesApi.md#list_status_transition_rules) | **GET** /insuranceservice/v1/status-transitions/rules | List status transition rules
+*StatusTransitionRulesApi* | [**patch_status_transition_rule**](docs/StatusTransitionRulesApi.md#patch_status_transition_rule) | **PATCH** /insuranceservice/v1/status-transitions/rules/{code} | Patch the status transition rule
+*StatusTransitionRulesApi* | [**update_status_transition_rule**](docs/StatusTransitionRulesApi.md#update_status_transition_rule) | **PUT** /insuranceservice/v1/status-transitions/rules/{code} | Update the status transition rule
 *DefaultApi* | [**check**](docs/DefaultApi.md#check) | **GET** /insuranceservice/health | 
 
 
 ## Documentation For Models
 
  - [ActivatePolicyRequestDto](docs/ActivatePolicyRequestDto.md)
  - [ActivatePolicyResponseClass](docs/ActivatePolicyResponseClass.md)
@@ -195,21 +203,24 @@
  - [CreatePolicyResponseClass](docs/CreatePolicyResponseClass.md)
  - [CreatePremiumFormulaRequestDto](docs/CreatePremiumFormulaRequestDto.md)
  - [CreatePremiumFormulaResponseClass](docs/CreatePremiumFormulaResponseClass.md)
  - [CreateProductFieldRequestDto](docs/CreateProductFieldRequestDto.md)
  - [CreateProductFieldResponseClass](docs/CreateProductFieldResponseClass.md)
  - [CreateProductRequestDto](docs/CreateProductRequestDto.md)
  - [CreateProductResponseClass](docs/CreateProductResponseClass.md)
+ - [CreateStatusTransitionRuleRequestDto](docs/CreateStatusTransitionRuleRequestDto.md)
+ - [CreateStatusTransitionRuleResponseClass](docs/CreateStatusTransitionRuleResponseClass.md)
  - [CsvProductFactorDto](docs/CsvProductFactorDto.md)
- - [DeleteRequestDto](docs/DeleteRequestDto.md)
  - [DeleteResponseClass](docs/DeleteResponseClass.md)
  - [EmptyResponseClass](docs/EmptyResponseClass.md)
  - [GetInsuredObjectResponseClass](docs/GetInsuredObjectResponseClass.md)
  - [GetLeadResponseClass](docs/GetLeadResponseClass.md)
  - [GetLeadStatusResponseClass](docs/GetLeadStatusResponseClass.md)
+ - [GetLeadVersionRequestDto](docs/GetLeadVersionRequestDto.md)
+ - [GetLeadVersionResponseClass](docs/GetLeadVersionResponseClass.md)
  - [GetNamedRangeResponseClass](docs/GetNamedRangeResponseClass.md)
  - [GetPolicyDataByDateRequestDto](docs/GetPolicyDataByDateRequestDto.md)
  - [GetPolicyRequestDto](docs/GetPolicyRequestDto.md)
  - [GetPolicyResponseClass](docs/GetPolicyResponseClass.md)
  - [GetPremiumFormulaRequestDto](docs/GetPremiumFormulaRequestDto.md)
  - [GetPremiumFormulaResponseClass](docs/GetPremiumFormulaResponseClass.md)
  - [GetProductFactorResponseClass](docs/GetProductFactorResponseClass.md)
@@ -219,14 +230,15 @@
  - [GetProductFactorsForVersionResponseClass](docs/GetProductFactorsForVersionResponseClass.md)
  - [GetProductFieldRequestDto](docs/GetProductFieldRequestDto.md)
  - [GetProductFieldResponseClass](docs/GetProductFieldResponseClass.md)
  - [GetProductRequestDto](docs/GetProductRequestDto.md)
  - [GetProductResponseClass](docs/GetProductResponseClass.md)
  - [GetProductVersionRequestDto](docs/GetProductVersionRequestDto.md)
  - [GetProductVersionResponseClass](docs/GetProductVersionResponseClass.md)
+ - [GetStatusTransitionRuleResponseClass](docs/GetStatusTransitionRuleResponseClass.md)
  - [GroupedProductFactorClass](docs/GroupedProductFactorClass.md)
  - [GroupedProductFactorValueClass](docs/GroupedProductFactorValueClass.md)
  - [GroupedProductFactorsResponseClass](docs/GroupedProductFactorsResponseClass.md)
  - [GrpcPatchLeadRequestDto](docs/GrpcPatchLeadRequestDto.md)
  - [GrpcUpdateLeadRequestDto](docs/GrpcUpdateLeadRequestDto.md)
  - [InlineResponse200](docs/InlineResponse200.md)
  - [InlineResponse503](docs/InlineResponse503.md)
@@ -236,28 +248,32 @@
  - [InvoiceStatusClass](docs/InvoiceStatusClass.md)
  - [LeadBankAccountClass](docs/LeadBankAccountClass.md)
  - [LeadClass](docs/LeadClass.md)
  - [LeadStatusClass](docs/LeadStatusClass.md)
  - [ListInsuredObjectTypesResponseClass](docs/ListInsuredObjectTypesResponseClass.md)
  - [ListInsuredObjectsResponseClass](docs/ListInsuredObjectsResponseClass.md)
  - [ListLeadStatusesResponseClass](docs/ListLeadStatusesResponseClass.md)
+ - [ListLeadVersionsResponseClass](docs/ListLeadVersionsResponseClass.md)
  - [ListLeadsResponseClass](docs/ListLeadsResponseClass.md)
  - [ListNamedRangesResponseClass](docs/ListNamedRangesResponseClass.md)
  - [ListPoliciesResponseClass](docs/ListPoliciesResponseClass.md)
  - [ListPremiumFormulasResponseClass](docs/ListPremiumFormulasResponseClass.md)
  - [ListProductFactorsResponseClass](docs/ListProductFactorsResponseClass.md)
  - [ListProductFieldTypesResponseClass](docs/ListProductFieldTypesResponseClass.md)
  - [ListProductFieldsResponseClass](docs/ListProductFieldsResponseClass.md)
  - [ListProductsResponseClass](docs/ListProductsResponseClass.md)
  - [ListRequestDto](docs/ListRequestDto.md)
+ - [ListStatusTransitionRulesResponseClass](docs/ListStatusTransitionRulesResponseClass.md)
  - [NamedRangeClass](docs/NamedRangeClass.md)
  - [PatchLeadRequestDto](docs/PatchLeadRequestDto.md)
  - [PatchLeadResponseClass](docs/PatchLeadResponseClass.md)
  - [PatchPolicyRequestDto](docs/PatchPolicyRequestDto.md)
  - [PatchPolicyResponseClass](docs/PatchPolicyResponseClass.md)
+ - [PatchStatusTransitionRuleRequestDto](docs/PatchStatusTransitionRuleRequestDto.md)
+ - [PatchStatusTransitionRuleResponseClass](docs/PatchStatusTransitionRuleResponseClass.md)
  - [PolicyClass](docs/PolicyClass.md)
  - [PolicyObjectClass](docs/PolicyObjectClass.md)
  - [PolicyObjectDto](docs/PolicyObjectDto.md)
  - [PolicyPremiumClass](docs/PolicyPremiumClass.md)
  - [PolicyPremiumItemClass](docs/PolicyPremiumItemClass.md)
  - [PolicyVersionClass](docs/PolicyVersionClass.md)
  - [PremiumFormulaClass](docs/PremiumFormulaClass.md)
@@ -275,14 +291,15 @@
  - [SepaDto](docs/SepaDto.md)
  - [SharedCreateLeadPolicyRequestDto](docs/SharedCreateLeadPolicyRequestDto.md)
  - [SharedInvoiceClass](docs/SharedInvoiceClass.md)
  - [SharedLeadPolicyObjectDto](docs/SharedLeadPolicyObjectDto.md)
  - [SharedProductFieldClass](docs/SharedProductFieldClass.md)
  - [SharedUpdateNamedRangeRequestDto](docs/SharedUpdateNamedRangeRequestDto.md)
  - [SharedUpdatePremiumFormulaRequestDto](docs/SharedUpdatePremiumFormulaRequestDto.md)
+ - [StatusTransitionRuleClass](docs/StatusTransitionRuleClass.md)
  - [StoreProductFactorsRequestDto](docs/StoreProductFactorsRequestDto.md)
  - [StoreProductFactorsResponseClass](docs/StoreProductFactorsResponseClass.md)
  - [SuspendPolicyRequestDto](docs/SuspendPolicyRequestDto.md)
  - [SuspendPolicyResponseClass](docs/SuspendPolicyResponseClass.md)
  - [SwapPremiumFormulasOrderRequestDto](docs/SwapPremiumFormulasOrderRequestDto.md)
  - [TerminatePolicyRequestDto](docs/TerminatePolicyRequestDto.md)
  - [TerminatePolicyResponseClass](docs/TerminatePolicyResponseClass.md)
@@ -298,14 +315,16 @@
  - [UpdatePremiumFormulaResponseClass](docs/UpdatePremiumFormulaResponseClass.md)
  - [UpdateProductFieldRequestDto](docs/UpdateProductFieldRequestDto.md)
  - [UpdateProductFieldResponseClass](docs/UpdateProductFieldResponseClass.md)
  - [UpdateProductRequestDto](docs/UpdateProductRequestDto.md)
  - [UpdateProductResponseClass](docs/UpdateProductResponseClass.md)
  - [UpdateProductVersionRequestDto](docs/UpdateProductVersionRequestDto.md)
  - [UpdateProductVersionResponseClass](docs/UpdateProductVersionResponseClass.md)
+ - [UpdateStatusTransitionRuleRequestDto](docs/UpdateStatusTransitionRuleRequestDto.md)
+ - [UpdateStatusTransitionRuleResponseClass](docs/UpdateStatusTransitionRuleResponseClass.md)
  - [UploadedDocumentDto](docs/UploadedDocumentDto.md)
  - [ValidateProductFactorsRequestDto](docs/ValidateProductFactorsRequestDto.md)
  - [WithdrawPolicyResponseClass](docs/WithdrawPolicyResponseClass.md)
 
 
 ## Documentation For Authorization
```

### Comparing `eis-insurance-1.30.0/eis/insurance/__init__.py` & `eis-insurance-1.31.0/eis/insurance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.30.0"
+__version__ = "1.31.0"
 
 # import ApiClient
 from eis.insurance.api_client import ApiClient
 
 # import Configuration
 from eis.insurance.configuration import Configuration
```

### Comparing `eis-insurance-1.30.0/eis/insurance/api/default_api.py` & `eis-insurance-1.31.0/eis/insurance/api/default_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/insured_object_types_api.py` & `eis-insurance-1.31.0/eis/insurance/api/insured_object_types_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/insured_objects_api.py` & `eis-insurance-1.31.0/eis/insurance/api/insured_objects_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/lead_statuses_api.py` & `eis-insurance-1.31.0/eis/insurance/api/lead_statuses_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/leads_api.py` & `eis-insurance-1.31.0/eis/insurance/api/leads_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/named_ranges_api.py` & `eis-insurance-1.31.0/eis/insurance/api/named_ranges_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/policies_api.py` & `eis-insurance-1.31.0/eis/insurance/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/premium_formulas_api.py` & `eis-insurance-1.31.0/eis/insurance/api/premium_formulas_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/product_factors_api.py` & `eis-insurance-1.31.0/eis/insurance/api/product_factors_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/product_fields_api.py` & `eis-insurance-1.31.0/eis/insurance/api/product_fields_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/product_versions_api.py` & `eis-insurance-1.31.0/eis/insurance/api/product_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api/products_api.py` & `eis-insurance-1.31.0/eis/insurance/api/products_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/api_client.py` & `eis-insurance-1.31.0/eis/insurance/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.30.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.31.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `eis-insurance-1.30.0/eis/insurance/apis/__init__.py` & `eis-insurance-1.31.0/eis/insurance/apis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from eis.insurance.api.insured_object_types_api import InsuredObjectTypesApi
 from eis.insurance.api.insured_objects_api import InsuredObjectsApi
 from eis.insurance.api.lead_statuses_api import LeadStatusesApi
+from eis.insurance.api.lead_versions_api import LeadVersionsApi
 from eis.insurance.api.leads_api import LeadsApi
 from eis.insurance.api.named_ranges_api import NamedRangesApi
 from eis.insurance.api.policies_api import PoliciesApi
 from eis.insurance.api.premium_formulas_api import PremiumFormulasApi
 from eis.insurance.api.product_factors_api import ProductFactorsApi
 from eis.insurance.api.product_fields_api import ProductFieldsApi
 from eis.insurance.api.product_versions_api import ProductVersionsApi
 from eis.insurance.api.products_api import ProductsApi
+from eis.insurance.api.status_transition_rules_api import StatusTransitionRulesApi
 from eis.insurance.api.default_api import DefaultApi
```

### Comparing `eis-insurance-1.30.0/eis/insurance/configuration.py` & `eis-insurance-1.31.0/eis/insurance/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.30.0".\
+               "SDK Package Version: 1.31.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `eis-insurance-1.30.0/eis/insurance/exceptions.py` & `eis-insurance-1.31.0/eis/insurance/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/activate_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/activate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/activate_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/activate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/calculate_custom_premium_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/calculate_custom_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/calculate_premium_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/calculate_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/calculate_product_fields_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/calculate_product_fields_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/clone_product_version_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/clone_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_account_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_bank_account_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_custom_application_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_dummy_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_dummy_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_insured_object_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_insured_object_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_lead_async_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_lead_async_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_lead_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_lead_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_lead_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_lead_status_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_lead_status_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_lead_status_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_named_range_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_named_range_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_named_request_s3_data_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_named_request_s3_data_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_payment_method_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_payment_method_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_product_field_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_product_field_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_product_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/create_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/create_product_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/create_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/csv_product_factor_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/csv_product_factor_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/delete_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_field_request_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 
-class DeleteRequestDto(ModelNormal):
+class GetProductFieldRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -98,18 +98,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """DeleteRequestDto - a model defined in OpenAPI
+        """GetProductFieldRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Resource id.
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -187,18 +187,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """DeleteRequestDto - a model defined in OpenAPI
+        """GetProductFieldRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Resource id.
+            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `eis-insurance-1.30.0/eis/insurance/model/delete_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/empty_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/empty_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_insured_object_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_lead_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_lead_status_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_named_range_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_policy_data_by_date_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_policy_data_by_date_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_factor_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_factor_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_factor_value_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_factor_value_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_factors_for_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_factors_for_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_field_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_lead_version_request_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 
-class GetProductFieldRequestDto(ModelNormal):
+class GetLeadVersionRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (float,),  # noqa: E501
+            'code': (str,),  # noqa: E501
+            'version': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
+        'code': 'code',  # noqa: E501
+        'version': 'version',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """GetProductFieldRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, code, version, *args, **kwargs):  # noqa: E501
+        """GetLeadVersionRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str):
+            version (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +168,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
+        self.code = code
+        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """GetProductFieldRequestDto - a model defined in OpenAPI
+    def __init__(self, code, version, *args, **kwargs):  # noqa: E501
+        """GetLeadVersionRequestDto - a model defined in OpenAPI
 
         Args:
-            id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
+            code (str):
+            version (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +257,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
+        self.code = code
+        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_field_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_version_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/get_product_version_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/get_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_class.py` & `eis-insurance-1.31.0/eis/insurance/model/grouped_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_value_class.py` & `eis-insurance-1.31.0/eis/insurance/model/grouped_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/grouped_product_factors_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/grouped_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/grpc_patch_lead_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/grpc_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/grpc_update_lead_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/grpc_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/inline_response200.py` & `eis-insurance-1.31.0/eis/insurance/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/inline_response503.py` & `eis-insurance-1.31.0/eis/insurance/model/inline_response503.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/insured_object_class.py` & `eis-insurance-1.31.0/eis/insurance/model/insured_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/insured_object_type_class.py` & `eis-insurance-1.31.0/eis/insurance/model/insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/invoice_item_class.py` & `eis-insurance-1.31.0/eis/insurance/model/invoice_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/invoice_status_class.py` & `eis-insurance-1.31.0/eis/insurance/model/invoice_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/lead_bank_account_class.py` & `eis-insurance-1.31.0/eis/insurance/model/lead_bank_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/lead_class.py` & `eis-insurance-1.31.0/eis/insurance/model/lead_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
             'bank_account': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'custom_data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'uploaded_document': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'premium_override': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'product_slug': (str,),  # noqa: E501
             'quote': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'payment_method': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'version': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -140,14 +141,15 @@
         'bank_account': 'bankAccount',  # noqa: E501
         'custom_data': 'customData',  # noqa: E501
         'uploaded_document': 'uploadedDocument',  # noqa: E501
         'premium_override': 'premiumOverride',  # noqa: E501
         'product_slug': 'productSlug',  # noqa: E501
         'quote': 'quote',  # noqa: E501
         'payment_method': 'paymentMethod',  # noqa: E501
+        'version': 'version',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -203,14 +205,15 @@
             bank_account (bool, date, datetime, dict, float, int, list, str, none_type): Lead bank account, will be treated as a reference to payout customer claims.. [optional]  # noqa: E501
             custom_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom data for custom application creation.. [optional]  # noqa: E501
             uploaded_document (bool, date, datetime, dict, float, int, list, str, none_type): List of uploaded document codes.. [optional]  # noqa: E501
             premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Override for premium calculation. Leave null for default calculation.. [optional]  # noqa: E501
             product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
             quote (bool, date, datetime, dict, float, int, list, str, none_type): Quote or price details.. [optional]  # noqa: E501
             payment_method (bool, date, datetime, dict, float, int, list, str, none_type): Payment method. When a payment method is provided, it needs to be handled in the workflow based on its type.. [optional]  # noqa: E501
+            version (float): Lead version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -318,14 +321,15 @@
             bank_account (bool, date, datetime, dict, float, int, list, str, none_type): Lead bank account, will be treated as a reference to payout customer claims.. [optional]  # noqa: E501
             custom_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Custom data for custom application creation.. [optional]  # noqa: E501
             uploaded_document (bool, date, datetime, dict, float, int, list, str, none_type): List of uploaded document codes.. [optional]  # noqa: E501
             premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Override for premium calculation. Leave null for default calculation.. [optional]  # noqa: E501
             product_slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.. [optional]  # noqa: E501
             quote (bool, date, datetime, dict, float, int, list, str, none_type): Quote or price details.. [optional]  # noqa: E501
             payment_method (bool, date, datetime, dict, float, int, list, str, none_type): Payment method. When a payment method is provided, it needs to be handled in the workflow based on its type.. [optional]  # noqa: E501
+            version (float): Lead version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `eis-insurance-1.30.0/eis/insurance/model/lead_status_class.py` & `eis-insurance-1.31.0/eis/insurance/model/lead_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_insured_object_types_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_insured_object_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_insured_objects_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_insured_objects_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_lead_statuses_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_lead_statuses_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_leads_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_leads_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_named_ranges_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_named_ranges_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_policies_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_policies_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_premium_formulas_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_premium_formulas_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_product_factors_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_product_field_types_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_product_field_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_product_fields_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_product_fields_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_products_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/list_products_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/list_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/named_range_class.py` & `eis-insurance-1.31.0/eis/insurance/model/named_range_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/patch_lead_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/patch_lead_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/patch_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/patch_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/patch_policy_request_dto.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,27 +91,29 @@
         lazy_import()
         return {
             'policy_objects': ([PolicyObjectDto],),  # noqa: E501
             '_from': (datetime,),  # noqa: E501
             'to': (datetime,),  # noqa: E501
             'premium_override': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'policy_number': (str,),  # noqa: E501
+            'reason': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'policy_objects': 'policyObjects',  # noqa: E501
         '_from': 'from',  # noqa: E501
         'to': 'to',  # noqa: E501
         'premium_override': 'premiumOverride',  # noqa: E501
         'policy_number': 'policyNumber',  # noqa: E501
+        'reason': 'reason',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -154,14 +156,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             to (datetime): Date to which the policy should be updated. This will create a new timeline finishing at this date.. [optional]  # noqa: E501
             premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Premium Override. [optional]  # noqa: E501
             policy_number (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
+            reason (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -248,14 +251,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             to (datetime): Date to which the policy should be updated. This will create a new timeline finishing at this date.. [optional]  # noqa: E501
             premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Premium Override. [optional]  # noqa: E501
             policy_number (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
+            reason (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `eis-insurance-1.30.0/eis/insurance/model/patch_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/patch_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/policy_class.py` & `eis-insurance-1.31.0/eis/insurance/model/policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/policy_object_class.py` & `eis-insurance-1.31.0/eis/insurance/model/policy_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/policy_object_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/policy_premium_class.py` & `eis-insurance-1.31.0/eis/insurance/model/policy_premium_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/policy_premium_item_class.py` & `eis-insurance-1.31.0/eis/insurance/model/policy_premium_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/policy_version_class.py` & `eis-insurance-1.31.0/eis/insurance/model/policy_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/premium_formula_class.py` & `eis-insurance-1.31.0/eis/insurance/model/premium_formula_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/premium_override_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/premium_override_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/premium_override_request_class.py` & `eis-insurance-1.31.0/eis/insurance/model/premium_override_request_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/premium_override_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/premium_override_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_factor_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_factor_for_version_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_factor_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_factor_value_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_factor_value_for_version_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_factor_value_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_field_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_field_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,19 @@
             'is_required': (bool,),  # noqa: E501
             'is_hidden': (bool,),  # noqa: E501
             'is_hidden_customer_portal': (bool,),  # noqa: E501
             'is_editable_customer_portal': (bool,),  # noqa: E501
             'is_system': (bool,),  # noqa: E501
             'is_unique': (bool,),  # noqa: E501
             'default_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'expression': (str, none_type,),  # noqa: E501
             'min_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'max_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'updated_at': (datetime,),  # noqa: E501
+            'expression': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -119,29 +119,29 @@
         'is_required': 'isRequired',  # noqa: E501
         'is_hidden': 'isHidden',  # noqa: E501
         'is_hidden_customer_portal': 'isHiddenCustomerPortal',  # noqa: E501
         'is_editable_customer_portal': 'isEditableCustomerPortal',  # noqa: E501
         'is_system': 'isSystem',  # noqa: E501
         'is_unique': 'isUnique',  # noqa: E501
         'default_value': 'defaultValue',  # noqa: E501
-        'expression': 'expression',  # noqa: E501
         'min_value': 'minValue',  # noqa: E501
         'max_value': 'maxValue',  # noqa: E501
         'created_at': 'createdAt',  # noqa: E501
         'updated_at': 'updatedAt',  # noqa: E501
+        'expression': 'expression',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, expression, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
         """ProductFieldClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             name (str): Product field name.
             group (str): Product field group.
             label (str): Product field label.
@@ -151,15 +151,14 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -188,14 +187,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            expression (str, none_type): Expression to calculate the field.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -233,15 +233,14 @@
         self.is_required = is_required
         self.is_hidden = is_hidden
         self.is_hidden_customer_portal = is_hidden_customer_portal
         self.is_editable_customer_portal = is_editable_customer_portal
         self.is_system = is_system
         self.is_unique = is_unique
         self.default_value = default_value
-        self.expression = expression
         self.min_value = min_value
         self.max_value = max_value
         self.created_at = created_at
         self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
@@ -258,15 +257,15 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, expression, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
         """ProductFieldClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             name (str): Product field name.
             group (str): Product field group.
             label (str): Product field label.
@@ -276,15 +275,14 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -313,14 +311,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            expression (str, none_type): Expression to calculate the field.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -356,15 +355,14 @@
         self.is_required = is_required
         self.is_hidden = is_hidden
         self.is_hidden_customer_portal = is_hidden_customer_portal
         self.is_editable_customer_portal = is_editable_customer_portal
         self.is_system = is_system
         self.is_unique = is_unique
         self.default_value = default_value
-        self.expression = expression
         self.min_value = min_value
         self.max_value = max_value
         self.created_at = created_at
         self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
```

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_field_type_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_field_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/product_version_class.py` & `eis-insurance-1.31.0/eis/insurance/model/product_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/sepa_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/sepa_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/shared_create_lead_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/shared_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/shared_invoice_class.py` & `eis-insurance-1.31.0/eis/insurance/model/shared_invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/shared_lead_policy_object_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/shared_lead_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/shared_product_field_class.py` & `eis-insurance-1.31.0/eis/insurance/model/shared_product_field_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,19 @@
             'is_required': (bool,),  # noqa: E501
             'is_hidden': (bool,),  # noqa: E501
             'is_hidden_customer_portal': (bool,),  # noqa: E501
             'is_editable_customer_portal': (bool,),  # noqa: E501
             'is_system': (bool,),  # noqa: E501
             'is_unique': (bool,),  # noqa: E501
             'default_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'expression': (str, none_type,),  # noqa: E501
             'min_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'max_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'updated_at': (datetime,),  # noqa: E501
+            'expression': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -119,29 +119,29 @@
         'is_required': 'isRequired',  # noqa: E501
         'is_hidden': 'isHidden',  # noqa: E501
         'is_hidden_customer_portal': 'isHiddenCustomerPortal',  # noqa: E501
         'is_editable_customer_portal': 'isEditableCustomerPortal',  # noqa: E501
         'is_system': 'isSystem',  # noqa: E501
         'is_unique': 'isUnique',  # noqa: E501
         'default_value': 'defaultValue',  # noqa: E501
-        'expression': 'expression',  # noqa: E501
         'min_value': 'minValue',  # noqa: E501
         'max_value': 'maxValue',  # noqa: E501
         'created_at': 'createdAt',  # noqa: E501
         'updated_at': 'updatedAt',  # noqa: E501
+        'expression': 'expression',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, expression, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
         """SharedProductFieldClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             name (str): Product field name.
             group (str): Product field group.
             label (str): Product field label.
@@ -151,15 +151,14 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -188,14 +187,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            expression (str, none_type): Expression to calculate the field.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -233,15 +233,14 @@
         self.is_required = is_required
         self.is_hidden = is_hidden
         self.is_hidden_customer_portal = is_hidden_customer_portal
         self.is_editable_customer_portal = is_editable_customer_portal
         self.is_system = is_system
         self.is_unique = is_unique
         self.default_value = default_value
-        self.expression = expression
         self.min_value = min_value
         self.max_value = max_value
         self.created_at = created_at
         self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
@@ -258,15 +257,15 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, expression, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, name, group, label, type_entity, type_id, insured_object_id, is_required, is_hidden, is_hidden_customer_portal, is_editable_customer_portal, is_system, is_unique, default_value, min_value, max_value, created_at, updated_at, *args, **kwargs):  # noqa: E501
         """SharedProductFieldClass - a model defined in OpenAPI
 
         Args:
             id (float): Internal unique identifier for the object. You should not have to use this, use code instead.
             name (str): Product field name.
             group (str): Product field group.
             label (str): Product field label.
@@ -276,15 +275,14 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -313,14 +311,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            expression (str, none_type): Expression to calculate the field.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -356,15 +355,14 @@
         self.is_required = is_required
         self.is_hidden = is_hidden
         self.is_hidden_customer_portal = is_hidden_customer_portal
         self.is_editable_customer_portal = is_editable_customer_portal
         self.is_system = is_system
         self.is_unique = is_unique
         self.default_value = default_value
-        self.expression = expression
         self.min_value = min_value
         self.max_value = max_value
         self.created_at = created_at
         self.updated_at = updated_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
```

### Comparing `eis-insurance-1.30.0/eis/insurance/model/shared_update_named_range_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/shared_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/shared_update_premium_formula_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/shared_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/store_product_factors_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/store_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/store_product_factors_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/store_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/suspend_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/suspend_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/suspend_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/suspend_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/terminate_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/terminate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/terminate_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/terminate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/timeslice_class.py` & `eis-insurance-1.31.0/eis/insurance/model/timeslice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_insured_object_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_lead_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_lead_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/update_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_named_range_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_named_range_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/update_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_policy_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/update_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/update_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_product_field_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_product_field_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/update_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_product_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_product_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/update_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_product_version_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/update_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/update_product_version_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/update_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/uploaded_document_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/uploaded_document_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/validate_product_factors_request_dto.py` & `eis-insurance-1.31.0/eis/insurance/model/validate_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model/withdraw_policy_response_class.py` & `eis-insurance-1.31.0/eis/insurance/model/withdraw_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/model_utils.py` & `eis-insurance-1.31.0/eis/insurance/model_utils.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis/insurance/models/__init__.py` & `eis-insurance-1.31.0/eis/insurance/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,21 +35,24 @@
 from eis.insurance.model.create_policy_response_class import CreatePolicyResponseClass
 from eis.insurance.model.create_premium_formula_request_dto import CreatePremiumFormulaRequestDto
 from eis.insurance.model.create_premium_formula_response_class import CreatePremiumFormulaResponseClass
 from eis.insurance.model.create_product_field_request_dto import CreateProductFieldRequestDto
 from eis.insurance.model.create_product_field_response_class import CreateProductFieldResponseClass
 from eis.insurance.model.create_product_request_dto import CreateProductRequestDto
 from eis.insurance.model.create_product_response_class import CreateProductResponseClass
+from eis.insurance.model.create_status_transition_rule_request_dto import CreateStatusTransitionRuleRequestDto
+from eis.insurance.model.create_status_transition_rule_response_class import CreateStatusTransitionRuleResponseClass
 from eis.insurance.model.csv_product_factor_dto import CsvProductFactorDto
-from eis.insurance.model.delete_request_dto import DeleteRequestDto
 from eis.insurance.model.delete_response_class import DeleteResponseClass
 from eis.insurance.model.empty_response_class import EmptyResponseClass
 from eis.insurance.model.get_insured_object_response_class import GetInsuredObjectResponseClass
 from eis.insurance.model.get_lead_response_class import GetLeadResponseClass
 from eis.insurance.model.get_lead_status_response_class import GetLeadStatusResponseClass
+from eis.insurance.model.get_lead_version_request_dto import GetLeadVersionRequestDto
+from eis.insurance.model.get_lead_version_response_class import GetLeadVersionResponseClass
 from eis.insurance.model.get_named_range_response_class import GetNamedRangeResponseClass
 from eis.insurance.model.get_policy_data_by_date_request_dto import GetPolicyDataByDateRequestDto
 from eis.insurance.model.get_policy_request_dto import GetPolicyRequestDto
 from eis.insurance.model.get_policy_response_class import GetPolicyResponseClass
 from eis.insurance.model.get_premium_formula_request_dto import GetPremiumFormulaRequestDto
 from eis.insurance.model.get_premium_formula_response_class import GetPremiumFormulaResponseClass
 from eis.insurance.model.get_product_factor_response_class import GetProductFactorResponseClass
@@ -59,14 +62,15 @@
 from eis.insurance.model.get_product_factors_for_version_response_class import GetProductFactorsForVersionResponseClass
 from eis.insurance.model.get_product_field_request_dto import GetProductFieldRequestDto
 from eis.insurance.model.get_product_field_response_class import GetProductFieldResponseClass
 from eis.insurance.model.get_product_request_dto import GetProductRequestDto
 from eis.insurance.model.get_product_response_class import GetProductResponseClass
 from eis.insurance.model.get_product_version_request_dto import GetProductVersionRequestDto
 from eis.insurance.model.get_product_version_response_class import GetProductVersionResponseClass
+from eis.insurance.model.get_status_transition_rule_response_class import GetStatusTransitionRuleResponseClass
 from eis.insurance.model.grouped_product_factor_class import GroupedProductFactorClass
 from eis.insurance.model.grouped_product_factor_value_class import GroupedProductFactorValueClass
 from eis.insurance.model.grouped_product_factors_response_class import GroupedProductFactorsResponseClass
 from eis.insurance.model.grpc_patch_lead_request_dto import GrpcPatchLeadRequestDto
 from eis.insurance.model.grpc_update_lead_request_dto import GrpcUpdateLeadRequestDto
 from eis.insurance.model.inline_response200 import InlineResponse200
 from eis.insurance.model.inline_response503 import InlineResponse503
@@ -76,28 +80,32 @@
 from eis.insurance.model.invoice_status_class import InvoiceStatusClass
 from eis.insurance.model.lead_bank_account_class import LeadBankAccountClass
 from eis.insurance.model.lead_class import LeadClass
 from eis.insurance.model.lead_status_class import LeadStatusClass
 from eis.insurance.model.list_insured_object_types_response_class import ListInsuredObjectTypesResponseClass
 from eis.insurance.model.list_insured_objects_response_class import ListInsuredObjectsResponseClass
 from eis.insurance.model.list_lead_statuses_response_class import ListLeadStatusesResponseClass
+from eis.insurance.model.list_lead_versions_response_class import ListLeadVersionsResponseClass
 from eis.insurance.model.list_leads_response_class import ListLeadsResponseClass
 from eis.insurance.model.list_named_ranges_response_class import ListNamedRangesResponseClass
 from eis.insurance.model.list_policies_response_class import ListPoliciesResponseClass
 from eis.insurance.model.list_premium_formulas_response_class import ListPremiumFormulasResponseClass
 from eis.insurance.model.list_product_factors_response_class import ListProductFactorsResponseClass
 from eis.insurance.model.list_product_field_types_response_class import ListProductFieldTypesResponseClass
 from eis.insurance.model.list_product_fields_response_class import ListProductFieldsResponseClass
 from eis.insurance.model.list_products_response_class import ListProductsResponseClass
 from eis.insurance.model.list_request_dto import ListRequestDto
+from eis.insurance.model.list_status_transition_rules_response_class import ListStatusTransitionRulesResponseClass
 from eis.insurance.model.named_range_class import NamedRangeClass
 from eis.insurance.model.patch_lead_request_dto import PatchLeadRequestDto
 from eis.insurance.model.patch_lead_response_class import PatchLeadResponseClass
 from eis.insurance.model.patch_policy_request_dto import PatchPolicyRequestDto
 from eis.insurance.model.patch_policy_response_class import PatchPolicyResponseClass
+from eis.insurance.model.patch_status_transition_rule_request_dto import PatchStatusTransitionRuleRequestDto
+from eis.insurance.model.patch_status_transition_rule_response_class import PatchStatusTransitionRuleResponseClass
 from eis.insurance.model.policy_class import PolicyClass
 from eis.insurance.model.policy_object_class import PolicyObjectClass
 from eis.insurance.model.policy_object_dto import PolicyObjectDto
 from eis.insurance.model.policy_premium_class import PolicyPremiumClass
 from eis.insurance.model.policy_premium_item_class import PolicyPremiumItemClass
 from eis.insurance.model.policy_version_class import PolicyVersionClass
 from eis.insurance.model.premium_formula_class import PremiumFormulaClass
@@ -115,14 +123,15 @@
 from eis.insurance.model.sepa_dto import SepaDto
 from eis.insurance.model.shared_create_lead_policy_request_dto import SharedCreateLeadPolicyRequestDto
 from eis.insurance.model.shared_invoice_class import SharedInvoiceClass
 from eis.insurance.model.shared_lead_policy_object_dto import SharedLeadPolicyObjectDto
 from eis.insurance.model.shared_product_field_class import SharedProductFieldClass
 from eis.insurance.model.shared_update_named_range_request_dto import SharedUpdateNamedRangeRequestDto
 from eis.insurance.model.shared_update_premium_formula_request_dto import SharedUpdatePremiumFormulaRequestDto
+from eis.insurance.model.status_transition_rule_class import StatusTransitionRuleClass
 from eis.insurance.model.store_product_factors_request_dto import StoreProductFactorsRequestDto
 from eis.insurance.model.store_product_factors_response_class import StoreProductFactorsResponseClass
 from eis.insurance.model.suspend_policy_request_dto import SuspendPolicyRequestDto
 from eis.insurance.model.suspend_policy_response_class import SuspendPolicyResponseClass
 from eis.insurance.model.swap_premium_formulas_order_request_dto import SwapPremiumFormulasOrderRequestDto
 from eis.insurance.model.terminate_policy_request_dto import TerminatePolicyRequestDto
 from eis.insurance.model.terminate_policy_response_class import TerminatePolicyResponseClass
@@ -138,10 +147,12 @@
 from eis.insurance.model.update_premium_formula_response_class import UpdatePremiumFormulaResponseClass
 from eis.insurance.model.update_product_field_request_dto import UpdateProductFieldRequestDto
 from eis.insurance.model.update_product_field_response_class import UpdateProductFieldResponseClass
 from eis.insurance.model.update_product_request_dto import UpdateProductRequestDto
 from eis.insurance.model.update_product_response_class import UpdateProductResponseClass
 from eis.insurance.model.update_product_version_request_dto import UpdateProductVersionRequestDto
 from eis.insurance.model.update_product_version_response_class import UpdateProductVersionResponseClass
+from eis.insurance.model.update_status_transition_rule_request_dto import UpdateStatusTransitionRuleRequestDto
+from eis.insurance.model.update_status_transition_rule_response_class import UpdateStatusTransitionRuleResponseClass
 from eis.insurance.model.uploaded_document_dto import UploadedDocumentDto
 from eis.insurance.model.validate_product_factors_request_dto import ValidateProductFactorsRequestDto
 from eis.insurance.model.withdraw_policy_response_class import WithdrawPolicyResponseClass
```

### Comparing `eis-insurance-1.30.0/eis/insurance/rest.py` & `eis-insurance-1.31.0/eis/insurance/rest.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/eis_insurance.egg-info/SOURCES.txt` & `eis-insurance-1.31.0/eis_insurance.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 eis/insurance/model_utils.py
 eis/insurance/rest.py
 eis/insurance/api/__init__.py
 eis/insurance/api/default_api.py
 eis/insurance/api/insured_object_types_api.py
 eis/insurance/api/insured_objects_api.py
 eis/insurance/api/lead_statuses_api.py
+eis/insurance/api/lead_versions_api.py
 eis/insurance/api/leads_api.py
 eis/insurance/api/named_ranges_api.py
 eis/insurance/api/policies_api.py
 eis/insurance/api/premium_formulas_api.py
 eis/insurance/api/product_factors_api.py
 eis/insurance/api/product_fields_api.py
 eis/insurance/api/product_versions_api.py
 eis/insurance/api/products_api.py
+eis/insurance/api/status_transition_rules_api.py
 eis/insurance/apis/__init__.py
 eis/insurance/model/__init__.py
 eis/insurance/model/activate_policy_request_dto.py
 eis/insurance/model/activate_policy_response_class.py
 eis/insurance/model/calculate_custom_premium_request_dto.py
 eis/insurance/model/calculate_premium_request_dto.py
 eis/insurance/model/calculate_product_fields_request_dto.py
@@ -49,21 +51,24 @@
 eis/insurance/model/create_policy_response_class.py
 eis/insurance/model/create_premium_formula_request_dto.py
 eis/insurance/model/create_premium_formula_response_class.py
 eis/insurance/model/create_product_field_request_dto.py
 eis/insurance/model/create_product_field_response_class.py
 eis/insurance/model/create_product_request_dto.py
 eis/insurance/model/create_product_response_class.py
+eis/insurance/model/create_status_transition_rule_request_dto.py
+eis/insurance/model/create_status_transition_rule_response_class.py
 eis/insurance/model/csv_product_factor_dto.py
-eis/insurance/model/delete_request_dto.py
 eis/insurance/model/delete_response_class.py
 eis/insurance/model/empty_response_class.py
 eis/insurance/model/get_insured_object_response_class.py
 eis/insurance/model/get_lead_response_class.py
 eis/insurance/model/get_lead_status_response_class.py
+eis/insurance/model/get_lead_version_request_dto.py
+eis/insurance/model/get_lead_version_response_class.py
 eis/insurance/model/get_named_range_response_class.py
 eis/insurance/model/get_policy_data_by_date_request_dto.py
 eis/insurance/model/get_policy_request_dto.py
 eis/insurance/model/get_policy_response_class.py
 eis/insurance/model/get_premium_formula_request_dto.py
 eis/insurance/model/get_premium_formula_response_class.py
 eis/insurance/model/get_product_factor_response_class.py
@@ -73,14 +78,15 @@
 eis/insurance/model/get_product_factors_for_version_response_class.py
 eis/insurance/model/get_product_field_request_dto.py
 eis/insurance/model/get_product_field_response_class.py
 eis/insurance/model/get_product_request_dto.py
 eis/insurance/model/get_product_response_class.py
 eis/insurance/model/get_product_version_request_dto.py
 eis/insurance/model/get_product_version_response_class.py
+eis/insurance/model/get_status_transition_rule_response_class.py
 eis/insurance/model/grouped_product_factor_class.py
 eis/insurance/model/grouped_product_factor_value_class.py
 eis/insurance/model/grouped_product_factors_response_class.py
 eis/insurance/model/grpc_patch_lead_request_dto.py
 eis/insurance/model/grpc_update_lead_request_dto.py
 eis/insurance/model/inline_response200.py
 eis/insurance/model/inline_response503.py
@@ -90,28 +96,32 @@
 eis/insurance/model/invoice_status_class.py
 eis/insurance/model/lead_bank_account_class.py
 eis/insurance/model/lead_class.py
 eis/insurance/model/lead_status_class.py
 eis/insurance/model/list_insured_object_types_response_class.py
 eis/insurance/model/list_insured_objects_response_class.py
 eis/insurance/model/list_lead_statuses_response_class.py
+eis/insurance/model/list_lead_versions_response_class.py
 eis/insurance/model/list_leads_response_class.py
 eis/insurance/model/list_named_ranges_response_class.py
 eis/insurance/model/list_policies_response_class.py
 eis/insurance/model/list_premium_formulas_response_class.py
 eis/insurance/model/list_product_factors_response_class.py
 eis/insurance/model/list_product_field_types_response_class.py
 eis/insurance/model/list_product_fields_response_class.py
 eis/insurance/model/list_products_response_class.py
 eis/insurance/model/list_request_dto.py
+eis/insurance/model/list_status_transition_rules_response_class.py
 eis/insurance/model/named_range_class.py
 eis/insurance/model/patch_lead_request_dto.py
 eis/insurance/model/patch_lead_response_class.py
 eis/insurance/model/patch_policy_request_dto.py
 eis/insurance/model/patch_policy_response_class.py
+eis/insurance/model/patch_status_transition_rule_request_dto.py
+eis/insurance/model/patch_status_transition_rule_response_class.py
 eis/insurance/model/policy_class.py
 eis/insurance/model/policy_object_class.py
 eis/insurance/model/policy_object_dto.py
 eis/insurance/model/policy_premium_class.py
 eis/insurance/model/policy_premium_item_class.py
 eis/insurance/model/policy_version_class.py
 eis/insurance/model/premium_formula_class.py
@@ -129,14 +139,15 @@
 eis/insurance/model/sepa_dto.py
 eis/insurance/model/shared_create_lead_policy_request_dto.py
 eis/insurance/model/shared_invoice_class.py
 eis/insurance/model/shared_lead_policy_object_dto.py
 eis/insurance/model/shared_product_field_class.py
 eis/insurance/model/shared_update_named_range_request_dto.py
 eis/insurance/model/shared_update_premium_formula_request_dto.py
+eis/insurance/model/status_transition_rule_class.py
 eis/insurance/model/store_product_factors_request_dto.py
 eis/insurance/model/store_product_factors_response_class.py
 eis/insurance/model/suspend_policy_request_dto.py
 eis/insurance/model/suspend_policy_response_class.py
 eis/insurance/model/swap_premium_formulas_order_request_dto.py
 eis/insurance/model/terminate_policy_request_dto.py
 eis/insurance/model/terminate_policy_response_class.py
@@ -152,14 +163,16 @@
 eis/insurance/model/update_premium_formula_response_class.py
 eis/insurance/model/update_product_field_request_dto.py
 eis/insurance/model/update_product_field_response_class.py
 eis/insurance/model/update_product_request_dto.py
 eis/insurance/model/update_product_response_class.py
 eis/insurance/model/update_product_version_request_dto.py
 eis/insurance/model/update_product_version_response_class.py
+eis/insurance/model/update_status_transition_rule_request_dto.py
+eis/insurance/model/update_status_transition_rule_response_class.py
 eis/insurance/model/uploaded_document_dto.py
 eis/insurance/model/validate_product_factors_request_dto.py
 eis/insurance/model/withdraw_policy_response_class.py
 eis/insurance/models/__init__.py
 eis_insurance.egg-info/PKG-INFO
 eis_insurance.egg-info/SOURCES.txt
 eis_insurance.egg-info/dependency_links.txt
@@ -191,22 +204,25 @@
 test/test_create_policy_response_class.py
 test/test_create_premium_formula_request_dto.py
 test/test_create_premium_formula_response_class.py
 test/test_create_product_field_request_dto.py
 test/test_create_product_field_response_class.py
 test/test_create_product_request_dto.py
 test/test_create_product_response_class.py
+test/test_create_status_transition_rule_request_dto.py
+test/test_create_status_transition_rule_response_class.py
 test/test_csv_product_factor_dto.py
 test/test_default_api.py
-test/test_delete_request_dto.py
 test/test_delete_response_class.py
 test/test_empty_response_class.py
 test/test_get_insured_object_response_class.py
 test/test_get_lead_response_class.py
 test/test_get_lead_status_response_class.py
+test/test_get_lead_version_request_dto.py
+test/test_get_lead_version_response_class.py
 test/test_get_named_range_response_class.py
 test/test_get_policy_data_by_date_request_dto.py
 test/test_get_policy_request_dto.py
 test/test_get_policy_response_class.py
 test/test_get_premium_formula_request_dto.py
 test/test_get_premium_formula_response_class.py
 test/test_get_product_factor_response_class.py
@@ -216,14 +232,15 @@
 test/test_get_product_factors_for_version_response_class.py
 test/test_get_product_field_request_dto.py
 test/test_get_product_field_response_class.py
 test/test_get_product_request_dto.py
 test/test_get_product_response_class.py
 test/test_get_product_version_request_dto.py
 test/test_get_product_version_response_class.py
+test/test_get_status_transition_rule_response_class.py
 test/test_grouped_product_factor_class.py
 test/test_grouped_product_factor_value_class.py
 test/test_grouped_product_factors_response_class.py
 test/test_grpc_patch_lead_request_dto.py
 test/test_grpc_update_lead_request_dto.py
 test/test_inline_response200.py
 test/test_inline_response503.py
@@ -233,33 +250,38 @@
 test/test_insured_objects_api.py
 test/test_invoice_item_class.py
 test/test_invoice_status_class.py
 test/test_lead_bank_account_class.py
 test/test_lead_class.py
 test/test_lead_status_class.py
 test/test_lead_statuses_api.py
+test/test_lead_versions_api.py
 test/test_leads_api.py
 test/test_list_insured_object_types_response_class.py
 test/test_list_insured_objects_response_class.py
 test/test_list_lead_statuses_response_class.py
+test/test_list_lead_versions_response_class.py
 test/test_list_leads_response_class.py
 test/test_list_named_ranges_response_class.py
 test/test_list_policies_response_class.py
 test/test_list_premium_formulas_response_class.py
 test/test_list_product_factors_response_class.py
 test/test_list_product_field_types_response_class.py
 test/test_list_product_fields_response_class.py
 test/test_list_products_response_class.py
 test/test_list_request_dto.py
+test/test_list_status_transition_rules_response_class.py
 test/test_named_range_class.py
 test/test_named_ranges_api.py
 test/test_patch_lead_request_dto.py
 test/test_patch_lead_response_class.py
 test/test_patch_policy_request_dto.py
 test/test_patch_policy_response_class.py
+test/test_patch_status_transition_rule_request_dto.py
+test/test_patch_status_transition_rule_response_class.py
 test/test_policies_api.py
 test/test_policy_class.py
 test/test_policy_object_class.py
 test/test_policy_object_dto.py
 test/test_policy_premium_class.py
 test/test_policy_premium_item_class.py
 test/test_policy_version_class.py
@@ -283,14 +305,16 @@
 test/test_sepa_dto.py
 test/test_shared_create_lead_policy_request_dto.py
 test/test_shared_invoice_class.py
 test/test_shared_lead_policy_object_dto.py
 test/test_shared_product_field_class.py
 test/test_shared_update_named_range_request_dto.py
 test/test_shared_update_premium_formula_request_dto.py
+test/test_status_transition_rule_class.py
+test/test_status_transition_rules_api.py
 test/test_store_product_factors_request_dto.py
 test/test_store_product_factors_response_class.py
 test/test_suspend_policy_request_dto.py
 test/test_suspend_policy_response_class.py
 test/test_swap_premium_formulas_order_request_dto.py
 test/test_terminate_policy_request_dto.py
 test/test_terminate_policy_response_class.py
@@ -306,10 +330,12 @@
 test/test_update_premium_formula_response_class.py
 test/test_update_product_field_request_dto.py
 test/test_update_product_field_response_class.py
 test/test_update_product_request_dto.py
 test/test_update_product_response_class.py
 test/test_update_product_version_request_dto.py
 test/test_update_product_version_response_class.py
+test/test_update_status_transition_rule_request_dto.py
+test/test_update_status_transition_rule_response_class.py
 test/test_uploaded_document_dto.py
 test/test_validate_product_factors_request_dto.py
 test/test_withdraw_policy_response_class.py
```

### Comparing `eis-insurance-1.30.0/setup.py` & `eis-insurance-1.31.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "eis-insurance"
-VERSION = "1.30.0"
+VERSION = "1.31.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `eis-insurance-1.30.0/test/test_activate_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_activate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_activate_policy_response_class.py` & `eis-insurance-1.31.0/test/test_activate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_calculate_custom_premium_request_dto.py` & `eis-insurance-1.31.0/test/test_calculate_custom_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_calculate_premium_request_dto.py` & `eis-insurance-1.31.0/test/test_calculate_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_calculate_product_fields_request_dto.py` & `eis-insurance-1.31.0/test/test_calculate_product_fields_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_clone_product_version_request_dto.py` & `eis-insurance-1.31.0/test/test_clone_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_account_request_dto.py` & `eis-insurance-1.31.0/test/test_create_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_bank_account_request_dto.py` & `eis-insurance-1.31.0/test/test_create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_custom_application_request_dto.py` & `eis-insurance-1.31.0/test/test_create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_dummy_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_create_dummy_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_insured_object_request_dto.py` & `eis-insurance-1.31.0/test/test_create_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_insured_object_response_class.py` & `eis-insurance-1.31.0/test/test_create_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_lead_async_response_class.py` & `eis-insurance-1.31.0/test/test_create_lead_async_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_lead_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_lead_request_dto.py` & `eis-insurance-1.31.0/test/test_create_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_lead_response_class.py` & `eis-insurance-1.31.0/test/test_create_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_lead_status_request_dto.py` & `eis-insurance-1.31.0/test/test_create_lead_status_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_lead_status_response_class.py` & `eis-insurance-1.31.0/test/test_create_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_named_range_request_dto.py` & `eis-insurance-1.31.0/test/test_create_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_named_range_response_class.py` & `eis-insurance-1.31.0/test/test_create_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_named_request_s3_data_class.py` & `eis-insurance-1.31.0/test/test_create_named_request_s3_data_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_payment_method_request_dto.py` & `eis-insurance-1.31.0/test/test_create_payment_method_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_create_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_policy_response_class.py` & `eis-insurance-1.31.0/test/test_create_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_premium_formula_request_dto.py` & `eis-insurance-1.31.0/test/test_create_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_premium_formula_response_class.py` & `eis-insurance-1.31.0/test/test_create_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_product_field_request_dto.py` & `eis-insurance-1.31.0/test/test_create_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_product_field_response_class.py` & `eis-insurance-1.31.0/test/test_create_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_product_request_dto.py` & `eis-insurance-1.31.0/test/test_create_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_create_product_response_class.py` & `eis-insurance-1.31.0/test/test_create_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_csv_product_factor_dto.py` & `eis-insurance-1.31.0/test/test_csv_product_factor_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_default_api.py` & `eis-insurance-1.31.0/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_delete_request_dto.py` & `eis-insurance-1.31.0/test/test_terminate_policy_request_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.insurance
-from eis.insurance.model.delete_request_dto import DeleteRequestDto
+from eis.insurance.model.terminate_policy_request_dto import TerminatePolicyRequestDto
 
 
-class TestDeleteRequestDto(unittest.TestCase):
-    """DeleteRequestDto unit test stubs"""
+class TestTerminatePolicyRequestDto(unittest.TestCase):
+    """TerminatePolicyRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDeleteRequestDto(self):
-        """Test DeleteRequestDto"""
+    def testTerminatePolicyRequestDto(self):
+        """Test TerminatePolicyRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DeleteRequestDto()  # noqa: E501
+        # model = TerminatePolicyRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-insurance-1.30.0/test/test_delete_response_class.py` & `eis-insurance-1.31.0/test/test_delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_empty_response_class.py` & `eis-insurance-1.31.0/test/test_empty_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_insured_object_response_class.py` & `eis-insurance-1.31.0/test/test_get_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_lead_response_class.py` & `eis-insurance-1.31.0/test/test_get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_lead_status_response_class.py` & `eis-insurance-1.31.0/test/test_get_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_named_range_response_class.py` & `eis-insurance-1.31.0/test/test_get_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_policy_data_by_date_request_dto.py` & `eis-insurance-1.31.0/test/test_get_policy_data_by_date_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_get_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_policy_response_class.py` & `eis-insurance-1.31.0/test/test_get_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_premium_formula_request_dto.py` & `eis-insurance-1.31.0/test/test_get_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_premium_formula_response_class.py` & `eis-insurance-1.31.0/test/test_get_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_factor_response_class.py` & `eis-insurance-1.31.0/test/test_get_product_factor_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_factor_value_request_dto.py` & `eis-insurance-1.31.0/test/test_get_product_factor_value_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_factor_value_response_class.py` & `eis-insurance-1.31.0/test/test_get_product_factor_value_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_factors_for_version_request_dto.py` & `eis-insurance-1.31.0/test/test_get_product_factors_for_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_factors_for_version_response_class.py` & `eis-insurance-1.31.0/test/test_get_product_factors_for_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_field_request_dto.py` & `eis-insurance-1.31.0/test/test_get_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_field_response_class.py` & `eis-insurance-1.31.0/test/test_get_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_request_dto.py` & `eis-insurance-1.31.0/test/test_get_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_response_class.py` & `eis-insurance-1.31.0/test/test_get_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_version_request_dto.py` & `eis-insurance-1.31.0/test/test_get_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_get_product_version_response_class.py` & `eis-insurance-1.31.0/test/test_get_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_grouped_product_factor_class.py` & `eis-insurance-1.31.0/test/test_grouped_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_grouped_product_factor_value_class.py` & `eis-insurance-1.31.0/test/test_grouped_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_grouped_product_factors_response_class.py` & `eis-insurance-1.31.0/test/test_grouped_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_grpc_patch_lead_request_dto.py` & `eis-insurance-1.31.0/test/test_grpc_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_grpc_update_lead_request_dto.py` & `eis-insurance-1.31.0/test/test_grpc_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_inline_response200.py` & `eis-insurance-1.31.0/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_inline_response503.py` & `eis-insurance-1.31.0/test/test_inline_response503.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_insured_object_class.py` & `eis-insurance-1.31.0/test/test_insured_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_insured_object_type_class.py` & `eis-insurance-1.31.0/test/test_insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_insured_object_types_api.py` & `eis-insurance-1.31.0/test/test_insured_object_types_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_insured_objects_api.py` & `eis-insurance-1.31.0/test/test_insured_objects_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_invoice_item_class.py` & `eis-insurance-1.31.0/test/test_invoice_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_invoice_status_class.py` & `eis-insurance-1.31.0/test/test_invoice_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_lead_bank_account_class.py` & `eis-insurance-1.31.0/test/test_lead_bank_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_lead_class.py` & `eis-insurance-1.31.0/test/test_lead_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_lead_status_class.py` & `eis-insurance-1.31.0/test/test_lead_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_lead_statuses_api.py` & `eis-insurance-1.31.0/test/test_lead_statuses_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_leads_api.py` & `eis-insurance-1.31.0/test/test_leads_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_insured_object_types_response_class.py` & `eis-insurance-1.31.0/test/test_list_insured_object_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_insured_objects_response_class.py` & `eis-insurance-1.31.0/test/test_list_insured_objects_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_lead_statuses_response_class.py` & `eis-insurance-1.31.0/test/test_list_lead_statuses_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_leads_response_class.py` & `eis-insurance-1.31.0/test/test_list_leads_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_named_ranges_response_class.py` & `eis-insurance-1.31.0/test/test_list_named_ranges_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_policies_response_class.py` & `eis-insurance-1.31.0/test/test_list_policies_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_premium_formulas_response_class.py` & `eis-insurance-1.31.0/test/test_list_premium_formulas_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_product_factors_response_class.py` & `eis-insurance-1.31.0/test/test_list_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_product_field_types_response_class.py` & `eis-insurance-1.31.0/test/test_list_product_field_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_product_fields_response_class.py` & `eis-insurance-1.31.0/test/test_list_product_fields_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_products_response_class.py` & `eis-insurance-1.31.0/test/test_list_products_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_list_request_dto.py` & `eis-insurance-1.31.0/test/test_list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_named_range_class.py` & `eis-insurance-1.31.0/test/test_named_range_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_named_ranges_api.py` & `eis-insurance-1.31.0/test/test_named_ranges_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_patch_lead_request_dto.py` & `eis-insurance-1.31.0/test/test_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_patch_lead_response_class.py` & `eis-insurance-1.31.0/test/test_patch_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_patch_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_patch_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_patch_policy_response_class.py` & `eis-insurance-1.31.0/test/test_patch_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_policies_api.py` & `eis-insurance-1.31.0/test/test_policies_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_policy_class.py` & `eis-insurance-1.31.0/test/test_policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_policy_object_class.py` & `eis-insurance-1.31.0/test/test_policy_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_policy_object_dto.py` & `eis-insurance-1.31.0/test/test_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_policy_premium_class.py` & `eis-insurance-1.31.0/test/test_policy_premium_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_policy_premium_item_class.py` & `eis-insurance-1.31.0/test/test_policy_premium_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_policy_version_class.py` & `eis-insurance-1.31.0/test/test_policy_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_premium_formula_class.py` & `eis-insurance-1.31.0/test/test_premium_formula_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_premium_formulas_api.py` & `eis-insurance-1.31.0/test/test_premium_formulas_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_premium_override_dto.py` & `eis-insurance-1.31.0/test/test_premium_override_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_premium_override_request_class.py` & `eis-insurance-1.31.0/test/test_premium_override_request_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_premium_override_request_dto.py` & `eis-insurance-1.31.0/test/test_premium_override_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_class.py` & `eis-insurance-1.31.0/test/test_product_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_factor_class.py` & `eis-insurance-1.31.0/test/test_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_factor_for_version_class.py` & `eis-insurance-1.31.0/test/test_product_factor_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_factor_value_class.py` & `eis-insurance-1.31.0/test/test_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_factor_value_for_version_class.py` & `eis-insurance-1.31.0/test/test_product_factor_value_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_factors_api.py` & `eis-insurance-1.31.0/test/test_product_factors_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_field_class.py` & `eis-insurance-1.31.0/test/test_product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_field_type_class.py` & `eis-insurance-1.31.0/test/test_product_field_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_fields_api.py` & `eis-insurance-1.31.0/test/test_product_fields_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_version_class.py` & `eis-insurance-1.31.0/test/test_product_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_product_versions_api.py` & `eis-insurance-1.31.0/test/test_product_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_products_api.py` & `eis-insurance-1.31.0/test/test_products_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_sepa_dto.py` & `eis-insurance-1.31.0/test/test_sepa_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_shared_create_lead_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_shared_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_shared_invoice_class.py` & `eis-insurance-1.31.0/test/test_shared_invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_shared_lead_policy_object_dto.py` & `eis-insurance-1.31.0/test/test_shared_lead_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_shared_product_field_class.py` & `eis-insurance-1.31.0/test/test_shared_product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_shared_update_named_range_request_dto.py` & `eis-insurance-1.31.0/test/test_shared_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_shared_update_premium_formula_request_dto.py` & `eis-insurance-1.31.0/test/test_shared_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_store_product_factors_request_dto.py` & `eis-insurance-1.31.0/test/test_store_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_store_product_factors_response_class.py` & `eis-insurance-1.31.0/test/test_store_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_suspend_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_suspend_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_suspend_policy_response_class.py` & `eis-insurance-1.31.0/test/test_suspend_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_swap_premium_formulas_order_request_dto.py` & `eis-insurance-1.31.0/test/test_swap_premium_formulas_order_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_terminate_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_update_policy_request_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 """
 
 
 import sys
 import unittest
 
 import eis.insurance
-from eis.insurance.model.terminate_policy_request_dto import TerminatePolicyRequestDto
+from eis.insurance.model.policy_object_dto import PolicyObjectDto
+from eis.insurance.model.premium_override_request_dto import PremiumOverrideRequestDto
+globals()['PolicyObjectDto'] = PolicyObjectDto
+globals()['PremiumOverrideRequestDto'] = PremiumOverrideRequestDto
+from eis.insurance.model.update_policy_request_dto import UpdatePolicyRequestDto
 
 
-class TestTerminatePolicyRequestDto(unittest.TestCase):
-    """TerminatePolicyRequestDto unit test stubs"""
+class TestUpdatePolicyRequestDto(unittest.TestCase):
+    """UpdatePolicyRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTerminatePolicyRequestDto(self):
-        """Test TerminatePolicyRequestDto"""
+    def testUpdatePolicyRequestDto(self):
+        """Test UpdatePolicyRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TerminatePolicyRequestDto()  # noqa: E501
+        # model = UpdatePolicyRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-insurance-1.30.0/test/test_terminate_policy_response_class.py` & `eis-insurance-1.31.0/test/test_terminate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_timeslice_class.py` & `eis-insurance-1.31.0/test/test_timeslice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_insured_object_request_dto.py` & `eis-insurance-1.31.0/test/test_update_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_lead_request_dto.py` & `eis-insurance-1.31.0/test/test_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_lead_response_class.py` & `eis-insurance-1.31.0/test/test_update_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_named_range_request_dto.py` & `eis-insurance-1.31.0/test/test_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_named_range_response_class.py` & `eis-insurance-1.31.0/test/test_update_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_policy_request_dto.py` & `eis-insurance-1.31.0/test/test_update_product_field_request_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,32 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.insurance
-from eis.insurance.model.policy_object_dto import PolicyObjectDto
-from eis.insurance.model.premium_override_request_dto import PremiumOverrideRequestDto
-globals()['PolicyObjectDto'] = PolicyObjectDto
-globals()['PremiumOverrideRequestDto'] = PremiumOverrideRequestDto
-from eis.insurance.model.update_policy_request_dto import UpdatePolicyRequestDto
+from eis.insurance.model.update_product_field_request_dto import UpdateProductFieldRequestDto
 
 
-class TestUpdatePolicyRequestDto(unittest.TestCase):
-    """UpdatePolicyRequestDto unit test stubs"""
+class TestUpdateProductFieldRequestDto(unittest.TestCase):
+    """UpdateProductFieldRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdatePolicyRequestDto(self):
-        """Test UpdatePolicyRequestDto"""
+    def testUpdateProductFieldRequestDto(self):
+        """Test UpdateProductFieldRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UpdatePolicyRequestDto()  # noqa: E501
+        # model = UpdateProductFieldRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-insurance-1.30.0/test/test_update_policy_response_class.py` & `eis-insurance-1.31.0/test/test_update_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_premium_formula_request_dto.py` & `eis-insurance-1.31.0/test/test_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_premium_formula_response_class.py` & `eis-insurance-1.31.0/test/test_update_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_product_field_request_dto.py` & `eis-insurance-1.31.0/test/test_get_lead_version_request_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import eis.insurance
-from eis.insurance.model.update_product_field_request_dto import UpdateProductFieldRequestDto
+from eis.insurance.model.get_lead_version_request_dto import GetLeadVersionRequestDto
 
 
-class TestUpdateProductFieldRequestDto(unittest.TestCase):
-    """UpdateProductFieldRequestDto unit test stubs"""
+class TestGetLeadVersionRequestDto(unittest.TestCase):
+    """GetLeadVersionRequestDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdateProductFieldRequestDto(self):
-        """Test UpdateProductFieldRequestDto"""
+    def testGetLeadVersionRequestDto(self):
+        """Test GetLeadVersionRequestDto"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UpdateProductFieldRequestDto()  # noqa: E501
+        # model = GetLeadVersionRequestDto()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `eis-insurance-1.30.0/test/test_update_product_field_response_class.py` & `eis-insurance-1.31.0/test/test_update_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_product_request_dto.py` & `eis-insurance-1.31.0/test/test_update_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_product_response_class.py` & `eis-insurance-1.31.0/test/test_update_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_product_version_request_dto.py` & `eis-insurance-1.31.0/test/test_update_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_update_product_version_response_class.py` & `eis-insurance-1.31.0/test/test_update_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_uploaded_document_dto.py` & `eis-insurance-1.31.0/test/test_uploaded_document_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_validate_product_factors_request_dto.py` & `eis-insurance-1.31.0/test/test_validate_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.30.0/test/test_withdraw_policy_response_class.py` & `eis-insurance-1.31.0/test/test_withdraw_policy_response_class.py`

 * *Files identical despite different names*


# Comparing `tmp/credsweeper-1.6.2.tar.gz` & `tmp/credsweeper-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.6.2.tar", last modified: Tue Mar 26 08:07:39 2024, max compression
+gzip compressed data, was "credsweeper-1.6.3.tar", last modified: Wed Apr 24 08:22:04 2024, max compression
```

## Comparing `credsweeper-1.6.2.tar` & `credsweeper-1.6.3.tar`

### file list

```diff
@@ -1,168 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.296153 credsweeper-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-26 08:07:35.000000 credsweeper-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-03-26 08:07:39.296153 credsweeper-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-03-26 08:07:35.000000 credsweeper-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.268153 credsweeper-1.6.2/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18012 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.268153 credsweeper-1.6.2/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/common/morpheme_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.268153 credsweeper-1.6.2/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.272153 credsweeper-1.6.2/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.272153 credsweeper-1.6.2/credsweeper/deep_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/docx_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/eml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/jks_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/pkcs12_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/deep_scanner/zip_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.276153 credsweeper-1.6.2/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/patch_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/file_handler/text_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.284153 credsweeper-1.6.2/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.284153 credsweeper-1.6.2/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/group/weird_base64_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_atlassian_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_base64_data_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_base64_encoded_pem_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_base64_key_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_entropy_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_github_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_ip_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_jfrog_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_not_part_encoded_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_number_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_token_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.284153 credsweeper-1.6.2/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.288153 credsweeper-1.6.2/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (127)  1483399 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.288153 credsweeper-1.6.2/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.288153 credsweeper-1.6.2/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.292153 credsweeper-1.6.2/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.292153 credsweeper-1.6.2/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.292153 credsweeper-1.6.2/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/utils/entropy_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/utils/pem_key_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    24067 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.292153 credsweeper-1.6.2/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-26 08:07:35.000000 credsweeper-1.6.2/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.296153 credsweeper-1.6.2/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-03-26 08:07:39.000000 credsweeper-1.6.2/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-03-26 08:07:39.000000 credsweeper-1.6.2/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:07:39.000000 credsweeper-1.6.2/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 08:07:39.000000 credsweeper-1.6.2/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-26 08:07:39.000000 credsweeper-1.6.2/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-26 08:07:39.000000 credsweeper-1.6.2/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-26 08:07:39.296153 credsweeper-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-26 08:07:35.000000 credsweeper-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:07:39.296153 credsweeper-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    32156 2024-03-26 08:07:35.000000 credsweeper-1.6.2/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-26 08:07:35.000000 credsweeper-1.6.2/tests/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-03-26 08:07:35.000000 credsweeper-1.6.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.284752 credsweeper-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-24 08:22:00.000000 credsweeper-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-24 08:22:04.284752 credsweeper-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-24 08:22:00.000000 credsweeper-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.260752 credsweeper-1.6.3/credsweeper/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18285 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.260752 credsweeper-1.6.3/credsweeper/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/morpheme_checklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.260752 credsweeper-1.6.3/credsweeper/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.264752 credsweeper-1.6.3/credsweeper/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/line_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.264752 credsweeper-1.6.3/credsweeper/deep_scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/docx_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/eml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/jks_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/pkcs12_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/zip_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.268752 credsweeper-1.6.3/credsweeper/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/abstract_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/patches_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/text_content_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.272752 credsweeper-1.6.3/credsweeper/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/filters/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/line_git_binary_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_atlassian_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base64_encoded_pem_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base64_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_github_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_hex_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_ip_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_jfrog_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_method_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/variable_not_allowed_pattern_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/ml_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)   868645 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24774 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/rules/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/scanner/scan_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/secret/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/secret/log.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/entropy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/pem_key_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24067 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/validations/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/apply_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 08:22:04.284752 credsweeper-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-24 08:22:00.000000 credsweeper-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    32156 2024-04-24 08:22:00.000000 credsweeper-1.6.3/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-24 08:22:00.000000 credsweeper-1.6.3/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41777 2024-04-24 08:22:00.000000 credsweeper-1.6.3/tests/test_main.py
```

### Comparing `credsweeper-1.6.2/LICENSE` & `credsweeper-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/PKG-INFO` & `credsweeper-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.6.2
+Version: 1.6.3
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.6.2/README.md` & `credsweeper-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/__init__.py` & `credsweeper-1.6.3/credsweeper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.6.2"
+__version__ = "1.6.3"
```

### Comparing `credsweeper-1.6.2/credsweeper/__main__.py` & `credsweeper-1.6.3/credsweeper/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
 from typing import Any, Union, Optional, Dict
 
 from credsweeper import __version__
 from credsweeper.app import APP_PATH, CredSweeper
 from credsweeper.common.constants import ThresholdPreset, Severity, RuleType, DiffRowType
+from credsweeper.file_handler.abstract_provider import AbstractProvider
 from credsweeper.file_handler.files_provider import FilesProvider
-from credsweeper.file_handler.patch_provider import PatchProvider
-from credsweeper.file_handler.text_provider import TextProvider
+from credsweeper.file_handler.patches_provider import PatchesProvider
 from credsweeper.logger.logger import Logger
 from credsweeper.utils import Util
 
 EXIT_SUCCESS = 0
 EXIT_FAILURE = 1
 
 logger = logging.getLogger(__name__)
@@ -253,15 +253,15 @@
     if json_filename is None:
         return None, None
     added_json_filename = json_filename[:-5] + "_added.json"
     deleted_json_filename = json_filename[:-5] + "_deleted.json"
     return added_json_filename, deleted_json_filename
 
 
-def scan(args: Namespace, content_provider: FilesProvider, json_filename: Optional[str],
+def scan(args: Namespace, content_provider: AbstractProvider, json_filename: Optional[str],
          xlsx_filename: Optional[str]) -> int:
     """Scan content_provider data, print results or save them to json_filename is not None
 
     Args:
         args: arguments of the application
         content_provider: FilesProvider instance to scan data from
         json_filename: json type report file path or None
@@ -311,29 +311,29 @@
     if args.banner:
         print(f"CredSweeper {__version__} crc32:{check_integrity():08x}")
     Logger.init_logging(args.log, args.log_config_path)
     logger.info(f"Init CredSweeper object with arguments: {args}")
     summary: Dict[str, int] = {}
     if args.path:
         logger.info(f"Run analyzer on path: {args.path}")
-        content_provider: FilesProvider = TextProvider(args.path, skip_ignored=args.skip_ignored)
+        content_provider: AbstractProvider = FilesProvider(args.path, skip_ignored=args.skip_ignored)
         credentials_number = scan(args, content_provider, args.json_filename, args.xlsx_filename)
         summary["Detected Credentials"] = credentials_number
         if 0 <= credentials_number:
             result = EXIT_SUCCESS
     elif args.diff_path:
         added_json_filename, deleted_json_filename = get_json_filenames(args.json_filename)
         # Analyze added data
         logger.info(f"Run analyzer on added rows from patch files: {args.diff_path}")
-        content_provider = PatchProvider(args.diff_path, change_type=DiffRowType.ADDED)
+        content_provider = PatchesProvider(args.diff_path, change_type=DiffRowType.ADDED)
         add_credentials_number = scan(args, content_provider, added_json_filename, args.xlsx_filename)
         summary["Added File Credentials"] = add_credentials_number
         # Analyze deleted data
         logger.info(f"Run analyzer on deleted rows from patch files: {args.diff_path}")
-        content_provider = PatchProvider(args.diff_path, change_type=DiffRowType.DELETED)
+        content_provider = PatchesProvider(args.diff_path, change_type=DiffRowType.DELETED)
         del_credentials_number = scan(args, content_provider, deleted_json_filename, args.xlsx_filename)
         summary["Deleted File Credentials"] = del_credentials_number
         if 0 <= add_credentials_number and 0 <= del_credentials_number:
             result = EXIT_SUCCESS
     elif args.export_config:
         logging.info(f"Exporting default config to file: {args.export_config}")
         config_dict = Util.json_load(APP_PATH / "secret" / "config.json")
```

### Comparing `credsweeper-1.6.2/credsweeper/app.py` & `credsweeper-1.6.3/credsweeper/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import itertools
 import logging
 import multiprocessing
 import signal
 import sys
 from pathlib import Path
-from typing import Any, List, Optional, Union, Dict
+from typing import Any, List, Optional, Union, Dict, Sequence
 
 import pandas as pd
 
 # Directory of credsweeper sources MUST be placed before imports to avoid circular import error
 APP_PATH = Path(__file__).resolve().parent
 
 from credsweeper.common.constants import KeyValidationOption, Severity, ThresholdPreset
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate, CredentialManager
 from credsweeper.deep_scanner.deep_scanner import DeepScanner
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
-from credsweeper.file_handler.files_provider import FilesProvider
+from credsweeper.file_handler.abstract_provider import AbstractProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
 from credsweeper.scanner import Scanner
 from credsweeper.utils import Util
 from credsweeper.validations.apply_validation import ApplyValidation
 
 logger = logging.getLogger(__name__)
 
@@ -50,15 +50,15 @@
                  ml_batch_size: Optional[int] = 16,
                  ml_threshold: Union[float, ThresholdPreset] = ThresholdPreset.medium,
                  azure: bool = False,
                  cuda: bool = False,
                  find_by_ext: bool = False,
                  depth: int = 0,
                  doc: bool = False,
-                 severity: Severity = Severity.INFO,
+                 severity: Union[Severity, str] = Severity.INFO,
                  size_limit: Optional[str] = None,
                  exclude_lines: Optional[List[str]] = None,
                  exclude_values: Optional[List[str]] = None,
                  log_level: Optional[str] = None) -> None:
         """Initialize Advanced credential scanner.
 
         Args:
@@ -83,21 +83,24 @@
             size_limit: optional string integer or human-readable format to skip oversize files
             exclude_lines: lines to omit in scan. Will be added to the lines already in config
             exclude_values: values to omit in scan. Will be added to the values already in config
             log_level: str - level for pool initializer according logging levels (UPPERCASE)
 
         """
         self.pool_count: int = int(pool_count) if int(pool_count) > 1 else 1
+        if not (_severity := Severity.get(severity)):
+            raise RuntimeError(f"Severity level provided: {severity}"
+                               f" -- must be one of: {' | '.join([i.value for i in Severity])}")
         config_dict = self._get_config_dict(config_path=config_path,
                                             api_validation=api_validation,
                                             use_filters=use_filters,
                                             find_by_ext=find_by_ext,
                                             depth=depth,
                                             doc=doc,
-                                            severity=severity,
+                                            severity=_severity,
                                             size_limit=size_limit,
                                             exclude_lines=exclude_lines,
                                             exclude_values=exclude_values)
         self.config = Config(config_dict)
         self.scanner = Scanner(self.config, rule_path)
         self.deep_scanner = DeepScanner(self.config, self.scanner)
         self.credential_manager = CredentialManager()
@@ -211,48 +214,48 @@
     @config.setter
     def config(self, config: Config) -> None:
         """config setter"""
         self.__config = config
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    def run(self, content_provider: FilesProvider) -> int:
+    def run(self, content_provider: AbstractProvider) -> int:
         """Run an analysis of 'content_provider' object.
 
         Args:
             content_provider: path objects to scan
 
         """
-        _empty_list: List[Union[DiffContentProvider, TextContentProvider]] = []
-        file_extractors: List[Union[DiffContentProvider, TextContentProvider]] = \
+        _empty_list: Sequence[Union[DiffContentProvider, TextContentProvider]] = []
+        file_extractors: Sequence[Union[DiffContentProvider, TextContentProvider]] = \
             content_provider.get_scannable_files(self.config) if content_provider else _empty_list
         logger.info(f"Start Scanner for {len(file_extractors)} providers")
         self.scan(file_extractors)
         self.post_processing()
         self.export_results()
 
         return len(self.credential_manager.get_credentials())
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    def scan(self, content_providers: List[Union[DiffContentProvider, TextContentProvider]]) -> None:
+    def scan(self, content_providers: Sequence[Union[DiffContentProvider, TextContentProvider]]) -> None:
         """Run scanning of files from an argument "content_providers".
 
         Args:
             content_providers: file objects to scan
 
         """
         if 1 < self.pool_count:
             self.__multi_jobs_scan(content_providers)
         else:
             self.__single_job_scan(content_providers)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    def __single_job_scan(self, content_providers: List[Union[DiffContentProvider, TextContentProvider]]) -> None:
+    def __single_job_scan(self, content_providers: Sequence[Union[DiffContentProvider, TextContentProvider]]) -> None:
         """Performs scan in main thread"""
         all_cred: List[Candidate] = []
         for i in content_providers:
             candidates = self.file_scan(i)
             all_cred.extend(candidates)
         if self.config.api_validation:
             api_validation = ApplyValidation()
@@ -261,15 +264,15 @@
                 cred.api_validation = api_validation.validate(cred)
                 self.credential_manager.add_credential(cred)
         else:
             self.credential_manager.set_credentials(all_cred)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    def __multi_jobs_scan(self, content_providers: List[Union[DiffContentProvider, TextContentProvider]]) -> None:
+    def __multi_jobs_scan(self, content_providers: Sequence[Union[DiffContentProvider, TextContentProvider]]) -> None:
         """Performs scan with multiple jobs"""
         # use this separation to satisfy YAPF formatter
         yapfix = "%(asctime)s | %(levelname)s | %(processName)s:%(threadName)s | %(filename)s:%(lineno)s | %(message)s"
         log_kwargs = {"format": yapfix}
         if isinstance(self.__log_level, str):
             # is not None
             if "SILENCE" == self.__log_level:
```

### Comparing `credsweeper-1.6.2/credsweeper/common/constants.py` & `credsweeper-1.6.3/credsweeper/common/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             return other is not Confidence.WEAK
         elif self == Confidence.MODERATE:
             return other is Confidence.STRONG
         return False
 
     @staticmethod
     def get(confidence: Union[str, "Confidence"]) -> Optional["Confidence"]:
-        """returns Severity value from string or None"""
+        """returns Confidence value from string or None"""
         if isinstance(confidence, Confidence):
             return confidence
         if isinstance(confidence, str):
             value = getattr(Confidence, confidence.strip().upper(), None)
             if isinstance(value, Confidence):
                 return value
         return None
```

### Comparing `credsweeper-1.6.2/credsweeper/common/keyword_checklist.py` & `credsweeper-1.6.3/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.6.3/credsweeper/common/keyword_checklist.txt`

 * *Files 0% similar despite different names*

```diff
@@ -767,14 +767,15 @@
 sidebar
 sign
 similar
 simple
 since
 single
 sites
+size
 sizing
 sleep
 slice
 slick
 slide
 small
 smart
```

### Comparing `credsweeper-1.6.2/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.6.3/credsweeper/common/morpheme_checklist.txt`

 * *Files 0% similar despite different names*

```diff
@@ -582,14 +582,15 @@
 firm
 first
 fix
 flas
 flat
 fleet
 flick
+flix
 float
 floor
 fluent
 fluid
 flush
 focus
 foo
@@ -642,14 +643,15 @@
 gregor
 gress
 grid
 gro
 grpc
 guard
 guest
+guid
 guish
 ha1-
 ha1_
 ha2-
 ha256
 ha2_
 ha394
```

### Comparing `credsweeper-1.6.2/credsweeper/config/config.py` & `credsweeper-1.6.3/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.6.3/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/credentials/candidate.py` & `credsweeper-1.6.3/credsweeper/credentials/candidate.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.config = config
         self.validations: List[Validation] = validations if validations is not None else []
         self.use_ml = use_ml
         self.confidence = confidence
 
         self.api_validation = KeyValidationOption.NOT_AVAILABLE
         self.ml_validation = KeyValidationOption.NOT_AVAILABLE
-        self.ml_probability: Optional[bool] = None
+        self.ml_probability: Optional[float] = None
 
     @staticmethod
     def _encode(value: Any) -> Any:
         """Encode value to the base string ascii
 
         Args:
             value: Any type of value to be encoded
```

### Comparing `credsweeper-1.6.2/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.6.3/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/credentials/candidate_key.py` & `credsweeper-1.6.3/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/credentials/credential_manager.py` & `credsweeper-1.6.3/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/credentials/line_data.py` & `credsweeper-1.6.3/credsweeper/credentials/line_data.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/byte_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/deep_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/docx_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/docx_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/eml_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/eml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/html_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/jks_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/jks_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/pkcs12_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/pkcs12_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.6.3/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/__init__.py` & `credsweeper-1.6.3/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/analysis_target.py` & `credsweeper-1.6.3/credsweeper/file_handler/analysis_target.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/content_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/data_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.6.3/credsweeper/file_handler/file_path_extractor.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/files_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/abstract_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import io
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List, Union, Tuple
+from typing import Union, Tuple, Sequence
 
 from credsweeper.config import Config
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
 
 
-class FilesProvider(ABC):
+class AbstractProvider(ABC):
     """Base class for all files provider objects."""
 
-    def __init__(self, paths: List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]) -> None:
+    def __init__(self, paths: Sequence[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]) -> None:
         """Initialize Files Provider object for 'paths'.
 
         Args:
             paths: file paths list to scan or io.BytesIO or tuple with both
 
         """
         self.paths = paths
 
     @property
-    def paths(self) -> List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]:
+    def paths(self) -> Sequence[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]:
         """paths getter"""
         return self.__paths
 
     @paths.setter
-    def paths(self, paths: List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]) -> None:
+    def paths(self, paths: Sequence[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]) -> None:
         """paths setter"""
         self.__paths = paths
 
     @abstractmethod
-    def get_scannable_files(self, config: Config) -> List[Union[DiffContentProvider, TextContentProvider]]:
+    def get_scannable_files(self, config: Config) -> Sequence[Union[DiffContentProvider, TextContentProvider]]:
         """Get list of file object for analysis based on attribute "paths".
 
         Args:
             config: dict of credsweeper configuration
 
         Return:
             file objects to analyse
```

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/patch_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/patches_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 import io
 import logging
 from pathlib import Path
-from typing import List, Union, Tuple
+from typing import List, Union, Tuple, Sequence
 
 from credsweeper import TextContentProvider
 from credsweeper.common.constants import DiffRowType
 from credsweeper.config import Config
+from credsweeper.file_handler.abstract_provider import AbstractProvider
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
-from credsweeper.file_handler.files_provider import FilesProvider
 from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
 
 
-class PatchProvider(FilesProvider):
+class PatchesProvider(AbstractProvider):
     """Provide data from a list of `.patch` files.
-
-    Allows to scan for data that has changed between git commits, rather than the entire project.
-
-    Parameters:
-        paths: file paths list to scan. All files should be in `.patch` format
-        change_type: string, type of analyses changes in patch (added or deleted)
-        skip_ignored: boolean variable, Checking the directory to the list
-          of ignored directories from the gitignore file
-
     """
 
-    def __init__(self, paths: List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]],
+    def __init__(self, paths: Sequence[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]],
                  change_type: DiffRowType) -> None:
         """Initialize Files Patch Provider for patch files from 'paths'.
 
         Args:
             paths: file paths list to scan. All files should be in `.patch` format
-            change_type: string, type of analyses changes in patch (added or deleted)
-            skip_ignored: boolean variable, Checking the directory to the list
+            change_type: DiffRowType, type of analyses changes in patch (added or deleted)
               of ignored directories from the gitignore file
 
         """
         super().__init__(paths)
         self.change_type = change_type
 
     def load_patch_data(self, config: Config) -> List[List[str]]:
@@ -53,24 +43,25 @@
                 the_patch = Util.decode_bytes(file_path.read())
                 raw_patches.append(the_patch)
             else:
                 logger.error(f"Unknown path type: {file_path}")
 
         return raw_patches
 
-    def get_files_sequence(self, raw_patches: List[List[str]]) -> List[Union[DiffContentProvider, TextContentProvider]]:
+    def get_files_sequence(self,
+                           raw_patches: List[List[str]]) -> Sequence[Union[DiffContentProvider, TextContentProvider]]:
         """Returns sequence of files"""
         files: List[Union[DiffContentProvider, TextContentProvider]] = []
         for raw_patch in raw_patches:
             files_data = Util.patch2files_diff(raw_patch, self.change_type)
             for file_path, file_diff in files_data.items():
                 files.append(DiffContentProvider(file_path=file_path, change_type=self.change_type, diff=file_diff))
         return files
 
-    def get_scannable_files(self, config: Config) -> List[Union[DiffContentProvider, TextContentProvider]]:
+    def get_scannable_files(self, config: Config) -> Sequence[Union[DiffContentProvider, TextContentProvider]]:
         """Get files to scan. Output based on the `paths` field.
 
         Args:
             config: dict of credsweeper configuration
 
         Return:
             file objects for analysing
```

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/file_handler/text_provider.py` & `credsweeper-1.6.3/credsweeper/file_handler/files_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 import io
 import logging
 from pathlib import Path
-from typing import List, Optional, Union, Tuple
+from typing import List, Optional, Union, Tuple, Sequence
 
 from credsweeper import DiffContentProvider
 from credsweeper.config import Config
+from credsweeper.file_handler.abstract_provider import AbstractProvider
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
-from credsweeper.file_handler.files_provider import FilesProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
 
 logger = logging.getLogger(__name__)
 
 
-class TextProvider(FilesProvider):
-    """Provider of full text files analysing.
-
-    Parameters:
-        paths: list of string, list of parent path of files to scan
-        change_type: string, type of analyses changes in patch (added or deleted)
-        skip_ignored: boolean variable, Checking the directory to the list
-          of ignored directories from the gitignore file
-
-    """
+class FilesProvider(AbstractProvider):
+    """Provider of plain os files to be analysed."""
 
     def __init__(self,
-                 paths: List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]],
+                 paths: Sequence[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]],
                  skip_ignored: Optional[bool] = None) -> None:
         """Initialize Files Text Provider for files from 'paths'.
 
         Args:
             paths: list of parent paths of files to scan
                    OR tuple of path (info purpose) and io.BytesIO (reads the data from current pos)
             skip_ignored: boolean variable, Checking the directory to the list
                           of ignored directories from the gitignore file
 
         """
         super().__init__(paths)
         self.skip_ignored = skip_ignored
 
-    def get_scannable_files(self, config: Config) -> List[Union[DiffContentProvider, TextContentProvider]]:
+    def get_scannable_files(self, config: Config) -> Sequence[Union[DiffContentProvider, TextContentProvider]]:
         """Get list of full text file object for analysis of files with parent paths from "paths".
 
         Args:
             config: dict of credsweeper configuration
 
         Return:
             preprocessed file objects for analysis
```

### Comparing `credsweeper-1.6.2/credsweeper/filters/__init__.py` & `credsweeper-1.6.3/credsweeper/filters/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from credsweeper.filters.filter import Filter  # isort:skip
 
+from credsweeper.filters.line_git_binary_check import LineGitBinaryCheck
 from credsweeper.filters.line_specific_key_check import LineSpecificKeyCheck
 from credsweeper.filters.separator_unusual_check import SeparatorUnusualCheck
 from credsweeper.filters.value_allowlist_check import ValueAllowlistCheck
 from credsweeper.filters.value_array_dictionary_check import ValueArrayDictionaryCheck
 from credsweeper.filters.value_atlassian_token_check import ValueAtlassianTokenCheck
 from credsweeper.filters.value_base32_data_check import ValueBase32DataCheck
 from credsweeper.filters.value_base64_data_check import ValueBase64DataCheck
@@ -17,14 +18,15 @@
 from credsweeper.filters.value_entropy_base32_check import ValueEntropyBase32Check
 from credsweeper.filters.value_entropy_base36_check import ValueEntropyBase36Check
 from credsweeper.filters.value_entropy_base64_check import ValueEntropyBase64Check
 from credsweeper.filters.value_file_path_check import ValueFilePathCheck
 from credsweeper.filters.value_first_word_check import ValueFirstWordCheck
 from credsweeper.filters.value_github_check import ValueGitHubCheck
 from credsweeper.filters.value_grafana_check import ValueGrafanaCheck
+from credsweeper.filters.value_hex_number_check import ValueHexNumberCheck
 from credsweeper.filters.value_ip_check import ValueIPCheck
 from credsweeper.filters.value_jfrog_token_check import ValueJfrogTokenCheck
 from credsweeper.filters.value_json_web_token_check import ValueJsonWebTokenCheck
 from credsweeper.filters.value_last_word_check import ValueLastWordCheck
 from credsweeper.filters.value_length_check import ValueLengthCheck
 from credsweeper.filters.value_method_check import ValueMethodCheck
 from credsweeper.filters.value_not_allowed_pattern_check import ValueNotAllowedPatternCheck
```

### Comparing `credsweeper-1.6.2/credsweeper/filters/filter.py` & `credsweeper-1.6.3/credsweeper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/group/__init__.py` & `credsweeper-1.6.3/credsweeper/filters/group/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/group/group.py` & `credsweeper-1.6.3/credsweeper/filters/group/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from credsweeper.common.constants import GroupType
 from credsweeper.config import Config
 from credsweeper.filters import (Filter, LineSpecificKeyCheck, SeparatorUnusualCheck, ValueAllowlistCheck,
                                  ValueArrayDictionaryCheck, ValueBlocklistCheck, ValueCamelCaseCheck,
                                  ValueFilePathCheck, ValueFirstWordCheck, ValueLastWordCheck, ValueLengthCheck,
                                  ValueMethodCheck, ValueNotAllowedPatternCheck, ValuePatternCheck, ValueSimilarityCheck,
                                  ValueStringTypeCheck, ValueTokenCheck, VariableNotAllowedPatternCheck,
-                                 ValuePatternLengthCheck)
+                                 ValuePatternLengthCheck, ValueHexNumberCheck)
 
 
 class Group(ABC):
     """Abstract Group class"""
 
     def __init__(self, config: Config, rule_type: GroupType = GroupType.DEFAULT) -> None:
         if rule_type == GroupType.KEYWORD:
@@ -39,14 +39,15 @@
             SeparatorUnusualCheck(),
             ValueAllowlistCheck(),
             ValueArrayDictionaryCheck(),
             ValueBlocklistCheck(),
             ValueCamelCaseCheck(),
             ValueFilePathCheck(),
             ValueFirstWordCheck(),
+            ValueHexNumberCheck(),
             ValueLastWordCheck(),
             ValueLengthCheck(config),
             ValueMethodCheck(),
             ValueSimilarityCheck(),
             ValueStringTypeCheck(config),
             ValueTokenCheck(),
             VariableNotAllowedPatternCheck(),
```

### Comparing `credsweeper-1.6.2/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.6.3/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.6.3/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.6.3/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/group/weird_base64_token.py` & `credsweeper-1.6.3/credsweeper/filters/group/weird_base64_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.6.3/credsweeper/filters/line_specific_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.6.3/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_atlassian_token_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_atlassian_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_base32_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_base64_data_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_base64_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_base64_encoded_pem_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_base64_encoded_pem_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_base64_key_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_base64_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_couple_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_entropy_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_entropy_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_entropy_base64_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_entropy_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_github_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_github_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_grafana_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_ip_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_ip_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_jfrog_token_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_jfrog_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_json_web_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_length_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_method_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_method_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_not_part_encoded_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_not_part_encoded_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_number_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_split_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_token_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_token_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_token_base64_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_token_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_token_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.6.3/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.6.3/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class VariableNotAllowedPatternCheck(Filter):
     """Check if candidate variable is a regex placeholder or ends with match character (like + or >)."""
 
-    NOT_ALLOWED = [r"^([<]|\{\{).*", r"(@.*)", r"[!><+*/^|)](\s)?$", r".*(public|pubkey)"]
+    NOT_ALLOWED = [
+        r"^([<]|\{\{).*", r"(@.*)", r"[!><+*/^|)](\s)?$", r".*public", r".*pubkey", r".*_id$", r".*name$", r".*type$"
+    ]
     NOT_ALLOWED_PATTERN = re.compile(  #
         Util.get_regex_combine_or(NOT_ALLOWED),  #
         flags=re.IGNORECASE)
 
     def __init__(self, config: Config = None) -> None:
         pass
```

### Comparing `credsweeper-1.6.2/credsweeper/logger/logger.py` & `credsweeper-1.6.3/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/ml_model/features.py` & `credsweeper-1.6.3/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.6.3/credsweeper/ml_model/ml_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 self.unique_feature_list.append(feature)
             else:
                 self.common_feature_list.append(feature)
 
     def encode(self, line, char_to_index) -> np.ndarray:
         """Encodes line to array"""
         num_classes = len(char_to_index) + 1
-        result_array = np.zeros((self.maxlen, num_classes))
+        result_array = np.zeros((self.maxlen, num_classes), dtype=np.float32)
         line = line.strip().lower()[-self.maxlen:]
         for i in range(self.maxlen):
             if i < len(line):
                 c = line[i]
                 if c in char_to_index:
                     result_array[i, char_to_index[c]] = 1
                 else:
@@ -85,27 +85,27 @@
     def _call_model(self, line_input: np.ndarray, feature_input: np.ndarray) -> Any:
         line_input = line_input.astype(np.float32)
         feature_input = feature_input.astype(np.float32)
         return self.model_session.run(None, {"line_input": line_input, "feature_input": feature_input})[0]
 
     def extract_common_features(self, candidates: List[Candidate]) -> np.ndarray:
         """Extract features that are guaranteed to be the same for all candidates on the same line with same value."""
-        feature_array = np.array([], dtype=float)
+        feature_array = np.array([], dtype=np.float32)
         # Extract features from credential candidate
         default_candidate = candidates[0]
         for feature in self.common_feature_list:
             new_feature = feature([default_candidate])[0]
             if not isinstance(new_feature, np.ndarray):
                 new_feature = np.array([new_feature])
             feature_array = np.append(feature_array, new_feature)
         return feature_array
 
     def extract_unique_features(self, candidates: List[Candidate]) -> np.ndarray:
-        """Extract features that can by different between candidates. Join them with or operator."""
-        feature_array = np.array([], dtype=bool)
+        """Extract features that can be different between candidates. Join them with or operator."""
+        feature_array = np.array([], dtype=np.int8)
         default_candidate = candidates[0]
         for feature in self.unique_feature_list:
             new_feature = feature([default_candidate])[0]
             if not isinstance(new_feature, np.ndarray):
                 new_feature = np.array([new_feature])
             feature_array = np.append(feature_array, new_feature)
         for candidate in candidates[1:]:
```

### Comparing `credsweeper-1.6.2/credsweeper/ml_model/model_config.json` & `credsweeper-1.6.3/credsweeper/ml_model/model_config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'thresholds'": "{'lowest': 0.22917, 'low': 0.35739, 'medium': 0.62204, 'high': 0.79791, "*

 * *                 "'highest': 0.92996}"}*

```diff
@@ -398,14 +398,14 @@
                 ]
             },
             "type": "RuleName"
         }
     ],
     "max_len": 160,
     "thresholds": {
-        "high": 0.7979102,
-        "highest": 0.9299587,
-        "low": 0.3573966,
-        "lowest": 0.22916731,
-        "medium": 0.62203974
+        "high": 0.79791,
+        "highest": 0.92996,
+        "low": 0.35739,
+        "lowest": 0.22917,
+        "medium": 0.62204
     }
 }
```

### Comparing `credsweeper-1.6.2/credsweeper/rules/config.yaml` & `credsweeper-1.6.3/credsweeper/rules/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,17 @@
   type: pattern
   values:
     - (?P<variable>[`'\"]?(?i:(?<!id[ :/])pa[as]swo?r?ds?|pwd?|p/w|비밀번호|비번|패스워드|암호)[`'\"]?)((\s)*[=:](\s)*)(?P<quote>[`'\"(])?(?P<value>(?-i:(?P<a>[A-Z])|(?P<b>[a-z])|(?P<c>[0-9/_+=~!@#$%^&*;:?-])){4,31}(?(a)(?(b)(?(c)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x))(?(quote)[)`'\"])
   filter_type:
     - ValueAllowlistCheck
     - ValuePatternCheck
     - ValueDictionaryKeywordCheck
+    - LineGitBinaryCheck
+    - ValueFilePathCheck
+    - ValueHexNumberCheck
   min_line_len: 10
   required_substrings:
     - pass
     - sword
     - ":"
     - "/"
     - "="
@@ -105,15 +108,15 @@
   doc_only: true
 
 - name: API
   severity: medium
   confidence: moderate
   type: keyword
   values:
-    - api
+    - api(?!tal)
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 11
   required_substrings:
     - api
   doc_available: false
 
@@ -455,15 +458,15 @@
   min_line_len: 15
 
 - name: Slack Webhook
   severity: high
   confidence: strong
   type: pattern
   values:
-    - (?P<value>hooks\.slack\.com/services/T\w{8}/B\w{8}/\w{24})
+    - (?P<value>hooks\.slack\.com/services/T[0-9A-Z]{8,16}/B[0-9A-Z]{8,16}/\w{24})
   filter_type: GeneralPattern
   required_substrings:
     - hooks.slack.com/services/T
   min_line_len: 61
 
 - name: Stripe Standard API Key
   severity: high
@@ -527,15 +530,15 @@
   min_line_len: 50
 
 - name: Token
   severity: medium
   confidence: moderate
   type: keyword
   values:
-    - token
+    - token(?!ize)
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 13
   required_substrings:
     - token
   doc_available: false
 
@@ -577,15 +580,15 @@
   doc_available: false
 
 - name: Key
   severity: medium
   confidence: moderate
   type: keyword
   values:
-    - key(?!word)
+    - key(?!word|board|pad|name)
   filter_type: GeneralKeyword
   use_ml: true
   min_line_len: 11
   required_substrings:
     - key
   doc_available: false
 
@@ -984,7 +987,27 @@
     - ValueCoupleKeywordCheck
     - ValuePatternCheck
     - ValueEntropyBase32Check
     - ValueBase32DataCheck
     - ValueTokenBase32Check
   min_line_len: 16
   required_regex: "[a-zA-Z0-9_/+-]{15,80}"
+
+- name: OpenAI Token
+  severity: high
+  confidence: strong
+  type: pattern
+  values:
+    - (?<![.0-9A-Za-z_/+-])(?P<value>sk-\w{20}T3BlbkFJ\w{20})(?![=0-9A-Za-z_/+-])
+  min_line_len: 51
+  required_regex: T3BlbkFJ
+
+- name: Docker Swarm Token
+  severity: high
+  confidence: strong
+  type: pattern
+  values:
+    - (?<![.0-9A-Za-z_/+-])(?P<value>SWMTKN-1-[0-9a-z]{50}-[0-9a-z]{25})(?![=0-9A-Za-z_/+-])
+  min_line_len: 85
+  filter_type:
+    - ValueCoupleKeywordCheck
+  required_regex: SWMTKN-1-
```

### Comparing `credsweeper-1.6.2/credsweeper/rules/rule.py` & `credsweeper-1.6.3/credsweeper/rules/rule.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.6.3/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.6.3/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.6.3/credsweeper/scanner/scan_type/scan_type.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.6.3/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/scanner/scanner.py` & `credsweeper-1.6.3/credsweeper/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/secret/config.json` & `credsweeper-1.6.3/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/secret/log.yaml` & `credsweeper-1.6.3/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/utils/entropy_validator.py` & `credsweeper-1.6.3/credsweeper/utils/entropy_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/utils/pem_key_detector.py` & `credsweeper-1.6.3/credsweeper/utils/pem_key_detector.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/utils/util.py` & `credsweeper-1.6.3/credsweeper/utils/util.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/__init__.py` & `credsweeper-1.6.3/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/apply_validation.py` & `credsweeper-1.6.3/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/github_token_validation.py` & `credsweeper-1.6.3/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.6.3/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.6.3/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.6.3/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.6.3/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.6.3/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.6.3/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.6.3/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper/validations/validation.py` & `credsweeper-1.6.3/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/credsweeper.egg-info/PKG-INFO` & `credsweeper-1.6.3/credsweeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.6.2
+Version: 1.6.3
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.6.2/credsweeper.egg-info/SOURCES.txt` & `credsweeper-1.6.3/credsweeper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,29 +40,30 @@
 credsweeper/deep_scanner/lang_scanner.py
 credsweeper/deep_scanner/pdf_scanner.py
 credsweeper/deep_scanner/pkcs12_scanner.py
 credsweeper/deep_scanner/tar_scanner.py
 credsweeper/deep_scanner/xml_scanner.py
 credsweeper/deep_scanner/zip_scanner.py
 credsweeper/file_handler/__init__.py
+credsweeper/file_handler/abstract_provider.py
 credsweeper/file_handler/analysis_target.py
 credsweeper/file_handler/byte_content_provider.py
 credsweeper/file_handler/content_provider.py
 credsweeper/file_handler/data_content_provider.py
 credsweeper/file_handler/descriptor.py
 credsweeper/file_handler/diff_content_provider.py
 credsweeper/file_handler/file_path_extractor.py
 credsweeper/file_handler/files_provider.py
-credsweeper/file_handler/patch_provider.py
+credsweeper/file_handler/patches_provider.py
 credsweeper/file_handler/string_content_provider.py
 credsweeper/file_handler/struct_content_provider.py
 credsweeper/file_handler/text_content_provider.py
-credsweeper/file_handler/text_provider.py
 credsweeper/filters/__init__.py
 credsweeper/filters/filter.py
+credsweeper/filters/line_git_binary_check.py
 credsweeper/filters/line_specific_key_check.py
 credsweeper/filters/separator_unusual_check.py
 credsweeper/filters/value_allowlist_check.py
 credsweeper/filters/value_array_dictionary_check.py
 credsweeper/filters/value_atlassian_token_check.py
 credsweeper/filters/value_base32_data_check.py
 credsweeper/filters/value_base64_data_check.py
@@ -76,14 +77,15 @@
 credsweeper/filters/value_entropy_base32_check.py
 credsweeper/filters/value_entropy_base36_check.py
 credsweeper/filters/value_entropy_base64_check.py
 credsweeper/filters/value_file_path_check.py
 credsweeper/filters/value_first_word_check.py
 credsweeper/filters/value_github_check.py
 credsweeper/filters/value_grafana_check.py
+credsweeper/filters/value_hex_number_check.py
 credsweeper/filters/value_ip_check.py
 credsweeper/filters/value_jfrog_token_check.py
 credsweeper/filters/value_json_web_token_check.py
 credsweeper/filters/value_last_word_check.py
 credsweeper/filters/value_length_check.py
 credsweeper/filters/value_method_check.py
 credsweeper/filters/value_not_allowed_pattern_check.py
```

### Comparing `credsweeper-1.6.2/setup.py` & `credsweeper-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/tests/test_app.py` & `credsweeper-1.6.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.2/tests/test_doc.py` & `credsweeper-1.6.3/tests/test_doc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 import unittest
 
 import deepdiff  # type: ignore
 
 from credsweeper.app import CredSweeper
-from credsweeper.common.constants import Severity
+from credsweeper.file_handler.abstract_provider import AbstractProvider
 from credsweeper.file_handler.files_provider import FilesProvider
-from credsweeper.file_handler.text_provider import TextProvider
 from tests import SAMPLES_PATH
 
 
 class TestDoc(unittest.TestCase):
 
     def setUp(self) -> None:
         self.cred_sweeper = CredSweeper(doc=True, ml_threshold=0)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_secret_pair_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "doc_secret_pair"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "doc_secret_pair"])
         self.cred_sweeper.run(content_provider=content_provider)
         found_credentials = self.cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(18, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_passwd_pair_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "doc_passwd_pair"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "doc_passwd_pair"])
         self.cred_sweeper.run(content_provider=content_provider)
         found_credentials = self.cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(38, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_ip_id_passwd_triple_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "doc_ip_id_password_triple"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "doc_ip_id_password_triple"])
         self.cred_sweeper.run(content_provider=content_provider)
         found_credentials = self.cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(5, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_id_pair_passwd_pair_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "doc_id_pair_passwd_pair"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "doc_id_pair_passwd_pair"])
         self.cred_sweeper.run(content_provider=content_provider)
         found_credentials = self.cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(158, len(found_credentials), found_credentials)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_id_passwd_pair_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "doc_id_passwd_pair"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "doc_id_passwd_pair"])
         self.cred_sweeper.run(content_provider=content_provider)
         found_credentials = self.cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(25, len(found_credentials), found_credentials)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
```

### Comparing `credsweeper-1.6.2/tests/test_main.py` & `credsweeper-1.6.3/tests/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import copy
 import io
-import json
+import io
 import os
 import random
 import shutil
 import tempfile
 import unittest
 from argparse import ArgumentTypeError
 from pathlib import Path
@@ -19,17 +18,17 @@
 from credsweeper import ByteContentProvider, StringContentProvider
 from credsweeper import __main__ as app_main
 from credsweeper.__main__ import EXIT_FAILURE, EXIT_SUCCESS
 from credsweeper.app import APP_PATH
 from credsweeper.app import CredSweeper
 from credsweeper.common.constants import ThresholdPreset, Severity
 from credsweeper.credentials import Candidate
+from credsweeper.file_handler.abstract_provider import AbstractProvider
 from credsweeper.file_handler.files_provider import FilesProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
-from credsweeper.file_handler.text_provider import TextProvider
 from credsweeper.utils import Util
 from tests import SAMPLES_CRED_COUNT, SAMPLES_CRED_LINE_COUNT, SAMPLES_POST_CRED_COUNT, SAMPLES_PATH, AZ_STRING, \
     TESTS_PATH, SAMPLES_IN_DEEP_1, SAMPLES_IN_DEEP_3, SAMPLES_IN_DEEP_2, NEGLIGIBLE_ML_THRESHOLD
 from tests.data import DATA_TEST_CFG
 
 
 class TestMain(unittest.TestCase):
@@ -56,15 +55,15 @@
         cred_sweeper = CredSweeper(api_validation=False)
         self.assertFalse(cred_sweeper.config.api_validation)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_api_validators_p(self) -> None:
         cred_sweeper = CredSweeper(api_validation=True)
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH])
         file_extractors = content_provider.get_scannable_files(cred_sweeper.config)
         candidates: List[Candidate] = []
         for file in file_extractors:
             candidates += cred_sweeper.file_scan(file)
         known_validators: Set[str] = {  #
             "GithubTokenValidation",  #
             "GoogleApiKeyValidation",  #
@@ -159,14 +158,15 @@
                              json_filename=os.path.join(tmp_dir, f"{__name__}.json"),
                              xlsx_filename=None,
                              rule_path=None,
                              jobs=1,
                              ml_threshold=0.0,
                              depth=0,
                              doc=False,
+                             severity="info",
                              size_limit="1G",
                              api_validation=False,
                              denylist_path=None)
             mock_get_arguments.return_value = args_mock
             self.assertEqual(EXIT_SUCCESS, app_main.main())
             self.assertTrue(os.path.exists(os.path.join(tmp_dir, f"{__name__}_deleted.json")))
             self.assertTrue(os.path.exists(os.path.join(tmp_dir, f"{__name__}_added.json")))
@@ -190,14 +190,15 @@
                              xlsx_filename=None,
                              sort_output=False,
                              rule_path=None,
                              jobs=1,
                              ml_threshold=0.0,
                              depth=9,
                              doc=False,
+                             severity="info",
                              size_limit="1G",
                              api_validation=False,
                              denylist_path=None)
             mock_get_arguments.return_value = args_mock
             self.assertEqual(EXIT_SUCCESS, app_main.main())
             self.assertTrue(os.path.exists(os.path.join(tmp_dir, f"{__name__}_deleted.json")))
             self.assertTrue(os.path.exists(os.path.join(tmp_dir, f"{__name__}_added.json")))
@@ -299,14 +300,20 @@
 
     def test_threshold_or_float_n(self):
         with pytest.raises(ArgumentTypeError):
             app_main.threshold_or_float("DUMMY STRING")
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
+    def test_wrong_severity_n(self) -> None:
+        with self.assertRaises(RuntimeError):
+            CredSweeper(severity="wrong")
+
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
     def test_scan_bytes_p(self) -> None:
         to_scan = b"line one\npassword='in_line_2'"
         cred_sweeper = CredSweeper()
         provider = ByteContentProvider(to_scan)
         results = cred_sweeper.file_scan(provider)
         self.assertEqual(1, len(results))
         self.assertEqual("Password", results[0].rule_name)
@@ -367,241 +374,241 @@
         containers_extension_conflict = set(exclude_extension_items).intersection(exclude_containers_items)
         self.assertSetEqual(set(), containers_extension_conflict)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_multi_jobs_p(self) -> None:
         # real result might be shown in code coverage
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH])
         cred_sweeper = CredSweeper(pool_count=3)
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(SAMPLES_POST_CRED_COUNT, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_find_by_ext_p(self) -> None:
         # test for finding files by extension
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH])
         cred_sweeper = CredSweeper(find_by_ext=True)
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(SAMPLES_POST_CRED_COUNT + 3, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_find_by_ext_n(self) -> None:
         # test for finding files by extension
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH])
         cred_sweeper = CredSweeper(find_by_ext=False)
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(SAMPLES_POST_CRED_COUNT, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_tar_p(self) -> None:
         # deep scan in tar file. First level is bz2 archive to hide credentials with inflate
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "passwords.tar.bz2"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "passwords.tar.bz2"])
         cred_sweeper = CredSweeper(depth=2, ml_threshold=0)
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(3, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_tar_n(self) -> None:
         # test for bad tar - throws exception
         file_path = SAMPLES_PATH / "bad.tar.bz2"
-        content_provider: FilesProvider = TextProvider([file_path])
+        content_provider: AbstractProvider = FilesProvider([file_path])
         cred_sweeper = CredSweeper(depth=2)
         with patch('logging.Logger.error') as mocked_logger:
             cred_sweeper.run(content_provider=content_provider)
             self.assertEqual(0, len(cred_sweeper.credential_manager.get_credentials()))
             mocked_logger.assert_called_with(f"{file_path}:unexpected end of data")
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_p(self) -> None:
         # test for finding files with --depth
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH])
         cred_sweeper = CredSweeper(depth=1)
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(SAMPLES_IN_DEEP_1, len(cred_sweeper.credential_manager.get_credentials()))
         cred_sweeper.config.depth = 2
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(SAMPLES_IN_DEEP_2, len(cred_sweeper.credential_manager.get_credentials()))
         cred_sweeper.config.depth = 3
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(SAMPLES_IN_DEEP_3, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_n(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH])
         cred_sweeper = CredSweeper(depth=0)
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(SAMPLES_POST_CRED_COUNT, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_bzip2_p(self) -> None:
         # test for finding files by extension
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "pem_key.bz2"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "pem_key.bz2"])
         cred_sweeper = CredSweeper(depth=1)
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(1, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_bzip2_n(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             test_filename = os.path.join(tmp_dir, __name__)
             self.assertFalse(os.path.exists(test_filename))
             with open(test_filename, "wb") as f:
                 f.write(b"\x42\x5A\x68\x35\x31\x41\x59\x26\x53\x59")
-            content_provider: FilesProvider = TextProvider([test_filename])
+            content_provider: AbstractProvider = FilesProvider([test_filename])
             cred_sweeper = CredSweeper(depth=1)
             with patch('logging.Logger.error') as mocked_logger:
                 cred_sweeper.run(content_provider=content_provider)
                 mocked_logger.assert_called_with(
                     f"{test_filename}:Compressed data ended before the end-of-stream marker was reached")
             self.assertEqual(0, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_eml_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.eml"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "test.eml"])
         cred_sweeper = CredSweeper(doc=True)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(1, len(found_credentials))
         self.assertEqual("PW: H1ddEn#ema1l", found_credentials[0].line_data_list[0].line)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_pdf_p(self) -> None:
         # may be tested with
         # https://www.dcc.edu/documents/administration/offices/information-technology/password-examples.pdf
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "sample.pdf"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "sample.pdf"])
         cred_sweeper = CredSweeper(depth=33)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertSetEqual({"AWS Client ID", "Password", "Github Classic Token"},
                             set(i.rule_name for i in found_credentials))
         self.assertSetEqual({"Xdj@jcN834b", "AKIAGIREOGIAWSKEY123", "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"},
                             set(i.line_data_list[0].value for i in found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_pdf_n(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "sample.pdf"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "sample.pdf"])
         cred_sweeper = CredSweeper()
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(0, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_py_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "sample.py"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "sample.py"])
         cred_sweeper = CredSweeper(depth=3, ml_threshold=ThresholdPreset.lowest)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(1, len(found_credentials))
         self.assertSetEqual({"Password"}, set(i.rule_name for i in found_credentials))
         self.assertSetEqual({"WeR15tr0n6"}, set(i.line_data_list[0].value for i in found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_py_n(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "sample.py"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "sample.py"])
         cred_sweeper = CredSweeper()
         cred_sweeper.run(content_provider=content_provider)
         self.assertEqual(0, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_json_p(self) -> None:
         # test for finding credentials in JSON
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "struct.json"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "struct.json"])
         cred_sweeper = CredSweeper(depth=5)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(1, len(found_credentials))
         self.assertSetEqual({"Password"}, set(i.rule_name for i in found_credentials))
         self.assertSetEqual({"Axt4T0eO0lm9sS=="}, set(i.line_data_list[0].value for i in found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_json_n(self) -> None:
         # test to prove that no credentials are found without depth
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "struct.json"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "struct.json"])
         cred_sweeper = CredSweeper()
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(0, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_yaml_p(self) -> None:
         # test for finding credentials in YAML
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "binary.yaml"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "binary.yaml"])
         cred_sweeper = CredSweeper(depth=5)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(2, len(found_credentials))
         self.assertSetEqual({"Secret", "PEM Private Key"}, set(i.rule_name for i in found_credentials))
         self.assertSetEqual({"we5345d0f3da48544z1t1e275y05i161x995q485\n", "-----BEGIN RSA PRIVATE KEY-----"},
                             set(i.line_data_list[0].value for i in found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_yaml_n(self) -> None:
         # test to prove that no credentials are found without depth
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "binary.yaml"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "binary.yaml"])
         cred_sweeper = CredSweeper()
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(0, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_encoded_p(self) -> None:
         # test for finding credentials in ENCODED data
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "encoded_data"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "encoded_data"])
         cred_sweeper = CredSweeper(depth=5, ml_threshold=0)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(2, len(found_credentials))
         self.assertSetEqual({"Token", "Github Old Token"}, set(i.rule_name for i in found_credentials))
         self.assertEqual("gireogicracklecrackle1231567190113413981", found_credentials[0].line_data_list[0].value)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_docx_p(self) -> None:
         # test for finding credentials in docx
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "sample.docx"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "sample.docx"])
         cred_sweeper = CredSweeper(doc=True)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(2, len(found_credentials))
         self.assertEqual("WeR15tr0n6", found_credentials[0].line_data_list[0].value)
         self.assertEqual("ghs_00000000000000000000000000000004WZ4EQ", found_credentials[1].line_data_list[0].value)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_docx_n(self) -> None:
         # test docx  - no credential should be found without 'doc'
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "sample.docx"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "sample.docx"])
         cred_sweeper = CredSweeper(doc=False)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(0, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_html_p(self) -> None:
         # test for finding credentials in html
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.html"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "test.html"])
         cred_sweeper = CredSweeper(depth=5, ml_threshold=0)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         expected_credential_lines = [
             "508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0",
             "secret = Ndjbwu88s22ygavsdhgt5454v3h1x",
             "password = Cr3DeHTbIal",
@@ -624,15 +631,15 @@
             expected_credential_lines.remove(cred.line_data_list[0].line)
         self.assertEqual(0, len(expected_credential_lines), expected_credential_lines)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_html_n(self) -> None:
         # test_html  - no credential should be found without 'depth'
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.html"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "test.html"])
         cred_sweeper = CredSweeper()
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(0, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
     def test_exclude_value_p(self) -> None:
@@ -668,15 +675,15 @@
         files_provider = [TextContentProvider(file_path) for file_path in files]
         cred_sweeper.scan(files_provider)
         self.assertEqual(1, len(cred_sweeper.credential_manager.get_credentials()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_doc_p(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.html"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "test.html"])
         cred_sweeper = CredSweeper(doc=True)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         expected_credential_values = {
             "508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0",
             "ya29.dshMb48ehfXwydAj34D32J",
             "dop_v1_425522a565f532bc6532d453422e50334a42f5242a3090fbe553b543b124259b",
@@ -684,15 +691,15 @@
             "MU$T6Ef09#D!",
         }
         self.assertSetEqual(expected_credential_values, set(x.line_data_list[0].value for x in found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_doc_n(self) -> None:
-        content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.html"])
+        content_provider: AbstractProvider = FilesProvider([SAMPLES_PATH / "test.html"])
         cred_sweeper = CredSweeper(doc=False)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(0, len(found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
@@ -740,15 +747,15 @@
                 expected_result = Util.json_load(expected_report)
                 # informative parameter, relative with other tests counters. CredSweeper does not know it and fails
                 cred_count = cfg.pop("__cred_count")
                 prepare(expected_result)
                 tmp_file = Path(tmp_dir) / cfg["json_filename"]
                 # apply the current path to keep equivalence in path
                 os.chdir(TESTS_PATH.parent)
-                content_provider: FilesProvider = TextProvider(["tests/samples"])
+                content_provider: AbstractProvider = FilesProvider(["tests/samples"])
                 # replace output report file to place in tmp_dir
                 cfg["json_filename"] = str(tmp_file)
                 cred_sweeper = CredSweeper(**cfg)
                 cred_sweeper.run(content_provider=content_provider)
                 test_result = Util.json_load(tmp_file)
                 prepare(test_result)
                 # use the same dump as in output
@@ -762,21 +769,47 @@
                 # first run fails with the diff but next run will pass
                 self.assertDictEqual(diff, {}, cfg)
                 # only count of items must be corrected manually
                 self.assertEqual(cred_count, len(expected_result), cfg["json_filename"])
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
+    def test_param_n(self) -> None:
+        # internal parametrized tests for quick debug - no itms should be found
+        items = [  #
+            ("test.template", b" API_KEY_ID=00209332 "),  #
+            ("test.template", b" AUTH_API_KEY_NAME='temporally_secret_api' "),  #
+            ("pager.ts", b"pagerLimitKey: 'size',"),  #
+            ("pager.rs", b'    this_circleci_pass_secret_id="buratino-circle-pass"'),  #
+            ("pager.rs", b'      secret_type: "odobo".to_string(),'),  #
+            ("pager.rs", b"   secret_key: impl AsRef<str>,   "),  #
+            ("pager.rs", b"token: impl AsRef<str>,"),  #
+            ("pager.rs", b"    let tokens = quote::quote! {"),  #
+            ("pager.rs", b"  let cert_chain = x509_rx"),  #
+        ]
+        content_provider: AbstractProvider = FilesProvider([(file_name, io.BytesIO(data_line))
+                                                            for file_name, data_line in items])
+        cred_sweeper = CredSweeper()
+        cred_sweeper.run(content_provider=content_provider)
+        creds = cred_sweeper.credential_manager.get_credentials()
+        self.assertFalse(len(creds), [x for x in creds])
+
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
     def test_param_p(self) -> None:
-        # internal parametrized tests to keep
-        items = [("    STP_PASSWORD=qbgomdtpqch \\", "qbgomdtpqch")]
-        for i in items:
-            content_provider: FilesProvider = TextProvider([
-                ("test.template", io.BytesIO(i[0].encode())),
+        # internal parametrized tests for quick debug
+        items = [("test.template", b"    STP_PASSWORD=qbgomdtpqch \\", "STP_PASSWORD", "qbgomdtpqch"),
+                 ("accept.py", b"password='Ahga%$FiQ@Ei8'", "password", "Ahga%$FiQ@Ei8"),
+                 ("test.template", b" NAMED_API_KEY=qii7t1m6423127xto389xc914l34451qz5135865564sg ", "NAMED_API_KEY",
+                  "qii7t1m6423127xto389xc914l34451qz5135865564sg")]
+        for file_name, data_line, variable, value in items:
+            content_provider: AbstractProvider = FilesProvider([
+                (file_name, io.BytesIO(data_line)),
             ])
-            cred_sweeper = CredSweeper(ml_threshold=0)
+            cred_sweeper = CredSweeper()
             cred_sweeper.run(content_provider=content_provider)
             creds = cred_sweeper.credential_manager.get_credentials()
-            self.assertLessEqual(1, len(creds))
-            self.assertEqual(i[1], creds[0].line_data_list[0].value)
+            self.assertLessEqual(1, len(creds), data_line)
+            self.assertEqual(variable, creds[0].line_data_list[0].variable)
+            self.assertEqual(value, creds[0].line_data_list[0].value)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
```


# Comparing `tmp/octoai-0.0.1.tar.gz` & `tmp/octoai-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai-0.0.1.tar", max compression
+gzip compressed data, was "octoai-0.0.60.tar", max compression
```

## Comparing `octoai-0.0.1.tar` & `octoai-0.0.60.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     4931 2024-04-20 02:36:47.617504 octoai-0.0.1/README.md
--rw-r--r--   0        0        0      650 2024-04-20 02:36:47.617504 octoai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      302 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/__init__.py
--rw-r--r--   0        0        0    34720 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/client.py
--rw-r--r--   0        0        0      170 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2925 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/__init__.py
--rw-r--r--   0        0        0     2134 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/asset.py
--rw-r--r--   0        0        0      201 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/asset_type.py
--rw-r--r--   0        0        0      646 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/base_engine.py
--rw-r--r--   0        0        0      164 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/base_engine_type.py
--rw-r--r--   0        0        0     1241 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/checkpoint_data.py
--rw-r--r--   0        0        0      891 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/complete_asset_upload_response.py
--rw-r--r--   0        0        0     1257 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/create_asset_response.py
--rw-r--r--   0        0        0     1218 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/create_asset_response_transfer_api.py
--rw-r--r--   0        0        0     1870 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/data.py
--rw-r--r--   0        0        0      164 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/data_type.py
--rw-r--r--   0        0        0      986 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/delete_asset_response.py
--rw-r--r--   0        0        0     1133 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/file_data.py
--rw-r--r--   0        0        0      191 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/file_extension.py
--rw-r--r--   0        0        0      155 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/file_format.py
--rw-r--r--   0        0        0      181 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/file_structure.py
--rw-r--r--   0        0        0      955 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/http_validation_error.py
--rw-r--r--   0        0        0     1098 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/latent_data.py
--rw-r--r--   0        0        0     1137 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/list_assets_response.py
--rw-r--r--   0        0        0     1296 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/lora_data.py
--rw-r--r--   0        0        0     1096 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/no_transfer_api.py
--rw-r--r--   0        0        0     1003 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/presigned_url_transfer_api.py
--rw-r--r--   0        0        0     1128 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/retrieve_asset_response.py
--rw-r--r--   0        0        0     1241 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/retrieve_asset_response_transfer_api.py
--rw-r--r--   0        0        0      221 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/status.py
--rw-r--r--   0        0        0     1505 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/sts_transfer_api.py
--rw-r--r--   0        0        0     1370 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/textual_inversion_data.py
--rw-r--r--   0        0        0      163 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/transfer_api_type.py
--rw-r--r--   0        0        0     1234 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/vae_data.py
--rw-r--r--   0        0        0      974 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/asset_lake/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     5520 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/base_client.py
--rw-r--r--   0        0        0     3804 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/client.py
--rw-r--r--   0        0        0      853 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/api_error.py
--rw-r--r--   0        0        0     2224 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/core/request_options.py
--rw-r--r--   0        0        0      500 2024-04-20 02:36:47.617504 octoai-0.0.1/src/octoai/environment.py
--rw-r--r--   0        0        0     1032 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/__init__.py
--rw-r--r--   0        0        0    29452 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/client.py
--rw-r--r--   0        0        0      170 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     1266 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/__init__.py
--rw-r--r--   0        0        0      671 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/base_engine.py
--rw-r--r--   0        0        0      826 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/details.py
--rw-r--r--   0        0        0      955 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/http_validation_error.py
--rw-r--r--   0        0        0     1189 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/list_tunes_response.py
--rw-r--r--   0        0        0     1592 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/lora_tune.py
--rw-r--r--   0        0        0     1111 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/lora_tune_checkpoint.py
--rw-r--r--   0        0        0     1039 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/lora_tune_file.py
--rw-r--r--   0        0        0     1062 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py
--rw-r--r--   0        0        0     2273 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/tune.py
--rw-r--r--   0        0        0      846 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/tune_details.py
--rw-r--r--   0        0        0     1122 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/tune_result.py
--rw-r--r--   0        0        0      192 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/tune_status.py
--rw-r--r--   0        0        0      259 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/tune_type.py
--rw-r--r--   0        0        0      974 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/fine_tuning/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      668 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/__init__.py
--rw-r--r--   0        0        0    28997 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/client.py
--rw-r--r--   0        0        0      170 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      848 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/__init__.py
--rw-r--r--   0        0        0      955 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/http_validation_error.py
--rw-r--r--   0        0        0      152 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/image_encoding.py
--rw-r--r--   0        0        0     1245 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/image_generation.py
--rw-r--r--   0        0        0     4770 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/image_generation_request.py
--rw-r--r--   0        0        0      162 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/image_generation_request_seed.py
--rw-r--r--   0        0        0     1205 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/image_generation_response.py
--rw-r--r--   0        0        0      514 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/scheduler.py
--rw-r--r--   0        0        0     1880 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/sdxl_styles.py
--rw-r--r--   0        0        0      974 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/image_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0        0 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/py.typed
--rw-r--r--   0        0        0     1528 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/__init__.py
--rw-r--r--   0        0        0    53805 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/client.py
--rw-r--r--   0        0        0      248 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/errors/__init__.py
--rw-r--r--   0        0        0      290 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/errors/internal_server_error.py
--rw-r--r--   0        0        0      314 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2131 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_choice.py
--rw-r--r--   0        0        0     1815 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_chunk.py
--rw-r--r--   0        0        0     1133 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_chunk_choice.py
--rw-r--r--   0        0        0     1100 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_delta.py
--rw-r--r--   0        0        0     1118 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_request_ext.py
--rw-r--r--   0        0        0     1143 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py
--rw-r--r--   0        0        0     1185 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_response.py
--rw-r--r--   0        0        0     1054 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_completion_response_format.py
--rw-r--r--   0        0        0      947 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_fn_call.py
--rw-r--r--   0        0        0     1061 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/chat_message.py
--rw-r--r--   0        0        0      996 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/completion_choice.py
--rw-r--r--   0        0        0     1311 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/completion_response.py
--rw-r--r--   0        0        0      163 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/create_chat_completion_request_function_call.py
--rw-r--r--   0        0        0      169 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/create_chat_completion_stream_request_function_call.py
--rw-r--r--   0        0        0     1265 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/error_response.py
--rw-r--r--   0        0        0      153 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/error_response_validation_errors_value.py
--rw-r--r--   0        0        0      197 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/finish_reason.py
--rw-r--r--   0        0        0      982 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/function.py
--rw-r--r--   0        0        0      955 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/http_validation_error.py
--rw-r--r--   0        0        0     1178 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/log_probs.py
--rw-r--r--   0        0        0      174 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/prompt.py
--rw-r--r--   0        0        0      123 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/stop.py
--rw-r--r--   0        0        0      964 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/usage_stats.py
--rw-r--r--   0        0        0      974 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/text_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     7585 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/uploading_asset_lake.py
--rw-r--r--   0        0        0       74 2024-04-20 02:36:47.621505 octoai-0.0.1/src/octoai/version.py
--rw-r--r--   0        0        0     5535 1970-01-01 00:00:00.000000 octoai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4931 2024-04-23 20:23:31.068536 octoai-0.0.60/README.md
+-rw-r--r--   0        0        0      651 2024-04-23 20:23:31.068536 octoai-0.0.60/pyproject.toml
+-rw-r--r--   0        0        0      302 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/__init__.py
+-rw-r--r--   0        0        0    34720 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/client.py
+-rw-r--r--   0        0        0      170 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2925 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/__init__.py
+-rw-r--r--   0        0        0     2134 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/asset.py
+-rw-r--r--   0        0        0      201 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/asset_type.py
+-rw-r--r--   0        0        0      646 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/base_engine.py
+-rw-r--r--   0        0        0      164 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/base_engine_type.py
+-rw-r--r--   0        0        0     1241 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/checkpoint_data.py
+-rw-r--r--   0        0        0      891 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/complete_asset_upload_response.py
+-rw-r--r--   0        0        0     1257 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/create_asset_response.py
+-rw-r--r--   0        0        0     1218 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/create_asset_response_transfer_api.py
+-rw-r--r--   0        0        0     1870 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/data.py
+-rw-r--r--   0        0        0      164 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/data_type.py
+-rw-r--r--   0        0        0      986 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/delete_asset_response.py
+-rw-r--r--   0        0        0     1133 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/file_data.py
+-rw-r--r--   0        0        0      191 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/file_extension.py
+-rw-r--r--   0        0        0      155 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/file_format.py
+-rw-r--r--   0        0        0      181 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/file_structure.py
+-rw-r--r--   0        0        0      955 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/http_validation_error.py
+-rw-r--r--   0        0        0     1098 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/latent_data.py
+-rw-r--r--   0        0        0     1137 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/list_assets_response.py
+-rw-r--r--   0        0        0     1296 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/lora_data.py
+-rw-r--r--   0        0        0     1096 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/no_transfer_api.py
+-rw-r--r--   0        0        0     1003 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/presigned_url_transfer_api.py
+-rw-r--r--   0        0        0     1128 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/retrieve_asset_response.py
+-rw-r--r--   0        0        0     1241 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/retrieve_asset_response_transfer_api.py
+-rw-r--r--   0        0        0      221 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/status.py
+-rw-r--r--   0        0        0     1505 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/sts_transfer_api.py
+-rw-r--r--   0        0        0     1370 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/textual_inversion_data.py
+-rw-r--r--   0        0        0      163 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/transfer_api_type.py
+-rw-r--r--   0        0        0     1234 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/vae_data.py
+-rw-r--r--   0        0        0      974 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/asset_lake/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     5520 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/base_client.py
+-rw-r--r--   0        0        0     3804 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/client.py
+-rw-r--r--   0        0        0      853 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/api_error.py
+-rw-r--r--   0        0        0     2225 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/core/request_options.py
+-rw-r--r--   0        0        0      500 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/environment.py
+-rw-r--r--   0        0        0     1032 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/__init__.py
+-rw-r--r--   0        0        0    29452 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/client.py
+-rw-r--r--   0        0        0      170 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     1266 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/base_engine.py
+-rw-r--r--   0        0        0      826 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/details.py
+-rw-r--r--   0        0        0      955 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/http_validation_error.py
+-rw-r--r--   0        0        0     1189 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/list_tunes_response.py
+-rw-r--r--   0        0        0     1592 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune.py
+-rw-r--r--   0        0        0     1111 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune_checkpoint.py
+-rw-r--r--   0        0        0     1039 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune_file.py
+-rw-r--r--   0        0        0     1062 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py
+-rw-r--r--   0        0        0     2273 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/tune.py
+-rw-r--r--   0        0        0      846 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/tune_details.py
+-rw-r--r--   0        0        0     1122 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/tune_result.py
+-rw-r--r--   0        0        0      192 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/tune_status.py
+-rw-r--r--   0        0        0      259 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/tune_type.py
+-rw-r--r--   0        0        0      974 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/fine_tuning/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      668 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/__init__.py
+-rw-r--r--   0        0        0    28997 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/client.py
+-rw-r--r--   0        0        0      170 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      848 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/__init__.py
+-rw-r--r--   0        0        0      955 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/http_validation_error.py
+-rw-r--r--   0        0        0      152 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/image_encoding.py
+-rw-r--r--   0        0        0     1245 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/image_generation.py
+-rw-r--r--   0        0        0     4770 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/image_generation_request.py
+-rw-r--r--   0        0        0      162 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/image_generation_request_seed.py
+-rw-r--r--   0        0        0     1205 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/image_generation_response.py
+-rw-r--r--   0        0        0      514 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/scheduler.py
+-rw-r--r--   0        0        0     1880 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/sdxl_styles.py
+-rw-r--r--   0        0        0      974 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/image_gen/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/py.typed
+-rw-r--r--   0        0        0     1528 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/__init__.py
+-rw-r--r--   0        0        0    53805 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/client.py
+-rw-r--r--   0        0        0      248 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/errors/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/errors/internal_server_error.py
+-rw-r--r--   0        0        0      314 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2131 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/types/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_choice.py
+-rw-r--r--   0        0        0     1815 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_chunk.py
+-rw-r--r--   0        0        0     1133 2024-04-23 20:23:31.068536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_chunk_choice.py
+-rw-r--r--   0        0        0     1100 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_delta.py
+-rw-r--r--   0        0        0     1118 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_request_ext.py
+-rw-r--r--   0        0        0     1143 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py
+-rw-r--r--   0        0        0     1185 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_response.py
+-rw-r--r--   0        0        0     1054 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/chat_completion_response_format.py
+-rw-r--r--   0        0        0      947 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/chat_fn_call.py
+-rw-r--r--   0        0        0     1061 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/chat_message.py
+-rw-r--r--   0        0        0      996 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/completion_choice.py
+-rw-r--r--   0        0        0     1311 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/completion_response.py
+-rw-r--r--   0        0        0      163 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/create_chat_completion_request_function_call.py
+-rw-r--r--   0        0        0      169 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/create_chat_completion_stream_request_function_call.py
+-rw-r--r--   0        0        0     1265 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/error_response.py
+-rw-r--r--   0        0        0      153 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/error_response_validation_errors_value.py
+-rw-r--r--   0        0        0      197 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/finish_reason.py
+-rw-r--r--   0        0        0      982 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/function.py
+-rw-r--r--   0        0        0      955 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/http_validation_error.py
+-rw-r--r--   0        0        0     1178 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/log_probs.py
+-rw-r--r--   0        0        0      174 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/prompt.py
+-rw-r--r--   0        0        0      123 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/stop.py
+-rw-r--r--   0        0        0      964 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/usage_stats.py
+-rw-r--r--   0        0        0      974 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/text_gen/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     7585 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/uploading_asset_lake.py
+-rw-r--r--   0        0        0       74 2024-04-23 20:23:31.072536 octoai-0.0.60/src/octoai/version.py
+-rw-r--r--   0        0        0     5536 1970-01-01 00:00:00.000000 octoai-0.0.60/PKG-INFO
```

### Comparing `octoai-0.0.1/README.md` & `octoai-0.0.60/README.md`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/pyproject.toml` & `octoai-0.0.60/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octoai"
-version = "0.0.1"
+version = "0.0.60"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "octoai", from = "src"}
 ]
```

### Comparing `octoai-0.0.1/src/octoai/asset_lake/__init__.py` & `octoai-0.0.60/src/octoai/asset_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/client.py` & `octoai-0.0.60/src/octoai/asset_lake/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/__init__.py` & `octoai-0.0.60/src/octoai/asset_lake/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/asset.py` & `octoai-0.0.60/src/octoai/asset_lake/types/asset.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/base_engine.py` & `octoai-0.0.60/src/octoai/asset_lake/types/base_engine.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/checkpoint_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/checkpoint_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/complete_asset_upload_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/complete_asset_upload_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/create_asset_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/create_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/create_asset_response_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/create_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/delete_asset_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/delete_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/file_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/file_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/asset_lake/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/latent_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/latent_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/list_assets_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/list_assets_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/lora_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/lora_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/no_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/no_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/presigned_url_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/presigned_url_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/retrieve_asset_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/retrieve_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/retrieve_asset_response_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/retrieve_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/sts_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/sts_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/textual_inversion_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/textual_inversion_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/vae_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/vae_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/asset_lake/types/validation_error.py` & `octoai-0.0.60/src/octoai/asset_lake/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/base_client.py` & `octoai-0.0.60/src/octoai/base_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,17 @@
             httpx_client=httpx_client
             if httpx_client is not None
             else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.Client(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
-        self.asset_lake = AssetLakeClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = FineTuningClient(client_wrapper=self._client_wrapper)
         self.image_gen = ImageGenClient(client_wrapper=self._client_wrapper)
+        self.asset_lake = AssetLakeClient(client_wrapper=self._client_wrapper)
         self.text_gen = TextGenClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseOctoAI:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
@@ -103,11 +103,11 @@
             httpx_client=httpx_client
             if httpx_client is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
-        self.asset_lake = AsyncAssetLakeClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = AsyncFineTuningClient(client_wrapper=self._client_wrapper)
         self.image_gen = AsyncImageGenClient(client_wrapper=self._client_wrapper)
+        self.asset_lake = AsyncAssetLakeClient(client_wrapper=self._client_wrapper)
         self.text_gen = AsyncTextGenClient(client_wrapper=self._client_wrapper)
```

### Comparing `octoai-0.0.1/src/octoai/client.py` & `octoai-0.0.60/src/octoai/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/core/__init__.py` & `octoai-0.0.60/src/octoai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/core/client_wrapper.py` & `octoai-0.0.60/src/octoai/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._environment = environment
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "octoai",
-            "X-Fern-SDK-Version": "0.0.1",
+            "X-Fern-SDK-Version": "0.0.60",
         }
         api_key = self._get_api_key()
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
         return headers
 
     def _get_api_key(self) -> typing.Optional[str]:
```

### Comparing `octoai-0.0.1/src/octoai/core/datetime_utils.py` & `octoai-0.0.60/src/octoai/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/core/file.py` & `octoai-0.0.60/src/octoai/core/file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/core/http_client.py` & `octoai-0.0.60/src/octoai/core/http_client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/core/jsonable_encoder.py` & `octoai-0.0.60/src/octoai/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/core/request_options.py` & `octoai-0.0.60/src/octoai/core/request_options.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/__init__.py` & `octoai-0.0.60/src/octoai/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/client.py` & `octoai-0.0.60/src/octoai/fine_tuning/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/__init__.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/base_engine.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/base_engine.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/details.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/list_tunes_response.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/list_tunes_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/lora_tune.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/lora_tune_checkpoint.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune_checkpoint.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/lora_tune_file.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune_file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/tune.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/tune_details.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/tune_details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/tune_result.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/tune_result.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/fine_tuning/types/validation_error.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/__init__.py` & `octoai-0.0.60/src/octoai/image_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/client.py` & `octoai-0.0.60/src/octoai/image_gen/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/__init__.py` & `octoai-0.0.60/src/octoai/image_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/image_gen/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/image_generation.py` & `octoai-0.0.60/src/octoai/image_gen/types/image_generation.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/image_generation_request.py` & `octoai-0.0.60/src/octoai/image_gen/types/image_generation_request.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/image_generation_response.py` & `octoai-0.0.60/src/octoai/image_gen/types/image_generation_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/scheduler.py` & `octoai-0.0.60/src/octoai/image_gen/types/scheduler.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/sdxl_styles.py` & `octoai-0.0.60/src/octoai/image_gen/types/sdxl_styles.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/image_gen/types/validation_error.py` & `octoai-0.0.60/src/octoai/image_gen/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/__init__.py` & `octoai-0.0.60/src/octoai/text_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/client.py` & `octoai-0.0.60/src/octoai/text_gen/client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/__init__.py` & `octoai-0.0.60/src/octoai/text_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_choice.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_chunk.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_chunk_choice.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_chunk_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_delta.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_delta.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_request_ext.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_request_ext.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_response.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_completion_response_format.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_response_format.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_fn_call.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_fn_call.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/chat_message.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/completion_choice.py` & `octoai-0.0.60/src/octoai/text_gen/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/completion_response.py` & `octoai-0.0.60/src/octoai/text_gen/types/completion_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/error_response.py` & `octoai-0.0.60/src/octoai/text_gen/types/error_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/function.py` & `octoai-0.0.60/src/octoai/text_gen/types/function.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/text_gen/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/log_probs.py` & `octoai-0.0.60/src/octoai/text_gen/types/log_probs.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/usage_stats.py` & `octoai-0.0.60/src/octoai/text_gen/types/usage_stats.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/text_gen/types/validation_error.py` & `octoai-0.0.60/src/octoai/text_gen/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/src/octoai/uploading_asset_lake.py` & `octoai-0.0.60/src/octoai/uploading_asset_lake.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.1/PKG-INFO` & `octoai-0.0.60/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoai
-Version: 0.0.1
+Version: 0.0.60
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


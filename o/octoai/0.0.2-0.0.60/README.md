# Comparing `tmp/octoai-0.0.2.tar.gz` & `tmp/octoai-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai-0.0.2.tar", max compression
+gzip compressed data, was "octoai-0.0.60.tar", max compression
```

## Comparing `octoai-0.0.2.tar` & `octoai-0.0.60.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     4922 2024-04-24 19:06:36.158961 octoai-0.0.2/README.md
--rw-r--r--   0        0        0      649 2024-04-24 19:06:36.158961 octoai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      308 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/__init__.py
--rw-r--r--   0        0        0    34872 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/client.py
--rw-r--r--   0        0        0      170 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2925 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/__init__.py
--rw-r--r--   0        0        0     2134 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/asset.py
--rw-r--r--   0        0        0      201 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/asset_type.py
--rw-r--r--   0        0        0      646 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/base_engine.py
--rw-r--r--   0        0        0      164 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/base_engine_type.py
--rw-r--r--   0        0        0     1241 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/checkpoint_data.py
--rw-r--r--   0        0        0      891 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/complete_asset_upload_response.py
--rw-r--r--   0        0        0     1257 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/create_asset_response.py
--rw-r--r--   0        0        0     1218 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/create_asset_response_transfer_api.py
--rw-r--r--   0        0        0     1870 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/data.py
--rw-r--r--   0        0        0      164 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/data_type.py
--rw-r--r--   0        0        0      986 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/delete_asset_response.py
--rw-r--r--   0        0        0     1133 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/file_data.py
--rw-r--r--   0        0        0      191 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/file_extension.py
--rw-r--r--   0        0        0      155 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/file_format.py
--rw-r--r--   0        0        0      181 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/file_structure.py
--rw-r--r--   0        0        0      955 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/http_validation_error.py
--rw-r--r--   0        0        0     1098 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/latent_data.py
--rw-r--r--   0        0        0     1137 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/list_assets_response.py
--rw-r--r--   0        0        0     1296 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/lora_data.py
--rw-r--r--   0        0        0     1096 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/no_transfer_api.py
--rw-r--r--   0        0        0     1003 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/presigned_url_transfer_api.py
--rw-r--r--   0        0        0     1128 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/retrieve_asset_response.py
--rw-r--r--   0        0        0     1241 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py
--rw-r--r--   0        0        0      221 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/status.py
--rw-r--r--   0        0        0     1505 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/sts_transfer_api.py
--rw-r--r--   0        0        0     1370 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/textual_inversion_data.py
--rw-r--r--   0        0        0      163 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/transfer_api_type.py
--rw-r--r--   0        0        0     1234 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/vae_data.py
--rw-r--r--   0        0        0      974 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-24 19:06:36.158961 octoai-0.0.2/src/octoai/asset_library/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     5541 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/base_client.py
--rw-r--r--   0        0        0     3834 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/client.py
--rw-r--r--   0        0        0      853 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/api_error.py
--rw-r--r--   0        0        0     2224 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/core/request_options.py
--rw-r--r--   0        0        0      500 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/environment.py
--rw-r--r--   0        0        0     1032 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/__init__.py
--rw-r--r--   0        0        0    29562 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/client.py
--rw-r--r--   0        0        0      170 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     1266 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/__init__.py
--rw-r--r--   0        0        0      671 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/base_engine.py
--rw-r--r--   0        0        0      826 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/details.py
--rw-r--r--   0        0        0      955 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/http_validation_error.py
--rw-r--r--   0        0        0     1189 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/list_tunes_response.py
--rw-r--r--   0        0        0     1592 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/lora_tune.py
--rw-r--r--   0        0        0     1111 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/lora_tune_checkpoint.py
--rw-r--r--   0        0        0     1039 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/lora_tune_file.py
--rw-r--r--   0        0        0     1062 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py
--rw-r--r--   0        0        0     2273 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/tune.py
--rw-r--r--   0        0        0      846 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/tune_details.py
--rw-r--r--   0        0        0     1122 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/tune_result.py
--rw-r--r--   0        0        0      192 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/tune_status.py
--rw-r--r--   0        0        0      259 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/tune_type.py
--rw-r--r--   0        0        0      974 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/fine_tuning/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      668 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/__init__.py
--rw-r--r--   0        0        0    29227 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/client.py
--rw-r--r--   0        0        0      170 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      848 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/__init__.py
--rw-r--r--   0        0        0      955 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/http_validation_error.py
--rw-r--r--   0        0        0      152 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/image_encoding.py
--rw-r--r--   0        0        0     1245 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/image_generation.py
--rw-r--r--   0        0        0     4770 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/image_generation_request.py
--rw-r--r--   0        0        0      162 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/image_generation_request_seed.py
--rw-r--r--   0        0        0     1205 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/image_generation_response.py
--rw-r--r--   0        0        0      514 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/scheduler.py
--rw-r--r--   0        0        0     1880 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/sdxl_styles.py
--rw-r--r--   0        0        0      974 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/image_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0        0 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/py.typed
--rw-r--r--   0        0        0     1528 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/__init__.py
--rw-r--r--   0        0        0    53893 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/client.py
--rw-r--r--   0        0        0      248 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/errors/__init__.py
--rw-r--r--   0        0        0      290 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/errors/internal_server_error.py
--rw-r--r--   0        0        0      314 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2131 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_choice.py
--rw-r--r--   0        0        0     1815 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_chunk.py
--rw-r--r--   0        0        0     1133 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_chunk_choice.py
--rw-r--r--   0        0        0     1100 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_delta.py
--rw-r--r--   0        0        0     1118 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_request_ext.py
--rw-r--r--   0        0        0     1143 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py
--rw-r--r--   0        0        0     1185 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_response.py
--rw-r--r--   0        0        0     1054 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_completion_response_format.py
--rw-r--r--   0        0        0      947 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_fn_call.py
--rw-r--r--   0        0        0     1061 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/chat_message.py
--rw-r--r--   0        0        0      996 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/completion_choice.py
--rw-r--r--   0        0        0     1311 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/completion_response.py
--rw-r--r--   0        0        0      163 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/create_chat_completion_request_function_call.py
--rw-r--r--   0        0        0      169 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/create_chat_completion_stream_request_function_call.py
--rw-r--r--   0        0        0     1265 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/error_response.py
--rw-r--r--   0        0        0      153 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/error_response_validation_errors_value.py
--rw-r--r--   0        0        0      197 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/finish_reason.py
--rw-r--r--   0        0        0      982 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/function.py
--rw-r--r--   0        0        0      955 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/http_validation_error.py
--rw-r--r--   0        0        0     1178 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/log_probs.py
--rw-r--r--   0        0        0      174 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/prompt.py
--rw-r--r--   0        0        0      123 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/stop.py
--rw-r--r--   0        0        0      964 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/usage_stats.py
--rw-r--r--   0        0        0      974 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/text_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     7630 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/uploading_asset_library.py
--rw-r--r--   0        0        0       74 2024-04-24 19:06:36.162961 octoai-0.0.2/src/octoai/version.py
--rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 octoai-0.0.2/PKG-INFO
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

### Comparing `octoai-0.0.2/README.md` & `octoai-0.0.60/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 poetry add octoai
 ```
 <!-- End Installation  -->
 
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
-Simply import `OctoAI` and start making calls to our API.
+Simply import `OctoAI` and start making calls to our API. 
 
 ```python
 from octoai.client import OctoAI
 from octoai.text_gen import ChatMessage
 
 client = OctoAI(
     api_key="YOUR_API_KEY"  # Defaults to your OCTOAI_TOKEN environment variable
@@ -40,15 +40,15 @@
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 The SDK also exports an async client so that you can make non-blocking
-calls to our API.
+calls to our API. 
 
 ```python
 from octoai.client import AsyncOctoAI
 from octoai.text_gen import ChatMessage
 
 client = AsyncOctoAI(
   api_key="YOUR_API_KEY" # Defaults to your OCTOAI_TOKEN environment variable
@@ -80,15 +80,15 @@
 # The image generation service
 client.image_gen.generate_sd(...)
 
 # The text generation service
 client.text_gen.create_chat_completion(...)
 
 # The asset library service
-client.asset_library.create(...)
+client.asset_lake.create(...)
 
 # The fine-tuning service
 client.fine_tuning.create(...)
 ```
 
 ## Exception Handling
 All errors thrown by the SDK will be subclasses of [`ApiError`](./src/octoai/core/api_error.py).
@@ -112,30 +112,30 @@
 
 A request is deemed retriable when any of the following HTTP status codes is returned:
 
 - [408](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/408) (Timeout)
 - [409](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/409) (Conflict)
 - [429](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/429) (Too Many Requests)
 - [5XX](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/500) (Internal Server Errors)
-
-Use the `max_retries` request option to configure this behavior.
+  
+Use the `max_retries` request option to configure this behavior. 
 
 ```python
 from octoai.client import OctoAI
 
 client = OctoAI(...)
 
 # Override retries for a specific method
 client.text_gen.create_chat_completion(..., {
     max_retries=5
 })
 ```
 
 ### Timeouts
-By default, requests time out after 60 seconds. You can configure this with a
+By default, requests time out after 60 seconds. You can configure this with a 
 timeout option at the client or request level.
 
 ```python
 from octoai.client import OctoAI
 
 client = OctoAI(
     # All timeouts are 20 seconds
@@ -145,15 +145,15 @@
 # Override timeout for a specific method
 client.text_gen.create_chat_completion(..., {
     timeout_in_seconds=20.0
 })
 ```
 
 ### Custom HTTP client
-You can override the httpx client to customize it for your use-case. Some common use-cases
+You can override the httpx client to customize it for your use-case. Some common use-cases 
 include support for proxies and transports.
 
 ```python
 import httpx
 
 from octoai.client import OctoAI
 
@@ -164,24 +164,24 @@
     ),
 )
 ```
 
 <!-- Begin Status, generated by Fern  -->
 # Beta Status
 
-This SDK is in beta, and there may be breaking changes between versions without a major
-version update. Therefore, we recommend pinning the package version to a specific version.
+This SDK is in beta, and there may be breaking changes between versions without a major 
+version update. Therefore, we recommend pinning the package version to a specific version. 
 This way, you can install the same version each time without breaking changes.
 <!-- End Status  -->
 
 <!-- Begin Contributing, generated by Fern  -->
 # Contributing
 
-While we value open-source contributions to this SDK, this library is generated programmatically.
-Additions made directly to this library would have to be moved over to our generation code,
+While we value open-source contributions to this SDK, this library is generated programmatically. 
+Additions made directly to this library would have to be moved over to our generation code, 
 otherwise they would be overwritten upon the next generated release. Feel free to open a PR as
- a proof of concept, but know that we will not be able to merge it as-is. We suggest opening
+ a proof of concept, but know that we will not be able to merge it as-is. We suggest opening 
 an issue first to discuss with us!
 
 On the other hand, contributions to the README are always very welcome!
 <!-- End Contributing  -->
```

### Comparing `octoai-0.0.2/pyproject.toml` & `octoai-0.0.60/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octoai"
-version = "0.0.2"
+version = "0.0.60"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "octoai", from = "src"}
 ]
 
@@ -14,15 +14,15 @@
 httpx = ">=0.21.2"
 httpx-sse = "0.4.0"
 pydantic = ">= 1.9.2"
 types-boto3 = "^1.0"
 typing_extensions = ">= 4.0.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "1.9.0"
+mypy = "^1.8.0"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.5"
 python-dateutil = "^2.9.0"
 
 [tool.pytest.ini_options]
 testpaths = [ "tests" ]
 asyncio_mode = "auto"
```

### Comparing `octoai-0.0.2/src/octoai/asset_library/__init__.py` & `octoai-0.0.60/src/octoai/asset_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/client.py` & `octoai-0.0.60/src/octoai/asset_lake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .types.retrieve_asset_response import RetrieveAssetResponse
 from .types.transfer_api_type import TransferApiType
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class AssetLibraryClient:
+class AssetLakeClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(
         self,
         *,
         name: typing.Optional[str] = None,
@@ -75,19 +75,19 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
-        client.asset_library.list()
+        client.asset_lake.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "name": name,
                         "is_public": is_public,
                         "data_type": data_type,
                         "asset_type": asset_type,
@@ -167,21 +167,21 @@
 
             - transfer_api_type: typing.Optional[TransferApiType]. Transfer API type.
 
             - url: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from octoai.asset_library import Data_Checkpoint
+        from octoai.asset_lake import Data_Checkpoint
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
-        client.asset_library.create(
+        client.asset_lake.create(
             asset_type="file",
             data=Data_Checkpoint(
                 data_type="fp16",
                 engine="text/llama-2-7b",
                 file_format="safetensors",
             ),
             description="string",
@@ -206,16 +206,16 @@
         if skip_validation is not OMIT:
             _request["skip_validation"] = skip_validation
         if transfer_api_type is not OMIT:
             _request["transfer_api_type"] = transfer_api_type
         if url is not OMIT:
             _request["url"] = url
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -255,21 +255,21 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
-        client.asset_library.delete(
+        client.asset_lake.delete(
             asset_id="asset_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
+            "DELETE",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/assets/{jsonable_encoder(asset_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -313,24 +313,24 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
-        client.asset_library.complete_upload(
+        client.asset_lake.complete_upload(
             asset_id="asset_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if token is not OMIT:
             _request["token"] = token
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
+            "POST",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/",
                 f"v1/assets/{jsonable_encoder(asset_id)}/complete-upload",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -381,22 +381,22 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
-        client.asset_library.get(
+        client.asset_lake.get(
             asset_owner_and_name_or_id="string",
             transfer_api_type="presigned-url",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
+            "GET",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/",
                 f"v1/assets/{jsonable_encoder(asset_owner_and_name_or_id)}",
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "transfer_api_type": transfer_api_type,
@@ -431,15 +431,15 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncAssetLibraryClient:
+class AsyncAssetLakeClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(
         self,
         *,
         name: typing.Optional[str] = None,
@@ -482,19 +482,19 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
-        await client.asset_library.list()
+        await client.asset_lake.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "name": name,
                         "is_public": is_public,
                         "data_type": data_type,
                         "asset_type": asset_type,
@@ -574,21 +574,21 @@
 
             - transfer_api_type: typing.Optional[TransferApiType]. Transfer API type.
 
             - url: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from octoai.asset_library import Data_Checkpoint
+        from octoai.asset_lake import Data_Checkpoint
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
-        await client.asset_library.create(
+        await client.asset_lake.create(
             asset_type="file",
             data=Data_Checkpoint(
                 data_type="fp16",
                 engine="text/llama-2-7b",
                 file_format="safetensors",
             ),
             description="string",
@@ -613,16 +613,16 @@
         if skip_validation is not OMIT:
             _request["skip_validation"] = skip_validation
         if transfer_api_type is not OMIT:
             _request["transfer_api_type"] = transfer_api_type
         if url is not OMIT:
             _request["url"] = url
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/assets"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -664,21 +664,21 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
-        await client.asset_library.delete(
+        await client.asset_lake.delete(
             asset_id="asset_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
+            "DELETE",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/assets/{jsonable_encoder(asset_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -722,24 +722,24 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
-        await client.asset_library.complete_upload(
+        await client.asset_lake.complete_upload(
             asset_id="asset_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if token is not OMIT:
             _request["token"] = token
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
+            "POST",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/",
                 f"v1/assets/{jsonable_encoder(asset_id)}/complete-upload",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -790,22 +790,22 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
-        await client.asset_library.get(
+        await client.asset_lake.get(
             asset_owner_and_name_or_id="string",
             transfer_api_type="presigned-url",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
+            "GET",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/",
                 f"v1/assets/{jsonable_encoder(asset_owner_and_name_or_id)}",
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "transfer_api_type": transfer_api_type,
```

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/__init__.py` & `octoai-0.0.60/src/octoai/asset_lake/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/asset.py` & `octoai-0.0.60/src/octoai/asset_lake/types/asset.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/base_engine.py` & `octoai-0.0.60/src/octoai/asset_lake/types/base_engine.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/checkpoint_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/checkpoint_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/complete_asset_upload_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/complete_asset_upload_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/create_asset_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/create_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/create_asset_response_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/create_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/delete_asset_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/delete_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/file_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/file_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/asset_lake/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/latent_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/latent_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/list_assets_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/list_assets_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/lora_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/lora_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/no_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/no_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/presigned_url_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/presigned_url_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/retrieve_asset_response.py` & `octoai-0.0.60/src/octoai/asset_lake/types/retrieve_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/retrieve_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/sts_transfer_api.py` & `octoai-0.0.60/src/octoai/asset_lake/types/sts_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/textual_inversion_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/textual_inversion_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/vae_data.py` & `octoai-0.0.60/src/octoai/asset_lake/types/vae_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/asset_library/types/validation_error.py` & `octoai-0.0.60/src/octoai/asset_lake/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/base_client.py` & `octoai-0.0.60/src/octoai/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import os
 import typing
 
 import httpx
 
-from .asset_library.client import AssetLibraryClient, AsyncAssetLibraryClient
+from .asset_lake.client import AssetLakeClient, AsyncAssetLakeClient
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .environment import OctoAIEnvironment
 from .fine_tuning.client import AsyncFineTuningClient, FineTuningClient
 from .image_gen.client import AsyncImageGenClient, ImageGenClient
 from .text_gen.client import AsyncTextGenClient, TextGenClient
 
 
@@ -39,32 +39,32 @@
 
     def __init__(
         self,
         *,
         environment: OctoAIEnvironment = OctoAIEnvironment.PRODUCTION,
         api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = os.getenv("OCTOAI_TOKEN"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = True,
+        follow_redirects: typing.Optional[bool] = None,
         httpx_client: typing.Optional[httpx.Client] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = SyncClientWrapper(
             environment=environment,
             api_key=api_key,
             httpx_client=httpx_client
             if httpx_client is not None
             else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.Client(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
-        self.asset_library = AssetLibraryClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = FineTuningClient(client_wrapper=self._client_wrapper)
-        self.text_gen = TextGenClient(client_wrapper=self._client_wrapper)
         self.image_gen = ImageGenClient(client_wrapper=self._client_wrapper)
+        self.asset_lake = AssetLakeClient(client_wrapper=self._client_wrapper)
+        self.text_gen = TextGenClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseOctoAI:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
@@ -89,25 +89,25 @@
 
     def __init__(
         self,
         *,
         environment: OctoAIEnvironment = OctoAIEnvironment.PRODUCTION,
         api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = os.getenv("OCTOAI_TOKEN"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = True,
+        follow_redirects: typing.Optional[bool] = None,
         httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = AsyncClientWrapper(
             environment=environment,
             api_key=api_key,
             httpx_client=httpx_client
             if httpx_client is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
-        self.asset_library = AsyncAssetLibraryClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = AsyncFineTuningClient(client_wrapper=self._client_wrapper)
-        self.text_gen = AsyncTextGenClient(client_wrapper=self._client_wrapper)
         self.image_gen = AsyncImageGenClient(client_wrapper=self._client_wrapper)
+        self.asset_lake = AsyncAssetLakeClient(client_wrapper=self._client_wrapper)
+        self.text_gen = AsyncTextGenClient(client_wrapper=self._client_wrapper)
```

### Comparing `octoai-0.0.2/src/octoai/client.py` & `octoai-0.0.60/src/octoai/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from octoai.uploading_asset_library import AsyncUploadingAssetLibraryClient, UploadingAssetLibraryClient
+from octoai.uploading_asset_lake import AsyncUploadingAssetLakeClient, UploadingAssetLakeClient
 from .base_client import BaseOctoAI, AsyncBaseOctoAI
 
 import os
 import typing
 import httpx
 
-from .asset_library.client import AssetLibraryClient, AsyncAssetLibraryClient
+from .asset_lake.client import AssetLakeClient, AsyncAssetLakeClient
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .environment import OctoAIEnvironment
 from .fine_tuning.client import AsyncFineTuningClient, FineTuningClient
 from .image_gen.client import AsyncImageGenClient, ImageGenClient
 from .text_gen.client import AsyncTextGenClient, TextGenClient
 
 
@@ -46,15 +46,15 @@
         super().__init__(
             environment=environment,
             api_key=api_key,
             timeout=timeout,
             httpx_client=httpx_client
         )
 
-        self.asset_library = UploadingAssetLibraryClient(client_wrapper=self._client_wrapper)
+        self.asset_lake = UploadingAssetLakeClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncOctoAI(AsyncBaseOctoAI):
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
@@ -86,8 +86,8 @@
         super().__init__(
             environment=environment,
             api_key=api_key,
             timeout=timeout,
             httpx_client=httpx_client
         )
 
-        self.asset_library = AsyncUploadingAssetLibraryClient(client_wrapper=self._client_wrapper)
+        self.asset_lake = AsyncUploadingAssetLakeClient(client_wrapper=self._client_wrapper)
```

### Comparing `octoai-0.0.2/src/octoai/core/__init__.py` & `octoai-0.0.60/src/octoai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/core/client_wrapper.py` & `octoai-0.0.60/src/octoai/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._environment = environment
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "octoai",
-            "X-Fern-SDK-Version": "0.0.2",
+            "X-Fern-SDK-Version": "0.0.60",
         }
         api_key = self._get_api_key()
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
         return headers
 
     def _get_api_key(self) -> typing.Optional[str]:
```

### Comparing `octoai-0.0.2/src/octoai/core/datetime_utils.py` & `octoai-0.0.60/src/octoai/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/core/file.py` & `octoai-0.0.60/src/octoai/core/file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/core/http_client.py` & `octoai-0.0.60/src/octoai/core/http_client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/core/jsonable_encoder.py` & `octoai-0.0.60/src/octoai/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/core/request_options.py` & `octoai-0.0.60/src/octoai/core/request_options.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/__init__.py` & `octoai-0.0.60/src/octoai/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/client.py` & `octoai-0.0.60/src/octoai/fine_tuning/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {"details": details, "name": name}
         if continue_on_rejection is not OMIT:
             _request["continue_on_rejection"] = continue_on_rejection
         if description is not OMIT:
             _request["description"] = description
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tune"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tune"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -130,16 +130,16 @@
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.get(
             tune_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
+            "GET",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/tune/{jsonable_encoder(tune_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -184,16 +184,16 @@
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.delete(
             tune_id="tune_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
+            "DELETE",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/tune/{jsonable_encoder(tune_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -236,16 +236,16 @@
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.cancel(
             tune_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
+            "POST",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/tune/{jsonable_encoder(tune_id)}/cancel"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -312,16 +312,16 @@
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tunes"),
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tunes"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "offset": offset,
                         "limit": limit,
                         "name": name,
                         "tune_type": tune_type,
@@ -416,16 +416,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {"details": details, "name": name}
         if continue_on_rejection is not OMIT:
             _request["continue_on_rejection"] = continue_on_rejection
         if description is not OMIT:
             _request["description"] = description
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tune"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tune"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -472,16 +472,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.get(
             tune_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
+            "GET",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/tune/{jsonable_encoder(tune_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -526,16 +526,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.delete(
             tune_id="tune_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
+            "DELETE",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/tune/{jsonable_encoder(tune_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -578,16 +578,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.cancel(
             tune_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
+            "POST",
+            urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/tune/{jsonable_encoder(tune_id)}/cancel"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
@@ -654,16 +654,16 @@
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tunes"),
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/tunes"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "offset": offset,
                         "limit": limit,
                         "name": name,
                         "tune_type": tune_type,
```

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/__init__.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/base_engine.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/base_engine.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/details.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/list_tunes_response.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/list_tunes_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/lora_tune.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/lora_tune_checkpoint.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune_checkpoint.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/lora_tune_file.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/lora_tune_file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/tune.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/tune_details.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/tune_details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/tune_result.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/tune_result.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/fine_tuning/types/validation_error.py` & `octoai-0.0.60/src/octoai/fine_tuning/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/__init__.py` & `octoai-0.0.60/src/octoai/image_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/client.py` & `octoai-0.0.60/src/octoai/image_gen/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         client.image_gen.generate_ssd(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/ssd"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/ssd"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -104,18 +104,16 @@
         client.image_gen.generate_controlnet_sdxl(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sdxl"
-            ),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sdxl"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -167,18 +165,16 @@
         client.image_gen.generate_controlnet_sd15(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sd15"
-            ),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sd15"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -230,16 +226,16 @@
         client.image_gen.generate_sdxl(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sdxl"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sdxl"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -291,16 +287,16 @@
         client.image_gen.generate_sd(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sd"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sd"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -357,16 +353,16 @@
         await client.image_gen.generate_ssd(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/ssd"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/ssd"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -418,18 +414,16 @@
         await client.image_gen.generate_controlnet_sdxl(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sdxl"
-            ),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sdxl"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -481,18 +475,16 @@
         await client.image_gen.generate_controlnet_sd15(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sd15"
-            ),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/controlnet-sd15"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -544,16 +536,16 @@
         await client.image_gen.generate_sdxl(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sdxl"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sdxl"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -605,16 +597,16 @@
         await client.image_gen.generate_sd(
             request=ImageGenerationRequest(
                 prompt="An octopus playing chess, masterpiece, photorealistic",
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sd"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().image_gen}/", "generate/sd"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
```

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/__init__.py` & `octoai-0.0.60/src/octoai/image_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/image_gen/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/image_generation.py` & `octoai-0.0.60/src/octoai/image_gen/types/image_generation.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/image_generation_request.py` & `octoai-0.0.60/src/octoai/image_gen/types/image_generation_request.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/image_generation_response.py` & `octoai-0.0.60/src/octoai/image_gen/types/image_generation_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/scheduler.py` & `octoai-0.0.60/src/octoai/image_gen/types/scheduler.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/sdxl_styles.py` & `octoai-0.0.60/src/octoai/image_gen/types/sdxl_styles.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/image_gen/types/validation_error.py` & `octoai-0.0.60/src/octoai/image_gen/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/__init__.py` & `octoai-0.0.60/src/octoai/text_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/client.py` & `octoai-0.0.60/src/octoai/text_gen/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,16 +181,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         with self._client_wrapper.httpx_client.stream(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -333,16 +333,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -491,16 +491,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         with self._client_wrapper.httpx_client.stream(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -636,16 +636,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -826,16 +826,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         async with self._client_wrapper.httpx_client.stream(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -978,16 +978,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/chat/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -1136,16 +1136,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         async with self._client_wrapper.httpx_client.stream(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -1281,16 +1281,16 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if user is not OMIT:
             _request["user"] = user
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_environment().text_gen}/", "v1/completions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
```

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/__init__.py` & `octoai-0.0.60/src/octoai/text_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_choice.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_chunk.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_chunk_choice.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_chunk_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_delta.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_delta.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_request_ext.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_request_ext.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_response.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_completion_response_format.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_completion_response_format.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_fn_call.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_fn_call.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/chat_message.py` & `octoai-0.0.60/src/octoai/text_gen/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/completion_choice.py` & `octoai-0.0.60/src/octoai/text_gen/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/completion_response.py` & `octoai-0.0.60/src/octoai/text_gen/types/completion_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/error_response.py` & `octoai-0.0.60/src/octoai/text_gen/types/error_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/function.py` & `octoai-0.0.60/src/octoai/text_gen/types/function.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/http_validation_error.py` & `octoai-0.0.60/src/octoai/text_gen/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/log_probs.py` & `octoai-0.0.60/src/octoai/text_gen/types/log_probs.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/usage_stats.py` & `octoai-0.0.60/src/octoai/text_gen/types/usage_stats.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/text_gen/types/validation_error.py` & `octoai-0.0.60/src/octoai/text_gen/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.2/src/octoai/uploading_asset_library.py` & `octoai-0.0.60/src/octoai/uploading_asset_lake.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import asyncio
 import contextlib
 import functools
 from time import sleep
 import time
 import typing
 
-from octoai.asset_library.types.status import Status
-from .asset_library.client import AsyncAssetLibraryClient
-from .asset_library.types.create_asset_response import CreateAssetResponse
-from .asset_library.types.create_asset_response_transfer_api import CreateAssetResponseTransferApi, CreateAssetResponseTransferApi_PresignedUrl, CreateAssetResponseTransferApi_Sts
+from octoai.asset_lake.types.status import Status
+from .asset_lake.client import AsyncAssetLakeClient
+from .asset_lake.types.create_asset_response import CreateAssetResponse
+from .asset_lake.types.create_asset_response_transfer_api import CreateAssetResponseTransferApi, CreateAssetResponseTransferApi_PresignedUrl, CreateAssetResponseTransferApi_Sts
 import boto3
 from .core.client_wrapper import AsyncClientWrapper
 import httpx
-from octoai.asset_library.types.asset import Asset
+from octoai.asset_lake.types.asset import Asset
 
-from .asset_library.client import OMIT
-from .asset_library.types.data import Data
-from .asset_library.types.transfer_api_type import TransferApiType
+from .asset_lake.client import OMIT
+from .asset_lake.types.data import Data
+from .asset_lake.types.transfer_api_type import TransferApiType
 from .core.request_options import RequestOptions
 from .core.client_wrapper import SyncClientWrapper
-from .asset_library.client import AssetLibraryClient
+from .asset_lake.client import AssetLakeClient
 from .core.api_error import ApiError
 
 
 _TERMINAL_STATUSES: typing.Set[Status] = {"ready", "deleted", "rejected", "error"}
 
 
 class AssetReadyTimeout(Exception):
@@ -43,15 +43,15 @@
     )
     try:
         s3_client.upload_file(file, x_api.s3bucket, x_api.s3key)
     except Exception as e:
         raise Exception(f"Error uploading file to server: {e}")
 
 
-class UploadingAssetLibraryClient(AssetLibraryClient):
+class UploadingAssetLakeClient(AssetLakeClient):
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         super().__init__(client_wrapper=client_wrapper)
 
     def create_from_file(
         self,
         file: typing.Union[str, typing.BinaryIO],
         data: Data,
@@ -122,15 +122,15 @@
                     url=transfer_api_used.put_url, content=file_data, timeout=60000
                 )
                 upload_resp.raise_for_status()
         elif isinstance(transfer_api_used, CreateAssetResponseTransferApi_Sts):
             _sts_upload(transfer_api_used, file)
 
 
-class AsyncUploadingAssetLibraryClient(AsyncAssetLibraryClient):
+class AsyncUploadingAssetLakeClient(AsyncAssetLakeClient):
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         super().__init__(client_wrapper=client_wrapper)
         self._signed_url_client = httpx.AsyncClient()
 
     async def create_from_file(
         self,
         file: typing.Union[str, typing.BinaryIO],
```

### Comparing `octoai-0.0.2/PKG-INFO` & `octoai-0.0.60/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoai
-Version: 0.0.2
+Version: 0.0.60
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -34,15 +34,15 @@
 poetry add octoai
 ```
 <!-- End Installation  -->
 
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
-Simply import `OctoAI` and start making calls to our API.
+Simply import `OctoAI` and start making calls to our API. 
 
 ```python
 from octoai.client import OctoAI
 from octoai.text_gen import ChatMessage
 
 client = OctoAI(
     api_key="YOUR_API_KEY"  # Defaults to your OCTOAI_TOKEN environment variable
@@ -58,15 +58,15 @@
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 The SDK also exports an async client so that you can make non-blocking
-calls to our API.
+calls to our API. 
 
 ```python
 from octoai.client import AsyncOctoAI
 from octoai.text_gen import ChatMessage
 
 client = AsyncOctoAI(
   api_key="YOUR_API_KEY" # Defaults to your OCTOAI_TOKEN environment variable
@@ -98,15 +98,15 @@
 # The image generation service
 client.image_gen.generate_sd(...)
 
 # The text generation service
 client.text_gen.create_chat_completion(...)
 
 # The asset library service
-client.asset_library.create(...)
+client.asset_lake.create(...)
 
 # The fine-tuning service
 client.fine_tuning.create(...)
 ```
 
 ## Exception Handling
 All errors thrown by the SDK will be subclasses of [`ApiError`](./src/octoai/core/api_error.py).
@@ -130,30 +130,30 @@
 
 A request is deemed retriable when any of the following HTTP status codes is returned:
 
 - [408](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/408) (Timeout)
 - [409](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/409) (Conflict)
 - [429](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/429) (Too Many Requests)
 - [5XX](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/500) (Internal Server Errors)
-
-Use the `max_retries` request option to configure this behavior.
+  
+Use the `max_retries` request option to configure this behavior. 
 
 ```python
 from octoai.client import OctoAI
 
 client = OctoAI(...)
 
 # Override retries for a specific method
 client.text_gen.create_chat_completion(..., {
     max_retries=5
 })
 ```
 
 ### Timeouts
-By default, requests time out after 60 seconds. You can configure this with a
+By default, requests time out after 60 seconds. You can configure this with a 
 timeout option at the client or request level.
 
 ```python
 from octoai.client import OctoAI
 
 client = OctoAI(
     # All timeouts are 20 seconds
@@ -163,15 +163,15 @@
 # Override timeout for a specific method
 client.text_gen.create_chat_completion(..., {
     timeout_in_seconds=20.0
 })
 ```
 
 ### Custom HTTP client
-You can override the httpx client to customize it for your use-case. Some common use-cases
+You can override the httpx client to customize it for your use-case. Some common use-cases 
 include support for proxies and transports.
 
 ```python
 import httpx
 
 from octoai.client import OctoAI
 
@@ -182,25 +182,25 @@
     ),
 )
 ```
 
 <!-- Begin Status, generated by Fern  -->
 # Beta Status
 
-This SDK is in beta, and there may be breaking changes between versions without a major
-version update. Therefore, we recommend pinning the package version to a specific version.
+This SDK is in beta, and there may be breaking changes between versions without a major 
+version update. Therefore, we recommend pinning the package version to a specific version. 
 This way, you can install the same version each time without breaking changes.
 <!-- End Status  -->
 
 <!-- Begin Contributing, generated by Fern  -->
 # Contributing
 
-While we value open-source contributions to this SDK, this library is generated programmatically.
-Additions made directly to this library would have to be moved over to our generation code,
+While we value open-source contributions to this SDK, this library is generated programmatically. 
+Additions made directly to this library would have to be moved over to our generation code, 
 otherwise they would be overwritten upon the next generated release. Feel free to open a PR as
- a proof of concept, but know that we will not be able to merge it as-is. We suggest opening
+ a proof of concept, but know that we will not be able to merge it as-is. We suggest opening 
 an issue first to discuss with us!
 
 On the other hand, contributions to the README are always very welcome!
 <!-- End Contributing  -->
```


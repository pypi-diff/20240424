# Comparing `tmp/openai_mealuet-1.16.2.tar.gz` & `tmp/openai_mealuet-1.23.4.tar.gz`

## Comparing `openai_mealuet-1.16.2.tar` & `openai_mealuet-1.23.4.tar`

### file list

```diff
@@ -1,234 +1,264 @@
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/__main__.py
--rw-r--r--   0        0        0    63755 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_base_client.py
--rw-r--r--   0        0        0    20194 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_compat.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_constants.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_exceptions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_files.py
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_legacy_response.py
--rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_models.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_module_client.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_resource.py
--rw-r--r--   0        0        0    28577 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_response.py
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_streaming.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_types.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_version.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/py.typed
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/version.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_extras/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_extras/_common.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_extras/numpy_proxy.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_extras/pandas_proxy.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/_utils/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/__init__.py
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_cli.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_errors.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_models.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_progress.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/_main.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/audio.py
--rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/completions.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/files.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/image.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/models.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/chat/__init__.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_api/chat/completions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_tools/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_tools/_main.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_tools/fine_tunes.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/cli/_tools/migrate.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/lib/.keep
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/lib/_old_api.py
--rw-r--r--   0        0        0    35189 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/lib/_validators.py
--rw-r--r--   0        0        0    21021 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/lib/azure.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/lib/streaming/__init__.py
--rw-r--r--   0        0        0    40467 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/lib/streaming/_assistants.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/__init__.py
--rw-r--r--   0        0        0    57139 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/completions.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/embeddings.py
--rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/files.py
--rw-r--r--   0        0        0    24782 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/images.py
--rw-r--r--   0        0        0    10183 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/models.py
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/moderations.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/audio/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/audio/audio.py
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/audio/speech.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/audio/translations.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/__init__.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/beta.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/assistants/__init__.py
--rw-r--r--   0        0        0    30704 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/assistants/assistants.py
--rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/assistants/files.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/__init__.py
--rw-r--r--   0        0        0    54379 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/threads.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/messages/files.py
--rw-r--r--   0        0        0    23786 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/messages/messages.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0    96872 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/runs/runs.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/beta/threads/runs/steps.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/chat/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/chat/chat.py
--rw-r--r--   0        0        0    72429 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/chat/completions.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/fine_tuning/__init__.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0    24536 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/resources/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/completion.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/completion_choice.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/completion_create_params.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/completion_usage.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/create_embedding_response.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/embedding.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/embedding_create_params.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/file_content.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/file_create_params.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/file_deleted.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/file_list_params.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/file_object.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/image.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/image_create_variation_params.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/image_edit_params.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/image_generate_params.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/images_response.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/model.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/model_deleted.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/moderation.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/moderation_create_params.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/moderation_create_response.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/audio/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/audio/speech_create_params.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/audio/transcription.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/audio/translation.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/audio/translation_create_params.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/__init__.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant_create_params.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant_deleted.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant_list_params.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant_stream_event.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant_tool.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant_tool_param.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistant_update_params.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/code_interpreter_tool.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/code_interpreter_tool_param.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/function_tool.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/function_tool_param.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/retrieval_tool.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/retrieval_tool_param.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/thread.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/thread_create_and_run_params.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/thread_create_params.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/thread_deleted.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/thread_update_params.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistants/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistants/assistant_file.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistants/file_create_params.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistants/file_delete_response.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/assistants/file_list_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/chat/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/annotation.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/annotation_delta.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/file_citation_annotation.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/file_citation_delta_annotation.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/file_path_annotation.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/file_path_delta_annotation.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/image_file.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/image_file_content_block.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/image_file_delta.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/image_file_delta_block.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message_content.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message_content_delta.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message_create_params.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message_delta.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message_delta_event.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message_list_params.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/message_update_params.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/required_action_function_tool_call.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/run.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/run_create_params.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/run_list_params.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/run_status.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/run_submit_tool_outputs_params.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/run_update_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/text.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/text_content_block.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/text_delta.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/text_delta_block.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/messages/file_list_params.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/messages/message_file.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/code_interpreter_logs.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/code_interpreter_output_image.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/function_tool_call.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/function_tool_call_delta.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/message_creation_step_details.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/retrieval_tool_call.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/retrieval_tool_call_delta.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/run_step.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/run_step_delta.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/run_step_delta_event.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/run_step_delta_message_delta.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/step_list_params.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/tool_call.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/tool_call_delta.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/tool_call_delta_object.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/tool_calls_step_details.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_assistant_message_param.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_content_part_image_param.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_content_part_param.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_content_part_text_param.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_function_call_option_param.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_function_message_param.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message_param.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message_tool_call.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message_tool_call_param.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_named_tool_choice_param.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_role.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_system_message_param.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_token_logprob.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_tool_choice_option_param.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_tool_message_param.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_tool_param.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_user_message_param.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/chat/completion_create_params.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/fine_tuning/job_list_events_params.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/fine_tuning/job_list_params.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/shared/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/shared/error_object.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/shared/function_definition.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/shared/function_parameters.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/shared_params/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/shared_params/function_definition.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/src/openai/types/shared_params/function_parameters.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/LICENSE
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/pyproject.toml
--rw-r--r--   0        0        0    21899 2020-02-02 00:00:00.000000 openai_mealuet-1.16.2/PKG-INFO
+-rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/__main__.py
+-rw-r--r--   0        0        0    65122 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_base_client.py
+-rw-r--r--   0        0        0    21771 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_compat.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_constants.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_exceptions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_files.py
+-rw-r--r--   0        0        0    15575 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_legacy_response.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_models.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_module_client.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_resource.py
+-rw-r--r--   0        0        0    28873 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_response.py
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_streaming.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_types.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_version.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/py.typed
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/version.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_extras/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_extras/_common.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_extras/numpy_proxy.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_extras/pandas_proxy.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/_utils/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/__init__.py
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_cli.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_errors.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_models.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_progress.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_utils.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/_main.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/audio.py
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/completions.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/files.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/image.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/models.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/chat/__init__.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_api/chat/completions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_tools/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_tools/_main.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_tools/fine_tunes.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/cli/_tools/migrate.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/lib/.keep
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/lib/_old_api.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/lib/_validators.py
+-rw-r--r--   0        0        0    21479 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/lib/azure.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/lib/streaming/__init__.py
+-rw-r--r--   0        0        0    40467 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/lib/streaming/_assistants.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/__init__.py
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/batches.py
+-rw-r--r--   0        0        0    57169 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/completions.py
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/embeddings.py
+-rw-r--r--   0        0        0    26152 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/files.py
+-rw-r--r--   0        0        0    24796 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/images.py
+-rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/models.py
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/moderations.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/audio/__init__.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/audio/audio.py
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/audio/speech.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/audio/transcriptions.py
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/audio/translations.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/__init__.py
+-rw-r--r--   0        0        0    39350 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/assistants.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/beta.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/threads/__init__.py
+-rw-r--r--   0        0        0    22605 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/threads/messages.py
+-rw-r--r--   0        0        0    98886 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/threads/threads.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0   146623 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/threads/runs/runs.py
+-rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/threads/runs/steps.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/vector_stores/__init__.py
+-rw-r--r--   0        0        0    29533 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/vector_stores/file_batches.py
+-rw-r--r--   0        0        0    27046 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/vector_stores/files.py
+-rw-r--r--   0        0        0    27141 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/beta/vector_stores/vector_stores.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/chat/chat.py
+-rw-r--r--   0        0        0    66971 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/chat/completions.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/fine_tuning/jobs/__init__.py
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/fine_tuning/jobs/checkpoints.py
+-rw-r--r--   0        0        0    26850 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/resources/fine_tuning/jobs/jobs.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/__init__.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/batch.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/batch_create_params.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/batch_error.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/batch_list_params.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/batch_request_counts.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat_model.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/completion.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/completion_choice.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/completion_create_params.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/completion_usage.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/create_embedding_response.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/embedding.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/embedding_create_params.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/file_content.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/file_create_params.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/file_deleted.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/file_list_params.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/file_object.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/image.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/image_create_variation_params.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/image_edit_params.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/image_generate_params.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/images_response.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/model.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/model_deleted.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/moderation.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/moderation_create_response.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/audio/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/audio/speech_create_params.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/audio/transcription.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/audio/transcription_create_params.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/audio/translation.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/audio/translation_create_params.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/__init__.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_create_params.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_deleted.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_list_params.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_response_format.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_response_format_option.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_response_format_option_param.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_response_format_param.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_stream_event.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool_choice.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool_choice_function.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool_choice_function_param.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool_choice_option.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool_choice_option_param.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool_choice_param.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_tool_param.py
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/assistant_update_params.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/code_interpreter_tool.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/code_interpreter_tool_param.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/file_search_tool.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/file_search_tool_param.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/function_tool.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/function_tool_param.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/thread.py
+-rw-r--r--   0        0        0    12416 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/thread_create_and_run_params.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/thread_create_params.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/thread_deleted.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/thread_update_params.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_store.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_store_create_params.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_store_deleted.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_store_list_params.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_store_update_params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/chat/__init__.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/annotation.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/annotation_delta.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/file_citation_annotation.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/file_citation_delta_annotation.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/file_path_annotation.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/file_path_delta_annotation.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/image_file.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/image_file_content_block.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/image_file_delta.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/image_file_delta_block.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message_content.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message_content_delta.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message_create_params.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message_delta.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message_delta_event.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message_list_params.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/message_update_params.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/required_action_function_tool_call.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/run.py
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/run_create_params.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/run_list_params.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/run_status.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/run_submit_tool_outputs_params.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/run_update_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/text.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/text_content_block.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/text_delta.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/text_delta_block.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/code_interpreter_logs.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/code_interpreter_output_image.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/code_interpreter_tool_call.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/file_search_tool_call.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/file_search_tool_call_delta.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/function_tool_call.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/function_tool_call_delta.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/message_creation_step_details.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step_delta.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step_delta_event.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step_delta_message_delta.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/step_list_params.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/tool_call.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/tool_call_delta.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/tool_call_delta_object.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/tool_calls_step_details.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/file_batch_create_params.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/file_batch_list_files_params.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/file_create_params.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/file_list_params.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/vector_store_file.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/vector_store_file_batch.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/vector_store_file_deleted.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_assistant_message_param.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_content_part_image_param.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_content_part_param.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_content_part_text_param.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_function_call_option_param.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_function_message_param.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message_param.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message_tool_call.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message_tool_call_param.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_named_tool_choice_param.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_role.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_system_message_param.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_token_logprob.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_tool_choice_option_param.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_tool_message_param.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_tool_param.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_user_message_param.py
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/fine_tuning_job_integration.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/fine_tuning_job_wandb_integration.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/fine_tuning_job_wandb_integration_object.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/job_list_events_params.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/job_list_params.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/jobs/__init__.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/jobs/checkpoint_list_params.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/fine_tuning/jobs/fine_tuning_job_checkpoint.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/shared/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/shared/error_object.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/shared/function_definition.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/shared/function_parameters.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/shared_params/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/shared_params/function_definition.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/src/openai/types/shared_params/function_parameters.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/LICENSE
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/pyproject.toml
+-rw-r--r--   0        0        0    22264 2020-02-02 00:00:00.000000 openai_mealuet-1.23.4/PKG-INFO
```

### Comparing `openai_mealuet-1.16.2/src/openai/__init__.py` & `openai_mealuet-1.23.4/src/openai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     APIConnectionError,
     AuthenticationError,
     InternalServerError,
     PermissionDeniedError,
     UnprocessableEntityError,
     APIResponseValidationError,
 )
+from ._base_client import DefaultHttpxClient, DefaultAsyncHttpxClient
 from ._utils._logs import setup_logging as _setup_logging
 
 __all__ = [
     "types",
     "__version__",
     "__title__",
     "NoneType",
@@ -63,14 +64,16 @@
     "OpenAI",
     "AsyncOpenAI",
     "file_from_path",
     "BaseModel",
     "DEFAULT_TIMEOUT",
     "DEFAULT_MAX_RETRIES",
     "DEFAULT_CONNECTION_LIMITS",
+    "DefaultHttpxClient",
+    "DefaultAsyncHttpxClient",
 ]
 
 from .lib import azure as _azure
 from .version import VERSION as VERSION
 from .lib.azure import AzureOpenAI as AzureOpenAI, AsyncAzureOpenAI as AsyncAzureOpenAI
 from .lib._old_api import *
 from .lib.streaming import (
@@ -101,14 +104,16 @@
 
 from ._base_client import DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES
 
 api_key: str | None = None
 
 organization: str | None = None
 
+project: str | None = None
+
 base_url: str | _httpx.URL | None = None
 
 timeout: float | Timeout | None = DEFAULT_TIMEOUT
 
 max_retries: int = DEFAULT_MAX_RETRIES
 
 default_headers: _t.Mapping[str, str] | None = None
@@ -152,14 +157,25 @@
 
     @organization.setter  # type: ignore
     def organization(self, value: str | None) -> None:  # type: ignore
         global organization
 
         organization = value
 
+    @property  # type: ignore
+    @override
+    def project(self) -> str | None:
+        return project
+
+    @project.setter  # type: ignore
+    def project(self, value: str | None) -> None:  # type: ignore
+        global project
+
+        project = value
+
     @property
     @override
     def base_url(self) -> _httpx.URL:
         if base_url is not None:
             return _httpx.URL(base_url)
 
         return super().base_url
@@ -303,14 +319,15 @@
                 http_client=http_client,
             )
             return _client
 
         _client = _ModuleClient(
             api_key=api_key,
             organization=organization,
+            project=project,
             base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
             default_headers=default_headers,
             default_query=default_query,
             http_client=http_client,
         )
@@ -328,12 +345,13 @@
 from ._module_client import (
     beta as beta,
     chat as chat,
     audio as audio,
     files as files,
     images as images,
     models as models,
+    batches as batches,
     embeddings as embeddings,
     completions as completions,
     fine_tuning as fine_tuning,
     moderations as moderations,
 )
```

### Comparing `openai_mealuet-1.16.2/src/openai/_base_client.py` & `openai_mealuet-1.23.4/src/openai/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     Iterator,
     Optional,
     Generator,
     AsyncIterator,
     cast,
     overload,
 )
-from functools import lru_cache
 from typing_extensions import Literal, override, get_origin
 
 import anyio
 import httpx
 import distro
 import pydantic
 from httpx import URL, Limits
@@ -57,15 +56,15 @@
     ProxiesTypes,
     RequestFiles,
     HttpxSendArgs,
     AsyncTransport,
     RequestOptions,
     ModelBuilderProtocol,
 )
-from ._utils import is_dict, is_list, is_given, is_mapping
+from ._utils import is_dict, is_list, is_given, lru_cache, is_mapping
 from ._compat import model_copy, model_dump
 from ._models import GenericModel, FinalRequestOptions, validate_type, construct_type
 from ._response import (
     APIResponse,
     BaseAPIResponse,
     AsyncAPIResponse,
     extract_response_type,
@@ -712,15 +711,35 @@
         log.debug("Not retrying")
         return False
 
     def _idempotency_key(self) -> str:
         return f"stainless-python-retry-{uuid.uuid4()}"
 
 
-class SyncHttpxClientWrapper(httpx.Client):
+class _DefaultHttpxClient(httpx.Client):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultHttpxClient = httpx.Client
+    """An alias to `httpx.Client` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.Client` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultHttpxClient = _DefaultHttpxClient
+
+
+class SyncHttpxClientWrapper(DefaultHttpxClient):
     def __del__(self) -> None:
         try:
             self.close()
         except Exception:
             pass
 
 
@@ -1258,15 +1277,35 @@
         options: RequestOptions = {},
         method: str = "get",
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
-class AsyncHttpxClientWrapper(httpx.AsyncClient):
+class _DefaultAsyncHttpxClient(httpx.AsyncClient):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultAsyncHttpxClient = httpx.AsyncClient
+    """An alias to `httpx.AsyncClient` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.AsyncClient` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultAsyncHttpxClient = _DefaultAsyncHttpxClient
+
+
+class AsyncHttpxClientWrapper(DefaultAsyncHttpxClient):
     def __del__(self) -> None:
         try:
             # TODO(someday): support non asyncio runtimes here
             asyncio.get_running_loop().create_task(self.aclose())
         except Exception:
             pass
```

### Comparing `openai_mealuet-1.16.2/src/openai/_client.py` & `openai_mealuet-1.23.4/src/openai/_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,32 +53,37 @@
     files: resources.Files
     images: resources.Images
     audio: resources.Audio
     moderations: resources.Moderations
     models: resources.Models
     fine_tuning: resources.FineTuning
     beta: resources.Beta
+    batches: resources.Batches
     with_raw_response: OpenAIWithRawResponse
     with_streaming_response: OpenAIWithStreamedResponse
 
     # client options
     api_key: str
     organization: str | None
+    project: str | None
 
     def __init__(
         self,
         *,
         api_key: str | None = None,
         organization: str | None = None,
+        project: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
         http_client: httpx.Client | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
@@ -87,27 +92,32 @@
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous openai client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
         - `api_key` from `OPENAI_API_KEY`
         - `organization` from `OPENAI_ORG_ID`
+        - `project` from `OPENAI_PROJECT_ID`
         """
         if api_key is None:
             api_key = os.environ.get("OPENAI_API_KEY")
         if api_key is None:
             raise OpenAIError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the OPENAI_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if organization is None:
             organization = os.environ.get("OPENAI_ORG_ID")
         self.organization = organization
 
+        if project is None:
+            project = os.environ.get("OPENAI_PROJECT_ID")
+        self.project = project
+
         if base_url is None:
             base_url = os.environ.get("OPENAI_BASE_URL")
         if base_url is None:
             base_url = f"https://openai-proxy.mealuet.com/v1"
 
         super().__init__(
             version=__version__,
@@ -128,14 +138,15 @@
         self.files = resources.Files(self)
         self.images = resources.Images(self)
         self.audio = resources.Audio(self)
         self.moderations = resources.Moderations(self)
         self.models = resources.Models(self)
         self.fine_tuning = resources.FineTuning(self)
         self.beta = resources.Beta(self)
+        self.batches = resources.Batches(self)
         self.with_raw_response = OpenAIWithRawResponse(self)
         self.with_streaming_response = OpenAIWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -149,22 +160,24 @@
     @property
     @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
             "X-Stainless-Async": "false",
             "OpenAI-Organization": self.organization if self.organization is not None else Omit(),
+            "OpenAI-Project": self.project if self.project is not None else Omit(),
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
         api_key: str | None = None,
         organization: str | None = None,
+        project: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.Client | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -192,14 +205,15 @@
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             api_key=api_key or self.api_key,
             organization=organization or self.organization,
+            project=project or self.project,
             base_url=base_url or self.base_url,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
@@ -251,32 +265,37 @@
     files: resources.AsyncFiles
     images: resources.AsyncImages
     audio: resources.AsyncAudio
     moderations: resources.AsyncModerations
     models: resources.AsyncModels
     fine_tuning: resources.AsyncFineTuning
     beta: resources.AsyncBeta
+    batches: resources.AsyncBatches
     with_raw_response: AsyncOpenAIWithRawResponse
     with_streaming_response: AsyncOpenAIWithStreamedResponse
 
     # client options
     api_key: str
     organization: str | None
+    project: str | None
 
     def __init__(
         self,
         *,
         api_key: str | None = None,
         organization: str | None = None,
+        project: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultAsyncHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
         http_client: httpx.AsyncClient | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
@@ -285,27 +304,32 @@
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async openai client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
         - `api_key` from `OPENAI_API_KEY`
         - `organization` from `OPENAI_ORG_ID`
+        - `project` from `OPENAI_PROJECT_ID`
         """
         if api_key is None:
             api_key = os.environ.get("OPENAI_API_KEY")
         if api_key is None:
             raise OpenAIError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the OPENAI_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if organization is None:
             organization = os.environ.get("OPENAI_ORG_ID")
         self.organization = organization
 
+        if project is None:
+            project = os.environ.get("OPENAI_PROJECT_ID")
+        self.project = project
+
         if base_url is None:
             base_url = os.environ.get("OPENAI_BASE_URL")
         if base_url is None:
             base_url = f"https://openai-proxy.mealuet.com/v1"
 
         super().__init__(
             version=__version__,
@@ -326,14 +350,15 @@
         self.files = resources.AsyncFiles(self)
         self.images = resources.AsyncImages(self)
         self.audio = resources.AsyncAudio(self)
         self.moderations = resources.AsyncModerations(self)
         self.models = resources.AsyncModels(self)
         self.fine_tuning = resources.AsyncFineTuning(self)
         self.beta = resources.AsyncBeta(self)
+        self.batches = resources.AsyncBatches(self)
         self.with_raw_response = AsyncOpenAIWithRawResponse(self)
         self.with_streaming_response = AsyncOpenAIWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -347,22 +372,24 @@
     @property
     @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
             "X-Stainless-Async": f"async:{get_async_library()}",
             "OpenAI-Organization": self.organization if self.organization is not None else Omit(),
+            "OpenAI-Project": self.project if self.project is not None else Omit(),
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
         api_key: str | None = None,
         organization: str | None = None,
+        project: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.AsyncClient | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -390,14 +417,15 @@
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             api_key=api_key or self.api_key,
             organization=organization or self.organization,
+            project=project or self.project,
             base_url=base_url or self.base_url,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
@@ -450,54 +478,58 @@
         self.files = resources.FilesWithRawResponse(client.files)
         self.images = resources.ImagesWithRawResponse(client.images)
         self.audio = resources.AudioWithRawResponse(client.audio)
         self.moderations = resources.ModerationsWithRawResponse(client.moderations)
         self.models = resources.ModelsWithRawResponse(client.models)
         self.fine_tuning = resources.FineTuningWithRawResponse(client.fine_tuning)
         self.beta = resources.BetaWithRawResponse(client.beta)
+        self.batches = resources.BatchesWithRawResponse(client.batches)
 
 
 class AsyncOpenAIWithRawResponse:
     def __init__(self, client: AsyncOpenAI) -> None:
         self.completions = resources.AsyncCompletionsWithRawResponse(client.completions)
         self.chat = resources.AsyncChatWithRawResponse(client.chat)
         self.embeddings = resources.AsyncEmbeddingsWithRawResponse(client.embeddings)
         self.files = resources.AsyncFilesWithRawResponse(client.files)
         self.images = resources.AsyncImagesWithRawResponse(client.images)
         self.audio = resources.AsyncAudioWithRawResponse(client.audio)
         self.moderations = resources.AsyncModerationsWithRawResponse(client.moderations)
         self.models = resources.AsyncModelsWithRawResponse(client.models)
         self.fine_tuning = resources.AsyncFineTuningWithRawResponse(client.fine_tuning)
         self.beta = resources.AsyncBetaWithRawResponse(client.beta)
+        self.batches = resources.AsyncBatchesWithRawResponse(client.batches)
 
 
 class OpenAIWithStreamedResponse:
     def __init__(self, client: OpenAI) -> None:
         self.completions = resources.CompletionsWithStreamingResponse(client.completions)
         self.chat = resources.ChatWithStreamingResponse(client.chat)
         self.embeddings = resources.EmbeddingsWithStreamingResponse(client.embeddings)
         self.files = resources.FilesWithStreamingResponse(client.files)
         self.images = resources.ImagesWithStreamingResponse(client.images)
         self.audio = resources.AudioWithStreamingResponse(client.audio)
         self.moderations = resources.ModerationsWithStreamingResponse(client.moderations)
         self.models = resources.ModelsWithStreamingResponse(client.models)
         self.fine_tuning = resources.FineTuningWithStreamingResponse(client.fine_tuning)
         self.beta = resources.BetaWithStreamingResponse(client.beta)
+        self.batches = resources.BatchesWithStreamingResponse(client.batches)
 
 
 class AsyncOpenAIWithStreamedResponse:
     def __init__(self, client: AsyncOpenAI) -> None:
         self.completions = resources.AsyncCompletionsWithStreamingResponse(client.completions)
         self.chat = resources.AsyncChatWithStreamingResponse(client.chat)
         self.embeddings = resources.AsyncEmbeddingsWithStreamingResponse(client.embeddings)
         self.files = resources.AsyncFilesWithStreamingResponse(client.files)
         self.images = resources.AsyncImagesWithStreamingResponse(client.images)
         self.audio = resources.AsyncAudioWithStreamingResponse(client.audio)
         self.moderations = resources.AsyncModerationsWithStreamingResponse(client.moderations)
         self.models = resources.AsyncModelsWithStreamingResponse(client.models)
         self.fine_tuning = resources.AsyncFineTuningWithStreamingResponse(client.fine_tuning)
         self.beta = resources.AsyncBetaWithStreamingResponse(client.beta)
+        self.batches = resources.AsyncBatchesWithStreamingResponse(client.batches)
 
 
 Client = OpenAI
 
 AsyncClient = AsyncOpenAI
```

### Comparing `openai_mealuet-1.16.2/src/openai/_compat.py` & `openai_mealuet-1.23.4/src/openai/_compat.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_exceptions.py` & `openai_mealuet-1.23.4/src/openai/_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,19 +72,21 @@
 
 
 class APIStatusError(APIError):
     """Raised when an API response has a status code of 4xx or 5xx."""
 
     response: httpx.Response
     status_code: int
+    request_id: str | None
 
     def __init__(self, message: str, *, response: httpx.Response, body: object | None) -> None:
         super().__init__(message, response.request, body=body)
         self.response = response
         self.status_code = response.status_code
+        self.request_id = response.headers.get("x-request-id")
 
 
 class APIConnectionError(APIError):
     def __init__(self, *, message: str = "Connection error.", request: httpx.Request) -> None:
         super().__init__(message, request, body=None)
```

### Comparing `openai_mealuet-1.16.2/src/openai/_files.py` & `openai_mealuet-1.23.4/src/openai/_files.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_legacy_response.py` & `openai_mealuet-1.23.4/src/openai/_legacy_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,18 @@
         self._client = client
         self._parsed_by_type = {}
         self._stream = stream
         self._stream_cls = stream_cls
         self._options = options
         self.http_response = raw
 
+    @property
+    def request_id(self) -> str | None:
+        return self.http_response.headers.get("x-request-id")  # type: ignore[no-any-return]
+
     @overload
     def parse(self, *, to: type[_T]) -> _T:
         ...
 
     @overload
     def parse(self) -> R:
         ...
```

### Comparing `openai_mealuet-1.16.2/src/openai/_models.py` & `openai_mealuet-1.23.4/src/openai/_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import os
 import inspect
 from typing import TYPE_CHECKING, Any, Type, Union, Generic, TypeVar, Callable, cast
 from datetime import date, datetime
-from functools import lru_cache
 from typing_extensions import (
     Unpack,
     Literal,
     ClassVar,
     Protocol,
     Required,
     TypedDict,
@@ -33,14 +32,15 @@
     AnyMapping,
     HttpxRequestFiles,
 )
 from ._utils import (
     PropertyInfo,
     is_list,
     is_given,
+    lru_cache,
     is_mapping,
     parse_date,
     coerce_boolean,
     parse_datetime,
     strip_not_given,
     extract_type_arg,
     is_annotated_type,
@@ -86,14 +86,87 @@
         def model_fields_set(self) -> set[str]:
             # a forwards-compat shim for pydantic v2
             return self.__fields_set__  # type: ignore
 
         class Config(pydantic.BaseConfig):  # pyright: ignore[reportDeprecated]
             extra: Any = pydantic.Extra.allow  # type: ignore
 
+    def to_dict(
+        self,
+        *,
+        mode: Literal["json", "python"] = "python",
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> dict[str, object]:
+        """Recursively generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            mode:
+                If mode is 'json', the dictionary will only contain JSON serializable types. e.g. `datetime` will be turned into a string, `"2024-3-22T18:11:19.117000Z"`.
+                If mode is 'python', the dictionary may contain any Python objects. e.g. `datetime(2024, 3, 22)`
+
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that are set to their default value from the output.
+            exclude_none: Whether to exclude fields that have a value of `None` from the output.
+            warnings: Whether to log warnings when invalid fields are encountered. This is only supported in Pydantic v2.
+        """
+        return self.model_dump(
+            mode=mode,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
+    def to_json(
+        self,
+        *,
+        indent: int | None = 2,
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> str:
+        """Generates a JSON string representing this model as it would be received from or sent to the API (but with indentation).
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            indent: Indentation to use in the JSON output. If `None` is passed, the output will be compact. Defaults to `2`
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that have the default value.
+            exclude_none: Whether to exclude fields that have a value of `None`.
+            warnings: Whether to show any warnings that occurred during serialization. This is only supported in Pydantic v2.
+        """
+        return self.model_dump_json(
+            indent=indent,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
     @override
     def __str__(self) -> str:
         # mypy complains about an invalid self arg
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'  # type: ignore[misc]
 
     # Override the 'construct' method in a way that supports recursive parsing without validation.
     # Based on https://github.com/samuelcolvin/pydantic/issues/1168#issuecomment-817742836.
@@ -301,15 +374,15 @@
     """
     # we allow `object` as the input type because otherwise, passing things like
     # `Literal['value']` will be reported as a type error by type checkers
     type_ = cast("type[object]", type_)
 
     # unwrap `Annotated[T, ...]` -> `T`
     if is_annotated_type(type_):
-        meta = get_args(type_)[1:]
+        meta: tuple[Any, ...] = get_args(type_)[1:]
         type_ = extract_type_arg(type_, 0)
     else:
         meta = tuple()
 
     # we need to use the origin class for any types that are subscripted generics
     # e.g. Dict[str, object]
     origin = get_origin(type_) or type_
```

### Comparing `openai_mealuet-1.16.2/src/openai/_module_client.py` & `openai_mealuet-1.23.4/src/openai/_module_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 
 class ModelsProxy(LazyProxy[resources.Models]):
     @override
     def __load__(self) -> resources.Models:
         return _load_client().models
 
 
+class BatchesProxy(LazyProxy[resources.Batches]):
+    @override
+    def __load__(self) -> resources.Batches:
+        return _load_client().batches
+
+
 class EmbeddingsProxy(LazyProxy[resources.Embeddings]):
     @override
     def __load__(self) -> resources.Embeddings:
         return _load_client().embeddings
 
 
 class CompletionsProxy(LazyProxy[resources.Completions]):
@@ -68,11 +74,12 @@
 
 chat: resources.Chat = ChatProxy().__as_proxied__()
 beta: resources.Beta = BetaProxy().__as_proxied__()
 files: resources.Files = FilesProxy().__as_proxied__()
 audio: resources.Audio = AudioProxy().__as_proxied__()
 images: resources.Images = ImagesProxy().__as_proxied__()
 models: resources.Models = ModelsProxy().__as_proxied__()
+batches: resources.Batches = BatchesProxy().__as_proxied__()
 embeddings: resources.Embeddings = EmbeddingsProxy().__as_proxied__()
 completions: resources.Completions = CompletionsProxy().__as_proxied__()
 moderations: resources.Moderations = ModerationsProxy().__as_proxied__()
 fine_tuning: resources.FineTuning = FineTuningProxy().__as_proxied__()
```

### Comparing `openai_mealuet-1.16.2/src/openai/_qs.py` & `openai_mealuet-1.23.4/src/openai/_qs.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_resource.py` & `openai_mealuet-1.23.4/src/openai/_resource.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_response.py` & `openai_mealuet-1.23.4/src/openai/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,18 @@
             data=data,
             cast_to=cast_to,  # type: ignore
             response=response,
         )
 
 
 class APIResponse(BaseAPIResponse[R]):
+    @property
+    def request_id(self) -> str | None:
+        return self.http_response.headers.get("x-request-id")  # type: ignore[no-any-return]
+
     @overload
     def parse(self, *, to: type[_T]) -> _T:
         ...
 
     @overload
     def parse(self) -> R:
         ...
@@ -358,14 +362,18 @@
     def iter_lines(self) -> Iterator[str]:
         """Like `iter_text()` but will only yield chunks for each line"""
         for chunk in self.http_response.iter_lines():
             yield chunk
 
 
 class AsyncAPIResponse(BaseAPIResponse[R]):
+    @property
+    def request_id(self) -> str | None:
+        return self.http_response.headers.get("x-request-id")  # type: ignore[no-any-return]
+
     @overload
     async def parse(self, *, to: type[_T]) -> _T:
         ...
 
     @overload
     async def parse(self) -> R:
         ...
```

### Comparing `openai_mealuet-1.16.2/src/openai/_streaming.py` & `openai_mealuet-1.23.4/src/openai/_streaming.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_types.py` & `openai_mealuet-1.23.4/src/openai/_types.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/pagination.py` & `openai_mealuet-1.23.4/src/openai/pagination.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_extras/numpy_proxy.py` & `openai_mealuet-1.23.4/src/openai/_extras/numpy_proxy.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_extras/pandas_proxy.py` & `openai_mealuet-1.23.4/src/openai/_extras/pandas_proxy.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_utils/__init__.py` & `openai_mealuet-1.23.4/src/openai/_utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._proxy import LazyProxy as LazyProxy
 from ._utils import (
     flatten as flatten,
     is_dict as is_dict,
     is_list as is_list,
     is_given as is_given,
     is_tuple as is_tuple,
+    lru_cache as lru_cache,
     is_mapping as is_mapping,
     is_tuple_t as is_tuple_t,
     parse_date as parse_date,
     is_iterable as is_iterable,
     is_sequence as is_sequence,
     coerce_float as coerce_float,
     is_mapping_t as is_mapping_t,
```

### Comparing `openai_mealuet-1.16.2/src/openai/_utils/_logs.py` & `openai_mealuet-1.23.4/src/openai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_utils/_proxy.py` & `openai_mealuet-1.23.4/src/openai/_utils/_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 T = TypeVar("T")
 
 
 class LazyProxy(Generic[T], ABC):
     """Implements data methods to pretend that an instance is another instance.
 
-    This includes forwarding attribute access and othe methods.
+    This includes forwarding attribute access and other methods.
     """
 
     # Note: we have to special case proxies that themselves return proxies
     # to support using a proxy as a catch-all for any random access, e.g. `proxy.foo.bar.baz`
 
     def __getattr__(self, attr: str) -> object:
         proxied = self.__get_proxied__()
```

### Comparing `openai_mealuet-1.16.2/src/openai/_utils/_sync.py` & `openai_mealuet-1.23.4/src/openai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_utils/_transform.py` & `openai_mealuet-1.23.4/src/openai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_utils/_typing.py` & `openai_mealuet-1.23.4/src/openai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/_utils/_utils.py` & `openai_mealuet-1.23.4/src/openai/_utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,16 @@
             else:  # no break
                 if len(variants) > 1:
                     variations = human_join(
                         ["(" + human_join([quote(arg) for arg in variant], final="and") + ")" for variant in variants]
                     )
                     msg = f"Missing required arguments; Expected either {variations} arguments to be given"
                 else:
+                    assert len(variants) > 0
+
                     # TODO: this error message is not deterministic
                     missing = list(set(variants[0]) - given_params)
                     if len(missing) > 1:
                         msg = f"Missing required arguments: {human_join([quote(arg) for arg in missing])}"
                     else:
                         msg = f"Missing required argument: {quote(missing[0])}"
                 raise TypeError(msg)
@@ -385,7 +387,17 @@
 
 
 def get_async_library() -> str:
     try:
         return sniffio.current_async_library()
     except Exception:
         return "false"
+
+
+def lru_cache(*, maxsize: int | None = 128) -> Callable[[CallableT], CallableT]:
+    """A version of functools.lru_cache that retains the type signature
+    for the wrapped function arguments.
+    """
+    wrapper = functools.lru_cache(  # noqa: TID251
+        maxsize=maxsize,
+    )
+    return cast(Any, wrapper)  # type: ignore[no-any-return]
```

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_cli.py` & `openai_mealuet-1.23.4/src/openai/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_progress.py` & `openai_mealuet-1.23.4/src/openai/cli/_progress.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_utils.py` & `openai_mealuet-1.23.4/src/openai/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_api/audio.py` & `openai_mealuet-1.23.4/src/openai/cli/_api/audio.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_api/completions.py` & `openai_mealuet-1.23.4/src/openai/cli/_api/completions.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_api/files.py` & `openai_mealuet-1.23.4/src/openai/cli/_api/files.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_api/image.py` & `openai_mealuet-1.23.4/src/openai/cli/_api/image.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_api/models.py` & `openai_mealuet-1.23.4/src/openai/cli/_api/models.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_api/chat/completions.py` & `openai_mealuet-1.23.4/src/openai/cli/_api/chat/completions.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_tools/fine_tunes.py` & `openai_mealuet-1.23.4/src/openai/cli/_tools/fine_tunes.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/cli/_tools/migrate.py` & `openai_mealuet-1.23.4/src/openai/cli/_tools/migrate.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/lib/_old_api.py` & `openai_mealuet-1.23.4/src/openai/lib/_old_api.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/lib/_validators.py` & `openai_mealuet-1.23.4/src/openai/lib/_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,27 +674,31 @@
         if split:
             assert len(fnames) == 2 and "train" in fnames[0] and "valid" in fnames[1]
             MAX_VALID_EXAMPLES = 1000
             n_train = max(len(df) - MAX_VALID_EXAMPLES, int(len(df) * 0.8))
             df_train = df.sample(n=n_train, random_state=42)
             df_valid = df.drop(df_train.index)
             df_train[["prompt", "completion"]].to_json(  # type: ignore
-                fnames[0], lines=True, orient="records", force_ascii=False
+                fnames[0], lines=True, orient="records", force_ascii=False, indent=None
+            )
+            df_valid[["prompt", "completion"]].to_json(
+                fnames[1], lines=True, orient="records", force_ascii=False, indent=None
             )
-            df_valid[["prompt", "completion"]].to_json(fnames[1], lines=True, orient="records", force_ascii=False)
 
             n_classes, pos_class = get_classification_hyperparams(df)
             additional_params += " --compute_classification_metrics"
             if n_classes == 2:
                 additional_params += f' --classification_positive_class "{pos_class}"'
             else:
                 additional_params += f" --classification_n_classes {n_classes}"
         else:
             assert len(fnames) == 1
-            df[["prompt", "completion"]].to_json(fnames[0], lines=True, orient="records", force_ascii=False)
+            df[["prompt", "completion"]].to_json(
+                fnames[0], lines=True, orient="records", force_ascii=False, indent=None
+            )
 
         # Add -v VALID_FILE if we split the file into train / valid
         files_string = ("s" if split else "") + " to `" + ("` and `".join(fnames))
         valid_string = f' -v "{fnames[1]}"' if split else ""
         separator_reminder = (
             ""
             if len(common_prompt_suffix_new_line_handled) == 0
```

### Comparing `openai_mealuet-1.16.2/src/openai/lib/azure.py` & `openai_mealuet-1.23.4/src/openai/lib/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,27 +126,29 @@
         api_version: str | None = None,
         azure_endpoint: str | None = None,
         azure_deployment: str | None = None,
         api_key: str | None = None,
         azure_ad_token: str | None = None,
         azure_ad_token_provider: AzureADTokenProvider | None = None,
         organization: str | None = None,
+        project: str | None = None,
         base_url: str | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         http_client: httpx.Client | None = None,
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous azure openai client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
         - `api_key` from `AZURE_OPENAI_API_KEY`
         - `organization` from `OPENAI_ORG_ID`
+        - `project` from `OPENAI_PROJECT_ID`
         - `azure_ad_token` from `AZURE_OPENAI_AD_TOKEN`
         - `api_version` from `OPENAI_API_VERSION`
         - `azure_endpoint` from `AZURE_OPENAI_ENDPOINT`
 
         Args:
             azure_endpoint: Your Azure endpoint, including the resource, e.g. `https://example-resource.azure.openai.com/`
 
@@ -201,14 +203,15 @@
         if api_key is None:
             # define a sentinel value to avoid any typing issues
             api_key = API_KEY_SENTINEL
 
         super().__init__(
             api_key=api_key,
             organization=organization,
+            project=project,
             base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
             default_headers=default_headers,
             default_query=default_query,
             http_client=http_client,
             _strict_response_validation=_strict_response_validation,
@@ -219,14 +222,15 @@
 
     @override
     def copy(
         self,
         *,
         api_key: str | None = None,
         organization: str | None = None,
+        project: str | None = None,
         api_version: str | None = None,
         azure_ad_token: str | None = None,
         azure_ad_token_provider: AzureADTokenProvider | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.Client | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
@@ -238,14 +242,15 @@
     ) -> Self:
         """
         Create a new client instance re-using the same options given to the current client with optional overriding.
         """
         return super().copy(
             api_key=api_key,
             organization=organization,
+            project=project,
             base_url=base_url,
             timeout=timeout,
             http_client=http_client,
             max_retries=max_retries,
             default_headers=default_headers,
             set_default_headers=set_default_headers,
             default_query=default_query,
@@ -302,14 +307,15 @@
         azure_endpoint: str,
         azure_deployment: str | None = None,
         api_version: str | None = None,
         api_key: str | None = None,
         azure_ad_token: str | None = None,
         azure_ad_token_provider: AsyncAzureADTokenProvider | None = None,
         organization: str | None = None,
+        project: str | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         http_client: httpx.AsyncClient | None = None,
         _strict_response_validation: bool = False,
     ) -> None:
@@ -321,14 +327,15 @@
         *,
         azure_deployment: str | None = None,
         api_version: str | None = None,
         api_key: str | None = None,
         azure_ad_token: str | None = None,
         azure_ad_token_provider: AsyncAzureADTokenProvider | None = None,
         organization: str | None = None,
+        project: str | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         http_client: httpx.AsyncClient | None = None,
         _strict_response_validation: bool = False,
     ) -> None:
@@ -340,14 +347,15 @@
         *,
         base_url: str,
         api_version: str | None = None,
         api_key: str | None = None,
         azure_ad_token: str | None = None,
         azure_ad_token_provider: AsyncAzureADTokenProvider | None = None,
         organization: str | None = None,
+        project: str | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         http_client: httpx.AsyncClient | None = None,
         _strict_response_validation: bool = False,
     ) -> None:
@@ -359,27 +367,29 @@
         azure_endpoint: str | None = None,
         azure_deployment: str | None = None,
         api_version: str | None = None,
         api_key: str | None = None,
         azure_ad_token: str | None = None,
         azure_ad_token_provider: AsyncAzureADTokenProvider | None = None,
         organization: str | None = None,
+        project: str | None = None,
         base_url: str | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         http_client: httpx.AsyncClient | None = None,
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new asynchronous azure openai client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
         - `api_key` from `AZURE_OPENAI_API_KEY`
         - `organization` from `OPENAI_ORG_ID`
+        - `project` from `OPENAI_PROJECT_ID`
         - `azure_ad_token` from `AZURE_OPENAI_AD_TOKEN`
         - `api_version` from `OPENAI_API_VERSION`
         - `azure_endpoint` from `AZURE_OPENAI_ENDPOINT`
 
         Args:
             azure_endpoint: Your Azure endpoint, including the resource, e.g. `https://example-resource.azure.openai.com/`
 
@@ -434,14 +444,15 @@
         if api_key is None:
             # define a sentinel value to avoid any typing issues
             api_key = API_KEY_SENTINEL
 
         super().__init__(
             api_key=api_key,
             organization=organization,
+            project=project,
             base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
             default_headers=default_headers,
             default_query=default_query,
             http_client=http_client,
             _strict_response_validation=_strict_response_validation,
@@ -452,14 +463,15 @@
 
     @override
     def copy(
         self,
         *,
         api_key: str | None = None,
         organization: str | None = None,
+        project: str | None = None,
         api_version: str | None = None,
         azure_ad_token: str | None = None,
         azure_ad_token_provider: AsyncAzureADTokenProvider | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.AsyncClient | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
@@ -471,14 +483,15 @@
     ) -> Self:
         """
         Create a new client instance re-using the same options given to the current client with optional overriding.
         """
         return super().copy(
             api_key=api_key,
             organization=organization,
+            project=project,
             base_url=base_url,
             timeout=timeout,
             http_client=http_client,
             max_retries=max_retries,
             default_headers=default_headers,
             set_default_headers=set_default_headers,
             default_query=default_query,
```

### Comparing `openai_mealuet-1.16.2/src/openai/lib/streaming/_assistants.py` & `openai_mealuet-1.23.4/src/openai/lib/streaming/_assistants.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/__init__.py` & `openai_mealuet-1.23.4/src/openai/resources/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,22 @@
     Models,
     AsyncModels,
     ModelsWithRawResponse,
     AsyncModelsWithRawResponse,
     ModelsWithStreamingResponse,
     AsyncModelsWithStreamingResponse,
 )
+from .batches import (
+    Batches,
+    AsyncBatches,
+    BatchesWithRawResponse,
+    AsyncBatchesWithRawResponse,
+    BatchesWithStreamingResponse,
+    AsyncBatchesWithStreamingResponse,
+)
 from .embeddings import (
     Embeddings,
     AsyncEmbeddings,
     EmbeddingsWithRawResponse,
     AsyncEmbeddingsWithRawResponse,
     EmbeddingsWithStreamingResponse,
     AsyncEmbeddingsWithStreamingResponse,
@@ -138,8 +146,14 @@
     "AsyncFineTuningWithStreamingResponse",
     "Beta",
     "AsyncBeta",
     "BetaWithRawResponse",
     "AsyncBetaWithRawResponse",
     "BetaWithStreamingResponse",
     "AsyncBetaWithStreamingResponse",
+    "Batches",
+    "AsyncBatches",
+    "BatchesWithRawResponse",
+    "AsyncBatchesWithRawResponse",
+    "BatchesWithStreamingResponse",
+    "AsyncBatchesWithStreamingResponse",
 ]
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/completions.py` & `openai_mealuet-1.23.4/src/openai/resources/completions.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 
 from typing import Dict, List, Union, Iterable, Optional, overload
 from typing_extensions import Literal
 
 import httpx
 
 from .. import _legacy_response
-from ..types import Completion, completion_create_params
+from ..types import completion_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     required_args,
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from .._streaming import Stream, AsyncStream
 from .._base_client import (
     make_request_options,
 )
+from ..types.completion import Completion
 
 __all__ = ["Completions", "AsyncCompletions"]
 
 
 class Completions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> CompletionsWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/embeddings.py` & `openai_mealuet-1.23.4/src/openai/resources/embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import base64
 from typing import List, Union, Iterable, cast
 from typing_extensions import Literal
 
 import httpx
 
 from .. import _legacy_response
-from ..types import CreateEmbeddingResponse, embedding_create_params
+from ..types import embedding_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import is_given, maybe_transform
 from .._compat import cached_property
 from .._extras import numpy as np, has_numpy
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from .._base_client import (
     make_request_options,
 )
+from ..types.create_embedding_response import CreateEmbeddingResponse
 
 __all__ = ["Embeddings", "AsyncEmbeddings"]
 
 
 class Embeddings(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> EmbeddingsWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/files.py` & `openai_mealuet-1.23.4/src/openai/resources/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing_extensions
 from typing import Mapping, cast
 from typing_extensions import Literal
 
 import httpx
 
 from .. import _legacy_response
-from ..types import FileObject, FileDeleted, file_list_params, file_create_params
+from ..types import file_list_params, file_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
 from .._utils import (
     extract_files,
     maybe_transform,
     deepcopy_minimal,
     async_maybe_transform,
 )
@@ -29,14 +29,16 @@
     async_to_custom_streamed_response_wrapper,
 )
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ..types.file_object import FileObject
+from ..types.file_deleted import FileDeleted
 
 __all__ = ["Files", "AsyncFiles"]
 
 
 class Files(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> FilesWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/images.py` & `openai_mealuet-1.23.4/src/openai/resources/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,29 @@
 
 from typing import Union, Mapping, Optional, cast
 from typing_extensions import Literal
 
 import httpx
 
 from .. import _legacy_response
-from ..types import (
-    ImagesResponse,
-    image_edit_params,
-    image_generate_params,
-    image_create_variation_params,
-)
+from ..types import image_edit_params, image_generate_params, image_create_variation_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
 from .._utils import (
     extract_files,
     maybe_transform,
     deepcopy_minimal,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from .._base_client import (
     make_request_options,
 )
+from ..types.images_response import ImagesResponse
 
 __all__ = ["Images", "AsyncImages"]
 
 
 class Images(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> ImagesWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/models.py` & `openai_mealuet-1.23.4/src/openai/resources/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import httpx
 
 from .. import _legacy_response
-from ..types import Model, ModelDeleted
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..pagination import SyncPage, AsyncPage
+from ..types.model import Model
 from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ..types.model_deleted import ModelDeleted
 
 __all__ = ["Models", "AsyncModels"]
 
 
 class Models(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> ModelsWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/moderations.py` & `openai_mealuet-1.23.4/src/openai/resources/moderations.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 
 from typing import List, Union
 from typing_extensions import Literal
 
 import httpx
 
 from .. import _legacy_response
-from ..types import ModerationCreateResponse, moderation_create_params
+from ..types import moderation_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from .._base_client import (
     make_request_options,
 )
+from ..types.moderation_create_response import ModerationCreateResponse
 
 __all__ = ["Moderations", "AsyncModerations"]
 
 
 class Moderations(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> ModerationsWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/audio/__init__.py` & `openai_mealuet-1.23.4/src/openai/resources/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/audio/audio.py` & `openai_mealuet-1.23.4/src/openai/resources/audio/audio.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/audio/speech.py` & `openai_mealuet-1.23.4/src/openai/resources/audio/speech.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/audio/transcriptions.py` & `openai_mealuet-1.23.4/src/openai/resources/audio/transcriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     maybe_transform,
     deepcopy_minimal,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
-from ...types.audio import Transcription, transcription_create_params
+from ...types.audio import transcription_create_params
 from ..._base_client import (
     make_request_options,
 )
+from ...types.audio.transcription import Transcription
 
 __all__ = ["Transcriptions", "AsyncTranscriptions"]
 
 
 class Transcriptions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> TranscriptionsWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/audio/translations.py` & `openai_mealuet-1.23.4/src/openai/resources/audio/translations.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     maybe_transform,
     deepcopy_minimal,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
-from ...types.audio import Translation, translation_create_params
+from ...types.audio import translation_create_params
 from ..._base_client import (
     make_request_options,
 )
+from ...types.audio.translation import Translation
 
 __all__ = ["Translations", "AsyncTranslations"]
 
 
 class Translations(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> TranslationsWithRawResponse:
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/__init__.py` & `openai_mealuet-1.23.4/src/openai/resources/beta/threads/runs/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,33 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from .beta import (
-    Beta,
-    AsyncBeta,
-    BetaWithRawResponse,
-    AsyncBetaWithRawResponse,
-    BetaWithStreamingResponse,
-    AsyncBetaWithStreamingResponse,
+from .runs import (
+    Runs,
+    AsyncRuns,
+    RunsWithRawResponse,
+    AsyncRunsWithRawResponse,
+    RunsWithStreamingResponse,
+    AsyncRunsWithStreamingResponse,
 )
-from .threads import (
-    Threads,
-    AsyncThreads,
-    ThreadsWithRawResponse,
-    AsyncThreadsWithRawResponse,
-    ThreadsWithStreamingResponse,
-    AsyncThreadsWithStreamingResponse,
-)
-from .assistants import (
-    Assistants,
-    AsyncAssistants,
-    AssistantsWithRawResponse,
-    AsyncAssistantsWithRawResponse,
-    AssistantsWithStreamingResponse,
-    AsyncAssistantsWithStreamingResponse,
+from .steps import (
+    Steps,
+    AsyncSteps,
+    StepsWithRawResponse,
+    AsyncStepsWithRawResponse,
+    StepsWithStreamingResponse,
+    AsyncStepsWithStreamingResponse,
 )
 
 __all__ = [
-    "Assistants",
-    "AsyncAssistants",
-    "AssistantsWithRawResponse",
-    "AsyncAssistantsWithRawResponse",
-    "AssistantsWithStreamingResponse",
-    "AsyncAssistantsWithStreamingResponse",
-    "Threads",
-    "AsyncThreads",
-    "ThreadsWithRawResponse",
-    "AsyncThreadsWithRawResponse",
-    "ThreadsWithStreamingResponse",
-    "AsyncThreadsWithStreamingResponse",
-    "Beta",
-    "AsyncBeta",
-    "BetaWithRawResponse",
-    "AsyncBetaWithRawResponse",
-    "BetaWithStreamingResponse",
-    "AsyncBetaWithStreamingResponse",
+    "Steps",
+    "AsyncSteps",
+    "StepsWithRawResponse",
+    "AsyncStepsWithRawResponse",
+    "StepsWithStreamingResponse",
+    "AsyncStepsWithStreamingResponse",
+    "Runs",
+    "AsyncRuns",
+    "RunsWithRawResponse",
+    "AsyncRunsWithRawResponse",
+    "RunsWithStreamingResponse",
+    "AsyncRunsWithStreamingResponse",
 ]
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/assistants/assistants.py` & `openai_mealuet-1.23.4/src/openai/resources/beta/threads/messages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,273 +1,211 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import List, Iterable, Optional
+from typing import Iterable, Optional
 from typing_extensions import Literal
 
 import httpx
 
 from .... import _legacy_response
-from .files import (
-    Files,
-    AsyncFiles,
-    FilesWithRawResponse,
-    AsyncFilesWithRawResponse,
-    FilesWithStreamingResponse,
-    AsyncFilesWithStreamingResponse,
-)
 from ...._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ...._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from ...._compat import cached_property
 from ...._resource import SyncAPIResource, AsyncAPIResource
 from ...._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ....pagination import SyncCursorPage, AsyncCursorPage
-from ....types.beta import (
-    Assistant,
-    AssistantDeleted,
-    AssistantToolParam,
-    assistant_list_params,
-    assistant_create_params,
-    assistant_update_params,
-)
 from ...._base_client import (
     AsyncPaginator,
     make_request_options,
 )
+from ....types.beta.threads import message_list_params, message_create_params, message_update_params
+from ....types.beta.threads.message import Message
 
-__all__ = ["Assistants", "AsyncAssistants"]
+__all__ = ["Messages", "AsyncMessages"]
 
 
-class Assistants(SyncAPIResource):
-    @cached_property
-    def files(self) -> Files:
-        return Files(self._client)
-
+class Messages(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AssistantsWithRawResponse:
-        return AssistantsWithRawResponse(self)
+    def with_raw_response(self) -> MessagesWithRawResponse:
+        return MessagesWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AssistantsWithStreamingResponse:
-        return AssistantsWithStreamingResponse(self)
+    def with_streaming_response(self) -> MessagesWithStreamingResponse:
+        return MessagesWithStreamingResponse(self)
 
     def create(
         self,
+        thread_id: str,
         *,
-        model: str,
-        description: Optional[str] | NotGiven = NOT_GIVEN,
-        file_ids: List[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        content: str,
+        role: Literal["user", "assistant"],
+        attachments: Optional[Iterable[message_create_params.Attachment]] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        name: Optional[str] | NotGiven = NOT_GIVEN,
-        tools: Iterable[AssistantToolParam] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> Message:
         """
-        Create an assistant with a model and instructions.
+        Create a message.
 
         Args:
-          model: ID of the model to use. You can use the
-              [List models](https://platform.openai.com/docs/api-reference/models/list) API to
-              see all of your available models, or see our
-              [Model overview](https://platform.openai.com/docs/models/overview) for
-              descriptions of them.
-
-          description: The description of the assistant. The maximum length is 512 characters.
-
-          file_ids: A list of [file](https://platform.openai.com/docs/api-reference/files) IDs
-              attached to this assistant. There can be a maximum of 20 files attached to the
-              assistant. Files are ordered by their creation date in ascending order.
+          content: The content of the message.
 
-          instructions: The system instructions that the assistant uses. The maximum length is 32768
-              characters.
+          role:
+              The role of the entity that is creating the message. Allowed values include:
+
+              - `user`: Indicates the message is sent by an actual user and should be used in
+                most cases to represent user-generated messages.
+              - `assistant`: Indicates the message is generated by the assistant. Use this
+                value to insert messages from the assistant into the conversation.
+
+          attachments: A list of files attached to the message, and the tools they should be added to.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
-          name: The name of the assistant. The maximum length is 256 characters.
-
-          tools: A list of tool enabled on the assistant. There can be a maximum of 128 tools per
-              assistant. Tools can be of types `code_interpreter`, `retrieval`, or `function`.
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._post(
-            "/assistants",
+            f"/threads/{thread_id}/messages",
             body=maybe_transform(
                 {
-                    "model": model,
-                    "description": description,
-                    "file_ids": file_ids,
-                    "instructions": instructions,
+                    "content": content,
+                    "role": role,
+                    "attachments": attachments,
                     "metadata": metadata,
-                    "name": name,
-                    "tools": tools,
                 },
-                assistant_create_params.AssistantCreateParams,
+                message_create_params.MessageCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=Message,
         )
 
     def retrieve(
         self,
-        assistant_id: str,
+        message_id: str,
         *,
+        thread_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> Message:
         """
-        Retrieves an assistant.
+        Retrieve a message.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        if not message_id:
+            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._get(
-            f"/assistants/{assistant_id}",
+            f"/threads/{thread_id}/messages/{message_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=Message,
         )
 
     def update(
         self,
-        assistant_id: str,
+        message_id: str,
         *,
-        description: Optional[str] | NotGiven = NOT_GIVEN,
-        file_ids: List[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        thread_id: str,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: str | NotGiven = NOT_GIVEN,
-        name: Optional[str] | NotGiven = NOT_GIVEN,
-        tools: Iterable[AssistantToolParam] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
-        """Modifies an assistant.
+    ) -> Message:
+        """
+        Modifies a message.
 
         Args:
-          description: The description of the assistant.
-
-        The maximum length is 512 characters.
-
-          file_ids: A list of [File](https://platform.openai.com/docs/api-reference/files) IDs
-              attached to this assistant. There can be a maximum of 20 files attached to the
-              assistant. Files are ordered by their creation date in ascending order. If a
-              file was previously attached to the list but does not show up in the list, it
-              will be deleted from the assistant.
-
-          instructions: The system instructions that the assistant uses. The maximum length is 32768
-              characters.
-
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
-          model: ID of the model to use. You can use the
-              [List models](https://platform.openai.com/docs/api-reference/models/list) API to
-              see all of your available models, or see our
-              [Model overview](https://platform.openai.com/docs/models/overview) for
-              descriptions of them.
-
-          name: The name of the assistant. The maximum length is 256 characters.
-
-          tools: A list of tool enabled on the assistant. There can be a maximum of 128 tools per
-              assistant. Tools can be of types `code_interpreter`, `retrieval`, or `function`.
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        if not message_id:
+            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._post(
-            f"/assistants/{assistant_id}",
-            body=maybe_transform(
-                {
-                    "description": description,
-                    "file_ids": file_ids,
-                    "instructions": instructions,
-                    "metadata": metadata,
-                    "model": model,
-                    "name": name,
-                    "tools": tools,
-                },
-                assistant_update_params.AssistantUpdateParams,
-            ),
+            f"/threads/{thread_id}/messages/{message_id}",
+            body=maybe_transform({"metadata": metadata}, message_update_params.MessageUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=Message,
         )
 
     def list(
         self,
+        thread_id: str,
         *,
         after: str | NotGiven = NOT_GIVEN,
         before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
+        run_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SyncCursorPage[Assistant]:
-        """Returns a list of assistants.
+    ) -> SyncCursorPage[Message]:
+        """
+        Returns a list of messages for a given thread.
 
         Args:
-          after: A cursor for use in pagination.
-
-        `after` is an object ID that defines your place
+          after: A cursor for use in pagination. `after` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include after=obj_foo in order to
               fetch the next page of the list.
 
           before: A cursor for use in pagination. `before` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include before=obj_foo in order to
@@ -275,302 +213,225 @@
 
           limit: A limit on the number of objects to be returned. Limit can range between 1 and
               100, and the default is 20.
 
           order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
               order and `desc` for descending order.
 
+          run_id: Filter messages by the run ID that generated them.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._get_api_list(
-            "/assistants",
-            page=SyncCursorPage[Assistant],
+            f"/threads/{thread_id}/messages",
+            page=SyncCursorPage[Message],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
                         "before": before,
                         "limit": limit,
                         "order": order,
+                        "run_id": run_id,
                     },
-                    assistant_list_params.AssistantListParams,
+                    message_list_params.MessageListParams,
                 ),
             ),
-            model=Assistant,
+            model=Message,
         )
 
-    def delete(
-        self,
-        assistant_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantDeleted:
-        """
-        Delete an assistant.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._delete(
-            f"/assistants/{assistant_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=AssistantDeleted,
-        )
-
-
-class AsyncAssistants(AsyncAPIResource):
-    @cached_property
-    def files(self) -> AsyncFiles:
-        return AsyncFiles(self._client)
 
+class AsyncMessages(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncAssistantsWithRawResponse:
-        return AsyncAssistantsWithRawResponse(self)
+    def with_raw_response(self) -> AsyncMessagesWithRawResponse:
+        return AsyncMessagesWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncAssistantsWithStreamingResponse:
-        return AsyncAssistantsWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncMessagesWithStreamingResponse:
+        return AsyncMessagesWithStreamingResponse(self)
 
     async def create(
         self,
+        thread_id: str,
         *,
-        model: str,
-        description: Optional[str] | NotGiven = NOT_GIVEN,
-        file_ids: List[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        content: str,
+        role: Literal["user", "assistant"],
+        attachments: Optional[Iterable[message_create_params.Attachment]] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        name: Optional[str] | NotGiven = NOT_GIVEN,
-        tools: Iterable[AssistantToolParam] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> Message:
         """
-        Create an assistant with a model and instructions.
+        Create a message.
 
         Args:
-          model: ID of the model to use. You can use the
-              [List models](https://platform.openai.com/docs/api-reference/models/list) API to
-              see all of your available models, or see our
-              [Model overview](https://platform.openai.com/docs/models/overview) for
-              descriptions of them.
-
-          description: The description of the assistant. The maximum length is 512 characters.
-
-          file_ids: A list of [file](https://platform.openai.com/docs/api-reference/files) IDs
-              attached to this assistant. There can be a maximum of 20 files attached to the
-              assistant. Files are ordered by their creation date in ascending order.
+          content: The content of the message.
 
-          instructions: The system instructions that the assistant uses. The maximum length is 32768
-              characters.
+          role:
+              The role of the entity that is creating the message. Allowed values include:
+
+              - `user`: Indicates the message is sent by an actual user and should be used in
+                most cases to represent user-generated messages.
+              - `assistant`: Indicates the message is generated by the assistant. Use this
+                value to insert messages from the assistant into the conversation.
+
+          attachments: A list of files attached to the message, and the tools they should be added to.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
-          name: The name of the assistant. The maximum length is 256 characters.
-
-          tools: A list of tool enabled on the assistant. There can be a maximum of 128 tools per
-              assistant. Tools can be of types `code_interpreter`, `retrieval`, or `function`.
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return await self._post(
-            "/assistants",
+            f"/threads/{thread_id}/messages",
             body=await async_maybe_transform(
                 {
-                    "model": model,
-                    "description": description,
-                    "file_ids": file_ids,
-                    "instructions": instructions,
+                    "content": content,
+                    "role": role,
+                    "attachments": attachments,
                     "metadata": metadata,
-                    "name": name,
-                    "tools": tools,
                 },
-                assistant_create_params.AssistantCreateParams,
+                message_create_params.MessageCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=Message,
         )
 
     async def retrieve(
         self,
-        assistant_id: str,
+        message_id: str,
         *,
+        thread_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> Message:
         """
-        Retrieves an assistant.
+        Retrieve a message.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        if not message_id:
+            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return await self._get(
-            f"/assistants/{assistant_id}",
+            f"/threads/{thread_id}/messages/{message_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=Message,
         )
 
     async def update(
         self,
-        assistant_id: str,
+        message_id: str,
         *,
-        description: Optional[str] | NotGiven = NOT_GIVEN,
-        file_ids: List[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        thread_id: str,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: str | NotGiven = NOT_GIVEN,
-        name: Optional[str] | NotGiven = NOT_GIVEN,
-        tools: Iterable[AssistantToolParam] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
-        """Modifies an assistant.
+    ) -> Message:
+        """
+        Modifies a message.
 
         Args:
-          description: The description of the assistant.
-
-        The maximum length is 512 characters.
-
-          file_ids: A list of [File](https://platform.openai.com/docs/api-reference/files) IDs
-              attached to this assistant. There can be a maximum of 20 files attached to the
-              assistant. Files are ordered by their creation date in ascending order. If a
-              file was previously attached to the list but does not show up in the list, it
-              will be deleted from the assistant.
-
-          instructions: The system instructions that the assistant uses. The maximum length is 32768
-              characters.
-
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
-          model: ID of the model to use. You can use the
-              [List models](https://platform.openai.com/docs/api-reference/models/list) API to
-              see all of your available models, or see our
-              [Model overview](https://platform.openai.com/docs/models/overview) for
-              descriptions of them.
-
-          name: The name of the assistant. The maximum length is 256 characters.
-
-          tools: A list of tool enabled on the assistant. There can be a maximum of 128 tools per
-              assistant. Tools can be of types `code_interpreter`, `retrieval`, or `function`.
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        if not message_id:
+            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return await self._post(
-            f"/assistants/{assistant_id}",
-            body=await async_maybe_transform(
-                {
-                    "description": description,
-                    "file_ids": file_ids,
-                    "instructions": instructions,
-                    "metadata": metadata,
-                    "model": model,
-                    "name": name,
-                    "tools": tools,
-                },
-                assistant_update_params.AssistantUpdateParams,
-            ),
+            f"/threads/{thread_id}/messages/{message_id}",
+            body=await async_maybe_transform({"metadata": metadata}, message_update_params.MessageUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=Message,
         )
 
     def list(
         self,
+        thread_id: str,
         *,
         after: str | NotGiven = NOT_GIVEN,
         before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
+        run_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[Assistant, AsyncCursorPage[Assistant]]:
-        """Returns a list of assistants.
+    ) -> AsyncPaginator[Message, AsyncCursorPage[Message]]:
+        """
+        Returns a list of messages for a given thread.
 
         Args:
-          after: A cursor for use in pagination.
-
-        `after` is an object ID that defines your place
+          after: A cursor for use in pagination. `after` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include after=obj_foo in order to
               fetch the next page of the list.
 
           before: A cursor for use in pagination. `before` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include before=obj_foo in order to
@@ -578,170 +439,113 @@
 
           limit: A limit on the number of objects to be returned. Limit can range between 1 and
               100, and the default is 20.
 
           order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
               order and `desc` for descending order.
 
+          run_id: Filter messages by the run ID that generated them.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._get_api_list(
-            "/assistants",
-            page=AsyncCursorPage[Assistant],
+            f"/threads/{thread_id}/messages",
+            page=AsyncCursorPage[Message],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
                         "before": before,
                         "limit": limit,
                         "order": order,
+                        "run_id": run_id,
                     },
-                    assistant_list_params.AssistantListParams,
+                    message_list_params.MessageListParams,
                 ),
             ),
-            model=Assistant,
+            model=Message,
         )
 
-    async def delete(
-        self,
-        assistant_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantDeleted:
-        """
-        Delete an assistant.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return await self._delete(
-            f"/assistants/{assistant_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=AssistantDeleted,
-        )
 
-
-class AssistantsWithRawResponse:
-    def __init__(self, assistants: Assistants) -> None:
-        self._assistants = assistants
+class MessagesWithRawResponse:
+    def __init__(self, messages: Messages) -> None:
+        self._messages = messages
 
         self.create = _legacy_response.to_raw_response_wrapper(
-            assistants.create,
+            messages.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
-            assistants.retrieve,
+            messages.retrieve,
         )
         self.update = _legacy_response.to_raw_response_wrapper(
-            assistants.update,
+            messages.update,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
-            assistants.list,
-        )
-        self.delete = _legacy_response.to_raw_response_wrapper(
-            assistants.delete,
+            messages.list,
         )
 
-    @cached_property
-    def files(self) -> FilesWithRawResponse:
-        return FilesWithRawResponse(self._assistants.files)
-
 
-class AsyncAssistantsWithRawResponse:
-    def __init__(self, assistants: AsyncAssistants) -> None:
-        self._assistants = assistants
+class AsyncMessagesWithRawResponse:
+    def __init__(self, messages: AsyncMessages) -> None:
+        self._messages = messages
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
-            assistants.create,
+            messages.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
-            assistants.retrieve,
+            messages.retrieve,
         )
         self.update = _legacy_response.async_to_raw_response_wrapper(
-            assistants.update,
+            messages.update,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
-            assistants.list,
+            messages.list,
         )
-        self.delete = _legacy_response.async_to_raw_response_wrapper(
-            assistants.delete,
-        )
-
-    @cached_property
-    def files(self) -> AsyncFilesWithRawResponse:
-        return AsyncFilesWithRawResponse(self._assistants.files)
 
 
-class AssistantsWithStreamingResponse:
-    def __init__(self, assistants: Assistants) -> None:
-        self._assistants = assistants
+class MessagesWithStreamingResponse:
+    def __init__(self, messages: Messages) -> None:
+        self._messages = messages
 
         self.create = to_streamed_response_wrapper(
-            assistants.create,
+            messages.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            assistants.retrieve,
+            messages.retrieve,
         )
         self.update = to_streamed_response_wrapper(
-            assistants.update,
+            messages.update,
         )
         self.list = to_streamed_response_wrapper(
-            assistants.list,
+            messages.list,
         )
-        self.delete = to_streamed_response_wrapper(
-            assistants.delete,
-        )
-
-    @cached_property
-    def files(self) -> FilesWithStreamingResponse:
-        return FilesWithStreamingResponse(self._assistants.files)
 
 
-class AsyncAssistantsWithStreamingResponse:
-    def __init__(self, assistants: AsyncAssistants) -> None:
-        self._assistants = assistants
+class AsyncMessagesWithStreamingResponse:
+    def __init__(self, messages: AsyncMessages) -> None:
+        self._messages = messages
 
         self.create = async_to_streamed_response_wrapper(
-            assistants.create,
+            messages.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            assistants.retrieve,
+            messages.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
-            assistants.update,
+            messages.update,
         )
         self.list = async_to_streamed_response_wrapper(
-            assistants.list,
+            messages.list,
         )
-        self.delete = async_to_streamed_response_wrapper(
-            assistants.delete,
-        )
-
-    @cached_property
-    def files(self) -> AsyncFilesWithStreamingResponse:
-        return AsyncFilesWithStreamingResponse(self._assistants.files)
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/assistants/files.py` & `openai_mealuet-1.23.4/src/openai/resources/batches.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,483 +1,475 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
+from typing import Dict, Optional
 from typing_extensions import Literal
 
 import httpx
 
-from .... import _legacy_response
-from ...._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ...._utils import (
+from .. import _legacy_response
+from ..types import batch_list_params, batch_create_params
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
-from ...._compat import cached_property
-from ...._resource import SyncAPIResource, AsyncAPIResource
-from ...._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
-from ....pagination import SyncCursorPage, AsyncCursorPage
-from ...._base_client import (
+from .._compat import cached_property
+from .._resource import SyncAPIResource, AsyncAPIResource
+from .._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
+from ..pagination import SyncCursorPage, AsyncCursorPage
+from ..types.batch import Batch
+from .._base_client import (
     AsyncPaginator,
     make_request_options,
 )
-from ....types.beta.assistants import AssistantFile, FileDeleteResponse, file_list_params, file_create_params
 
-__all__ = ["Files", "AsyncFiles"]
+__all__ = ["Batches", "AsyncBatches"]
 
 
-class Files(SyncAPIResource):
+class Batches(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> FilesWithRawResponse:
-        return FilesWithRawResponse(self)
+    def with_raw_response(self) -> BatchesWithRawResponse:
+        return BatchesWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> FilesWithStreamingResponse:
-        return FilesWithStreamingResponse(self)
+    def with_streaming_response(self) -> BatchesWithStreamingResponse:
+        return BatchesWithStreamingResponse(self)
 
     def create(
         self,
-        assistant_id: str,
         *,
-        file_id: str,
+        completion_window: Literal["24h"],
+        endpoint: Literal["/v1/chat/completions"],
+        input_file_id: str,
+        metadata: Optional[Dict[str, str]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantFile:
+    ) -> Batch:
         """
-        Create an assistant file by attaching a
-        [File](https://platform.openai.com/docs/api-reference/files) to an
-        [assistant](https://platform.openai.com/docs/api-reference/assistants).
+        Creates and executes a batch from an uploaded file of requests
 
         Args:
-          file_id: A [File](https://platform.openai.com/docs/api-reference/files) ID (with
-              `purpose="assistants"`) that the assistant should use. Useful for tools like
-              `retrieval` and `code_interpreter` that can access files.
+          completion_window: The time frame within which the batch should be processed. Currently only `24h`
+              is supported.
+
+          endpoint: The endpoint to be used for all requests in the batch. Currently only
+              `/v1/chat/completions` is supported.
+
+          input_file_id: The ID of an uploaded file that contains requests for the new batch.
+
+              See [upload file](https://platform.openai.com/docs/api-reference/files/create)
+              for how to upload a file.
+
+              Your input file must be formatted as a
+              [JSONL file](https://platform.openai.com/docs/api-reference/batch/requestInput),
+              and must be uploaded with the purpose `batch`.
+
+          metadata: Optional custom metadata for the batch.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
         return self._post(
-            f"/assistants/{assistant_id}/files",
-            body=maybe_transform({"file_id": file_id}, file_create_params.FileCreateParams),
+            "/batches",
+            body=maybe_transform(
+                {
+                    "completion_window": completion_window,
+                    "endpoint": endpoint,
+                    "input_file_id": input_file_id,
+                    "metadata": metadata,
+                },
+                batch_create_params.BatchCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=AssistantFile,
+            cast_to=Batch,
         )
 
     def retrieve(
         self,
-        file_id: str,
+        batch_id: str,
         *,
-        assistant_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantFile:
+    ) -> Batch:
         """
-        Retrieves an AssistantFile.
+        Retrieves a batch.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        if not file_id:
-            raise ValueError(f"Expected a non-empty value for `file_id` but received {file_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not batch_id:
+            raise ValueError(f"Expected a non-empty value for `batch_id` but received {batch_id!r}")
         return self._get(
-            f"/assistants/{assistant_id}/files/{file_id}",
+            f"/batches/{batch_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=AssistantFile,
+            cast_to=Batch,
         )
 
     def list(
         self,
-        assistant_id: str,
         *,
         after: str | NotGiven = NOT_GIVEN,
-        before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SyncCursorPage[AssistantFile]:
-        """
-        Returns a list of assistant files.
+    ) -> SyncCursorPage[Batch]:
+        """List your organization's batches.
 
         Args:
-          after: A cursor for use in pagination. `after` is an object ID that defines your place
+          after: A cursor for use in pagination.
+
+        `after` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include after=obj_foo in order to
               fetch the next page of the list.
 
-          before: A cursor for use in pagination. `before` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include before=obj_foo in order to
-              fetch the previous page of the list.
-
           limit: A limit on the number of objects to be returned. Limit can range between 1 and
               100, and the default is 20.
 
-          order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
-              order and `desc` for descending order.
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
         return self._get_api_list(
-            f"/assistants/{assistant_id}/files",
-            page=SyncCursorPage[AssistantFile],
+            "/batches",
+            page=SyncCursorPage[Batch],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
-                        "before": before,
                         "limit": limit,
-                        "order": order,
                     },
-                    file_list_params.FileListParams,
+                    batch_list_params.BatchListParams,
                 ),
             ),
-            model=AssistantFile,
+            model=Batch,
         )
 
-    def delete(
+    def cancel(
         self,
-        file_id: str,
+        batch_id: str,
         *,
-        assistant_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> FileDeleteResponse:
+    ) -> Batch:
         """
-        Delete an assistant file.
+        Cancels an in-progress batch.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        if not file_id:
-            raise ValueError(f"Expected a non-empty value for `file_id` but received {file_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._delete(
-            f"/assistants/{assistant_id}/files/{file_id}",
+        if not batch_id:
+            raise ValueError(f"Expected a non-empty value for `batch_id` but received {batch_id!r}")
+        return self._post(
+            f"/batches/{batch_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=FileDeleteResponse,
+            cast_to=Batch,
         )
 
 
-class AsyncFiles(AsyncAPIResource):
+class AsyncBatches(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncFilesWithRawResponse:
-        return AsyncFilesWithRawResponse(self)
+    def with_raw_response(self) -> AsyncBatchesWithRawResponse:
+        return AsyncBatchesWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncFilesWithStreamingResponse:
-        return AsyncFilesWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncBatchesWithStreamingResponse:
+        return AsyncBatchesWithStreamingResponse(self)
 
     async def create(
         self,
-        assistant_id: str,
         *,
-        file_id: str,
+        completion_window: Literal["24h"],
+        endpoint: Literal["/v1/chat/completions"],
+        input_file_id: str,
+        metadata: Optional[Dict[str, str]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantFile:
+    ) -> Batch:
         """
-        Create an assistant file by attaching a
-        [File](https://platform.openai.com/docs/api-reference/files) to an
-        [assistant](https://platform.openai.com/docs/api-reference/assistants).
+        Creates and executes a batch from an uploaded file of requests
 
         Args:
-          file_id: A [File](https://platform.openai.com/docs/api-reference/files) ID (with
-              `purpose="assistants"`) that the assistant should use. Useful for tools like
-              `retrieval` and `code_interpreter` that can access files.
+          completion_window: The time frame within which the batch should be processed. Currently only `24h`
+              is supported.
+
+          endpoint: The endpoint to be used for all requests in the batch. Currently only
+              `/v1/chat/completions` is supported.
+
+          input_file_id: The ID of an uploaded file that contains requests for the new batch.
+
+              See [upload file](https://platform.openai.com/docs/api-reference/files/create)
+              for how to upload a file.
+
+              Your input file must be formatted as a
+              [JSONL file](https://platform.openai.com/docs/api-reference/batch/requestInput),
+              and must be uploaded with the purpose `batch`.
+
+          metadata: Optional custom metadata for the batch.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
         return await self._post(
-            f"/assistants/{assistant_id}/files",
-            body=await async_maybe_transform({"file_id": file_id}, file_create_params.FileCreateParams),
+            "/batches",
+            body=await async_maybe_transform(
+                {
+                    "completion_window": completion_window,
+                    "endpoint": endpoint,
+                    "input_file_id": input_file_id,
+                    "metadata": metadata,
+                },
+                batch_create_params.BatchCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=AssistantFile,
+            cast_to=Batch,
         )
 
     async def retrieve(
         self,
-        file_id: str,
+        batch_id: str,
         *,
-        assistant_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantFile:
+    ) -> Batch:
         """
-        Retrieves an AssistantFile.
+        Retrieves a batch.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        if not file_id:
-            raise ValueError(f"Expected a non-empty value for `file_id` but received {file_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not batch_id:
+            raise ValueError(f"Expected a non-empty value for `batch_id` but received {batch_id!r}")
         return await self._get(
-            f"/assistants/{assistant_id}/files/{file_id}",
+            f"/batches/{batch_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=AssistantFile,
+            cast_to=Batch,
         )
 
     def list(
         self,
-        assistant_id: str,
         *,
         after: str | NotGiven = NOT_GIVEN,
-        before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[AssistantFile, AsyncCursorPage[AssistantFile]]:
-        """
-        Returns a list of assistant files.
+    ) -> AsyncPaginator[Batch, AsyncCursorPage[Batch]]:
+        """List your organization's batches.
 
         Args:
-          after: A cursor for use in pagination. `after` is an object ID that defines your place
+          after: A cursor for use in pagination.
+
+        `after` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include after=obj_foo in order to
               fetch the next page of the list.
 
-          before: A cursor for use in pagination. `before` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include before=obj_foo in order to
-              fetch the previous page of the list.
-
           limit: A limit on the number of objects to be returned. Limit can range between 1 and
               100, and the default is 20.
 
-          order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
-              order and `desc` for descending order.
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
         return self._get_api_list(
-            f"/assistants/{assistant_id}/files",
-            page=AsyncCursorPage[AssistantFile],
+            "/batches",
+            page=AsyncCursorPage[Batch],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
-                        "before": before,
                         "limit": limit,
-                        "order": order,
                     },
-                    file_list_params.FileListParams,
+                    batch_list_params.BatchListParams,
                 ),
             ),
-            model=AssistantFile,
+            model=Batch,
         )
 
-    async def delete(
+    async def cancel(
         self,
-        file_id: str,
+        batch_id: str,
         *,
-        assistant_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> FileDeleteResponse:
+    ) -> Batch:
         """
-        Delete an assistant file.
+        Cancels an in-progress batch.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not assistant_id:
-            raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
-        if not file_id:
-            raise ValueError(f"Expected a non-empty value for `file_id` but received {file_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return await self._delete(
-            f"/assistants/{assistant_id}/files/{file_id}",
+        if not batch_id:
+            raise ValueError(f"Expected a non-empty value for `batch_id` but received {batch_id!r}")
+        return await self._post(
+            f"/batches/{batch_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=FileDeleteResponse,
+            cast_to=Batch,
         )
 
 
-class FilesWithRawResponse:
-    def __init__(self, files: Files) -> None:
-        self._files = files
+class BatchesWithRawResponse:
+    def __init__(self, batches: Batches) -> None:
+        self._batches = batches
 
         self.create = _legacy_response.to_raw_response_wrapper(
-            files.create,
+            batches.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
-            files.retrieve,
+            batches.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
-            files.list,
+            batches.list,
         )
-        self.delete = _legacy_response.to_raw_response_wrapper(
-            files.delete,
+        self.cancel = _legacy_response.to_raw_response_wrapper(
+            batches.cancel,
         )
 
 
-class AsyncFilesWithRawResponse:
-    def __init__(self, files: AsyncFiles) -> None:
-        self._files = files
+class AsyncBatchesWithRawResponse:
+    def __init__(self, batches: AsyncBatches) -> None:
+        self._batches = batches
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
-            files.create,
+            batches.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
-            files.retrieve,
+            batches.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
-            files.list,
+            batches.list,
         )
-        self.delete = _legacy_response.async_to_raw_response_wrapper(
-            files.delete,
+        self.cancel = _legacy_response.async_to_raw_response_wrapper(
+            batches.cancel,
         )
 
 
-class FilesWithStreamingResponse:
-    def __init__(self, files: Files) -> None:
-        self._files = files
+class BatchesWithStreamingResponse:
+    def __init__(self, batches: Batches) -> None:
+        self._batches = batches
 
         self.create = to_streamed_response_wrapper(
-            files.create,
+            batches.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            files.retrieve,
+            batches.retrieve,
         )
         self.list = to_streamed_response_wrapper(
-            files.list,
+            batches.list,
         )
-        self.delete = to_streamed_response_wrapper(
-            files.delete,
+        self.cancel = to_streamed_response_wrapper(
+            batches.cancel,
         )
 
 
-class AsyncFilesWithStreamingResponse:
-    def __init__(self, files: AsyncFiles) -> None:
-        self._files = files
+class AsyncBatchesWithStreamingResponse:
+    def __init__(self, batches: AsyncBatches) -> None:
+        self._batches = batches
 
         self.create = async_to_streamed_response_wrapper(
-            files.create,
+            batches.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            files.retrieve,
+            batches.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
-            files.list,
+            batches.list,
         )
-        self.delete = async_to_streamed_response_wrapper(
-            files.delete,
+        self.cancel = async_to_streamed_response_wrapper(
+            batches.cancel,
         )
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/threads/__init__.py` & `openai_mealuet-1.23.4/src/openai/resources/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/threads/messages/__init__.py` & `openai_mealuet-1.23.4/src/openai/resources/beta/vector_stores/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,30 +4,44 @@
     Files,
     AsyncFiles,
     FilesWithRawResponse,
     AsyncFilesWithRawResponse,
     FilesWithStreamingResponse,
     AsyncFilesWithStreamingResponse,
 )
-from .messages import (
-    Messages,
-    AsyncMessages,
-    MessagesWithRawResponse,
-    AsyncMessagesWithRawResponse,
-    MessagesWithStreamingResponse,
-    AsyncMessagesWithStreamingResponse,
+from .file_batches import (
+    FileBatches,
+    AsyncFileBatches,
+    FileBatchesWithRawResponse,
+    AsyncFileBatchesWithRawResponse,
+    FileBatchesWithStreamingResponse,
+    AsyncFileBatchesWithStreamingResponse,
+)
+from .vector_stores import (
+    VectorStores,
+    AsyncVectorStores,
+    VectorStoresWithRawResponse,
+    AsyncVectorStoresWithRawResponse,
+    VectorStoresWithStreamingResponse,
+    AsyncVectorStoresWithStreamingResponse,
 )
 
 __all__ = [
     "Files",
     "AsyncFiles",
     "FilesWithRawResponse",
     "AsyncFilesWithRawResponse",
     "FilesWithStreamingResponse",
     "AsyncFilesWithStreamingResponse",
-    "Messages",
-    "AsyncMessages",
-    "MessagesWithRawResponse",
-    "AsyncMessagesWithRawResponse",
-    "MessagesWithStreamingResponse",
-    "AsyncMessagesWithStreamingResponse",
+    "FileBatches",
+    "AsyncFileBatches",
+    "FileBatchesWithRawResponse",
+    "AsyncFileBatchesWithRawResponse",
+    "FileBatchesWithStreamingResponse",
+    "AsyncFileBatchesWithStreamingResponse",
+    "VectorStores",
+    "AsyncVectorStores",
+    "VectorStoresWithRawResponse",
+    "AsyncVectorStoresWithRawResponse",
+    "VectorStoresWithStreamingResponse",
+    "AsyncVectorStoresWithStreamingResponse",
 ]
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/threads/messages/files.py` & `openai_mealuet-1.23.4/src/openai/resources/beta/threads/runs/steps.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,90 +13,90 @@
 from ....._resource import SyncAPIResource, AsyncAPIResource
 from ....._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from .....pagination import SyncCursorPage, AsyncCursorPage
 from ....._base_client import (
     AsyncPaginator,
     make_request_options,
 )
-from .....types.beta.threads.messages import MessageFile, file_list_params
+from .....types.beta.threads.runs import step_list_params
+from .....types.beta.threads.runs.run_step import RunStep
 
-__all__ = ["Files", "AsyncFiles"]
+__all__ = ["Steps", "AsyncSteps"]
 
 
-class Files(SyncAPIResource):
+class Steps(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> FilesWithRawResponse:
-        return FilesWithRawResponse(self)
+    def with_raw_response(self) -> StepsWithRawResponse:
+        return StepsWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> FilesWithStreamingResponse:
-        return FilesWithStreamingResponse(self)
+    def with_streaming_response(self) -> StepsWithStreamingResponse:
+        return StepsWithStreamingResponse(self)
 
     def retrieve(
         self,
-        file_id: str,
+        step_id: str,
         *,
         thread_id: str,
-        message_id: str,
+        run_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> MessageFile:
+    ) -> RunStep:
         """
-        Retrieves a message file.
+        Retrieves a run step.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         if not thread_id:
             raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        if not file_id:
-            raise ValueError(f"Expected a non-empty value for `file_id` but received {file_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
+        if not step_id:
+            raise ValueError(f"Expected a non-empty value for `step_id` but received {step_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._get(
-            f"/threads/{thread_id}/messages/{message_id}/files/{file_id}",
+            f"/threads/{thread_id}/runs/{run_id}/steps/{step_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=MessageFile,
+            cast_to=RunStep,
         )
 
     def list(
         self,
-        message_id: str,
+        run_id: str,
         *,
         thread_id: str,
         after: str | NotGiven = NOT_GIVEN,
         before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SyncCursorPage[MessageFile]:
-        """Returns a list of message files.
+    ) -> SyncCursorPage[RunStep]:
+        """
+        Returns a list of run steps belonging to a run.
 
         Args:
-          after: A cursor for use in pagination.
-
-        `after` is an object ID that defines your place
+          after: A cursor for use in pagination. `after` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include after=obj_foo in order to
               fetch the next page of the list.
 
           before: A cursor for use in pagination. `before` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include before=obj_foo in order to
@@ -114,110 +114,109 @@
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         if not thread_id:
             raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._get_api_list(
-            f"/threads/{thread_id}/messages/{message_id}/files",
-            page=SyncCursorPage[MessageFile],
+            f"/threads/{thread_id}/runs/{run_id}/steps",
+            page=SyncCursorPage[RunStep],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
                         "before": before,
                         "limit": limit,
                         "order": order,
                     },
-                    file_list_params.FileListParams,
+                    step_list_params.StepListParams,
                 ),
             ),
-            model=MessageFile,
+            model=RunStep,
         )
 
 
-class AsyncFiles(AsyncAPIResource):
+class AsyncSteps(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncFilesWithRawResponse:
-        return AsyncFilesWithRawResponse(self)
+    def with_raw_response(self) -> AsyncStepsWithRawResponse:
+        return AsyncStepsWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncFilesWithStreamingResponse:
-        return AsyncFilesWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncStepsWithStreamingResponse:
+        return AsyncStepsWithStreamingResponse(self)
 
     async def retrieve(
         self,
-        file_id: str,
+        step_id: str,
         *,
         thread_id: str,
-        message_id: str,
+        run_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> MessageFile:
+    ) -> RunStep:
         """
-        Retrieves a message file.
+        Retrieves a run step.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         if not thread_id:
             raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        if not file_id:
-            raise ValueError(f"Expected a non-empty value for `file_id` but received {file_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
+        if not step_id:
+            raise ValueError(f"Expected a non-empty value for `step_id` but received {step_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return await self._get(
-            f"/threads/{thread_id}/messages/{message_id}/files/{file_id}",
+            f"/threads/{thread_id}/runs/{run_id}/steps/{step_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=MessageFile,
+            cast_to=RunStep,
         )
 
     def list(
         self,
-        message_id: str,
+        run_id: str,
         *,
         thread_id: str,
         after: str | NotGiven = NOT_GIVEN,
         before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[MessageFile, AsyncCursorPage[MessageFile]]:
-        """Returns a list of message files.
+    ) -> AsyncPaginator[RunStep, AsyncCursorPage[RunStep]]:
+        """
+        Returns a list of run steps belonging to a run.
 
         Args:
-          after: A cursor for use in pagination.
-
-        `after` is an object ID that defines your place
+          after: A cursor for use in pagination. `after` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include after=obj_foo in order to
               fetch the next page of the list.
 
           before: A cursor for use in pagination. `before` is an object ID that defines your place
               in the list. For instance, if you make a list request and receive 100 objects,
               ending with obj_foo, your subsequent call can include before=obj_foo in order to
@@ -235,78 +234,78 @@
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         if not thread_id:
             raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._get_api_list(
-            f"/threads/{thread_id}/messages/{message_id}/files",
-            page=AsyncCursorPage[MessageFile],
+            f"/threads/{thread_id}/runs/{run_id}/steps",
+            page=AsyncCursorPage[RunStep],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
                         "before": before,
                         "limit": limit,
                         "order": order,
                     },
-                    file_list_params.FileListParams,
+                    step_list_params.StepListParams,
                 ),
             ),
-            model=MessageFile,
+            model=RunStep,
         )
 
 
-class FilesWithRawResponse:
-    def __init__(self, files: Files) -> None:
-        self._files = files
+class StepsWithRawResponse:
+    def __init__(self, steps: Steps) -> None:
+        self._steps = steps
 
         self.retrieve = _legacy_response.to_raw_response_wrapper(
-            files.retrieve,
+            steps.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
-            files.list,
+            steps.list,
         )
 
 
-class AsyncFilesWithRawResponse:
-    def __init__(self, files: AsyncFiles) -> None:
-        self._files = files
+class AsyncStepsWithRawResponse:
+    def __init__(self, steps: AsyncSteps) -> None:
+        self._steps = steps
 
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
-            files.retrieve,
+            steps.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
-            files.list,
+            steps.list,
         )
 
 
-class FilesWithStreamingResponse:
-    def __init__(self, files: Files) -> None:
-        self._files = files
+class StepsWithStreamingResponse:
+    def __init__(self, steps: Steps) -> None:
+        self._steps = steps
 
         self.retrieve = to_streamed_response_wrapper(
-            files.retrieve,
+            steps.retrieve,
         )
         self.list = to_streamed_response_wrapper(
-            files.list,
+            steps.list,
         )
 
 
-class AsyncFilesWithStreamingResponse:
-    def __init__(self, files: AsyncFiles) -> None:
-        self._files = files
+class AsyncStepsWithStreamingResponse:
+    def __init__(self, steps: AsyncSteps) -> None:
+        self._steps = steps
 
         self.retrieve = async_to_streamed_response_wrapper(
-            files.retrieve,
+            steps.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
-            files.list,
+            steps.list,
         )
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/threads/messages/messages.py` & `openai_mealuet-1.23.4/src/openai/resources/fine_tuning/jobs/jobs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,588 +1,686 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import Union, Iterable, Optional
 from typing_extensions import Literal
 
 import httpx
 
-from ..... import _legacy_response
-from .files import (
-    Files,
-    AsyncFiles,
-    FilesWithRawResponse,
-    AsyncFilesWithRawResponse,
-    FilesWithStreamingResponse,
-    AsyncFilesWithStreamingResponse,
-)
-from ....._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ....._utils import (
+from .... import _legacy_response
+from ...._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ...._utils import (
     maybe_transform,
     async_maybe_transform,
 )
-from ....._compat import cached_property
-from ....._resource import SyncAPIResource, AsyncAPIResource
-from ....._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
-from .....pagination import SyncCursorPage, AsyncCursorPage
-from ....._base_client import (
+from ...._compat import cached_property
+from .checkpoints import (
+    Checkpoints,
+    AsyncCheckpoints,
+    CheckpointsWithRawResponse,
+    AsyncCheckpointsWithRawResponse,
+    CheckpointsWithStreamingResponse,
+    AsyncCheckpointsWithStreamingResponse,
+)
+from ...._resource import SyncAPIResource, AsyncAPIResource
+from ...._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
+from ....pagination import SyncCursorPage, AsyncCursorPage
+from ...._base_client import (
     AsyncPaginator,
     make_request_options,
 )
-from .....types.beta.threads import Message, message_list_params, message_create_params, message_update_params
+from ....types.fine_tuning import job_list_params, job_create_params, job_list_events_params
+from ....types.fine_tuning.fine_tuning_job import FineTuningJob
+from ....types.fine_tuning.fine_tuning_job_event import FineTuningJobEvent
 
-__all__ = ["Messages", "AsyncMessages"]
+__all__ = ["Jobs", "AsyncJobs"]
 
 
-class Messages(SyncAPIResource):
+class Jobs(SyncAPIResource):
     @cached_property
-    def files(self) -> Files:
-        return Files(self._client)
+    def checkpoints(self) -> Checkpoints:
+        return Checkpoints(self._client)
 
     @cached_property
-    def with_raw_response(self) -> MessagesWithRawResponse:
-        return MessagesWithRawResponse(self)
+    def with_raw_response(self) -> JobsWithRawResponse:
+        return JobsWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> MessagesWithStreamingResponse:
-        return MessagesWithStreamingResponse(self)
+    def with_streaming_response(self) -> JobsWithStreamingResponse:
+        return JobsWithStreamingResponse(self)
 
     def create(
         self,
-        thread_id: str,
         *,
-        content: str,
-        role: Literal["user", "assistant"],
-        file_ids: List[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[str, Literal["babbage-002", "davinci-002", "gpt-3.5-turbo"]],
+        training_file: str,
+        hyperparameters: job_create_params.Hyperparameters | NotGiven = NOT_GIVEN,
+        integrations: Optional[Iterable[job_create_params.Integration]] | NotGiven = NOT_GIVEN,
+        seed: Optional[int] | NotGiven = NOT_GIVEN,
+        suffix: Optional[str] | NotGiven = NOT_GIVEN,
+        validation_file: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> FineTuningJob:
         """
-        Create a message.
+        Creates a fine-tuning job which begins the process of creating a new model from
+        a given dataset.
+
+        Response includes details of the enqueued job including job status and the name
+        of the fine-tuned models once complete.
+
+        [Learn more about fine-tuning](https://platform.openai.com/docs/guides/fine-tuning)
 
         Args:
-          content: The content of the message.
+          model: The name of the model to fine-tune. You can select one of the
+              [supported models](https://platform.openai.com/docs/guides/fine-tuning/what-models-can-be-fine-tuned).
+
+          training_file: The ID of an uploaded file that contains training data.
+
+              See [upload file](https://platform.openai.com/docs/api-reference/files/create)
+              for how to upload a file.
+
+              Your dataset must be formatted as a JSONL file. Additionally, you must upload
+              your file with the purpose `fine-tune`.
+
+              See the [fine-tuning guide](https://platform.openai.com/docs/guides/fine-tuning)
+              for more details.
 
-          role:
-              The role of the entity that is creating the message. Allowed values include:
+          hyperparameters: The hyperparameters used for the fine-tuning job.
 
-              - `user`: Indicates the message is sent by an actual user and should be used in
-                most cases to represent user-generated messages.
-              - `assistant`: Indicates the message is generated by the assistant. Use this
-                value to insert messages from the assistant into the conversation.
-
-          file_ids: A list of [File](https://platform.openai.com/docs/api-reference/files) IDs that
-              the message should use. There can be a maximum of 10 files attached to a
-              message. Useful for tools like `retrieval` and `code_interpreter` that can
-              access and use files.
-
-          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
-              for storing additional information about the object in a structured format. Keys
-              can be a maximum of 64 characters long and values can be a maxium of 512
-              characters long.
+          integrations: A list of integrations to enable for your fine-tuning job.
+
+          seed: The seed controls the reproducibility of the job. Passing in the same seed and
+              job parameters should produce the same results, but may differ in rare cases. If
+              a seed is not specified, one will be generated for you.
+
+          suffix: A string of up to 18 characters that will be added to your fine-tuned model
+              name.
+
+              For example, a `suffix` of "custom-model-name" would produce a model name like
+              `ft:gpt-3.5-turbo:openai:custom-model-name:7p4lURel`.
+
+          validation_file: The ID of an uploaded file that contains validation data.
+
+              If you provide this file, the data is used to generate validation metrics
+              periodically during fine-tuning. These metrics can be viewed in the fine-tuning
+              results file. The same data should not be present in both train and validation
+              files.
+
+              Your dataset must be formatted as a JSONL file. You must upload your file with
+              the purpose `fine-tune`.
+
+              See the [fine-tuning guide](https://platform.openai.com/docs/guides/fine-tuning)
+              for more details.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
         return self._post(
-            f"/threads/{thread_id}/messages",
+            "/fine_tuning/jobs",
             body=maybe_transform(
                 {
-                    "content": content,
-                    "role": role,
-                    "file_ids": file_ids,
-                    "metadata": metadata,
+                    "model": model,
+                    "training_file": training_file,
+                    "hyperparameters": hyperparameters,
+                    "integrations": integrations,
+                    "seed": seed,
+                    "suffix": suffix,
+                    "validation_file": validation_file,
                 },
-                message_create_params.MessageCreateParams,
+                job_create_params.JobCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=FineTuningJob,
         )
 
     def retrieve(
         self,
-        message_id: str,
+        fine_tuning_job_id: str,
         *,
-        thread_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> FineTuningJob:
         """
-        Retrieve a message.
+        Get info about a fine-tuning job.
+
+        [Learn more about fine-tuning](https://platform.openai.com/docs/guides/fine-tuning)
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not fine_tuning_job_id:
+            raise ValueError(f"Expected a non-empty value for `fine_tuning_job_id` but received {fine_tuning_job_id!r}")
         return self._get(
-            f"/threads/{thread_id}/messages/{message_id}",
+            f"/fine_tuning/jobs/{fine_tuning_job_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=FineTuningJob,
         )
 
-    def update(
+    def list(
         self,
-        message_id: str,
         *,
-        thread_id: str,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        after: str | NotGiven = NOT_GIVEN,
+        limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> SyncCursorPage[FineTuningJob]:
         """
-        Modifies a message.
+        List your organization's fine-tuning jobs
 
         Args:
-          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
-              for storing additional information about the object in a structured format. Keys
-              can be a maximum of 64 characters long and values can be a maxium of 512
-              characters long.
+          after: Identifier for the last job from the previous pagination request.
+
+          limit: Number of fine-tuning jobs to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return self._get_api_list(
+            "/fine_tuning/jobs",
+            page=SyncCursorPage[FineTuningJob],
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                query=maybe_transform(
+                    {
+                        "after": after,
+                        "limit": limit,
+                    },
+                    job_list_params.JobListParams,
+                ),
+            ),
+            model=FineTuningJob,
+        )
 
+    def cancel(
+        self,
+        fine_tuning_job_id: str,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> FineTuningJob:
+        """
+        Immediately cancel a fine-tune job.
+
+        Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not fine_tuning_job_id:
+            raise ValueError(f"Expected a non-empty value for `fine_tuning_job_id` but received {fine_tuning_job_id!r}")
         return self._post(
-            f"/threads/{thread_id}/messages/{message_id}",
-            body=maybe_transform({"metadata": metadata}, message_update_params.MessageUpdateParams),
+            f"/fine_tuning/jobs/{fine_tuning_job_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=FineTuningJob,
         )
 
-    def list(
+    def list_events(
         self,
-        thread_id: str,
+        fine_tuning_job_id: str,
         *,
         after: str | NotGiven = NOT_GIVEN,
-        before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
-        run_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SyncCursorPage[Message]:
+    ) -> SyncCursorPage[FineTuningJobEvent]:
         """
-        Returns a list of messages for a given thread.
+        Get status updates for a fine-tuning job.
 
         Args:
-          after: A cursor for use in pagination. `after` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include after=obj_foo in order to
-              fetch the next page of the list.
-
-          before: A cursor for use in pagination. `before` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include before=obj_foo in order to
-              fetch the previous page of the list.
+          after: Identifier for the last event from the previous pagination request.
 
-          limit: A limit on the number of objects to be returned. Limit can range between 1 and
-              100, and the default is 20.
-
-          order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
-              order and `desc` for descending order.
-
-          run_id: Filter messages by the run ID that generated them.
+          limit: Number of events to retrieve.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not fine_tuning_job_id:
+            raise ValueError(f"Expected a non-empty value for `fine_tuning_job_id` but received {fine_tuning_job_id!r}")
         return self._get_api_list(
-            f"/threads/{thread_id}/messages",
-            page=SyncCursorPage[Message],
+            f"/fine_tuning/jobs/{fine_tuning_job_id}/events",
+            page=SyncCursorPage[FineTuningJobEvent],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
-                        "before": before,
                         "limit": limit,
-                        "order": order,
-                        "run_id": run_id,
                     },
-                    message_list_params.MessageListParams,
+                    job_list_events_params.JobListEventsParams,
                 ),
             ),
-            model=Message,
+            model=FineTuningJobEvent,
         )
 
 
-class AsyncMessages(AsyncAPIResource):
+class AsyncJobs(AsyncAPIResource):
     @cached_property
-    def files(self) -> AsyncFiles:
-        return AsyncFiles(self._client)
+    def checkpoints(self) -> AsyncCheckpoints:
+        return AsyncCheckpoints(self._client)
 
     @cached_property
-    def with_raw_response(self) -> AsyncMessagesWithRawResponse:
-        return AsyncMessagesWithRawResponse(self)
+    def with_raw_response(self) -> AsyncJobsWithRawResponse:
+        return AsyncJobsWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncMessagesWithStreamingResponse:
-        return AsyncMessagesWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncJobsWithStreamingResponse:
+        return AsyncJobsWithStreamingResponse(self)
 
     async def create(
         self,
-        thread_id: str,
         *,
-        content: str,
-        role: Literal["user", "assistant"],
-        file_ids: List[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[str, Literal["babbage-002", "davinci-002", "gpt-3.5-turbo"]],
+        training_file: str,
+        hyperparameters: job_create_params.Hyperparameters | NotGiven = NOT_GIVEN,
+        integrations: Optional[Iterable[job_create_params.Integration]] | NotGiven = NOT_GIVEN,
+        seed: Optional[int] | NotGiven = NOT_GIVEN,
+        suffix: Optional[str] | NotGiven = NOT_GIVEN,
+        validation_file: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> FineTuningJob:
         """
-        Create a message.
+        Creates a fine-tuning job which begins the process of creating a new model from
+        a given dataset.
+
+        Response includes details of the enqueued job including job status and the name
+        of the fine-tuned models once complete.
+
+        [Learn more about fine-tuning](https://platform.openai.com/docs/guides/fine-tuning)
 
         Args:
-          content: The content of the message.
+          model: The name of the model to fine-tune. You can select one of the
+              [supported models](https://platform.openai.com/docs/guides/fine-tuning/what-models-can-be-fine-tuned).
+
+          training_file: The ID of an uploaded file that contains training data.
+
+              See [upload file](https://platform.openai.com/docs/api-reference/files/create)
+              for how to upload a file.
+
+              Your dataset must be formatted as a JSONL file. Additionally, you must upload
+              your file with the purpose `fine-tune`.
 
-          role:
-              The role of the entity that is creating the message. Allowed values include:
+              See the [fine-tuning guide](https://platform.openai.com/docs/guides/fine-tuning)
+              for more details.
 
-              - `user`: Indicates the message is sent by an actual user and should be used in
-                most cases to represent user-generated messages.
-              - `assistant`: Indicates the message is generated by the assistant. Use this
-                value to insert messages from the assistant into the conversation.
-
-          file_ids: A list of [File](https://platform.openai.com/docs/api-reference/files) IDs that
-              the message should use. There can be a maximum of 10 files attached to a
-              message. Useful for tools like `retrieval` and `code_interpreter` that can
-              access and use files.
-
-          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
-              for storing additional information about the object in a structured format. Keys
-              can be a maximum of 64 characters long and values can be a maxium of 512
-              characters long.
+          hyperparameters: The hyperparameters used for the fine-tuning job.
+
+          integrations: A list of integrations to enable for your fine-tuning job.
+
+          seed: The seed controls the reproducibility of the job. Passing in the same seed and
+              job parameters should produce the same results, but may differ in rare cases. If
+              a seed is not specified, one will be generated for you.
+
+          suffix: A string of up to 18 characters that will be added to your fine-tuned model
+              name.
+
+              For example, a `suffix` of "custom-model-name" would produce a model name like
+              `ft:gpt-3.5-turbo:openai:custom-model-name:7p4lURel`.
+
+          validation_file: The ID of an uploaded file that contains validation data.
+
+              If you provide this file, the data is used to generate validation metrics
+              periodically during fine-tuning. These metrics can be viewed in the fine-tuning
+              results file. The same data should not be present in both train and validation
+              files.
+
+              Your dataset must be formatted as a JSONL file. You must upload your file with
+              the purpose `fine-tune`.
+
+              See the [fine-tuning guide](https://platform.openai.com/docs/guides/fine-tuning)
+              for more details.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
         return await self._post(
-            f"/threads/{thread_id}/messages",
+            "/fine_tuning/jobs",
             body=await async_maybe_transform(
                 {
-                    "content": content,
-                    "role": role,
-                    "file_ids": file_ids,
-                    "metadata": metadata,
+                    "model": model,
+                    "training_file": training_file,
+                    "hyperparameters": hyperparameters,
+                    "integrations": integrations,
+                    "seed": seed,
+                    "suffix": suffix,
+                    "validation_file": validation_file,
                 },
-                message_create_params.MessageCreateParams,
+                job_create_params.JobCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=FineTuningJob,
         )
 
     async def retrieve(
         self,
-        message_id: str,
+        fine_tuning_job_id: str,
         *,
-        thread_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> FineTuningJob:
         """
-        Retrieve a message.
+        Get info about a fine-tuning job.
+
+        [Learn more about fine-tuning](https://platform.openai.com/docs/guides/fine-tuning)
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not fine_tuning_job_id:
+            raise ValueError(f"Expected a non-empty value for `fine_tuning_job_id` but received {fine_tuning_job_id!r}")
         return await self._get(
-            f"/threads/{thread_id}/messages/{message_id}",
+            f"/fine_tuning/jobs/{fine_tuning_job_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=FineTuningJob,
         )
 
-    async def update(
+    def list(
         self,
-        message_id: str,
         *,
-        thread_id: str,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        after: str | NotGiven = NOT_GIVEN,
+        limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> AsyncPaginator[FineTuningJob, AsyncCursorPage[FineTuningJob]]:
         """
-        Modifies a message.
+        List your organization's fine-tuning jobs
 
         Args:
-          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
-              for storing additional information about the object in a structured format. Keys
-              can be a maximum of 64 characters long and values can be a maxium of 512
-              characters long.
+          after: Identifier for the last job from the previous pagination request.
+
+          limit: Number of fine-tuning jobs to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return self._get_api_list(
+            "/fine_tuning/jobs",
+            page=AsyncCursorPage[FineTuningJob],
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                query=maybe_transform(
+                    {
+                        "after": after,
+                        "limit": limit,
+                    },
+                    job_list_params.JobListParams,
+                ),
+            ),
+            model=FineTuningJob,
+        )
+
+    async def cancel(
+        self,
+        fine_tuning_job_id: str,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> FineTuningJob:
+        """
+        Immediately cancel a fine-tune job.
 
+        Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not message_id:
-            raise ValueError(f"Expected a non-empty value for `message_id` but received {message_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not fine_tuning_job_id:
+            raise ValueError(f"Expected a non-empty value for `fine_tuning_job_id` but received {fine_tuning_job_id!r}")
         return await self._post(
-            f"/threads/{thread_id}/messages/{message_id}",
-            body=await async_maybe_transform({"metadata": metadata}, message_update_params.MessageUpdateParams),
+            f"/fine_tuning/jobs/{fine_tuning_job_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=FineTuningJob,
         )
 
-    def list(
+    def list_events(
         self,
-        thread_id: str,
+        fine_tuning_job_id: str,
         *,
         after: str | NotGiven = NOT_GIVEN,
-        before: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
-        run_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[Message, AsyncCursorPage[Message]]:
+    ) -> AsyncPaginator[FineTuningJobEvent, AsyncCursorPage[FineTuningJobEvent]]:
         """
-        Returns a list of messages for a given thread.
+        Get status updates for a fine-tuning job.
 
         Args:
-          after: A cursor for use in pagination. `after` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include after=obj_foo in order to
-              fetch the next page of the list.
-
-          before: A cursor for use in pagination. `before` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include before=obj_foo in order to
-              fetch the previous page of the list.
-
-          limit: A limit on the number of objects to be returned. Limit can range between 1 and
-              100, and the default is 20.
+          after: Identifier for the last event from the previous pagination request.
 
-          order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
-              order and `desc` for descending order.
-
-          run_id: Filter messages by the run ID that generated them.
+          limit: Number of events to retrieve.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        if not fine_tuning_job_id:
+            raise ValueError(f"Expected a non-empty value for `fine_tuning_job_id` but received {fine_tuning_job_id!r}")
         return self._get_api_list(
-            f"/threads/{thread_id}/messages",
-            page=AsyncCursorPage[Message],
+            f"/fine_tuning/jobs/{fine_tuning_job_id}/events",
+            page=AsyncCursorPage[FineTuningJobEvent],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "after": after,
-                        "before": before,
                         "limit": limit,
-                        "order": order,
-                        "run_id": run_id,
                     },
-                    message_list_params.MessageListParams,
+                    job_list_events_params.JobListEventsParams,
                 ),
             ),
-            model=Message,
+            model=FineTuningJobEvent,
         )
 
 
-class MessagesWithRawResponse:
-    def __init__(self, messages: Messages) -> None:
-        self._messages = messages
+class JobsWithRawResponse:
+    def __init__(self, jobs: Jobs) -> None:
+        self._jobs = jobs
 
         self.create = _legacy_response.to_raw_response_wrapper(
-            messages.create,
+            jobs.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
-            messages.retrieve,
-        )
-        self.update = _legacy_response.to_raw_response_wrapper(
-            messages.update,
+            jobs.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
-            messages.list,
+            jobs.list,
+        )
+        self.cancel = _legacy_response.to_raw_response_wrapper(
+            jobs.cancel,
+        )
+        self.list_events = _legacy_response.to_raw_response_wrapper(
+            jobs.list_events,
         )
 
     @cached_property
-    def files(self) -> FilesWithRawResponse:
-        return FilesWithRawResponse(self._messages.files)
+    def checkpoints(self) -> CheckpointsWithRawResponse:
+        return CheckpointsWithRawResponse(self._jobs.checkpoints)
 
 
-class AsyncMessagesWithRawResponse:
-    def __init__(self, messages: AsyncMessages) -> None:
-        self._messages = messages
+class AsyncJobsWithRawResponse:
+    def __init__(self, jobs: AsyncJobs) -> None:
+        self._jobs = jobs
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
-            messages.create,
+            jobs.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
-            messages.retrieve,
-        )
-        self.update = _legacy_response.async_to_raw_response_wrapper(
-            messages.update,
+            jobs.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
-            messages.list,
+            jobs.list,
+        )
+        self.cancel = _legacy_response.async_to_raw_response_wrapper(
+            jobs.cancel,
+        )
+        self.list_events = _legacy_response.async_to_raw_response_wrapper(
+            jobs.list_events,
         )
 
     @cached_property
-    def files(self) -> AsyncFilesWithRawResponse:
-        return AsyncFilesWithRawResponse(self._messages.files)
+    def checkpoints(self) -> AsyncCheckpointsWithRawResponse:
+        return AsyncCheckpointsWithRawResponse(self._jobs.checkpoints)
 
 
-class MessagesWithStreamingResponse:
-    def __init__(self, messages: Messages) -> None:
-        self._messages = messages
+class JobsWithStreamingResponse:
+    def __init__(self, jobs: Jobs) -> None:
+        self._jobs = jobs
 
         self.create = to_streamed_response_wrapper(
-            messages.create,
+            jobs.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            messages.retrieve,
-        )
-        self.update = to_streamed_response_wrapper(
-            messages.update,
+            jobs.retrieve,
         )
         self.list = to_streamed_response_wrapper(
-            messages.list,
+            jobs.list,
+        )
+        self.cancel = to_streamed_response_wrapper(
+            jobs.cancel,
+        )
+        self.list_events = to_streamed_response_wrapper(
+            jobs.list_events,
         )
 
     @cached_property
-    def files(self) -> FilesWithStreamingResponse:
-        return FilesWithStreamingResponse(self._messages.files)
+    def checkpoints(self) -> CheckpointsWithStreamingResponse:
+        return CheckpointsWithStreamingResponse(self._jobs.checkpoints)
 
 
-class AsyncMessagesWithStreamingResponse:
-    def __init__(self, messages: AsyncMessages) -> None:
-        self._messages = messages
+class AsyncJobsWithStreamingResponse:
+    def __init__(self, jobs: AsyncJobs) -> None:
+        self._jobs = jobs
 
         self.create = async_to_streamed_response_wrapper(
-            messages.create,
+            jobs.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            messages.retrieve,
-        )
-        self.update = async_to_streamed_response_wrapper(
-            messages.update,
+            jobs.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
-            messages.list,
+            jobs.list,
+        )
+        self.cancel = async_to_streamed_response_wrapper(
+            jobs.cancel,
+        )
+        self.list_events = async_to_streamed_response_wrapper(
+            jobs.list_events,
         )
 
     @cached_property
-    def files(self) -> AsyncFilesWithStreamingResponse:
-        return AsyncFilesWithStreamingResponse(self._messages.files)
+    def checkpoints(self) -> AsyncCheckpointsWithStreamingResponse:
+        return AsyncCheckpointsWithStreamingResponse(self._jobs.checkpoints)
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/beta/threads/runs/runs.py` & `openai_mealuet-1.23.4/src/openai/resources/beta/threads/threads.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,2223 +1,2124 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-import time
-import typing_extensions
-from typing import Iterable, Optional, overload
+from typing import Union, Iterable, Optional, overload
 from functools import partial
 from typing_extensions import Literal
 
 import httpx
 
-from ..... import _legacy_response
-from .steps import (
-    Steps,
-    AsyncSteps,
-    StepsWithRawResponse,
-    AsyncStepsWithRawResponse,
-    StepsWithStreamingResponse,
-    AsyncStepsWithStreamingResponse,
+from .... import _legacy_response
+from .runs import (
+    Runs,
+    AsyncRuns,
+    RunsWithRawResponse,
+    AsyncRunsWithRawResponse,
+    RunsWithStreamingResponse,
+    AsyncRunsWithStreamingResponse,
 )
-from ....._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ....._utils import (
-    is_given,
+from .messages import (
+    Messages,
+    AsyncMessages,
+    MessagesWithRawResponse,
+    AsyncMessagesWithRawResponse,
+    MessagesWithStreamingResponse,
+    AsyncMessagesWithStreamingResponse,
+)
+from ...._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ...._utils import (
     required_args,
     maybe_transform,
     async_maybe_transform,
 )
-from ....._compat import cached_property
-from ....._resource import SyncAPIResource, AsyncAPIResource
-from ....._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
-from ....._streaming import Stream, AsyncStream
-from .....pagination import SyncCursorPage, AsyncCursorPage
-from .....types.beta import AssistantToolParam, AssistantStreamEvent
-from ....._base_client import (
-    AsyncPaginator,
+from .runs.runs import Runs, AsyncRuns
+from ...._compat import cached_property
+from ...._resource import SyncAPIResource, AsyncAPIResource
+from ...._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
+from ...._streaming import Stream, AsyncStream
+from ....types.beta import (
+    thread_create_params,
+    thread_update_params,
+    thread_create_and_run_params,
+)
+from ...._base_client import (
     make_request_options,
 )
-from .....lib.streaming import (
+from ....lib.streaming import (
     AssistantEventHandler,
     AssistantEventHandlerT,
     AssistantStreamManager,
     AsyncAssistantEventHandler,
     AsyncAssistantEventHandlerT,
     AsyncAssistantStreamManager,
 )
-from .....types.beta.threads import (
-    Run,
-    run_list_params,
-    run_create_params,
-    run_update_params,
-    run_submit_tool_outputs_params,
-)
+from ....types.beta.thread import Thread
+from ....types.beta.threads.run import Run
+from ....types.beta.thread_deleted import ThreadDeleted
+from ....types.beta.assistant_stream_event import AssistantStreamEvent
+from ....types.beta.assistant_tool_choice_option_param import AssistantToolChoiceOptionParam
+from ....types.beta.assistant_response_format_option_param import AssistantResponseFormatOptionParam
 
-__all__ = ["Runs", "AsyncRuns"]
+__all__ = ["Threads", "AsyncThreads"]
 
 
-class Runs(SyncAPIResource):
+class Threads(SyncAPIResource):
     @cached_property
-    def steps(self) -> Steps:
-        return Steps(self._client)
+    def runs(self) -> Runs:
+        return Runs(self._client)
 
     @cached_property
-    def with_raw_response(self) -> RunsWithRawResponse:
-        return RunsWithRawResponse(self)
+    def messages(self) -> Messages:
+        return Messages(self._client)
 
     @cached_property
-    def with_streaming_response(self) -> RunsWithStreamingResponse:
-        return RunsWithStreamingResponse(self)
+    def with_raw_response(self) -> ThreadsWithRawResponse:
+        return ThreadsWithRawResponse(self)
+
+    @cached_property
+    def with_streaming_response(self) -> ThreadsWithStreamingResponse:
+        return ThreadsWithStreamingResponse(self)
 
-    @overload
     def create(
         self,
+        *,
+        messages: Iterable[thread_create_params.Message] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_params.ToolResources] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> Thread:
+        """
+        Create a thread.
+
+        Args:
+          messages: A list of [messages](https://platform.openai.com/docs/api-reference/messages) to
+              start the thread with.
+
+          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
+              for storing additional information about the object in a structured format. Keys
+              can be a maximum of 64 characters long and values can be a maxium of 512
+              characters long.
+
+          tool_resources: A set of resources that are made available to the assistant's tools in this
+              thread. The resources are specific to the type of tool. For example, the
+              `code_interpreter` tool requires a list of file IDs, while the `file_search`
+              tool requires a list of vector store IDs.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return self._post(
+            "/threads",
+            body=maybe_transform(
+                {
+                    "messages": messages,
+                    "metadata": metadata,
+                    "tool_resources": tool_resources,
+                },
+                thread_create_params.ThreadCreateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Thread,
+        )
+
+    def retrieve(
+        self,
         thread_id: str,
         *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> Thread:
+        """
+        Retrieves a thread.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return self._get(
+            f"/threads/{thread_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Thread,
+        )
+
+    def update(
+        self,
+        thread_id: str,
+        *,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_update_params.ToolResources] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> Thread:
+        """
+        Modifies a thread.
+
+        Args:
+          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
+              for storing additional information about the object in a structured format. Keys
+              can be a maximum of 64 characters long and values can be a maxium of 512
+              characters long.
+
+          tool_resources: A set of resources that are made available to the assistant's tools in this
+              thread. The resources are specific to the type of tool. For example, the
+              `code_interpreter` tool requires a list of file IDs, while the `file_search`
+              tool requires a list of vector store IDs.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return self._post(
+            f"/threads/{thread_id}",
+            body=maybe_transform(
+                {
+                    "metadata": metadata,
+                    "tool_resources": tool_resources,
+                },
+                thread_update_params.ThreadUpdateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Thread,
+        )
+
+    def delete(
+        self,
+        thread_id: str,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> ThreadDeleted:
+        """
+        Delete a thread.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return self._delete(
+            f"/threads/{thread_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=ThreadDeleted,
+        )
+
+    @overload
+    def create_and_run(
+        self,
+        *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run:
         """
-        Create a run.
+        Create a thread and run it in one request.
 
         Args:
           assistant_id: The ID of the
               [assistant](https://platform.openai.com/docs/api-reference/assistants) to use to
               execute this run.
 
-          additional_instructions: Appends additional instructions at the end of the instructions for the run. This
-              is useful for modifying the behavior on a per-run basis without overriding other
-              instructions.
-
-          instructions: Overrides the
-              [instructions](https://platform.openai.com/docs/api-reference/assistants/createAssistant)
-              of the assistant. This is useful for modifying the behavior on a per-run basis.
+          instructions: Override the default system message of the assistant. This is useful for
+              modifying the behavior on a per-run basis.
+
+          max_completion_tokens: The maximum number of completion tokens that may be used over the course of the
+              run. The run will make a best effort to use only the number of completion tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              completion tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
+
+          max_prompt_tokens: The maximum number of prompt tokens that may be used over the course of the run.
+              The run will make a best effort to use only the number of prompt tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              prompt tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
           model: The ID of the [Model](https://platform.openai.com/docs/api-reference/models) to
               be used to execute this run. If a value is provided here, it will override the
               model associated with the assistant. If not, the model associated with the
               assistant will be used.
 
+          response_format: Specifies the format that the model must output. Compatible with
+              [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
+              all GPT-3.5 Turbo models since `gpt-3.5-turbo-1106`.
+
+              Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
+              message the model generates is valid JSON.
+
+              **Important:** when using JSON mode, you **must** also instruct the model to
+              produce JSON yourself via a system or user message. Without this, the model may
+              generate an unending stream of whitespace until the generation reaches the token
+              limit, resulting in a long-running and seemingly "stuck" request. Also note that
+              the message content may be partially cut off if `finish_reason="length"`, which
+              indicates the generation exceeded `max_tokens` or the conversation exceeded the
+              max context length.
+
           stream: If `true`, returns a stream of events that happen during the Run as server-sent
               events, terminating when the Run enters a terminal state with a `data: [DONE]`
               message.
 
           temperature: What sampling temperature to use, between 0 and 2. Higher values like 0.8 will
               make the output more random, while lower values like 0.2 will make it more
               focused and deterministic.
 
+          thread: If no thread is provided, an empty thread will be created.
+
+          tool_choice: Controls which (if any) tool is called by the model. `none` means the model will
+              not call any tools and instead generates a message. `auto` is the default value
+              and means the model can pick between generating a message or calling a tool.
+              Specifying a particular tool like `{"type": "file_search"}` or
+              `{"type": "function", "function": {"name": "my_function"}}` forces the model to
+              call that tool.
+
+          tool_resources: A set of resources that are used by the assistant's tools. The resources are
+              specific to the type of tool. For example, the `code_interpreter` tool requires
+              a list of file IDs, while the `file_search` tool requires a list of vector store
+              IDs.
+
           tools: Override the tools the assistant can use for this run. This is useful for
               modifying the behavior on a per-run basis.
 
+          top_p: An alternative to sampling with temperature, called nucleus sampling, where the
+              model considers the results of the tokens with top_p probability mass. So 0.1
+              means only the tokens comprising the top 10% probability mass are considered.
+
+              We generally recommend altering this or temperature but not both.
+
+          truncation_strategy: Controls for how a thread will be truncated prior to the run. Use this to
+              control the intial context window of the run.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    def create(
+    def create_and_run(
         self,
-        thread_id: str,
         *,
         assistant_id: str,
         stream: Literal[True],
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Stream[AssistantStreamEvent]:
         """
-        Create a run.
+        Create a thread and run it in one request.
 
         Args:
           assistant_id: The ID of the
               [assistant](https://platform.openai.com/docs/api-reference/assistants) to use to
               execute this run.
 
           stream: If `true`, returns a stream of events that happen during the Run as server-sent
               events, terminating when the Run enters a terminal state with a `data: [DONE]`
               message.
 
-          additional_instructions: Appends additional instructions at the end of the instructions for the run. This
-              is useful for modifying the behavior on a per-run basis without overriding other
-              instructions.
-
-          instructions: Overrides the
-              [instructions](https://platform.openai.com/docs/api-reference/assistants/createAssistant)
-              of the assistant. This is useful for modifying the behavior on a per-run basis.
+          instructions: Override the default system message of the assistant. This is useful for
+              modifying the behavior on a per-run basis.
+
+          max_completion_tokens: The maximum number of completion tokens that may be used over the course of the
+              run. The run will make a best effort to use only the number of completion tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              completion tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
+
+          max_prompt_tokens: The maximum number of prompt tokens that may be used over the course of the run.
+              The run will make a best effort to use only the number of prompt tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              prompt tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
           model: The ID of the [Model](https://platform.openai.com/docs/api-reference/models) to
               be used to execute this run. If a value is provided here, it will override the
               model associated with the assistant. If not, the model associated with the
               assistant will be used.
 
+          response_format: Specifies the format that the model must output. Compatible with
+              [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
+              all GPT-3.5 Turbo models since `gpt-3.5-turbo-1106`.
+
+              Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
+              message the model generates is valid JSON.
+
+              **Important:** when using JSON mode, you **must** also instruct the model to
+              produce JSON yourself via a system or user message. Without this, the model may
+              generate an unending stream of whitespace until the generation reaches the token
+              limit, resulting in a long-running and seemingly "stuck" request. Also note that
+              the message content may be partially cut off if `finish_reason="length"`, which
+              indicates the generation exceeded `max_tokens` or the conversation exceeded the
+              max context length.
+
           temperature: What sampling temperature to use, between 0 and 2. Higher values like 0.8 will
               make the output more random, while lower values like 0.2 will make it more
               focused and deterministic.
 
+          thread: If no thread is provided, an empty thread will be created.
+
+          tool_choice: Controls which (if any) tool is called by the model. `none` means the model will
+              not call any tools and instead generates a message. `auto` is the default value
+              and means the model can pick between generating a message or calling a tool.
+              Specifying a particular tool like `{"type": "file_search"}` or
+              `{"type": "function", "function": {"name": "my_function"}}` forces the model to
+              call that tool.
+
+          tool_resources: A set of resources that are used by the assistant's tools. The resources are
+              specific to the type of tool. For example, the `code_interpreter` tool requires
+              a list of file IDs, while the `file_search` tool requires a list of vector store
+              IDs.
+
           tools: Override the tools the assistant can use for this run. This is useful for
               modifying the behavior on a per-run basis.
 
+          top_p: An alternative to sampling with temperature, called nucleus sampling, where the
+              model considers the results of the tokens with top_p probability mass. So 0.1
+              means only the tokens comprising the top 10% probability mass are considered.
+
+              We generally recommend altering this or temperature but not both.
+
+          truncation_strategy: Controls for how a thread will be truncated prior to the run. Use this to
+              control the intial context window of the run.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    def create(
+    def create_and_run(
         self,
-        thread_id: str,
         *,
         assistant_id: str,
         stream: bool,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run | Stream[AssistantStreamEvent]:
         """
-        Create a run.
+        Create a thread and run it in one request.
 
         Args:
           assistant_id: The ID of the
               [assistant](https://platform.openai.com/docs/api-reference/assistants) to use to
               execute this run.
 
           stream: If `true`, returns a stream of events that happen during the Run as server-sent
               events, terminating when the Run enters a terminal state with a `data: [DONE]`
               message.
 
-          additional_instructions: Appends additional instructions at the end of the instructions for the run. This
-              is useful for modifying the behavior on a per-run basis without overriding other
-              instructions.
-
-          instructions: Overrides the
-              [instructions](https://platform.openai.com/docs/api-reference/assistants/createAssistant)
-              of the assistant. This is useful for modifying the behavior on a per-run basis.
+          instructions: Override the default system message of the assistant. This is useful for
+              modifying the behavior on a per-run basis.
+
+          max_completion_tokens: The maximum number of completion tokens that may be used over the course of the
+              run. The run will make a best effort to use only the number of completion tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              completion tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
+
+          max_prompt_tokens: The maximum number of prompt tokens that may be used over the course of the run.
+              The run will make a best effort to use only the number of prompt tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              prompt tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
           model: The ID of the [Model](https://platform.openai.com/docs/api-reference/models) to
               be used to execute this run. If a value is provided here, it will override the
               model associated with the assistant. If not, the model associated with the
               assistant will be used.
 
+          response_format: Specifies the format that the model must output. Compatible with
+              [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
+              all GPT-3.5 Turbo models since `gpt-3.5-turbo-1106`.
+
+              Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
+              message the model generates is valid JSON.
+
+              **Important:** when using JSON mode, you **must** also instruct the model to
+              produce JSON yourself via a system or user message. Without this, the model may
+              generate an unending stream of whitespace until the generation reaches the token
+              limit, resulting in a long-running and seemingly "stuck" request. Also note that
+              the message content may be partially cut off if `finish_reason="length"`, which
+              indicates the generation exceeded `max_tokens` or the conversation exceeded the
+              max context length.
+
           temperature: What sampling temperature to use, between 0 and 2. Higher values like 0.8 will
               make the output more random, while lower values like 0.2 will make it more
               focused and deterministic.
 
+          thread: If no thread is provided, an empty thread will be created.
+
+          tool_choice: Controls which (if any) tool is called by the model. `none` means the model will
+              not call any tools and instead generates a message. `auto` is the default value
+              and means the model can pick between generating a message or calling a tool.
+              Specifying a particular tool like `{"type": "file_search"}` or
+              `{"type": "function", "function": {"name": "my_function"}}` forces the model to
+              call that tool.
+
+          tool_resources: A set of resources that are used by the assistant's tools. The resources are
+              specific to the type of tool. For example, the `code_interpreter` tool requires
+              a list of file IDs, while the `file_search` tool requires a list of vector store
+              IDs.
+
           tools: Override the tools the assistant can use for this run. This is useful for
               modifying the behavior on a per-run basis.
 
+          top_p: An alternative to sampling with temperature, called nucleus sampling, where the
+              model considers the results of the tokens with top_p probability mass. So 0.1
+              means only the tokens comprising the top 10% probability mass are considered.
+
+              We generally recommend altering this or temperature but not both.
+
+          truncation_strategy: Controls for how a thread will be truncated prior to the run. Use this to
+              control the intial context window of the run.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(["assistant_id"], ["assistant_id", "stream"])
-    def create(
+    def create_and_run(
         self,
-        thread_id: str,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run | Stream[AssistantStreamEvent]:
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return self._post(
-            f"/threads/{thread_id}/runs",
+            "/threads/runs",
             body=maybe_transform(
                 {
                     "assistant_id": assistant_id,
-                    "additional_instructions": additional_instructions,
                     "instructions": instructions,
+                    "max_completion_tokens": max_completion_tokens,
+                    "max_prompt_tokens": max_prompt_tokens,
                     "metadata": metadata,
                     "model": model,
+                    "response_format": response_format,
                     "stream": stream,
                     "temperature": temperature,
+                    "thread": thread,
+                    "tool_choice": tool_choice,
+                    "tool_resources": tool_resources,
                     "tools": tools,
+                    "top_p": top_p,
+                    "truncation_strategy": truncation_strategy,
                 },
-                run_create_params.RunCreateParams,
+                thread_create_and_run_params.ThreadCreateAndRunParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Run,
             stream=stream or False,
             stream_cls=Stream[AssistantStreamEvent],
         )
 
-    def retrieve(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        Retrieves a run.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._get(
-            f"/threads/{thread_id}/runs/{run_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-        )
-
-    def update(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        Modifies a run.
-
-        Args:
-          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
-              for storing additional information about the object in a structured format. Keys
-              can be a maximum of 64 characters long and values can be a maxium of 512
-              characters long.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._post(
-            f"/threads/{thread_id}/runs/{run_id}",
-            body=maybe_transform({"metadata": metadata}, run_update_params.RunUpdateParams),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-        )
-
-    def list(
-        self,
-        thread_id: str,
-        *,
-        after: str | NotGiven = NOT_GIVEN,
-        before: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
-        order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SyncCursorPage[Run]:
-        """
-        Returns a list of runs belonging to a thread.
-
-        Args:
-          after: A cursor for use in pagination. `after` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include after=obj_foo in order to
-              fetch the next page of the list.
-
-          before: A cursor for use in pagination. `before` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include before=obj_foo in order to
-              fetch the previous page of the list.
-
-          limit: A limit on the number of objects to be returned. Limit can range between 1 and
-              100, and the default is 20.
-
-          order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
-              order and `desc` for descending order.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._get_api_list(
-            f"/threads/{thread_id}/runs",
-            page=SyncCursorPage[Run],
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                timeout=timeout,
-                query=maybe_transform(
-                    {
-                        "after": after,
-                        "before": before,
-                        "limit": limit,
-                        "order": order,
-                    },
-                    run_list_params.RunListParams,
-                ),
-            ),
-            model=Run,
-        )
-
-    def cancel(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        Cancels a run that is `in_progress`.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._post(
-            f"/threads/{thread_id}/runs/{run_id}/cancel",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-        )
-
-    def create_and_poll(
+    def create_and_run_poll(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         poll_interval_ms: int | NotGiven = NOT_GIVEN,
-        thread_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run:
         """
-        A helper to create a run an poll for a terminal state. More information on Run
-        lifecycles can be found here:
+        A helper to create a thread, start a run and then poll for a terminal state.
+        More information on Run lifecycles can be found here:
         https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
         """
-        run = self.create(
-            thread_id=thread_id,
+        run = self.create_and_run(
             assistant_id=assistant_id,
-            additional_instructions=additional_instructions,
             instructions=instructions,
+            max_completion_tokens=max_completion_tokens,
+            max_prompt_tokens=max_prompt_tokens,
             metadata=metadata,
             model=model,
+            response_format=response_format,
             temperature=temperature,
-            # We assume we are not streaming when polling
             stream=False,
+            thread=thread,
+            tool_resources=tool_resources,
+            tool_choice=tool_choice,
+            truncation_strategy=truncation_strategy,
+            top_p=top_p,
             tools=tools,
             extra_headers=extra_headers,
             extra_query=extra_query,
             extra_body=extra_body,
             timeout=timeout,
         )
-        return self.poll(
-            run.id,
-            thread_id=thread_id,
-            extra_headers=extra_headers,
-            extra_query=extra_query,
-            extra_body=extra_body,
-            poll_interval_ms=poll_interval_ms,
-            timeout=timeout,
-        )
+        return self.runs.poll(run.id, run.thread_id, extra_headers, extra_query, extra_body, timeout, poll_interval_ms)
 
     @overload
-    @typing_extensions.deprecated("use `stream` instead")
-    def create_and_stream(
+    def create_and_run_stream(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AssistantStreamManager[AssistantEventHandler]:
-        """Create a Run stream"""
+        """Create a thread and stream the run back"""
         ...
 
     @overload
-    @typing_extensions.deprecated("use `stream` instead")
-    def create_and_stream(
+    def create_and_run_stream(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         event_handler: AssistantEventHandlerT,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AssistantStreamManager[AssistantEventHandlerT]:
-        """Create a Run stream"""
+        """Create a thread and stream the run back"""
         ...
 
-    @typing_extensions.deprecated("use `stream` instead")
-    def create_and_stream(
+    def create_and_run_stream(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         event_handler: AssistantEventHandlerT | None = None,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AssistantStreamManager[AssistantEventHandler] | AssistantStreamManager[AssistantEventHandlerT]:
-        """Create a Run stream"""
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-
+        """Create a thread and stream the run back"""
         extra_headers = {
-            "OpenAI-Beta": "assistants=v1",
-            "X-Stainless-Stream-Helper": "threads.runs.create_and_stream",
+            "OpenAI-Beta": "assistants=v2",
+            "X-Stainless-Stream-Helper": "threads.create_and_run_stream",
             "X-Stainless-Custom-Event-Handler": "true" if event_handler else "false",
             **(extra_headers or {}),
         }
         make_request = partial(
             self._post,
-            f"/threads/{thread_id}/runs",
+            "/threads/runs",
             body=maybe_transform(
                 {
                     "assistant_id": assistant_id,
-                    "additional_instructions": additional_instructions,
                     "instructions": instructions,
+                    "max_completion_tokens": max_completion_tokens,
+                    "max_prompt_tokens": max_prompt_tokens,
                     "metadata": metadata,
                     "model": model,
+                    "response_format": response_format,
                     "temperature": temperature,
+                    "tool_choice": tool_choice,
                     "stream": True,
+                    "thread": thread,
                     "tools": tools,
+                    "tool": tool_resources,
+                    "truncation_strategy": truncation_strategy,
+                    "top_p": top_p,
                 },
-                run_create_params.RunCreateParams,
+                thread_create_and_run_params.ThreadCreateAndRunParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Run,
             stream=True,
             stream_cls=Stream[AssistantStreamEvent],
         )
         return AssistantStreamManager(make_request, event_handler=event_handler or AssistantEventHandler())
 
-    def poll(
-        self,
-        run_id: str,
-        thread_id: str,
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-        poll_interval_ms: int | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        A helper to poll a run status until it reaches a terminal state. More
-        information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        extra_headers = {"X-Stainless-Poll-Helper": "true", **(extra_headers or {})}
-
-        if is_given(poll_interval_ms):
-            extra_headers["X-Stainless-Custom-Poll-Interval"] = str(poll_interval_ms)
 
-        terminal_states = {"requires_action", "cancelled", "completed", "failed", "expired"}
-        while True:
-            response = self.with_raw_response.retrieve(
-                thread_id=thread_id,
-                run_id=run_id,
-                extra_headers=extra_headers,
-                extra_body=extra_body,
-                extra_query=extra_query,
-                timeout=timeout,
-            )
-
-            run = response.parse()
-            # Return if we reached a terminal state
-            if run.status in terminal_states:
-                return run
-
-            if not is_given(poll_interval_ms):
-                from_header = response.headers.get("openai-poll-after-ms")
-                if from_header is not None:
-                    poll_interval_ms = int(from_header)
-                else:
-                    poll_interval_ms = 1000
+class AsyncThreads(AsyncAPIResource):
+    @cached_property
+    def runs(self) -> AsyncRuns:
+        return AsyncRuns(self._client)
 
-            time.sleep(poll_interval_ms / 1000)
+    @cached_property
+    def messages(self) -> AsyncMessages:
+        return AsyncMessages(self._client)
 
-    @overload
-    def stream(
-        self,
-        *,
-        assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantStreamManager[AssistantEventHandler]:
-        """Create a Run stream"""
-        ...
+    @cached_property
+    def with_raw_response(self) -> AsyncThreadsWithRawResponse:
+        return AsyncThreadsWithRawResponse(self)
 
-    @overload
-    def stream(
-        self,
-        *,
-        assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
-        event_handler: AssistantEventHandlerT,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantStreamManager[AssistantEventHandlerT]:
-        """Create a Run stream"""
-        ...
+    @cached_property
+    def with_streaming_response(self) -> AsyncThreadsWithStreamingResponse:
+        return AsyncThreadsWithStreamingResponse(self)
 
-    def stream(
+    async def create(
         self,
         *,
-        assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        messages: Iterable[thread_create_params.Message] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
-        event_handler: AssistantEventHandlerT | None = None,
+        tool_resources: Optional[thread_create_params.ToolResources] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantStreamManager[AssistantEventHandler] | AssistantStreamManager[AssistantEventHandlerT]:
-        """Create a Run stream"""
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-
-        extra_headers = {
-            "OpenAI-Beta": "assistants=v1",
-            "X-Stainless-Stream-Helper": "threads.runs.create_and_stream",
-            "X-Stainless-Custom-Event-Handler": "true" if event_handler else "false",
-            **(extra_headers or {}),
-        }
-        make_request = partial(
-            self._post,
-            f"/threads/{thread_id}/runs",
-            body=maybe_transform(
-                {
-                    "assistant_id": assistant_id,
-                    "additional_instructions": additional_instructions,
-                    "instructions": instructions,
-                    "metadata": metadata,
-                    "model": model,
-                    "temperature": temperature,
-                    "stream": True,
-                    "tools": tools,
-                },
-                run_create_params.RunCreateParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-            stream=True,
-            stream_cls=Stream[AssistantStreamEvent],
-        )
-        return AssistantStreamManager(make_request, event_handler=event_handler or AssistantEventHandler())
-
-    @overload
-    def submit_tool_outputs(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
+    ) -> Thread:
         """
-        When a run has the `status: "requires_action"` and `required_action.type` is
-        `submit_tool_outputs`, this endpoint can be used to submit the outputs from the
-        tool calls once they're all completed. All outputs must be submitted in a single
-        request.
+        Create a thread.
 
         Args:
-          tool_outputs: A list of tools for which the outputs are being submitted.
+          messages: A list of [messages](https://platform.openai.com/docs/api-reference/messages) to
+              start the thread with.
 
-          stream: If `true`, returns a stream of events that happen during the Run as server-sent
-              events, terminating when the Run enters a terminal state with a `data: [DONE]`
-              message.
+          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
+              for storing additional information about the object in a structured format. Keys
+              can be a maximum of 64 characters long and values can be a maxium of 512
+              characters long.
+
+          tool_resources: A set of resources that are made available to the assistant's tools in this
+              thread. The resources are specific to the type of tool. For example, the
+              `code_interpreter` tool requires a list of file IDs, while the `file_search`
+              tool requires a list of vector store IDs.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        ...
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return await self._post(
+            "/threads",
+            body=await async_maybe_transform(
+                {
+                    "messages": messages,
+                    "metadata": metadata,
+                    "tool_resources": tool_resources,
+                },
+                thread_create_params.ThreadCreateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Thread,
+        )
 
-    @overload
-    def submit_tool_outputs(
+    async def retrieve(
         self,
-        run_id: str,
-        *,
         thread_id: str,
-        stream: Literal[True],
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
+        *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Stream[AssistantStreamEvent]:
+    ) -> Thread:
         """
-        When a run has the `status: "requires_action"` and `required_action.type` is
-        `submit_tool_outputs`, this endpoint can be used to submit the outputs from the
-        tool calls once they're all completed. All outputs must be submitted in a single
-        request.
+        Retrieves a thread.
 
         Args:
-          stream: If `true`, returns a stream of events that happen during the Run as server-sent
-              events, terminating when the Run enters a terminal state with a `data: [DONE]`
-              message.
-
-          tool_outputs: A list of tools for which the outputs are being submitted.
-
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        ...
+        if not thread_id:
+            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return await self._get(
+            f"/threads/{thread_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Thread,
+        )
 
-    @overload
-    def submit_tool_outputs(
+    async def update(
         self,
-        run_id: str,
-        *,
         thread_id: str,
-        stream: bool,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
+        *,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_update_params.ToolResources] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run | Stream[AssistantStreamEvent]:
+    ) -> Thread:
         """
-        When a run has the `status: "requires_action"` and `required_action.type` is
-        `submit_tool_outputs`, this endpoint can be used to submit the outputs from the
-        tool calls once they're all completed. All outputs must be submitted in a single
-        request.
+        Modifies a thread.
 
         Args:
-          stream: If `true`, returns a stream of events that happen during the Run as server-sent
-              events, terminating when the Run enters a terminal state with a `data: [DONE]`
-              message.
+          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
+              for storing additional information about the object in a structured format. Keys
+              can be a maximum of 64 characters long and values can be a maxium of 512
+              characters long.
 
-          tool_outputs: A list of tools for which the outputs are being submitted.
+          tool_resources: A set of resources that are made available to the assistant's tools in this
+              thread. The resources are specific to the type of tool. For example, the
+              `code_interpreter` tool requires a list of file IDs, while the `file_search`
+              tool requires a list of vector store IDs.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        ...
-
-    @required_args(["thread_id", "tool_outputs"], ["thread_id", "stream", "tool_outputs"])
-    def submit_tool_outputs(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run | Stream[AssistantStreamEvent]:
         if not thread_id:
             raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._post(
-            f"/threads/{thread_id}/runs/{run_id}/submit_tool_outputs",
-            body=maybe_transform(
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return await self._post(
+            f"/threads/{thread_id}",
+            body=await async_maybe_transform(
                 {
-                    "tool_outputs": tool_outputs,
-                    "stream": stream,
+                    "metadata": metadata,
+                    "tool_resources": tool_resources,
                 },
-                run_submit_tool_outputs_params.RunSubmitToolOutputsParams,
+                thread_update_params.ThreadUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
-            stream=stream or False,
-            stream_cls=Stream[AssistantStreamEvent],
+            cast_to=Thread,
         )
 
-    def submit_tool_outputs_and_poll(
+    async def delete(
         self,
-        *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
         thread_id: str,
-        poll_interval_ms: int | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        A helper to submit a tool output to a run and poll for a terminal run state.
-        More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        run = self.submit_tool_outputs(
-            run_id=run_id,
-            thread_id=thread_id,
-            tool_outputs=tool_outputs,
-            stream=False,
-            extra_headers=extra_headers,
-            extra_query=extra_query,
-            extra_body=extra_body,
-            timeout=timeout,
-        )
-        return self.poll(
-            run_id=run.id,
-            thread_id=thread_id,
-            extra_headers=extra_headers,
-            extra_query=extra_query,
-            extra_body=extra_body,
-            timeout=timeout,
-            poll_interval_ms=poll_interval_ms,
-        )
-
-    @overload
-    def submit_tool_outputs_stream(
-        self,
         *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
-        thread_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantStreamManager[AssistantEventHandler]:
-        """
-        Submit the tool outputs from a previous run and stream the run to a terminal
-        state. More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
+    ) -> ThreadDeleted:
         """
-        ...
+        Delete a thread.
 
-    @overload
-    def submit_tool_outputs_stream(
-        self,
-        *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
-        thread_id: str,
-        event_handler: AssistantEventHandlerT,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantStreamManager[AssistantEventHandlerT]:
-        """
-        Submit the tool outputs from a previous run and stream the run to a terminal
-        state. More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        ...
+        Args:
+          extra_headers: Send extra headers
 
-    def submit_tool_outputs_stream(
-        self,
-        *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
-        thread_id: str,
-        event_handler: AssistantEventHandlerT | None = None,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AssistantStreamManager[AssistantEventHandler] | AssistantStreamManager[AssistantEventHandlerT]:
-        """
-        Submit the tool outputs from a previous run and stream the run to a terminal
-        state. More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
+          extra_query: Add additional query parameters to the request
 
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         if not thread_id:
             raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-
-        extra_headers = {
-            "OpenAI-Beta": "assistants=v1",
-            "X-Stainless-Stream-Helper": "threads.runs.submit_tool_outputs_stream",
-            "X-Stainless-Custom-Event-Handler": "true" if event_handler else "false",
-            **(extra_headers or {}),
-        }
-        request = partial(
-            self._post,
-            f"/threads/{thread_id}/runs/{run_id}/submit_tool_outputs",
-            body=maybe_transform(
-                {
-                    "tool_outputs": tool_outputs,
-                    "stream": True,
-                },
-                run_submit_tool_outputs_params.RunSubmitToolOutputsParams,
-            ),
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
+        return await self._delete(
+            f"/threads/{thread_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
-            stream=True,
-            stream_cls=Stream[AssistantStreamEvent],
+            cast_to=ThreadDeleted,
         )
-        return AssistantStreamManager(request, event_handler=event_handler or AssistantEventHandler())
-
-
-class AsyncRuns(AsyncAPIResource):
-    @cached_property
-    def steps(self) -> AsyncSteps:
-        return AsyncSteps(self._client)
-
-    @cached_property
-    def with_raw_response(self) -> AsyncRunsWithRawResponse:
-        return AsyncRunsWithRawResponse(self)
-
-    @cached_property
-    def with_streaming_response(self) -> AsyncRunsWithStreamingResponse:
-        return AsyncRunsWithStreamingResponse(self)
 
     @overload
-    async def create(
+    async def create_and_run(
         self,
-        thread_id: str,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run:
         """
-        Create a run.
+        Create a thread and run it in one request.
 
         Args:
           assistant_id: The ID of the
               [assistant](https://platform.openai.com/docs/api-reference/assistants) to use to
               execute this run.
 
-          additional_instructions: Appends additional instructions at the end of the instructions for the run. This
-              is useful for modifying the behavior on a per-run basis without overriding other
-              instructions.
-
-          instructions: Overrides the
-              [instructions](https://platform.openai.com/docs/api-reference/assistants/createAssistant)
-              of the assistant. This is useful for modifying the behavior on a per-run basis.
+          instructions: Override the default system message of the assistant. This is useful for
+              modifying the behavior on a per-run basis.
+
+          max_completion_tokens: The maximum number of completion tokens that may be used over the course of the
+              run. The run will make a best effort to use only the number of completion tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              completion tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
+
+          max_prompt_tokens: The maximum number of prompt tokens that may be used over the course of the run.
+              The run will make a best effort to use only the number of prompt tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              prompt tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
           model: The ID of the [Model](https://platform.openai.com/docs/api-reference/models) to
               be used to execute this run. If a value is provided here, it will override the
               model associated with the assistant. If not, the model associated with the
               assistant will be used.
 
+          response_format: Specifies the format that the model must output. Compatible with
+              [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
+              all GPT-3.5 Turbo models since `gpt-3.5-turbo-1106`.
+
+              Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
+              message the model generates is valid JSON.
+
+              **Important:** when using JSON mode, you **must** also instruct the model to
+              produce JSON yourself via a system or user message. Without this, the model may
+              generate an unending stream of whitespace until the generation reaches the token
+              limit, resulting in a long-running and seemingly "stuck" request. Also note that
+              the message content may be partially cut off if `finish_reason="length"`, which
+              indicates the generation exceeded `max_tokens` or the conversation exceeded the
+              max context length.
+
           stream: If `true`, returns a stream of events that happen during the Run as server-sent
               events, terminating when the Run enters a terminal state with a `data: [DONE]`
               message.
 
           temperature: What sampling temperature to use, between 0 and 2. Higher values like 0.8 will
               make the output more random, while lower values like 0.2 will make it more
               focused and deterministic.
 
+          thread: If no thread is provided, an empty thread will be created.
+
+          tool_choice: Controls which (if any) tool is called by the model. `none` means the model will
+              not call any tools and instead generates a message. `auto` is the default value
+              and means the model can pick between generating a message or calling a tool.
+              Specifying a particular tool like `{"type": "file_search"}` or
+              `{"type": "function", "function": {"name": "my_function"}}` forces the model to
+              call that tool.
+
+          tool_resources: A set of resources that are used by the assistant's tools. The resources are
+              specific to the type of tool. For example, the `code_interpreter` tool requires
+              a list of file IDs, while the `file_search` tool requires a list of vector store
+              IDs.
+
           tools: Override the tools the assistant can use for this run. This is useful for
               modifying the behavior on a per-run basis.
 
+          top_p: An alternative to sampling with temperature, called nucleus sampling, where the
+              model considers the results of the tokens with top_p probability mass. So 0.1
+              means only the tokens comprising the top 10% probability mass are considered.
+
+              We generally recommend altering this or temperature but not both.
+
+          truncation_strategy: Controls for how a thread will be truncated prior to the run. Use this to
+              control the intial context window of the run.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    async def create(
+    async def create_and_run(
         self,
-        thread_id: str,
         *,
         assistant_id: str,
         stream: Literal[True],
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncStream[AssistantStreamEvent]:
         """
-        Create a run.
+        Create a thread and run it in one request.
 
         Args:
           assistant_id: The ID of the
               [assistant](https://platform.openai.com/docs/api-reference/assistants) to use to
               execute this run.
 
           stream: If `true`, returns a stream of events that happen during the Run as server-sent
               events, terminating when the Run enters a terminal state with a `data: [DONE]`
               message.
 
-          additional_instructions: Appends additional instructions at the end of the instructions for the run. This
-              is useful for modifying the behavior on a per-run basis without overriding other
-              instructions.
-
-          instructions: Overrides the
-              [instructions](https://platform.openai.com/docs/api-reference/assistants/createAssistant)
-              of the assistant. This is useful for modifying the behavior on a per-run basis.
+          instructions: Override the default system message of the assistant. This is useful for
+              modifying the behavior on a per-run basis.
+
+          max_completion_tokens: The maximum number of completion tokens that may be used over the course of the
+              run. The run will make a best effort to use only the number of completion tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              completion tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
+
+          max_prompt_tokens: The maximum number of prompt tokens that may be used over the course of the run.
+              The run will make a best effort to use only the number of prompt tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              prompt tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
           model: The ID of the [Model](https://platform.openai.com/docs/api-reference/models) to
               be used to execute this run. If a value is provided here, it will override the
               model associated with the assistant. If not, the model associated with the
               assistant will be used.
 
+          response_format: Specifies the format that the model must output. Compatible with
+              [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
+              all GPT-3.5 Turbo models since `gpt-3.5-turbo-1106`.
+
+              Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
+              message the model generates is valid JSON.
+
+              **Important:** when using JSON mode, you **must** also instruct the model to
+              produce JSON yourself via a system or user message. Without this, the model may
+              generate an unending stream of whitespace until the generation reaches the token
+              limit, resulting in a long-running and seemingly "stuck" request. Also note that
+              the message content may be partially cut off if `finish_reason="length"`, which
+              indicates the generation exceeded `max_tokens` or the conversation exceeded the
+              max context length.
+
           temperature: What sampling temperature to use, between 0 and 2. Higher values like 0.8 will
               make the output more random, while lower values like 0.2 will make it more
               focused and deterministic.
 
+          thread: If no thread is provided, an empty thread will be created.
+
+          tool_choice: Controls which (if any) tool is called by the model. `none` means the model will
+              not call any tools and instead generates a message. `auto` is the default value
+              and means the model can pick between generating a message or calling a tool.
+              Specifying a particular tool like `{"type": "file_search"}` or
+              `{"type": "function", "function": {"name": "my_function"}}` forces the model to
+              call that tool.
+
+          tool_resources: A set of resources that are used by the assistant's tools. The resources are
+              specific to the type of tool. For example, the `code_interpreter` tool requires
+              a list of file IDs, while the `file_search` tool requires a list of vector store
+              IDs.
+
           tools: Override the tools the assistant can use for this run. This is useful for
               modifying the behavior on a per-run basis.
 
+          top_p: An alternative to sampling with temperature, called nucleus sampling, where the
+              model considers the results of the tokens with top_p probability mass. So 0.1
+              means only the tokens comprising the top 10% probability mass are considered.
+
+              We generally recommend altering this or temperature but not both.
+
+          truncation_strategy: Controls for how a thread will be truncated prior to the run. Use this to
+              control the intial context window of the run.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @overload
-    async def create(
+    async def create_and_run(
         self,
-        thread_id: str,
         *,
         assistant_id: str,
         stream: bool,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run | AsyncStream[AssistantStreamEvent]:
         """
-        Create a run.
+        Create a thread and run it in one request.
 
         Args:
           assistant_id: The ID of the
               [assistant](https://platform.openai.com/docs/api-reference/assistants) to use to
               execute this run.
 
           stream: If `true`, returns a stream of events that happen during the Run as server-sent
               events, terminating when the Run enters a terminal state with a `data: [DONE]`
               message.
 
-          additional_instructions: Appends additional instructions at the end of the instructions for the run. This
-              is useful for modifying the behavior on a per-run basis without overriding other
-              instructions.
-
-          instructions: Overrides the
-              [instructions](https://platform.openai.com/docs/api-reference/assistants/createAssistant)
-              of the assistant. This is useful for modifying the behavior on a per-run basis.
+          instructions: Override the default system message of the assistant. This is useful for
+              modifying the behavior on a per-run basis.
+
+          max_completion_tokens: The maximum number of completion tokens that may be used over the course of the
+              run. The run will make a best effort to use only the number of completion tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              completion tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
+
+          max_prompt_tokens: The maximum number of prompt tokens that may be used over the course of the run.
+              The run will make a best effort to use only the number of prompt tokens
+              specified, across multiple turns of the run. If the run exceeds the number of
+              prompt tokens specified, the run will end with status `incomplete`. See
+              `incomplete_details` for more info.
 
           metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
               for storing additional information about the object in a structured format. Keys
               can be a maximum of 64 characters long and values can be a maxium of 512
               characters long.
 
           model: The ID of the [Model](https://platform.openai.com/docs/api-reference/models) to
               be used to execute this run. If a value is provided here, it will override the
               model associated with the assistant. If not, the model associated with the
               assistant will be used.
 
+          response_format: Specifies the format that the model must output. Compatible with
+              [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
+              all GPT-3.5 Turbo models since `gpt-3.5-turbo-1106`.
+
+              Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
+              message the model generates is valid JSON.
+
+              **Important:** when using JSON mode, you **must** also instruct the model to
+              produce JSON yourself via a system or user message. Without this, the model may
+              generate an unending stream of whitespace until the generation reaches the token
+              limit, resulting in a long-running and seemingly "stuck" request. Also note that
+              the message content may be partially cut off if `finish_reason="length"`, which
+              indicates the generation exceeded `max_tokens` or the conversation exceeded the
+              max context length.
+
           temperature: What sampling temperature to use, between 0 and 2. Higher values like 0.8 will
               make the output more random, while lower values like 0.2 will make it more
               focused and deterministic.
 
+          thread: If no thread is provided, an empty thread will be created.
+
+          tool_choice: Controls which (if any) tool is called by the model. `none` means the model will
+              not call any tools and instead generates a message. `auto` is the default value
+              and means the model can pick between generating a message or calling a tool.
+              Specifying a particular tool like `{"type": "file_search"}` or
+              `{"type": "function", "function": {"name": "my_function"}}` forces the model to
+              call that tool.
+
+          tool_resources: A set of resources that are used by the assistant's tools. The resources are
+              specific to the type of tool. For example, the `code_interpreter` tool requires
+              a list of file IDs, while the `file_search` tool requires a list of vector store
+              IDs.
+
           tools: Override the tools the assistant can use for this run. This is useful for
               modifying the behavior on a per-run basis.
 
+          top_p: An alternative to sampling with temperature, called nucleus sampling, where the
+              model considers the results of the tokens with top_p probability mass. So 0.1
+              means only the tokens comprising the top 10% probability mass are considered.
+
+              We generally recommend altering this or temperature but not both.
+
+          truncation_strategy: Controls for how a thread will be truncated prior to the run. Use this to
+              control the intial context window of the run.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         ...
 
     @required_args(["assistant_id"], ["assistant_id", "stream"])
-    async def create(
+    async def create_and_run(
         self,
-        thread_id: str,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
         stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run | AsyncStream[AssistantStreamEvent]:
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
+        extra_headers = {"OpenAI-Beta": "assistants=v2", **(extra_headers or {})}
         return await self._post(
-            f"/threads/{thread_id}/runs",
+            "/threads/runs",
             body=await async_maybe_transform(
                 {
                     "assistant_id": assistant_id,
-                    "additional_instructions": additional_instructions,
                     "instructions": instructions,
+                    "max_completion_tokens": max_completion_tokens,
+                    "max_prompt_tokens": max_prompt_tokens,
                     "metadata": metadata,
                     "model": model,
+                    "response_format": response_format,
                     "stream": stream,
                     "temperature": temperature,
+                    "thread": thread,
+                    "tool_choice": tool_choice,
+                    "tool_resources": tool_resources,
                     "tools": tools,
+                    "top_p": top_p,
+                    "truncation_strategy": truncation_strategy,
                 },
-                run_create_params.RunCreateParams,
+                thread_create_and_run_params.ThreadCreateAndRunParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Run,
             stream=stream or False,
             stream_cls=AsyncStream[AssistantStreamEvent],
         )
 
-    async def retrieve(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        Retrieves a run.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return await self._get(
-            f"/threads/{thread_id}/runs/{run_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-        )
-
-    async def update(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        Modifies a run.
-
-        Args:
-          metadata: Set of 16 key-value pairs that can be attached to an object. This can be useful
-              for storing additional information about the object in a structured format. Keys
-              can be a maximum of 64 characters long and values can be a maxium of 512
-              characters long.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return await self._post(
-            f"/threads/{thread_id}/runs/{run_id}",
-            body=await async_maybe_transform({"metadata": metadata}, run_update_params.RunUpdateParams),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-        )
-
-    def list(
-        self,
-        thread_id: str,
-        *,
-        after: str | NotGiven = NOT_GIVEN,
-        before: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
-        order: Literal["asc", "desc"] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[Run, AsyncCursorPage[Run]]:
-        """
-        Returns a list of runs belonging to a thread.
-
-        Args:
-          after: A cursor for use in pagination. `after` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include after=obj_foo in order to
-              fetch the next page of the list.
-
-          before: A cursor for use in pagination. `before` is an object ID that defines your place
-              in the list. For instance, if you make a list request and receive 100 objects,
-              ending with obj_foo, your subsequent call can include before=obj_foo in order to
-              fetch the previous page of the list.
-
-          limit: A limit on the number of objects to be returned. Limit can range between 1 and
-              100, and the default is 20.
-
-          order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending
-              order and `desc` for descending order.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return self._get_api_list(
-            f"/threads/{thread_id}/runs",
-            page=AsyncCursorPage[Run],
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                timeout=timeout,
-                query=maybe_transform(
-                    {
-                        "after": after,
-                        "before": before,
-                        "limit": limit,
-                        "order": order,
-                    },
-                    run_list_params.RunListParams,
-                ),
-            ),
-            model=Run,
-        )
-
-    async def cancel(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        Cancels a run that is `in_progress`.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return await self._post(
-            f"/threads/{thread_id}/runs/{run_id}/cancel",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-        )
-
-    async def create_and_poll(
+    async def create_and_run_poll(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         poll_interval_ms: int | NotGiven = NOT_GIVEN,
-        thread_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Run:
         """
-        A helper to create a run an poll for a terminal state. More information on Run
-        lifecycles can be found here:
+        A helper to create a thread, start a run and then poll for a terminal state.
+        More information on Run lifecycles can be found here:
         https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
         """
-        run = await self.create(
-            thread_id=thread_id,
+        run = await self.create_and_run(
             assistant_id=assistant_id,
-            additional_instructions=additional_instructions,
             instructions=instructions,
+            max_completion_tokens=max_completion_tokens,
+            max_prompt_tokens=max_prompt_tokens,
             metadata=metadata,
             model=model,
+            response_format=response_format,
             temperature=temperature,
-            # We assume we are not streaming when polling
             stream=False,
+            thread=thread,
+            tool_resources=tool_resources,
+            tool_choice=tool_choice,
+            truncation_strategy=truncation_strategy,
+            top_p=top_p,
             tools=tools,
             extra_headers=extra_headers,
             extra_query=extra_query,
             extra_body=extra_body,
             timeout=timeout,
         )
-        return await self.poll(
-            run.id,
-            thread_id=thread_id,
-            extra_headers=extra_headers,
-            extra_query=extra_query,
-            extra_body=extra_body,
-            poll_interval_ms=poll_interval_ms,
-            timeout=timeout,
-        )
-
-    @overload
-    @typing_extensions.deprecated("use `stream` instead")
-    def create_and_stream(
-        self,
-        *,
-        assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncAssistantStreamManager[AsyncAssistantEventHandler]:
-        """Create a Run stream"""
-        ...
-
-    @overload
-    @typing_extensions.deprecated("use `stream` instead")
-    def create_and_stream(
-        self,
-        *,
-        assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
-        event_handler: AsyncAssistantEventHandlerT,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncAssistantStreamManager[AsyncAssistantEventHandlerT]:
-        """Create a Run stream"""
-        ...
-
-    @typing_extensions.deprecated("use `stream` instead")
-    def create_and_stream(
-        self,
-        *,
-        assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
-        event_handler: AsyncAssistantEventHandlerT | None = None,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> (
-        AsyncAssistantStreamManager[AsyncAssistantEventHandler]
-        | AsyncAssistantStreamManager[AsyncAssistantEventHandlerT]
-    ):
-        """Create a Run stream"""
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-
-        extra_headers = {
-            "OpenAI-Beta": "assistants=v1",
-            "X-Stainless-Stream-Helper": "threads.runs.create_and_stream",
-            "X-Stainless-Custom-Event-Handler": "true" if event_handler else "false",
-            **(extra_headers or {}),
-        }
-        request = self._post(
-            f"/threads/{thread_id}/runs",
-            body=maybe_transform(
-                {
-                    "assistant_id": assistant_id,
-                    "additional_instructions": additional_instructions,
-                    "instructions": instructions,
-                    "metadata": metadata,
-                    "model": model,
-                    "temperature": temperature,
-                    "stream": True,
-                    "tools": tools,
-                },
-                run_create_params.RunCreateParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-            stream=True,
-            stream_cls=AsyncStream[AssistantStreamEvent],
+        return await self.runs.poll(
+            run.id, run.thread_id, extra_headers, extra_query, extra_body, timeout, poll_interval_ms
         )
-        return AsyncAssistantStreamManager(request, event_handler=event_handler or AsyncAssistantEventHandler())
-
-    async def poll(
-        self,
-        run_id: str,
-        thread_id: str,
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-        poll_interval_ms: int | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        A helper to poll a run status until it reaches a terminal state. More
-        information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        extra_headers = {"X-Stainless-Poll-Helper": "true", **(extra_headers or {})}
-
-        if is_given(poll_interval_ms):
-            extra_headers["X-Stainless-Custom-Poll-Interval"] = str(poll_interval_ms)
-
-        terminal_states = {"requires_action", "cancelled", "completed", "failed", "expired"}
-        while True:
-            response = await self.with_raw_response.retrieve(
-                thread_id=thread_id,
-                run_id=run_id,
-                extra_headers=extra_headers,
-                extra_body=extra_body,
-                extra_query=extra_query,
-                timeout=timeout,
-            )
-
-            run = response.parse()
-            # Return if we reached a terminal state
-            if run.status in terminal_states:
-                return run
-
-            if not is_given(poll_interval_ms):
-                from_header = response.headers.get("openai-poll-after-ms")
-                if from_header is not None:
-                    poll_interval_ms = int(from_header)
-                else:
-                    poll_interval_ms = 1000
-
-            time.sleep(poll_interval_ms / 1000)
 
     @overload
-    def stream(
+    def create_and_run_stream(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncAssistantStreamManager[AsyncAssistantEventHandler]:
-        """Create a Run stream"""
+        """Create a thread and stream the run back"""
         ...
 
     @overload
-    def stream(
+    def create_and_run_stream(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         event_handler: AsyncAssistantEventHandlerT,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AsyncAssistantStreamManager[AsyncAssistantEventHandlerT]:
-        """Create a Run stream"""
+        """Create a thread and stream the run back"""
         ...
 
-    def stream(
+    def create_and_run_stream(
         self,
         *,
         assistant_id: str,
-        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
-        metadata: Optional[object] | NotGiven = NOT_GIVEN,
-        model: Optional[str] | NotGiven = NOT_GIVEN,
-        temperature: Optional[float] | NotGiven = NOT_GIVEN,
-        tools: Optional[Iterable[AssistantToolParam]] | NotGiven = NOT_GIVEN,
-        thread_id: str,
+        max_completion_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        max_prompt_tokens: Optional[int] | NotGiven = NOT_GIVEN,
+        metadata: Optional[object] | NotGiven = NOT_GIVEN,
+        model: Union[
+            str,
+            Literal[
+                "gpt-4-turbo",
+                "gpt-4-turbo-2024-04-09",
+                "gpt-4-0125-preview",
+                "gpt-4-turbo-preview",
+                "gpt-4-1106-preview",
+                "gpt-4-vision-preview",
+                "gpt-4",
+                "gpt-4-0314",
+                "gpt-4-0613",
+                "gpt-4-32k",
+                "gpt-4-32k-0314",
+                "gpt-4-32k-0613",
+                "gpt-3.5-turbo",
+                "gpt-3.5-turbo-16k",
+                "gpt-3.5-turbo-0613",
+                "gpt-3.5-turbo-1106",
+                "gpt-3.5-turbo-0125",
+                "gpt-3.5-turbo-16k-0613",
+            ],
+            None,
+        ]
+        | NotGiven = NOT_GIVEN,
+        response_format: Optional[AssistantResponseFormatOptionParam] | NotGiven = NOT_GIVEN,
+        temperature: Optional[float] | NotGiven = NOT_GIVEN,
+        thread: thread_create_and_run_params.Thread | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[AssistantToolChoiceOptionParam] | NotGiven = NOT_GIVEN,
+        tool_resources: Optional[thread_create_and_run_params.ToolResources] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[thread_create_and_run_params.Tool]] | NotGiven = NOT_GIVEN,
+        top_p: Optional[float] | NotGiven = NOT_GIVEN,
+        truncation_strategy: Optional[thread_create_and_run_params.TruncationStrategy] | NotGiven = NOT_GIVEN,
         event_handler: AsyncAssistantEventHandlerT | None = None,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> (
         AsyncAssistantStreamManager[AsyncAssistantEventHandler]
         | AsyncAssistantStreamManager[AsyncAssistantEventHandlerT]
     ):
-        """Create a Run stream"""
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-
+        """Create a thread and stream the run back"""
         extra_headers = {
-            "OpenAI-Beta": "assistants=v1",
-            "X-Stainless-Stream-Helper": "threads.runs.create_and_stream",
+            "OpenAI-Beta": "assistants=v2",
+            "X-Stainless-Stream-Helper": "threads.create_and_run_stream",
             "X-Stainless-Custom-Event-Handler": "true" if event_handler else "false",
             **(extra_headers or {}),
         }
         request = self._post(
-            f"/threads/{thread_id}/runs",
+            "/threads/runs",
             body=maybe_transform(
                 {
                     "assistant_id": assistant_id,
-                    "additional_instructions": additional_instructions,
                     "instructions": instructions,
+                    "max_completion_tokens": max_completion_tokens,
+                    "max_prompt_tokens": max_prompt_tokens,
                     "metadata": metadata,
                     "model": model,
+                    "response_format": response_format,
                     "temperature": temperature,
+                    "tool_choice": tool_choice,
                     "stream": True,
+                    "thread": thread,
                     "tools": tools,
+                    "tool": tool_resources,
+                    "truncation_strategy": truncation_strategy,
+                    "top_p": top_p,
                 },
-                run_create_params.RunCreateParams,
+                thread_create_and_run_params.ThreadCreateAndRunParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Run,
             stream=True,
             stream_cls=AsyncStream[AssistantStreamEvent],
         )
         return AsyncAssistantStreamManager(request, event_handler=event_handler or AsyncAssistantEventHandler())
 
-    @overload
-    async def submit_tool_outputs(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        stream: Optional[Literal[False]] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        When a run has the `status: "requires_action"` and `required_action.type` is
-        `submit_tool_outputs`, this endpoint can be used to submit the outputs from the
-        tool calls once they're all completed. All outputs must be submitted in a single
-        request.
-
-        Args:
-          tool_outputs: A list of tools for which the outputs are being submitted.
 
-          stream: If `true`, returns a stream of events that happen during the Run as server-sent
-              events, terminating when the Run enters a terminal state with a `data: [DONE]`
-              message.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        ...
-
-    @overload
-    async def submit_tool_outputs(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        stream: Literal[True],
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncStream[AssistantStreamEvent]:
-        """
-        When a run has the `status: "requires_action"` and `required_action.type` is
-        `submit_tool_outputs`, this endpoint can be used to submit the outputs from the
-        tool calls once they're all completed. All outputs must be submitted in a single
-        request.
-
-        Args:
-          stream: If `true`, returns a stream of events that happen during the Run as server-sent
-              events, terminating when the Run enters a terminal state with a `data: [DONE]`
-              message.
-
-          tool_outputs: A list of tools for which the outputs are being submitted.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        ...
-
-    @overload
-    async def submit_tool_outputs(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        stream: bool,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run | AsyncStream[AssistantStreamEvent]:
-        """
-        When a run has the `status: "requires_action"` and `required_action.type` is
-        `submit_tool_outputs`, this endpoint can be used to submit the outputs from the
-        tool calls once they're all completed. All outputs must be submitted in a single
-        request.
-
-        Args:
-          stream: If `true`, returns a stream of events that happen during the Run as server-sent
-              events, terminating when the Run enters a terminal state with a `data: [DONE]`
-              message.
-
-          tool_outputs: A list of tools for which the outputs are being submitted.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        ...
-
-    @required_args(["thread_id", "tool_outputs"], ["thread_id", "stream", "tool_outputs"])
-    async def submit_tool_outputs(
-        self,
-        run_id: str,
-        *,
-        thread_id: str,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        stream: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run | AsyncStream[AssistantStreamEvent]:
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-        extra_headers = {"OpenAI-Beta": "assistants=v1", **(extra_headers or {})}
-        return await self._post(
-            f"/threads/{thread_id}/runs/{run_id}/submit_tool_outputs",
-            body=await async_maybe_transform(
-                {
-                    "tool_outputs": tool_outputs,
-                    "stream": stream,
-                },
-                run_submit_tool_outputs_params.RunSubmitToolOutputsParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-            stream=stream or False,
-            stream_cls=AsyncStream[AssistantStreamEvent],
-        )
-
-    async def submit_tool_outputs_and_poll(
-        self,
-        *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
-        thread_id: str,
-        poll_interval_ms: int | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
-        """
-        A helper to submit a tool output to a run and poll for a terminal run state.
-        More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        run = await self.submit_tool_outputs(
-            run_id=run_id,
-            thread_id=thread_id,
-            tool_outputs=tool_outputs,
-            stream=False,
-            extra_headers=extra_headers,
-            extra_query=extra_query,
-            extra_body=extra_body,
-            timeout=timeout,
-        )
-        return await self.poll(
-            run_id=run.id,
-            thread_id=thread_id,
-            extra_headers=extra_headers,
-            extra_query=extra_query,
-            extra_body=extra_body,
-            timeout=timeout,
-            poll_interval_ms=poll_interval_ms,
-        )
-
-    @overload
-    def submit_tool_outputs_stream(
-        self,
-        *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
-        thread_id: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncAssistantStreamManager[AsyncAssistantEventHandler]:
-        """
-        Submit the tool outputs from a previous run and stream the run to a terminal
-        state. More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        ...
-
-    @overload
-    def submit_tool_outputs_stream(
-        self,
-        *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
-        thread_id: str,
-        event_handler: AsyncAssistantEventHandlerT,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncAssistantStreamManager[AsyncAssistantEventHandlerT]:
-        """
-        Submit the tool outputs from a previous run and stream the run to a terminal
-        state. More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        ...
-
-    def submit_tool_outputs_stream(
-        self,
-        *,
-        tool_outputs: Iterable[run_submit_tool_outputs_params.ToolOutput],
-        run_id: str,
-        thread_id: str,
-        event_handler: AsyncAssistantEventHandlerT | None = None,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> (
-        AsyncAssistantStreamManager[AsyncAssistantEventHandler]
-        | AsyncAssistantStreamManager[AsyncAssistantEventHandlerT]
-    ):
-        """
-        Submit the tool outputs from a previous run and stream the run to a terminal
-        state. More information on Run lifecycles can be found here:
-        https://platform.openai.com/docs/assistants/how-it-works/runs-and-run-steps
-        """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
-
-        if not thread_id:
-            raise ValueError(f"Expected a non-empty value for `thread_id` but received {thread_id!r}")
-
-        extra_headers = {
-            "OpenAI-Beta": "assistants=v1",
-            "X-Stainless-Stream-Helper": "threads.runs.submit_tool_outputs_stream",
-            "X-Stainless-Custom-Event-Handler": "true" if event_handler else "false",
-            **(extra_headers or {}),
-        }
-        request = self._post(
-            f"/threads/{thread_id}/runs/{run_id}/submit_tool_outputs",
-            body=maybe_transform(
-                {
-                    "tool_outputs": tool_outputs,
-                    "stream": True,
-                },
-                run_submit_tool_outputs_params.RunSubmitToolOutputsParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Run,
-            stream=True,
-            stream_cls=AsyncStream[AssistantStreamEvent],
-        )
-        return AsyncAssistantStreamManager(request, event_handler=event_handler or AsyncAssistantEventHandler())
-
-
-class RunsWithRawResponse:
-    def __init__(self, runs: Runs) -> None:
-        self._runs = runs
+class ThreadsWithRawResponse:
+    def __init__(self, threads: Threads) -> None:
+        self._threads = threads
 
         self.create = _legacy_response.to_raw_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = _legacy_response.to_raw_response_wrapper(
-            runs.update,
+            threads.update,
         )
-        self.list = _legacy_response.to_raw_response_wrapper(
-            runs.list,
+        self.delete = _legacy_response.to_raw_response_wrapper(
+            threads.delete,
         )
-        self.cancel = _legacy_response.to_raw_response_wrapper(
-            runs.cancel,
-        )
-        self.submit_tool_outputs = _legacy_response.to_raw_response_wrapper(
-            runs.submit_tool_outputs,
+        self.create_and_run = _legacy_response.to_raw_response_wrapper(
+            threads.create_and_run,
         )
 
     @cached_property
-    def steps(self) -> StepsWithRawResponse:
-        return StepsWithRawResponse(self._runs.steps)
+    def runs(self) -> RunsWithRawResponse:
+        return RunsWithRawResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> MessagesWithRawResponse:
+        return MessagesWithRawResponse(self._threads.messages)
 
 
-class AsyncRunsWithRawResponse:
-    def __init__(self, runs: AsyncRuns) -> None:
-        self._runs = runs
+class AsyncThreadsWithRawResponse:
+    def __init__(self, threads: AsyncThreads) -> None:
+        self._threads = threads
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = _legacy_response.async_to_raw_response_wrapper(
-            runs.update,
-        )
-        self.list = _legacy_response.async_to_raw_response_wrapper(
-            runs.list,
+            threads.update,
         )
-        self.cancel = _legacy_response.async_to_raw_response_wrapper(
-            runs.cancel,
+        self.delete = _legacy_response.async_to_raw_response_wrapper(
+            threads.delete,
         )
-        self.submit_tool_outputs = _legacy_response.async_to_raw_response_wrapper(
-            runs.submit_tool_outputs,
+        self.create_and_run = _legacy_response.async_to_raw_response_wrapper(
+            threads.create_and_run,
         )
 
     @cached_property
-    def steps(self) -> AsyncStepsWithRawResponse:
-        return AsyncStepsWithRawResponse(self._runs.steps)
+    def runs(self) -> AsyncRunsWithRawResponse:
+        return AsyncRunsWithRawResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> AsyncMessagesWithRawResponse:
+        return AsyncMessagesWithRawResponse(self._threads.messages)
 
 
-class RunsWithStreamingResponse:
-    def __init__(self, runs: Runs) -> None:
-        self._runs = runs
+class ThreadsWithStreamingResponse:
+    def __init__(self, threads: Threads) -> None:
+        self._threads = threads
 
         self.create = to_streamed_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = to_streamed_response_wrapper(
-            runs.update,
+            threads.update,
         )
-        self.list = to_streamed_response_wrapper(
-            runs.list,
+        self.delete = to_streamed_response_wrapper(
+            threads.delete,
         )
-        self.cancel = to_streamed_response_wrapper(
-            runs.cancel,
-        )
-        self.submit_tool_outputs = to_streamed_response_wrapper(
-            runs.submit_tool_outputs,
+        self.create_and_run = to_streamed_response_wrapper(
+            threads.create_and_run,
         )
 
     @cached_property
-    def steps(self) -> StepsWithStreamingResponse:
-        return StepsWithStreamingResponse(self._runs.steps)
+    def runs(self) -> RunsWithStreamingResponse:
+        return RunsWithStreamingResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> MessagesWithStreamingResponse:
+        return MessagesWithStreamingResponse(self._threads.messages)
 
 
-class AsyncRunsWithStreamingResponse:
-    def __init__(self, runs: AsyncRuns) -> None:
-        self._runs = runs
+class AsyncThreadsWithStreamingResponse:
+    def __init__(self, threads: AsyncThreads) -> None:
+        self._threads = threads
 
         self.create = async_to_streamed_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
-            runs.update,
-        )
-        self.list = async_to_streamed_response_wrapper(
-            runs.list,
+            threads.update,
         )
-        self.cancel = async_to_streamed_response_wrapper(
-            runs.cancel,
+        self.delete = async_to_streamed_response_wrapper(
+            threads.delete,
         )
-        self.submit_tool_outputs = async_to_streamed_response_wrapper(
-            runs.submit_tool_outputs,
+        self.create_and_run = async_to_streamed_response_wrapper(
+            threads.create_and_run,
         )
 
     @cached_property
-    def steps(self) -> AsyncStepsWithStreamingResponse:
-        return AsyncStepsWithStreamingResponse(self._runs.steps)
+    def runs(self) -> AsyncRunsWithStreamingResponse:
+        return AsyncRunsWithStreamingResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> AsyncMessagesWithStreamingResponse:
+        return AsyncMessagesWithStreamingResponse(self._threads.messages)
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/chat/__init__.py` & `openai_mealuet-1.23.4/src/openai/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/chat/chat.py` & `openai_mealuet-1.23.4/src/openai/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/chat/completions.py` & `openai_mealuet-1.23.4/src/openai/resources/chat/completions.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,24 @@
     maybe_transform,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_streamed_response_wrapper, async_to_streamed_response_wrapper
 from ..._streaming import Stream, AsyncStream
-from ...types.chat import (
-    ChatCompletion,
-    ChatCompletionChunk,
-    ChatCompletionToolParam,
-    ChatCompletionMessageParam,
-    ChatCompletionToolChoiceOptionParam,
-    completion_create_params,
-)
+from ...types.chat import completion_create_params
 from ..._base_client import (
     make_request_options,
 )
+from ...types.chat_model import ChatModel
+from ...types.chat.chat_completion import ChatCompletion
+from ...types.chat.chat_completion_chunk import ChatCompletionChunk
+from ...types.chat.chat_completion_tool_param import ChatCompletionToolParam
+from ...types.chat.chat_completion_message_param import ChatCompletionMessageParam
+from ...types.chat.chat_completion_tool_choice_option_param import ChatCompletionToolChoiceOptionParam
 
 __all__ = ["Completions", "AsyncCompletions"]
 
 
 class Completions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> CompletionsWithRawResponse:
@@ -43,36 +42,15 @@
         return CompletionsWithStreamingResponse(self)
 
     @overload
     def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
@@ -133,16 +111,15 @@
               bias is added to the logits generated by the model prior to sampling. The exact
               effect will vary per model, but values between -1 and 1 should decrease or
               increase likelihood of selection; values like -100 or 100 should result in a ban
               or exclusive selection of the relevant token.
 
           logprobs: Whether to return log probabilities of the output tokens or not. If true,
               returns the log probabilities of each output token returned in the `content` of
-              `message`. This option is currently not available on the `gpt-4-vision-preview`
-              model.
+              `message`.
 
           max_tokens: The maximum number of [tokens](/tokenizer) that can be generated in the chat
               completion.
 
               The total length of input tokens and generated tokens is limited by the model's
               context length.
               [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken)
@@ -233,36 +210,15 @@
         ...
 
     @overload
     def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         stream: Literal[True],
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
@@ -330,16 +286,15 @@
               bias is added to the logits generated by the model prior to sampling. The exact
               effect will vary per model, but values between -1 and 1 should decrease or
               increase likelihood of selection; values like -100 or 100 should result in a ban
               or exclusive selection of the relevant token.
 
           logprobs: Whether to return log probabilities of the output tokens or not. If true,
               returns the log probabilities of each output token returned in the `content` of
-              `message`. This option is currently not available on the `gpt-4-vision-preview`
-              model.
+              `message`.
 
           max_tokens: The maximum number of [tokens](/tokenizer) that can be generated in the chat
               completion.
 
               The total length of input tokens and generated tokens is limited by the model's
               context length.
               [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken)
@@ -423,36 +378,15 @@
         ...
 
     @overload
     def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         stream: bool,
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
@@ -520,16 +454,15 @@
               bias is added to the logits generated by the model prior to sampling. The exact
               effect will vary per model, but values between -1 and 1 should decrease or
               increase likelihood of selection; values like -100 or 100 should result in a ban
               or exclusive selection of the relevant token.
 
           logprobs: Whether to return log probabilities of the output tokens or not. If true,
               returns the log probabilities of each output token returned in the `content` of
-              `message`. This option is currently not available on the `gpt-4-vision-preview`
-              model.
+              `message`.
 
           max_tokens: The maximum number of [tokens](/tokenizer) that can be generated in the chat
               completion.
 
               The total length of input tokens and generated tokens is limited by the model's
               context length.
               [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken)
@@ -613,36 +546,15 @@
         ...
 
     @required_args(["messages", "model"], ["messages", "model", "stream"])
     def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
@@ -710,36 +622,15 @@
         return AsyncCompletionsWithStreamingResponse(self)
 
     @overload
     async def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
@@ -800,16 +691,15 @@
               bias is added to the logits generated by the model prior to sampling. The exact
               effect will vary per model, but values between -1 and 1 should decrease or
               increase likelihood of selection; values like -100 or 100 should result in a ban
               or exclusive selection of the relevant token.
 
           logprobs: Whether to return log probabilities of the output tokens or not. If true,
               returns the log probabilities of each output token returned in the `content` of
-              `message`. This option is currently not available on the `gpt-4-vision-preview`
-              model.
+              `message`.
 
           max_tokens: The maximum number of [tokens](/tokenizer) that can be generated in the chat
               completion.
 
               The total length of input tokens and generated tokens is limited by the model's
               context length.
               [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken)
@@ -900,36 +790,15 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         stream: Literal[True],
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
@@ -997,16 +866,15 @@
               bias is added to the logits generated by the model prior to sampling. The exact
               effect will vary per model, but values between -1 and 1 should decrease or
               increase likelihood of selection; values like -100 or 100 should result in a ban
               or exclusive selection of the relevant token.
 
           logprobs: Whether to return log probabilities of the output tokens or not. If true,
               returns the log probabilities of each output token returned in the `content` of
-              `message`. This option is currently not available on the `gpt-4-vision-preview`
-              model.
+              `message`.
 
           max_tokens: The maximum number of [tokens](/tokenizer) that can be generated in the chat
               completion.
 
               The total length of input tokens and generated tokens is limited by the model's
               context length.
               [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken)
@@ -1090,36 +958,15 @@
         ...
 
     @overload
     async def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         stream: bool,
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
@@ -1187,16 +1034,15 @@
               bias is added to the logits generated by the model prior to sampling. The exact
               effect will vary per model, but values between -1 and 1 should decrease or
               increase likelihood of selection; values like -100 or 100 should result in a ban
               or exclusive selection of the relevant token.
 
           logprobs: Whether to return log probabilities of the output tokens or not. If true,
               returns the log probabilities of each output token returned in the `content` of
-              `message`. This option is currently not available on the `gpt-4-vision-preview`
-              model.
+              `message`.
 
           max_tokens: The maximum number of [tokens](/tokenizer) that can be generated in the chat
               completion.
 
               The total length of input tokens and generated tokens is limited by the model's
               context length.
               [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken)
@@ -1280,36 +1126,15 @@
         ...
 
     @required_args(["messages", "model"], ["messages", "model", "stream"])
     async def create(
         self,
         *,
         messages: Iterable[ChatCompletionMessageParam],
-        model: Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ],
+        model: Union[str, ChatModel],
         frequency_penalty: Optional[float] | NotGiven = NOT_GIVEN,
         function_call: completion_create_params.FunctionCall | NotGiven = NOT_GIVEN,
         functions: Iterable[completion_create_params.Function] | NotGiven = NOT_GIVEN,
         logit_bias: Optional[Dict[str, int]] | NotGiven = NOT_GIVEN,
         logprobs: Optional[bool] | NotGiven = NOT_GIVEN,
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         n: Optional[int] | NotGiven = NOT_GIVEN,
```

### Comparing `openai_mealuet-1.16.2/src/openai/resources/fine_tuning/__init__.py` & `openai_mealuet-1.23.4/src/openai/resources/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/resources/fine_tuning/fine_tuning.py` & `openai_mealuet-1.23.4/src/openai/resources/fine_tuning/fine_tuning.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     AsyncJobs,
     JobsWithRawResponse,
     AsyncJobsWithRawResponse,
     JobsWithStreamingResponse,
     AsyncJobsWithStreamingResponse,
 )
 from ..._compat import cached_property
+from .jobs.jobs import Jobs, AsyncJobs
 from ..._resource import SyncAPIResource, AsyncAPIResource
 
 __all__ = ["FineTuning", "AsyncFineTuning"]
 
 
 class FineTuning(SyncAPIResource):
     @cached_property
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/__init__.py` & `openai_mealuet-1.23.4/src/openai/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
+from .batch import Batch as Batch
 from .image import Image as Image
 from .model import Model as Model
 from .shared import (
     ErrorObject as ErrorObject,
     FunctionDefinition as FunctionDefinition,
     FunctionParameters as FunctionParameters,
 )
 from .embedding import Embedding as Embedding
+from .chat_model import ChatModel as ChatModel
 from .completion import Completion as Completion
 from .moderation import Moderation as Moderation
+from .batch_error import BatchError as BatchError
 from .file_object import FileObject as FileObject
 from .file_content import FileContent as FileContent
 from .file_deleted import FileDeleted as FileDeleted
 from .model_deleted import ModelDeleted as ModelDeleted
 from .images_response import ImagesResponse as ImagesResponse
 from .completion_usage import CompletionUsage as CompletionUsage
 from .file_list_params import FileListParams as FileListParams
+from .batch_list_params import BatchListParams as BatchListParams
 from .completion_choice import CompletionChoice as CompletionChoice
 from .image_edit_params import ImageEditParams as ImageEditParams
 from .file_create_params import FileCreateParams as FileCreateParams
+from .batch_create_params import BatchCreateParams as BatchCreateParams
+from .batch_request_counts import BatchRequestCounts as BatchRequestCounts
 from .image_generate_params import ImageGenerateParams as ImageGenerateParams
 from .embedding_create_params import EmbeddingCreateParams as EmbeddingCreateParams
 from .completion_create_params import CompletionCreateParams as CompletionCreateParams
 from .moderation_create_params import ModerationCreateParams as ModerationCreateParams
 from .create_embedding_response import CreateEmbeddingResponse as CreateEmbeddingResponse
 from .moderation_create_response import ModerationCreateResponse as ModerationCreateResponse
 from .image_create_variation_params import ImageCreateVariationParams as ImageCreateVariationParams
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/completion.py` & `openai_mealuet-1.23.4/src/openai/types/completion.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/completion_choice.py` & `openai_mealuet-1.23.4/src/openai/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/completion_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/create_embedding_response.py` & `openai_mealuet-1.23.4/src/openai/types/create_embedding_response.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/embedding.py` & `openai_mealuet-1.23.4/src/openai/types/embedding.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/embedding_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/embedding_create_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/file_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/file_create_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/file_object.py` & `openai_mealuet-1.23.4/src/openai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/image.py` & `openai_mealuet-1.23.4/src/openai/types/image.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/image_create_variation_params.py` & `openai_mealuet-1.23.4/src/openai/types/image_create_variation_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/image_edit_params.py` & `openai_mealuet-1.23.4/src/openai/types/image_edit_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/image_generate_params.py` & `openai_mealuet-1.23.4/src/openai/types/image_generate_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/model.py` & `openai_mealuet-1.23.4/src/openai/types/model.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/moderation.py` & `openai_mealuet-1.23.4/src/openai/types/moderation.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/moderation_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/moderation_create_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/audio/speech_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/audio/speech_create_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/audio/transcription_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/audio/transcription_create_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/audio/translation_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/audio/translation_create_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/assistant_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/thread.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from __future__ import annotations
+from typing import List, Optional
+from typing_extensions import Literal
 
-from typing import List, Iterable, Optional
-from typing_extensions import Required, TypedDict
+from ..._models import BaseModel
 
-from .assistant_tool_param import AssistantToolParam
+__all__ = ["Thread", "ToolResources", "ToolResourcesCodeInterpreter", "ToolResourcesFileSearch"]
 
-__all__ = ["AssistantCreateParams"]
 
-
-class AssistantCreateParams(TypedDict, total=False):
-    model: Required[str]
-    """ID of the model to use.
-
-    You can use the
-    [List models](https://platform.openai.com/docs/api-reference/models/list) API to
-    see all of your available models, or see our
-    [Model overview](https://platform.openai.com/docs/models/overview) for
-    descriptions of them.
+class ToolResourcesCodeInterpreter(BaseModel):
+    file_ids: Optional[List[str]] = None
+    """
+    A list of [file](https://platform.openai.com/docs/api-reference/files) IDs made
+    available to the `code_interpreter` tool. There can be a maximum of 20 files
+    associated with the tool.
     """
 
-    description: Optional[str]
-    """The description of the assistant. The maximum length is 512 characters."""
 
-    file_ids: List[str]
+class ToolResourcesFileSearch(BaseModel):
+    vector_store_ids: Optional[List[str]] = None
     """
-    A list of [file](https://platform.openai.com/docs/api-reference/files) IDs
-    attached to this assistant. There can be a maximum of 20 files attached to the
-    assistant. Files are ordered by their creation date in ascending order.
+    The
+    [vector store](https://platform.openai.com/docs/api-reference/vector-stores/object)
+    attached to this thread. There can be a maximum of 1 vector store attached to
+    the thread.
     """
 
-    instructions: Optional[str]
-    """The system instructions that the assistant uses.
 
-    The maximum length is 32768 characters.
-    """
+class ToolResources(BaseModel):
+    code_interpreter: Optional[ToolResourcesCodeInterpreter] = None
+
+    file_search: Optional[ToolResourcesFileSearch] = None
 
-    metadata: Optional[object]
+
+class Thread(BaseModel):
+    id: str
+    """The identifier, which can be referenced in API endpoints."""
+
+    created_at: int
+    """The Unix timestamp (in seconds) for when the thread was created."""
+
+    metadata: Optional[object] = None
     """Set of 16 key-value pairs that can be attached to an object.
 
     This can be useful for storing additional information about the object in a
     structured format. Keys can be a maximum of 64 characters long and values can be
     a maxium of 512 characters long.
     """
 
-    name: Optional[str]
-    """The name of the assistant. The maximum length is 256 characters."""
+    object: Literal["thread"]
+    """The object type, which is always `thread`."""
 
-    tools: Iterable[AssistantToolParam]
-    """A list of tool enabled on the assistant.
-
-    There can be a maximum of 128 tools per assistant. Tools can be of types
-    `code_interpreter`, `retrieval`, or `function`.
+    tool_resources: Optional[ToolResources] = None
+    """
+    A set of resources that are made available to the assistant's tools in this
+    thread. The resources are specific to the type of tool. For example, the
+    `code_interpreter` tool requires a list of file IDs, while the `file_search`
+    tool requires a list of vector store IDs.
     """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/assistant_list_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/assistant_list_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/assistant_stream_event.py` & `openai_mealuet-1.23.4/src/openai/types/beta/assistant_stream_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Union
 from typing_extensions import Literal, Annotated
 
 from .thread import Thread
-from ..shared import ErrorObject
-from .threads import Run, Message, MessageDeltaEvent
 from ..._utils import PropertyInfo
 from ..._models import BaseModel
-from .threads.runs import RunStep, RunStepDeltaEvent
+from .threads.run import Run
+from .threads.message import Message
+from ..shared.error_object import ErrorObject
+from .threads.runs.run_step import RunStep
+from .threads.message_delta_event import MessageDeltaEvent
+from .threads.runs.run_step_delta_event import RunStepDeltaEvent
 
 __all__ = [
     "AssistantStreamEvent",
     "ThreadCreated",
     "ThreadRunCreated",
     "ThreadRunQueued",
     "ThreadRunInProgress",
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/thread.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/run_update_params.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from typing import Optional
-from typing_extensions import Literal
-
-from ..._models import BaseModel
+from __future__ import annotations
 
-__all__ = ["Thread"]
+from typing import Optional
+from typing_extensions import Required, TypedDict
 
+__all__ = ["RunUpdateParams"]
 
-class Thread(BaseModel):
-    id: str
-    """The identifier, which can be referenced in API endpoints."""
 
-    created_at: int
-    """The Unix timestamp (in seconds) for when the thread was created."""
+class RunUpdateParams(TypedDict, total=False):
+    thread_id: Required[str]
 
-    metadata: Optional[object] = None
+    metadata: Optional[object]
     """Set of 16 key-value pairs that can be attached to an object.
 
     This can be useful for storing additional information about the object in a
     structured format. Keys can be a maximum of 64 characters long and values can be
     a maxium of 512 characters long.
     """
-
-    object: Literal["thread"]
-    """The object type, which is always `thread`."""
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/thread_create_and_run_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/assistant.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,136 +1,126 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from __future__ import annotations
+from typing import List, Optional
+from typing_extensions import Literal
 
-from typing import List, Union, Iterable, Optional
-from typing_extensions import Literal, Required, TypedDict
+from ..._models import BaseModel
+from .assistant_tool import AssistantTool
+from .assistant_response_format_option import AssistantResponseFormatOption
 
-from .function_tool_param import FunctionToolParam
-from .retrieval_tool_param import RetrievalToolParam
-from .code_interpreter_tool_param import CodeInterpreterToolParam
-
-__all__ = [
-    "ThreadCreateAndRunParamsBase",
-    "Thread",
-    "ThreadMessage",
-    "Tool",
-    "ThreadCreateAndRunParamsNonStreaming",
-    "ThreadCreateAndRunParamsStreaming",
-]
+__all__ = ["Assistant", "ToolResources", "ToolResourcesCodeInterpreter", "ToolResourcesFileSearch"]
 
 
-class ThreadCreateAndRunParamsBase(TypedDict, total=False):
-    assistant_id: Required[str]
+class ToolResourcesCodeInterpreter(BaseModel):
+    file_ids: Optional[List[str]] = None
     """
-    The ID of the
-    [assistant](https://platform.openai.com/docs/api-reference/assistants) to use to
-    execute this run.
+    A list of [file](https://platform.openai.com/docs/api-reference/files) IDs made
+    available to the `code_interpreter`` tool. There can be a maximum of 20 files
+    associated with the tool.
     """
 
-    instructions: Optional[str]
-    """Override the default system message of the assistant.
 
-    This is useful for modifying the behavior on a per-run basis.
+class ToolResourcesFileSearch(BaseModel):
+    vector_store_ids: Optional[List[str]] = None
     """
-
-    metadata: Optional[object]
-    """Set of 16 key-value pairs that can be attached to an object.
-
-    This can be useful for storing additional information about the object in a
-    structured format. Keys can be a maximum of 64 characters long and values can be
-    a maxium of 512 characters long.
-    """
-
-    model: Optional[str]
-    """
-    The ID of the [Model](https://platform.openai.com/docs/api-reference/models) to
-    be used to execute this run. If a value is provided here, it will override the
-    model associated with the assistant. If not, the model associated with the
-    assistant will be used.
+    The ID of the
+    [vector store](https://platform.openai.com/docs/api-reference/vector-stores/object)
+    attached to this assistant. There can be a maximum of 1 vector store attached to
+    the assistant.
     """
 
-    temperature: Optional[float]
-    """What sampling temperature to use, between 0 and 2.
-
-    Higher values like 0.8 will make the output more random, while lower values like
-    0.2 will make it more focused and deterministic.
-    """
 
-    thread: Thread
-    """If no thread is provided, an empty thread will be created."""
+class ToolResources(BaseModel):
+    code_interpreter: Optional[ToolResourcesCodeInterpreter] = None
 
-    tools: Optional[Iterable[Tool]]
-    """Override the tools the assistant can use for this run.
+    file_search: Optional[ToolResourcesFileSearch] = None
 
-    This is useful for modifying the behavior on a per-run basis.
-    """
 
+class Assistant(BaseModel):
+    id: str
+    """The identifier, which can be referenced in API endpoints."""
 
-class ThreadMessage(TypedDict, total=False):
-    content: Required[str]
-    """The content of the message."""
+    created_at: int
+    """The Unix timestamp (in seconds) for when the assistant was created."""
 
-    role: Required[Literal["user", "assistant"]]
-    """The role of the entity that is creating the message. Allowed values include:
+    description: Optional[str] = None
+    """The description of the assistant. The maximum length is 512 characters."""
 
-    - `user`: Indicates the message is sent by an actual user and should be used in
-      most cases to represent user-generated messages.
-    - `assistant`: Indicates the message is generated by the assistant. Use this
-      value to insert messages from the assistant into the conversation.
-    """
+    instructions: Optional[str] = None
+    """The system instructions that the assistant uses.
 
-    file_ids: List[str]
-    """
-    A list of [File](https://platform.openai.com/docs/api-reference/files) IDs that
-    the message should use. There can be a maximum of 10 files attached to a
-    message. Useful for tools like `retrieval` and `code_interpreter` that can
-    access and use files.
+    The maximum length is 256,000 characters.
     """
 
-    metadata: Optional[object]
+    metadata: Optional[object] = None
     """Set of 16 key-value pairs that can be attached to an object.
 
     This can be useful for storing additional information about the object in a
     structured format. Keys can be a maximum of 64 characters long and values can be
     a maxium of 512 characters long.
     """
 
+    model: str
+    """ID of the model to use.
 
-class Thread(TypedDict, total=False):
-    messages: Iterable[ThreadMessage]
-    """
-    A list of [messages](https://platform.openai.com/docs/api-reference/messages) to
-    start the thread with.
+    You can use the
+    [List models](https://platform.openai.com/docs/api-reference/models/list) API to
+    see all of your available models, or see our
+    [Model overview](https://platform.openai.com/docs/models/overview) for
+    descriptions of them.
     """
 
-    metadata: Optional[object]
-    """Set of 16 key-value pairs that can be attached to an object.
+    name: Optional[str] = None
+    """The name of the assistant. The maximum length is 256 characters."""
 
-    This can be useful for storing additional information about the object in a
-    structured format. Keys can be a maximum of 64 characters long and values can be
-    a maxium of 512 characters long.
+    object: Literal["assistant"]
+    """The object type, which is always `assistant`."""
+
+    tools: List[AssistantTool]
+    """A list of tool enabled on the assistant.
+
+    There can be a maximum of 128 tools per assistant. Tools can be of types
+    `code_interpreter`, `file_search`, or `function`.
     """
 
+    response_format: Optional[AssistantResponseFormatOption] = None
+    """Specifies the format that the model must output.
 
-Tool = Union[CodeInterpreterToolParam, RetrievalToolParam, FunctionToolParam]
+    Compatible with
+    [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
+    all GPT-3.5 Turbo models since `gpt-3.5-turbo-1106`.
 
+    Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
+    message the model generates is valid JSON.
 
-class ThreadCreateAndRunParamsNonStreaming(ThreadCreateAndRunParamsBase):
-    stream: Optional[Literal[False]]
-    """
-    If `true`, returns a stream of events that happen during the Run as server-sent
-    events, terminating when the Run enters a terminal state with a `data: [DONE]`
-    message.
+    **Important:** when using JSON mode, you **must** also instruct the model to
+    produce JSON yourself via a system or user message. Without this, the model may
+    generate an unending stream of whitespace until the generation reaches the token
+    limit, resulting in a long-running and seemingly "stuck" request. Also note that
+    the message content may be partially cut off if `finish_reason="length"`, which
+    indicates the generation exceeded `max_tokens` or the conversation exceeded the
+    max context length.
     """
 
+    temperature: Optional[float] = None
+    """What sampling temperature to use, between 0 and 2.
 
-class ThreadCreateAndRunParamsStreaming(ThreadCreateAndRunParamsBase):
-    stream: Required[Literal[True]]
+    Higher values like 0.8 will make the output more random, while lower values like
+    0.2 will make it more focused and deterministic.
     """
-    If `true`, returns a stream of events that happen during the Run as server-sent
-    events, terminating when the Run enters a terminal state with a `data: [DONE]`
-    message.
+
+    tool_resources: Optional[ToolResources] = None
+    """A set of resources that are used by the assistant's tools.
+
+    The resources are specific to the type of tool. For example, the
+    `code_interpreter` tool requires a list of file IDs, while the `file_search`
+    tool requires a list of vector store IDs.
     """
 
+    top_p: Optional[float] = None
+    """
+    An alternative to sampling with temperature, called nucleus sampling, where the
+    model considers the results of the tokens with top_p probability mass. So 0.1
+    means only the tokens comprising the top 10% probability mass are considered.
 
-ThreadCreateAndRunParams = Union[ThreadCreateAndRunParamsNonStreaming, ThreadCreateAndRunParamsStreaming]
+    We generally recommend altering this or temperature but not both.
+    """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/thread_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,89 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from __future__ import annotations
+from typing import List, Union, Optional
+from typing_extensions import Literal
 
-from typing import List, Iterable, Optional
-from typing_extensions import Literal, Required, TypedDict
+from ...._models import BaseModel
+from .message_content import MessageContent
+from ..file_search_tool import FileSearchTool
+from ..code_interpreter_tool import CodeInterpreterTool
 
-__all__ = ["ThreadCreateParams", "Message"]
+__all__ = ["Message", "Attachment", "AttachmentTool", "IncompleteDetails"]
 
+AttachmentTool = Union[CodeInterpreterTool, FileSearchTool]
 
-class ThreadCreateParams(TypedDict, total=False):
-    messages: Iterable[Message]
+
+class Attachment(BaseModel):
+    file_id: Optional[str] = None
+    """The ID of the file to attach to the message."""
+
+    tools: Optional[List[AttachmentTool]] = None
+    """The tools to add this file to."""
+
+
+class IncompleteDetails(BaseModel):
+    reason: Literal["content_filter", "max_tokens", "run_cancelled", "run_expired", "run_failed"]
+    """The reason the message is incomplete."""
+
+
+class Message(BaseModel):
+    id: str
+    """The identifier, which can be referenced in API endpoints."""
+
+    assistant_id: Optional[str] = None
     """
-    A list of [messages](https://platform.openai.com/docs/api-reference/messages) to
-    start the thread with.
+    If applicable, the ID of the
+    [assistant](https://platform.openai.com/docs/api-reference/assistants) that
+    authored this message.
     """
 
-    metadata: Optional[object]
+    attachments: Optional[List[Attachment]] = None
+    """A list of files attached to the message, and the tools they were added to."""
+
+    completed_at: Optional[int] = None
+    """The Unix timestamp (in seconds) for when the message was completed."""
+
+    content: List[MessageContent]
+    """The content of the message in array of text and/or images."""
+
+    created_at: int
+    """The Unix timestamp (in seconds) for when the message was created."""
+
+    incomplete_at: Optional[int] = None
+    """The Unix timestamp (in seconds) for when the message was marked as incomplete."""
+
+    incomplete_details: Optional[IncompleteDetails] = None
+    """On an incomplete message, details about why the message is incomplete."""
+
+    metadata: Optional[object] = None
     """Set of 16 key-value pairs that can be attached to an object.
 
     This can be useful for storing additional information about the object in a
     structured format. Keys can be a maximum of 64 characters long and values can be
     a maxium of 512 characters long.
     """
 
+    object: Literal["thread.message"]
+    """The object type, which is always `thread.message`."""
 
-class Message(TypedDict, total=False):
-    content: Required[str]
-    """The content of the message."""
-
-    role: Required[Literal["user", "assistant"]]
-    """The role of the entity that is creating the message. Allowed values include:
+    role: Literal["user", "assistant"]
+    """The entity that produced the message. One of `user` or `assistant`."""
 
-    - `user`: Indicates the message is sent by an actual user and should be used in
-      most cases to represent user-generated messages.
-    - `assistant`: Indicates the message is generated by the assistant. Use this
-      value to insert messages from the assistant into the conversation.
+    run_id: Optional[str] = None
+    """
+    The ID of the [run](https://platform.openai.com/docs/api-reference/runs)
+    associated with the creation of this message. Value is `null` when messages are
+    created manually using the create message or create thread endpoints.
     """
 
-    file_ids: List[str]
+    status: Literal["in_progress", "incomplete", "completed"]
     """
-    A list of [File](https://platform.openai.com/docs/api-reference/files) IDs that
-    the message should use. There can be a maximum of 10 files attached to a
-    message. Useful for tools like `retrieval` and `code_interpreter` that can
-    access and use files.
+    The status of the message, which can be either `in_progress`, `incomplete`, or
+    `completed`.
     """
 
-    metadata: Optional[object]
-    """Set of 16 key-value pairs that can be attached to an object.
-
-    This can be useful for storing additional information about the object in a
-    structured format. Keys can be a maximum of 64 characters long and values can be
-    a maxium of 512 characters long.
+    thread_id: str
+    """
+    The [thread](https://platform.openai.com/docs/api-reference/threads) ID that
+    this message belongs to.
     """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/thread_update_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/message_update_params.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Optional
-from typing_extensions import TypedDict
+from typing_extensions import Required, TypedDict
 
-__all__ = ["ThreadUpdateParams"]
+__all__ = ["MessageUpdateParams"]
 
 
-class ThreadUpdateParams(TypedDict, total=False):
+class MessageUpdateParams(TypedDict, total=False):
+    thread_id: Required[str]
+
     metadata: Optional[object]
     """Set of 16 key-value pairs that can be attached to an object.
 
     This can be useful for storing additional information about the object in a
     structured format. Keys can be a maximum of 64 characters long and values can be
     a maxium of 512 characters long.
     """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/assistants/file_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/file_batch_create_params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
+from typing import List
 from typing_extensions import Required, TypedDict
 
-__all__ = ["FileCreateParams"]
+__all__ = ["FileBatchCreateParams"]
 
 
-class FileCreateParams(TypedDict, total=False):
-    file_id: Required[str]
+class FileBatchCreateParams(TypedDict, total=False):
+    file_ids: Required[List[str]]
     """
-    A [File](https://platform.openai.com/docs/api-reference/files) ID (with
-    `purpose="assistants"`) that the assistant should use. Useful for tools like
-    `retrieval` and `code_interpreter` that can access files.
+    A list of [File](https://platform.openai.com/docs/api-reference/files) IDs that
+    the vector store should use. Useful for tools like `file_search` that can access
+    files.
     """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/assistants/file_list_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/run_list_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing_extensions import Literal, TypedDict
 
-__all__ = ["FileListParams"]
+__all__ = ["RunListParams"]
 
 
-class FileListParams(TypedDict, total=False):
+class RunListParams(TypedDict, total=False):
     after: str
     """A cursor for use in pagination.
 
     `after` is an object ID that defines your place in the list. For instance, if
     you make a list request and receive 100 objects, ending with obj_foo, your
     subsequent call can include after=obj_foo in order to fetch the next page of the
     list.
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/__init__.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/file_citation_annotation.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/file_citation_annotation.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/file_citation_delta_annotation.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/file_citation_delta_annotation.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/file_path_annotation.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/file_path_annotation.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/file_path_delta_annotation.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/file_path_delta_annotation.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/message.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,110 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from typing import List, Optional
-from typing_extensions import Literal
+from typing import Union, Optional
+from typing_extensions import Literal, Annotated
 
-from ...._models import BaseModel
-from .message_content import MessageContent
+from ....._utils import PropertyInfo
+from ....._models import BaseModel
+from .tool_calls_step_details import ToolCallsStepDetails
+from .message_creation_step_details import MessageCreationStepDetails
 
-__all__ = ["Message", "IncompleteDetails"]
+__all__ = ["RunStep", "LastError", "StepDetails", "Usage"]
 
 
-class IncompleteDetails(BaseModel):
-    reason: Literal["content_filter", "max_tokens", "run_cancelled", "run_expired", "run_failed"]
-    """The reason the message is incomplete."""
+class LastError(BaseModel):
+    code: Literal["server_error", "rate_limit_exceeded"]
+    """One of `server_error` or `rate_limit_exceeded`."""
 
+    message: str
+    """A human-readable description of the error."""
 
-class Message(BaseModel):
+
+StepDetails = Annotated[Union[MessageCreationStepDetails, ToolCallsStepDetails], PropertyInfo(discriminator="type")]
+
+
+class Usage(BaseModel):
+    completion_tokens: int
+    """Number of completion tokens used over the course of the run step."""
+
+    prompt_tokens: int
+    """Number of prompt tokens used over the course of the run step."""
+
+    total_tokens: int
+    """Total number of tokens used (prompt + completion)."""
+
+
+class RunStep(BaseModel):
     id: str
-    """The identifier, which can be referenced in API endpoints."""
+    """The identifier of the run step, which can be referenced in API endpoints."""
 
-    assistant_id: Optional[str] = None
+    assistant_id: str
     """
-    If applicable, the ID of the
-    [assistant](https://platform.openai.com/docs/api-reference/assistants) that
-    authored this message.
+    The ID of the
+    [assistant](https://platform.openai.com/docs/api-reference/assistants)
+    associated with the run step.
     """
 
-    completed_at: Optional[int] = None
-    """The Unix timestamp (in seconds) for when the message was completed."""
+    cancelled_at: Optional[int] = None
+    """The Unix timestamp (in seconds) for when the run step was cancelled."""
 
-    content: List[MessageContent]
-    """The content of the message in array of text and/or images."""
+    completed_at: Optional[int] = None
+    """The Unix timestamp (in seconds) for when the run step completed."""
 
     created_at: int
-    """The Unix timestamp (in seconds) for when the message was created."""
+    """The Unix timestamp (in seconds) for when the run step was created."""
 
-    file_ids: List[str]
-    """
-    A list of [file](https://platform.openai.com/docs/api-reference/files) IDs that
-    the assistant should use. Useful for tools like retrieval and code_interpreter
-    that can access files. A maximum of 10 files can be attached to a message.
+    expired_at: Optional[int] = None
+    """The Unix timestamp (in seconds) for when the run step expired.
+
+    A step is considered expired if the parent run is expired.
     """
 
-    incomplete_at: Optional[int] = None
-    """The Unix timestamp (in seconds) for when the message was marked as incomplete."""
+    failed_at: Optional[int] = None
+    """The Unix timestamp (in seconds) for when the run step failed."""
+
+    last_error: Optional[LastError] = None
+    """The last error associated with this run step.
 
-    incomplete_details: Optional[IncompleteDetails] = None
-    """On an incomplete message, details about why the message is incomplete."""
+    Will be `null` if there are no errors.
+    """
 
     metadata: Optional[object] = None
     """Set of 16 key-value pairs that can be attached to an object.
 
     This can be useful for storing additional information about the object in a
     structured format. Keys can be a maximum of 64 characters long and values can be
     a maxium of 512 characters long.
     """
 
-    object: Literal["thread.message"]
-    """The object type, which is always `thread.message`."""
+    object: Literal["thread.run.step"]
+    """The object type, which is always `thread.run.step`."""
 
-    role: Literal["user", "assistant"]
-    """The entity that produced the message. One of `user` or `assistant`."""
-
-    run_id: Optional[str] = None
+    run_id: str
     """
-    The ID of the [run](https://platform.openai.com/docs/api-reference/runs)
-    associated with the creation of this message. Value is `null` when messages are
-    created manually using the create message or create thread endpoints.
+    The ID of the [run](https://platform.openai.com/docs/api-reference/runs) that
+    this run step is a part of.
     """
 
-    status: Literal["in_progress", "incomplete", "completed"]
+    status: Literal["in_progress", "cancelled", "failed", "completed", "expired"]
     """
-    The status of the message, which can be either `in_progress`, `incomplete`, or
-    `completed`.
+    The status of the run step, which can be either `in_progress`, `cancelled`,
+    `failed`, `completed`, or `expired`.
     """
 
+    step_details: StepDetails
+    """The details of the run step."""
+
     thread_id: str
     """
-    The [thread](https://platform.openai.com/docs/api-reference/threads) ID that
-    this message belongs to.
+    The ID of the [thread](https://platform.openai.com/docs/api-reference/threads)
+    that was run.
+    """
+
+    type: Literal["message_creation", "tool_calls"]
+    """The type of run step, which can be either `message_creation` or `tool_calls`."""
+
+    usage: Optional[Usage] = None
+    """Usage statistics related to the run step.
+
+    This value will be `null` while the run step's status is `in_progress`.
     """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/message_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/message_create_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import Union, Iterable, Optional
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["MessageCreateParams"]
+from ..file_search_tool_param import FileSearchToolParam
+from ..code_interpreter_tool_param import CodeInterpreterToolParam
+
+__all__ = ["MessageCreateParams", "Attachment", "AttachmentTool"]
 
 
 class MessageCreateParams(TypedDict, total=False):
     content: Required[str]
     """The content of the message."""
 
     role: Required[Literal["user", "assistant"]]
@@ -17,22 +20,28 @@
 
     - `user`: Indicates the message is sent by an actual user and should be used in
       most cases to represent user-generated messages.
     - `assistant`: Indicates the message is generated by the assistant. Use this
       value to insert messages from the assistant into the conversation.
     """
 
-    file_ids: List[str]
-    """
-    A list of [File](https://platform.openai.com/docs/api-reference/files) IDs that
-    the message should use. There can be a maximum of 10 files attached to a
-    message. Useful for tools like `retrieval` and `code_interpreter` that can
-    access and use files.
-    """
+    attachments: Optional[Iterable[Attachment]]
+    """A list of files attached to the message, and the tools they should be added to."""
 
     metadata: Optional[object]
     """Set of 16 key-value pairs that can be attached to an object.
 
     This can be useful for storing additional information about the object in a
     structured format. Keys can be a maximum of 64 characters long and values can be
     a maxium of 512 characters long.
     """
+
+
+AttachmentTool = Union[CodeInterpreterToolParam, FileSearchToolParam]
+
+
+class Attachment(TypedDict, total=False):
+    file_id: str
+    """The ID of the file to attach to the message."""
+
+    tools: Iterable[AttachmentTool]
+    """The tools to add this file to."""
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/message_delta_event.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/message_delta_event.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/message_list_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/message_list_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/required_action_function_tool_call.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/required_action_function_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/run_list_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/vector_store_list_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing_extensions import Literal, TypedDict
 
-__all__ = ["RunListParams"]
+__all__ = ["VectorStoreListParams"]
 
 
-class RunListParams(TypedDict, total=False):
+class VectorStoreListParams(TypedDict, total=False):
     after: str
     """A cursor for use in pagination.
 
     `after` is an object ID that defines your place in the list. For instance, if
     you make a list request and receive 100 objects, ending with obj_foo, your
     subsequent call can include after=obj_foo in order to fetch the next page of the
     list.
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/run_submit_tool_outputs_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/run_submit_tool_outputs_params.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/run_update_params.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_function_message_param.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Optional
-from typing_extensions import Required, TypedDict
+from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["RunUpdateParams"]
+__all__ = ["ChatCompletionFunctionMessageParam"]
 
 
-class RunUpdateParams(TypedDict, total=False):
-    thread_id: Required[str]
+class ChatCompletionFunctionMessageParam(TypedDict, total=False):
+    content: Required[Optional[str]]
+    """The contents of the function message."""
 
-    metadata: Optional[object]
-    """Set of 16 key-value pairs that can be attached to an object.
+    name: Required[str]
+    """The name of the function to call."""
 
-    This can be useful for storing additional information about the object in a
-    structured format. Keys can be a maximum of 64 characters long and values can be
-    a maxium of 512 characters long.
-    """
+    role: Required[Literal["function"]]
+    """The role of the messages author, in this case `function`."""
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/messages/file_list_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/step_list_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["FileListParams"]
+__all__ = ["StepListParams"]
 
 
-class FileListParams(TypedDict, total=False):
+class StepListParams(TypedDict, total=False):
     thread_id: Required[str]
 
     after: str
     """A cursor for use in pagination.
 
     `after` is an object ID that defines your place in the list. For instance, if
     you make a list request and receive 100 objects, ending with obj_foo, your
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/__init__.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from .run_step import RunStep as RunStep
 from .tool_call import ToolCall as ToolCall
 from .run_step_delta import RunStepDelta as RunStepDelta
 from .tool_call_delta import ToolCallDelta as ToolCallDelta
 from .step_list_params import StepListParams as StepListParams
 from .function_tool_call import FunctionToolCall as FunctionToolCall
-from .retrieval_tool_call import RetrievalToolCall as RetrievalToolCall
 from .run_step_delta_event import RunStepDeltaEvent as RunStepDeltaEvent
 from .code_interpreter_logs import CodeInterpreterLogs as CodeInterpreterLogs
+from .file_search_tool_call import FileSearchToolCall as FileSearchToolCall
 from .tool_call_delta_object import ToolCallDeltaObject as ToolCallDeltaObject
 from .tool_calls_step_details import ToolCallsStepDetails as ToolCallsStepDetails
 from .function_tool_call_delta import FunctionToolCallDelta as FunctionToolCallDelta
-from .retrieval_tool_call_delta import RetrievalToolCallDelta as RetrievalToolCallDelta
 from .code_interpreter_tool_call import CodeInterpreterToolCall as CodeInterpreterToolCall
+from .file_search_tool_call_delta import FileSearchToolCallDelta as FileSearchToolCallDelta
 from .run_step_delta_message_delta import RunStepDeltaMessageDelta as RunStepDeltaMessageDelta
 from .code_interpreter_output_image import CodeInterpreterOutputImage as CodeInterpreterOutputImage
 from .message_creation_step_details import MessageCreationStepDetails as MessageCreationStepDetails
 from .code_interpreter_tool_call_delta import CodeInterpreterToolCallDelta as CodeInterpreterToolCallDelta
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/code_interpreter_output_image.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/code_interpreter_output_image.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/code_interpreter_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/code_interpreter_tool_call_delta.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/function_tool_call.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/function_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/function_tool_call_delta.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/function_tool_call_delta.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/run_step_delta.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step_delta.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/run_step_delta_event.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step_delta_event.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/run_step_delta_message_delta.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/run_step_delta_message_delta.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/step_list_params.py` & `openai_mealuet-1.23.4/src/openai/types/beta/vector_stores/file_batch_list_files_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["StepListParams"]
+__all__ = ["FileBatchListFilesParams"]
 
 
-class StepListParams(TypedDict, total=False):
-    thread_id: Required[str]
+class FileBatchListFilesParams(TypedDict, total=False):
+    vector_store_id: Required[str]
 
     after: str
     """A cursor for use in pagination.
 
     `after` is an object ID that defines your place in the list. For instance, if
     you make a list request and receive 100 objects, ending with obj_foo, your
     subsequent call can include after=obj_foo in order to fetch the next page of the
@@ -24,14 +24,20 @@
 
     `before` is an object ID that defines your place in the list. For instance, if
     you make a list request and receive 100 objects, ending with obj_foo, your
     subsequent call can include before=obj_foo in order to fetch the previous page
     of the list.
     """
 
+    filter: Literal["in_progress", "completed", "failed", "cancelled"]
+    """Filter by file status.
+
+    One of `in_progress`, `completed`, `failed`, `cancelled`.
+    """
+
     limit: int
     """A limit on the number of objects to be returned.
 
     Limit can range between 1 and 100, and the default is 20.
     """
 
     order: Literal["asc", "desc"]
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/tool_call_delta.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/tool_call_delta.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Union
 from typing_extensions import Annotated
 
 from ....._utils import PropertyInfo
 from .function_tool_call_delta import FunctionToolCallDelta
-from .retrieval_tool_call_delta import RetrievalToolCallDelta
+from .file_search_tool_call_delta import FileSearchToolCallDelta
 from .code_interpreter_tool_call_delta import CodeInterpreterToolCallDelta
 
 __all__ = ["ToolCallDelta"]
 
 ToolCallDelta = Annotated[
-    Union[CodeInterpreterToolCallDelta, RetrievalToolCallDelta, FunctionToolCallDelta],
+    Union[CodeInterpreterToolCallDelta, FileSearchToolCallDelta, FunctionToolCallDelta],
     PropertyInfo(discriminator="type"),
 ]
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/tool_call_delta_object.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/tool_call_delta_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     type: Literal["tool_calls"]
     """Always `tool_calls`."""
 
     tool_calls: Optional[List[ToolCallDelta]] = None
     """An array of tool calls the run step was involved in.
 
     These can be associated with one of three types of tools: `code_interpreter`,
-    `retrieval`, or `function`.
+    `file_search`, or `function`.
     """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/beta/threads/runs/tool_calls_step_details.py` & `openai_mealuet-1.23.4/src/openai/types/beta/threads/runs/tool_calls_step_details.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 
 class ToolCallsStepDetails(BaseModel):
     tool_calls: List[ToolCall]
     """An array of tool calls the run step was involved in.
 
     These can be associated with one of three types of tools: `code_interpreter`,
-    `retrieval`, or `function`.
+    `file_search`, or `function`.
     """
 
     type: Literal["tool_calls"]
     """Always `tool_calls`."""
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/__init__.py` & `openai_mealuet-1.23.4/src/openai/types/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_assistant_message_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_assistant_message_param.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_chunk.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_content_part_image_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_content_part_image_param.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_function_message_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_system_message_param.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Optional
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["ChatCompletionFunctionMessageParam"]
+__all__ = ["ChatCompletionSystemMessageParam"]
 
 
-class ChatCompletionFunctionMessageParam(TypedDict, total=False):
-    content: Required[Optional[str]]
-    """The contents of the function message."""
+class ChatCompletionSystemMessageParam(TypedDict, total=False):
+    content: Required[str]
+    """The contents of the system message."""
 
-    name: Required[str]
-    """The name of the function to call."""
+    role: Required[Literal["system"]]
+    """The role of the messages author, in this case `system`."""
 
-    role: Required[Literal["function"]]
-    """The role of the messages author, in this case `function`."""
+    name: str
+    """An optional name for the participant.
+
+    Provides the model information to differentiate between participants of the same
+    role.
+    """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message_param.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message_tool_call.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_message_tool_call_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_message_tool_call_param.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_named_tool_choice_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_named_tool_choice_param.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_system_message_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_user_message_param.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
+from typing import Union, Iterable
 from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["ChatCompletionSystemMessageParam"]
+from .chat_completion_content_part_param import ChatCompletionContentPartParam
 
+__all__ = ["ChatCompletionUserMessageParam"]
 
-class ChatCompletionSystemMessageParam(TypedDict, total=False):
-    content: Required[str]
-    """The contents of the system message."""
 
-    role: Required[Literal["system"]]
-    """The role of the messages author, in this case `system`."""
+class ChatCompletionUserMessageParam(TypedDict, total=False):
+    content: Required[Union[str, Iterable[ChatCompletionContentPartParam]]]
+    """The contents of the user message."""
+
+    role: Required[Literal["user"]]
+    """The role of the messages author, in this case `user`."""
 
     name: str
     """An optional name for the participant.
 
     Provides the model information to differentiate between participants of the same
     role.
     """
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_token_logprob.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_token_logprob.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/chat_completion_tool_message_param.py` & `openai_mealuet-1.23.4/src/openai/types/chat/chat_completion_tool_message_param.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/chat/completion_create_params.py` & `openai_mealuet-1.23.4/src/openai/types/chat/completion_create_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Dict, List, Union, Iterable, Optional
 from typing_extensions import Literal, Required, TypedDict
 
 from ...types import shared_params
+from ..chat_model import ChatModel
 from .chat_completion_tool_param import ChatCompletionToolParam
 from .chat_completion_message_param import ChatCompletionMessageParam
 from .chat_completion_tool_choice_option_param import ChatCompletionToolChoiceOptionParam
 from .chat_completion_function_call_option_param import ChatCompletionFunctionCallOptionParam
 
 __all__ = [
     "CompletionCreateParamsBase",
@@ -24,38 +25,15 @@
 class CompletionCreateParamsBase(TypedDict, total=False):
     messages: Required[Iterable[ChatCompletionMessageParam]]
     """A list of messages comprising the conversation so far.
 
     [Example Python code](https://cookbook.openai.com/examples/how_to_format_inputs_to_chatgpt_models).
     """
 
-    model: Required[
-        Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ]
-    ]
+    model: Required[Union[str, ChatModel]]
     """ID of the model to use.
 
     See the
     [model endpoint compatibility](https://platform.openai.com/docs/models/model-endpoint-compatibility)
     table for details on which models work with the Chat API.
     """
 
@@ -98,16 +76,15 @@
     or exclusive selection of the relevant token.
     """
 
     logprobs: Optional[bool]
     """Whether to return log probabilities of the output tokens or not.
 
     If true, returns the log probabilities of each output token returned in the
-    `content` of `message`. This option is currently not available on the
-    `gpt-4-vision-preview` model.
+    `content` of `message`.
     """
 
     max_tokens: Optional[int]
     """
     The maximum number of [tokens](/tokenizer) that can be generated in the chat
     completion.
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/fine_tuning/fine_tuning_job.py` & `openai_mealuet-1.23.4/src/openai/types/fine_tuning/fine_tuning_job.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import List, Union, Optional
 from typing_extensions import Literal
 
 from ..._models import BaseModel
+from .fine_tuning_job_wandb_integration_object import FineTuningJobWandbIntegrationObject
 
 __all__ = ["FineTuningJob", "Error", "Hyperparameters"]
 
 
 class Error(BaseModel):
     code: str
     """A machine-readable error code."""
@@ -76,14 +77,17 @@
     result_files: List[str]
     """The compiled results file ID(s) for the fine-tuning job.
 
     You can retrieve the results with the
     [Files API](https://platform.openai.com/docs/api-reference/files/retrieve-contents).
     """
 
+    seed: int
+    """The seed used for the fine-tuning job."""
+
     status: Literal["validating_files", "queued", "running", "succeeded", "failed", "cancelled"]
     """
     The current status of the fine-tuning job, which can be either
     `validating_files`, `queued`, `running`, `succeeded`, `failed`, or `cancelled`.
     """
 
     trained_tokens: Optional[int] = None
@@ -101,7 +105,10 @@
 
     validation_file: Optional[str] = None
     """The file ID used for validation.
 
     You can retrieve the validation results with the
     [Files API](https://platform.openai.com/docs/api-reference/files/retrieve-contents).
     """
+
+    integrations: Optional[List[FineTuningJobWandbIntegrationObject]] = None
+    """A list of integrations to enable for this fine-tuning job."""
```

### Comparing `openai_mealuet-1.16.2/src/openai/types/shared/function_definition.py` & `openai_mealuet-1.23.4/src/openai/types/shared/function_definition.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/src/openai/types/shared_params/function_definition.py` & `openai_mealuet-1.23.4/src/openai/types/shared_params/function_definition.py`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/LICENSE` & `openai_mealuet-1.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_mealuet-1.16.2/pyproject.toml` & `openai_mealuet-1.23.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai-mealuet"
-version = "1.16.2"
+version = "1.23.4"
 description = "Python library of OpenAI API proxied by mealuet"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "OpenAI", email = "support@openai.com" },
 { name = "Zack Zhu", email = "kressety@outlook.com" }
 ]
@@ -37,16 +37,16 @@
   "License :: OSI Approved :: Apache Software License"
 ]
 
 [project.optional-dependencies]
 datalib = ["numpy >= 1", "pandas >= 1.2.3", "pandas-stubs >= 1.1.0.11"]
 
 [project.urls]
-Homepage = "https://github.com/kressety/openai-python-mealuet"
-Repository = "https://github.com/kressety/openai-python-mealuet"
+Homepage = "https://github.com/openai/openai-python"
+Repository = "https://github.com/openai/openai-python"
 
 [project.scripts]
 openai = "openai.cli:main"
 
 [tool.rye]
 managed = true
 # version pins are in requirements-dev.lock
@@ -110,15 +110,15 @@
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 # replace relative links with absolute links
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
-replacement = '[\1](https://github.com/kressety/openai-python-mealuet/tree/main/\g<2>)'
+replacement = '[\1](https://github.com/openai/openai-python/tree/main/\g<2>)'
 
 [tool.black]
 line-length = 120
 target-version = ["py37"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `openai_mealuet-1.16.2/PKG-INFO` & `openai_mealuet-1.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: openai-mealuet
-Version: 1.16.2
+Version: 1.23.4
 Summary: Python library of OpenAI API proxied by mealuet
-Project-URL: Homepage, https://github.com/kressety/openai-python-mealuet
-Project-URL: Repository, https://github.com/kressety/openai-python-mealuet
+Project-URL: Homepage, https://github.com/openai/openai-python
+Project-URL: Repository, https://github.com/openai/openai-python
 Author-email: OpenAI <support@openai.com>, Zack Zhu <kressety@outlook.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -52,29 +52,29 @@
 
 The `base_url` of original lib has been redirected to `openai-proxy.mealuet.com` in order to access OpenAI service in some unsupported areas. 
 
 NOTE: this kind of proxy is for personal use, so availability is NOT guaranteed all the time!
 
 ## Documentation
 
-The REST API documentation can be found [on platform.openai.com](https://platform.openai.com/docs). The full API of this library can be found in [api.md](https://github.com/kressety/openai-python-mealuet/tree/main/api.md).
+The REST API documentation can be found [on platform.openai.com](https://platform.openai.com/docs). The full API of this library can be found in [api.md](https://github.com/openai/openai-python/tree/main/api.md).
 
 ## Installation
 
 > [!IMPORTANT]
 > The SDK was rewritten in v1, which was released November 6th 2023. See the [v1 migration guide](https://github.com/openai/openai-python/discussions/742), which includes scripts to automatically update your code.
 
 ```sh
 # install from PyPI
 pip install openai-mealuet
 ```
 
 ## Usage
 
-The full API of this library can be found in [api.md](https://github.com/kressety/openai-python-mealuet/tree/main/api.md).
+The full API of this library can be found in [api.md](https://github.com/openai/openai-python/tree/main/api.md).
 
 ```python
 import os
 from openai import OpenAI
 
 client = OpenAI(
     # This is the default and can be omitted
@@ -95,15 +95,15 @@
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `OPENAI_API_KEY="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
 ### Polling Helpers
 
-When interacting with the API some actions such as starting a Run may take time to complete. The SDK includes
+When interacting with the API some actions such as starting a Run and adding files to vector stores are asynchronous and take time to complete. The SDK includes
 helper functions which will poll the status until it reaches a terminal state and then return the resulting object.
 If an API method results in an action which could benefit from polling there will be a corresponding version of the
 method ending in '\_and_poll'.
 
 For instance to create a Run and poll until it reaches a terminal state you can run:
 
 ```python
@@ -111,14 +111,28 @@
     thread_id=thread.id,
     assistant_id=assistant.id,
 )
 ```
 
 More information on the lifecycle of a Run can be found in the [Run Lifecycle Documentation](https://platform.openai.com/docs/assistants/how-it-works/run-lifecycle)
 
+### Bulk Upload Helpers
+
+When creating an interacting with vector stores, you can use the polling helpers to monitor the status of operations.
+For convenience, we also provide a bulk upload helper to allow you to simultaneously upload several files at once.
+
+```python
+sample_files = [Path("sample-paper.pdf"), ...]
+
+batch = await client.vector_stores.file_batches.upload_and_poll(
+    store.id,
+    files=sample_files,
+)
+```
+
 ### Streaming Helpers
 
 The SDK also includes helpers to process streams and handle the incoming events.
 
 ```python
 with client.beta.threads.runs.stream(
     thread_id=thread.id,
@@ -127,15 +141,15 @@
 ) as stream:
     for event in stream:
         # Print the text from text delta events
         if event.type == "thread.message.delta" and event.data.delta.content:
             print(event.data.delta.content[0].text)
 ```
 
-More information on streaming helpers can be found in the dedicated documentation: [helpers.md](https://github.com/kressety/openai-python-mealuet/tree/main/helpers.md)
+More information on streaming helpers can be found in the dedicated documentation: [helpers.md](https://github.com/openai/openai-python/tree/main/helpers.md)
 
 ## Async usage
 
 Simply import `AsyncOpenAI` instead of `OpenAI` and use `await` with each API call:
 
 ```python
 import os
@@ -242,18 +256,18 @@
 - It can be difficult to reason about where client options are configured
 - It's not possible to change certain client options without potentially causing race conditions
 - It's harder to mock for testing purposes
 - It's not possible to control cleanup of network connections
 
 ## Using types
 
-Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev), which provide helper methods for things like:
+Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev) which also provide helper methods for things like:
 
-- Serializing back into JSON, `model.model_dump_json(indent=2, exclude_unset=True)`
-- Converting to a dictionary, `model.model_dump(exclude_unset=True)`
+- Serializing back into JSON, `model.to_json()`
+- Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Pagination
 
 List methods in the OpenAI API are paginated.
 
@@ -465,15 +479,15 @@
     ],
     model="gpt-3.5-turbo",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
-Note that requests that time out are [retried twice by default](https://github.com/kressety/openai-python-mealuet/tree/main/#retries).
+Note that requests that time out are [retried twice by default](https://github.com/openai/openai-python/tree/main/#retries).
 
 ## Advanced
 
 ### Logging
 
 We use the standard library [`logging`](https://docs.python.org/3/library/logging.html) module.
 
@@ -549,15 +563,15 @@
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
 
 ### Making custom/undocumented requests
 
-This library is typed for convenient access the documented API.
+This library is typed for convenient access to the documented API.
 
 If you need to access undocumented endpoints, params, or response properties, the library can still be used.
 
 #### Undocumented endpoints
 
 To make requests to undocumented endpoints, you can make requests using `client.get`, `client.post`, and other
 http verbs. Options on the client will be respected (such as retries) will be respected when making this
@@ -591,21 +605,20 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-import httpx
-from openai import OpenAI
+from openai import OpenAI, DefaultHttpxClient
 
 client = OpenAI(
     # Or use the `OPENAI_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
-    http_client=httpx.Client(
+    http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
 )
 ```
 
 ### Managing HTTP resources
@@ -637,15 +650,15 @@
     messages=[
         {
             "role": "user",
             "content": "How do I output all files in a directory using Python?",
         },
     ],
 )
-print(completion.model_dump_json(indent=2))
+print(completion.to_json())
 ```
 
 In addition to the options provided in the base `OpenAI` client, the following options are provided:
 
 - `azure_endpoint` (or the `AZURE_OPENAI_ENDPOINT` environment variable)
 - `azure_deployment`
 - `api_version` (or the `OPENAI_API_VERSION` environment variable)
```


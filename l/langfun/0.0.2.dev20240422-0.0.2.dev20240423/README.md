# Comparing `tmp/langfun-0.0.2.dev20240422.tar.gz` & `tmp/langfun-0.0.2.dev20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240422.tar", last modified: Mon Apr 22 08:03:53 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240423.tar", last modified: Tue Apr 23 08:03:39 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240422.tar` & `langfun-0.0.2.dev20240423.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.088337 langfun-0.0.2.dev20240422/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-22 08:03:53.088337 langfun-0.0.2.dev20240422/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.068336 langfun-0.0.2.dev20240422/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.076336 langfun-0.0.2.dev20240422/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.076336 langfun-0.0.2.dev20240422/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.076336 langfun-0.0.2.dev20240422/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.076336 langfun-0.0.2.dev20240422/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.080336 langfun-0.0.2.dev20240422/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.080336 langfun-0.0.2.dev20240422/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.080336 langfun-0.0.2.dev20240422/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.084336 langfun-0.0.2.dev20240422/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.084336 langfun-0.0.2.dev20240422/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.088337 langfun-0.0.2.dev20240422/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:53.088337 langfun-0.0.2.dev20240422/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-22 08:03:53.000000 langfun-0.0.2.dev20240422/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-22 08:03:53.000000 langfun-0.0.2.dev20240422/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:03:53.000000 langfun-0.0.2.dev20240422/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-22 08:03:53.000000 langfun-0.0.2.dev20240422/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:03:53.000000 langfun-0.0.2.dev20240422/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:03:53.088337 langfun-0.0.2.dev20240422/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-22 08:03:34.000000 langfun-0.0.2.dev20240422/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.105427 langfun-0.0.2.dev20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-23 08:03:39.105427 langfun-0.0.2.dev20240423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.085427 langfun-0.0.2.dev20240423/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.089427 langfun-0.0.2.dev20240423/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.089427 langfun-0.0.2.dev20240423/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.093427 langfun-0.0.2.dev20240423/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.093427 langfun-0.0.2.dev20240423/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.097427 langfun-0.0.2.dev20240423/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.097427 langfun-0.0.2.dev20240423/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.097427 langfun-0.0.2.dev20240423/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.097427 langfun-0.0.2.dev20240423/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.101427 langfun-0.0.2.dev20240423/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18447 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.105427 langfun-0.0.2.dev20240423/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:03:39.105427 langfun-0.0.2.dev20240423/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-23 08:03:39.000000 langfun-0.0.2.dev20240423/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-23 08:03:39.000000 langfun-0.0.2.dev20240423/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:03:39.000000 langfun-0.0.2.dev20240423/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 08:03:39.000000 langfun-0.0.2.dev20240423/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:03:39.000000 langfun-0.0.2.dev20240423/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:03:39.105427 langfun-0.0.2.dev20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-23 08:03:14.000000 langfun-0.0.2.dev20240423/setup.py
```

### Comparing `langfun-0.0.2.dev20240422/LICENSE` & `langfun-0.0.2.dev20240423/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/PKG-INFO` & `langfun-0.0.2.dev20240423/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240422
+Version: 0.0.2.dev20240423
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240422/README.md` & `langfun-0.0.2.dev20240423/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/__init__.py` & `langfun-0.0.2.dev20240423/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240423/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/component.py` & `langfun-0.0.2.dev20240423/langfun/core/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,20 @@
 
 
 def get_contextual_override(var_name: str) -> ContextualOverride | None:
   """Returns the overriden contextual value in current scope."""
   return _get_scoped_value(_global_tls, _CONTEXT_OVERRIDES, var_name)
 
 
+def all_contextual_values() -> dict[str, Any]:
+  """Returns all contextual values provided from `lf.context` in scope."""
+  overrides = getattr(_global_tls, _CONTEXT_OVERRIDES, {})
+  return {k: v.value for k, v in overrides.items()}
+
+
 @contextlib.contextmanager
 def _contextual_scope(
     tls: threading.local, tls_key, **variables
 ) -> Iterator[dict[str, ContextualOverride]]:
   """Context manager to set variables within a scope."""
   previous_values = getattr(tls, tls_key, {})
   current_values = dict(previous_values)
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/component_test.py` & `langfun-0.0.2.dev20240423/langfun/core/component_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
               z=lf.ContextualOverride(3, cascade=False, override_attrs=False),
           ),
       )
       self.assertEqual(
           lf.get_contextual_override('y'),
           lf.ContextualOverride(3, cascade=False, override_attrs=False),
       )
+      self.assertEqual(lf.all_contextual_values(), dict(x=3, y=3, z=3))
 
       # Member attributes take precedence over `lf.context`.
       self.assertEqual(a1.x, 1)
       self.assertEqual(a1.y, 2)
 
       # Override attributes take precedence over member attribute.
       with a1.override(y=3):
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240423/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240423/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/console.py` & `langfun-0.0.2.dev20240423/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/console_test.py` & `langfun-0.0.2.dev20240423/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240423/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240423/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240423/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240423/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240423/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240423/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240423/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240423/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/language_model.py` & `langfun-0.0.2.dev20240423/langfun/core/language_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from typing import Annotated, Any, Callable, Sequence, Tuple, Type, Union
 from langfun.core import component
 from langfun.core import concurrent
 from langfun.core import console
 from langfun.core import message as message_lib
 import pyglove as pg
 
+TOKENS_PER_REQUEST = 250  # Estimated num tokens for a single request
+DEFAULT_MAX_CONCURRENCY = 1  # Use this as max concurrency if no RPM or TPM data
+
 
 class LMSample(pg.Object):
   """Response candidate."""
 
   response: pg.typing.Annotated[
       pg.typing.Object(
           message_lib.Message,
@@ -600,7 +603,18 @@
             title=f'COMPLETION #{i}',
             color='green',
         )
         console.write(
             f'score: {r.score}',
             color='blue',
         )
+
+  def rate_to_max_concurrency(
+      self, requests_per_min: float = 0, tokens_per_min: float = 0
+  ) -> int:
+    """Converts a rate to a max concurrency."""
+    if tokens_per_min > 0:
+      return max(int(tokens_per_min / TOKENS_PER_REQUEST / 60), 1)
+    elif requests_per_min > 0:
+      return max(int(requests_per_min / 60), 1)  # Max concurrency can't be zero
+    else:
+      return DEFAULT_MAX_CONCURRENCY  # Default of 1
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240423/langfun/core/language_model_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -390,10 +390,42 @@
       if debug_mode & lm_lib.LMDebugMode.PROMPT:
         self.assertIn('[0] MODALITY OBJECTS SENT TO LM', debug_info)
 
   def test_score_with_unsupported_model(self):
     with self.assertRaises(NotImplementedError):
       MockModel().score('hi', ['1', '2'])
 
+  def test_rate_to_max_concurrency_no_rpm_no_tpm(self) -> None:
+    lm = MockModel()
+    self.assertEqual(
+        lm_lib.DEFAULT_MAX_CONCURRENCY,
+        lm.rate_to_max_concurrency(requests_per_min=0, tokens_per_min=0),
+    )
+    self.assertEqual(
+        lm_lib.DEFAULT_MAX_CONCURRENCY,
+        lm.rate_to_max_concurrency(requests_per_min=-1, tokens_per_min=-1),
+    )
+
+  def test_rate_to_max_concurrency_only_rpm_specified_uses_rpm(self) -> None:
+    lm = MockModel()
+    test_rpm = 1e4
+    self.assertEqual(
+        lm.rate_to_max_concurrency(requests_per_min=test_rpm),
+        int(test_rpm / 60)
+    )
+
+  def test_rate_to_max_concurrency_tpm_specified_uses_tpm(self) -> None:
+    lm = MockModel()
+    test_tpm = 1e7
+    self.assertEqual(
+        lm.rate_to_max_concurrency(requests_per_min=1, tokens_per_min=test_tpm),
+        int(test_tpm / lm_lib.TOKENS_PER_REQUEST / 60),
+    )
+
+  def test_rate_to_max_concurrency_small_rate_returns_one(self) -> None:
+    lm = MockModel()
+    self.assertEqual(lm.rate_to_max_concurrency(requests_per_min=1), 1)
+    self.assertEqual(lm.rate_to_max_concurrency(tokens_per_min=1), 1)
+
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 from langfun.core import modalities as lf_modalities
 import pyglove as pg
 import requests
 
 
 SUPPORTED_MODELS_AND_SETTINGS = {
     # See https://docs.anthropic.com/claude/docs/models-overview
-    'claude-3-opus-20240229': pg.Dict(max_tokens=4096, max_concurrency=16),
-    'claude-3-sonnet-20240229': pg.Dict(max_tokens=4096, max_concurrency=16),
-    'claude-3-haiku-20240307': pg.Dict(max_tokens=4096, max_concurrency=16),
-    'claude-2.1': pg.Dict(max_tokens=4096, max_concurrency=16),
-    'claude-2.0': pg.Dict(max_tokens=4096, max_concurrency=16),
-    'claude-instant-1.2': pg.Dict(max_tokens=4096, max_concurrency=16),
+    # Rate limits from https://docs.anthropic.com/claude/reference/rate-limits
+    #     RPM/TPM for Claude-2.1, Claude-2.0, and Claude-Instant-1.2 estimated
+    #     as RPM/TPM of the largest-available model (Claude-3-Opus).
+    'claude-3-opus-20240229': pg.Dict(max_tokens=4096, rpm=4000, tpm=400000),
+    'claude-3-sonnet-20240229': pg.Dict(max_tokens=4096, rpm=4000, tpm=400000),
+    'claude-3-haiku-20240307': pg.Dict(max_tokens=4096, rpm=4000, tpm=400000),
+    'claude-2.1': pg.Dict(max_tokens=4096, rpm=4000, tpm=400000),
+    'claude-2.0': pg.Dict(max_tokens=4096, rpm=4000, tpm=400000),
+    'claude-instant-1.2': pg.Dict(max_tokens=4096, rpm=4000, tpm=400000),
 }
 
 
 class AnthropicError(Exception):  # pylint: disable=g-bad-exception-name
   """Base class for Anthropic errors."""
 
 
@@ -77,34 +80,50 @@
       ),
   ] = None
 
   def _on_bound(self):
     super()._on_bound()
     self._api_key = None
     self.__dict__.pop('_api_initialized', None)
+    self.__dict__.pop('_session', None)
 
   @functools.cached_property
   def _api_initialized(self):
     api_key = self.api_key or os.environ.get('ANTHROPIC_API_KEY', None)
     if not api_key:
       raise ValueError(
           'Please specify `api_key` during `__init__` or set environment '
           'variable `ANTHROPIC_API_KEY` with your Anthropic API key.'
       )
     self._api_key = api_key
     return True
 
+  @functools.cached_property
+  def _session(self) -> requests.Session:
+    assert self._api_initialized
+    s = requests.Session()
+    s.headers.update({
+        'x-api-key': self._api_key,
+        'anthropic-version': _ANTHROPIC_API_VERSION,
+        'content-type': 'application/json',
+    })
+    return s
+
   @property
   def model_id(self) -> str:
     """Returns a string to identify the model."""
     return self.model
 
   @property
   def max_concurrency(self) -> int:
-    return SUPPORTED_MODELS_AND_SETTINGS[self.model].max_concurrency
+    rpm = SUPPORTED_MODELS_AND_SETTINGS[self.model].get('rpm', 0)
+    tpm = SUPPORTED_MODELS_AND_SETTINGS[self.model].get('tpm', 0)
+    return self.rate_to_max_concurrency(
+        requests_per_min=rpm, tokens_per_min=tpm
+    )
 
   def _sample(self, prompts: list[lf.Message]) -> list[lf.LMSamplingResult]:
     assert self._api_initialized
     return self._parallel_execute_with_currency_control(
         self._sample_single, prompts, retry_on_errors=(RateLimitError)
     )
 
@@ -161,58 +180,53 @@
     return lf.AIMessage.from_chunks(
         [x['text'] for x in content if x['type'] == 'text']
     )
 
   def _parse_response(self, response: requests.Response) -> lf.LMSamplingResult:
     """Parses Anthropic's response."""
     # NOTE(daiyip): Refer https://docs.anthropic.com/claude/reference/errors
-    output = response.json()
     if response.status_code == 200:
+      output = response.json()
       message = self._message_from_content(output['content'])
       input_tokens = output['usage']['input_tokens']
       output_tokens = output['usage']['output_tokens']
       return lf.LMSamplingResult(
           [lf.LMSample(message)],
           usage=lf.LMSamplingUsage(
               prompt_tokens=input_tokens,
               completion_tokens=output_tokens,
               total_tokens=input_tokens + output_tokens,
           ),
       )
     else:
       if response.status_code == 429:
         error_cls = RateLimitError
-      elif response.status_code == 529:
+      elif response.status_code in (502, 529):
         error_cls = OverloadedError
       else:
         error_cls = AnthropicError
-      error = output['error']
-      raise error_cls(f'{error["type"]}: {error["message"]}')
+      raise error_cls(f'{response.status_code}: {response.content}')
 
   def _sample_single(self, prompt: lf.Message) -> lf.LMSamplingResult:
     request = dict()
     request.update(self._get_request_args(self.sampling_options))
     request.update(
         dict(
             messages=[
                 dict(role='user', content=self._content_from_message(prompt))
             ]
         )
     )
-    response = requests.post(
-        _ANTHROPIC_MESSAGE_API_ENDPOINT,
-        json=request,
-        headers={
-            'x-api-key': self._api_key,
-            'anthropic-version': _ANTHROPIC_API_VERSION,
-            'content-type': 'application/json',
-        },
-        timeout=self.timeout,
-    )
-    return self._parse_response(response)
+    try:
+      response = self._session.post(
+          _ANTHROPIC_MESSAGE_API_ENDPOINT, json=request, timeout=self.timeout,
+      )
+      return self._parse_response(response)
+    except ConnectionError as e:
+      raise OverloadedError(str(e)) from e
 
 
 class Claude3(Anthropic):
   """Base class for Claude 3 models. 200K input tokens and 4K output tokens."""
   multimodal = True
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/anthropic_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,40 +94,40 @@
         }
     ).encode()
     return response
 
   return _mock_requests
 
 
-class AuthropicTest(unittest.TestCase):
+class AnthropicTest(unittest.TestCase):
 
   def test_basics(self):
     self.assertEqual(
         anthropic.Claude3Haiku().model_id, 'claude-3-haiku-20240307'
     )
-    self.assertEqual(anthropic.Claude3Haiku().max_concurrency, 16)
+    self.assertGreater(anthropic.Claude3Haiku().max_concurrency, 0)
 
   def test_api_key(self):
     lm = anthropic.Claude3Haiku()
     with self.assertRaisesRegex(ValueError, 'Please specify `api_key`'):
       lm('hi')
 
-    with mock.patch('requests.post') as mock_request:
+    with mock.patch('requests.Session.post') as mock_request:
       mock_request.side_effect = mock_requests_post
 
       lm = anthropic.Claude3Haiku(api_key='fake key')
       self.assertRegex(lm('hi').text, 'hello.*')
 
       os.environ['ANTHROPIC_API_KEY'] = 'abc'
       lm = anthropic.Claude3Haiku()
       self.assertRegex(lm('hi').text, 'hello.*')
       del os.environ['ANTHROPIC_API_KEY']
 
   def test_call(self):
-    with mock.patch('requests.post') as mock_request:
+    with mock.patch('requests.Session.post') as mock_request:
       mock_request.side_effect = mock_requests_post
       lm = anthropic.Claude3Haiku(api_key='fake_key')
       response = lm('hello', temperature=0.0, top_k=0.1, top_p=0.2, stop=['\n'])
       self.assertEqual(
           response.text,
           (
               'hello with temperature=0.0, top_k=0.1, top_p=0.2, '
@@ -136,32 +136,32 @@
       )
       self.assertIsNotNone(response.usage)
       self.assertIsNotNone(response.usage.prompt_tokens, 2)
       self.assertIsNotNone(response.usage.completion_tokens, 1)
       self.assertIsNotNone(response.usage.total_tokens, 3)
 
   def test_mm_call(self):
-    with mock.patch('requests.post') as mock_mm_request:
+    with mock.patch('requests.Session.post') as mock_mm_request:
       mock_mm_request.side_effect = mock_mm_requests_post
       lm = anthropic.Claude3Haiku(api_key='fake_key')
       response = lm(lf_modalities.Image.from_bytes(image_content), lm=lm)
       self.assertEqual(response.text, 'image: image/png')
 
   def test_call_errors(self):
     for status_code, error_type, error_message in [
         (429, 'rate_limit', 'Rate limit exceeded.'),
         (529, 'service_unavailable', 'Service unavailable.'),
         (500, 'bad_request', 'Bad request.'),
     ]:
-      with mock.patch('requests.post') as mock_mm_request:
+      with mock.patch('requests.Session.post') as mock_mm_request:
         mock_mm_request.side_effect = mock_requests_post_error(
             status_code, error_type, error_message
         )
         lm = anthropic.Claude3Haiku(api_key='fake_key')
         with self.assertRaisesRegex(
-            Exception, f'{error_type}: {error_message}'
+            Exception, f'.*{status_code}: .*{error_message}'
         ):
           lm('hello', lm=lm, max_attempts=1)
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/groq.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,26 +74,37 @@
       ),
   ] = None
 
   def _on_bound(self):
     super()._on_bound()
     self._api_key = None
     self.__dict__.pop('_api_initialized', None)
+    self.__dict__.pop('_session', None)
 
   @functools.cached_property
   def _api_initialized(self):
     api_key = self.api_key or os.environ.get('GROQ_API_KEY', None)
     if not api_key:
       raise ValueError(
           'Please specify `api_key` during `__init__` or set environment '
-          'variable `GROQ_API_KEY` with your Anthropic API key.'
+          'variable `GROQ_API_KEY` with your Groq API key.'
       )
     self._api_key = api_key
     return True
 
+  @functools.cached_property
+  def _session(self) -> requests.Session:
+    assert self._api_initialized
+    s = requests.Session()
+    s.headers.update({
+        'Authorization': f'Bearer {self._api_key}',
+        'Content-Type': 'application/json',
+    })
+    return s
+
   @property
   def model_id(self) -> str:
     """Returns a string to identify the model."""
     return self.model
 
   @property
   def max_concurrency(self) -> int:
@@ -115,15 +126,15 @@
     if options.top_p is not None:
       args['top_p'] = options.top_p
     if options.stop:
       args['stop'] = options.stop
     return args
 
   def _content_from_message(self, prompt: lf.Message) -> list[dict[str, Any]]:
-    """Converts an message to Anthropic's content protocol (list of dicts)."""
+    """Converts an message to Groq's content protocol (list of dicts)."""
     # Refer: https://platform.openai.com/docs/api-reference/chat/create
     content = []
     for chunk in prompt.chunk():
       if isinstance(chunk, str):
         item = dict(type='text', text=chunk)
       elif (
           self.multimodal
@@ -134,28 +145,28 @@
         item = dict(type='image_url', image_url=chunk.uri)
       else:
         raise ValueError(f'Unsupported modality object: {chunk!r}.')
       content.append(item)
     return content
 
   def _message_from_choice(self, choice: dict[str, Any]) -> lf.Message:
-    """Converts Anthropic's content protocol to message."""
+    """Converts Groq's content protocol to message."""
     # Refer: https://platform.openai.com/docs/api-reference/chat/create
     content = choice['message']['content']
     if isinstance(content, str):
       return lf.AIMessage(content)
     return lf.AIMessage.from_chunks(
         [x['text'] for x in content if x['type'] == 'text']
     )
 
   def _parse_response(self, response: requests.Response) -> lf.LMSamplingResult:
-    """Parses Anthropic's response."""
+    """Parses Groq's response."""
     # Refer: https://platform.openai.com/docs/api-reference/chat/object
-    output = response.json()
     if response.status_code == 200:
+      output = response.json()
       samples = [
           lf.LMSample(self._message_from_choice(choice), score=0.0)
           for choice in output['choices']
       ]
       usage = output['usage']
       return lf.LMSamplingResult(
           samples,
@@ -165,20 +176,19 @@
               total_tokens=usage['total_tokens'],
           ),
       )
     else:
       # https://platform.openai.com/docs/guides/error-codes/api-errors
       if response.status_code == 429:
         error_cls = RateLimitError
-      elif response.status_code in (500, 503):
+      elif response.status_code in (500, 502, 503):
         error_cls = OverloadedError
       else:
         error_cls = GroqError
-      error = output['error']
-      raise error_cls(f'{error["type"]}: {error["message"]}')
+      raise error_cls(f'{response.status_code}: {response.content}')
 
   def _sample(self, prompts: list[lf.Message]) -> list[lf.LMSamplingResult]:
     assert self._api_initialized
     return self._parallel_execute_with_currency_control(
         self._sample_single,
         prompts,
         retry_on_errors=(RateLimitError, OverloadedError),
@@ -190,24 +200,23 @@
     request.update(
         dict(
             messages=[
                 dict(role='user', content=self._content_from_message(prompt))
             ]
         )
     )
-    response = requests.post(
-        _CHAT_COMPLETE_API_ENDPOINT,
-        json=request,
-        headers={
-            'Authorization': f'Bearer {self._api_key}',
-            'Content-Type': 'application/json',
-        },
-        timeout=self.timeout,
-    )
-    return self._parse_response(response)
+    try:
+      response = self._session.post(
+          _CHAT_COMPLETE_API_ENDPOINT,
+          json=request,
+          timeout=self.timeout,
+      )
+      return self._parse_response(response)
+    except ConnectionError as e:
+      raise OverloadedError(str(e)) from e
 
 
 class GroqLlama3_8B(Groq):  # pylint: disable=invalid-name
   """Llama3-8B with 8K context window.
 
   See: https://huggingface.co/meta-llama/Meta-Llama-3-8B
   """
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/groq_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,27 +103,27 @@
     self.assertEqual(groq.GroqMistral_8x7B().max_concurrency, 16)
 
   def test_api_key(self):
     lm = groq.GroqMistral_8x7B()
     with self.assertRaisesRegex(ValueError, 'Please specify `api_key`'):
       lm('hi')
 
-    with mock.patch('requests.post') as mock_request:
+    with mock.patch('requests.Session.post') as mock_request:
       mock_request.side_effect = mock_requests_post
 
       lm = groq.GroqMistral_8x7B(api_key='fake key')
       self.assertRegex(lm('hi').text, 'hello.*')
 
       os.environ['GROQ_API_KEY'] = 'abc'
       lm = groq.GroqMistral_8x7B()
       self.assertRegex(lm('hi').text, 'hello.*')
       del os.environ['GROQ_API_KEY']
 
   def test_call(self):
-    with mock.patch('requests.post') as mock_request:
+    with mock.patch('requests.Session.post') as mock_request:
       mock_request.side_effect = mock_requests_post
       lm = groq.GroqLlama3_70B(api_key='fake_key')
       response = lm(
           'hello',
           temperature=0.0,
           max_tokens=1024,
           top_k=0.1,
@@ -139,32 +139,32 @@
       )
       self.assertIsNotNone(response.usage)
       self.assertIsNotNone(response.usage.prompt_tokens, 2)
       self.assertIsNotNone(response.usage.completion_tokens, 1)
       self.assertIsNotNone(response.usage.total_tokens, 3)
 
   def test_mm_call(self):
-    with mock.patch('requests.post') as mock_mm_request:
+    with mock.patch('requests.Session.post') as mock_mm_request:
       mock_mm_request.side_effect = mock_mm_requests_post
       lm = groq.GroqLlama3_70B(multimodal=True, api_key='fake_key')
       response = lm(lf_modalities.Image.from_uri('https://fake/image.jpg'))
       self.assertEqual(response.text, 'https://fake/image.jpg')
 
   def test_call_errors(self):
     for status_code, error_type, error_message in [
         (429, 'rate_limit', 'Rate limit exceeded.'),
         (503, 'service_unavailable', 'Service unavailable.'),
         (500, 'bad_request', 'Bad request.'),
     ]:
-      with mock.patch('requests.post') as mock_mm_request:
+      with mock.patch('requests.Session.post') as mock_mm_request:
         mock_mm_request.side_effect = mock_requests_post_error(
             status_code, error_type, error_message
         )
         lm = groq.GroqLlama3_70B(api_key='fake_key')
         with self.assertRaisesRegex(
-            Exception, f'{error_type}: {error_message}'
+            Exception, f'{status_code}:.*{error_type}'
         ):
           lm('hello', lm=lm, max_attempts=1)
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/openai.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,71 +22,72 @@
 from langfun.core import modalities as lf_modalities
 import openai
 from openai import error as openai_error
 from openai import openai_object
 import pyglove as pg
 
 
-SUPPORTED_MODELS_AND_SETTINGS = [
-    # Model name, max concurrent requests.
-    # The concurrent requests is estimated by TPM/RPM from
-    # https://platform.openai.com/account/limits
-    # GPT-4 Turbo models.
-    ('gpt-4-turbo', 8),  # GPT-4 Turbo with Vision
-    ('gpt-4-turbo-2024-04-09', 8),  # GPT-4-Turbo with Vision, 04/09/2024
-    ('gpt-4-turbo-preview', 8),  # GPT-4 Turbo Preview
-    ('gpt-4-0125-preview', 8),  # GPT-4 Turbo Preview, 01/25/2024
-    ('gpt-4-1106-preview', 8),  # GPT-4 Turbo Preview, 11/06/2023
-    ('gpt-4-vision-preview', 8),  # GPT-4 Turbo Vision Preview.
-    ('gpt-4-1106-vision-preview', 8),  # GPT-4 Turbo Vision Preview, 11/06/2023
-    # GPT-4 models.
-    ('gpt-4', 4),
-    ('gpt-4-0613', 4),
-    ('gpt-4-0314', 4),
-    ('gpt-4-32k', 4),
-    ('gpt-4-32k-0613', 4),
-    ('gpt-4-32k-0314', 4),
-    # GPT-3.5 Turbo models.
-    ('gpt-3.5-turbo', 16),
-    ('gpt-3.5-turbo-0125', 16),
-    ('gpt-3.5-turbo-1106', 16),
-    ('gpt-3.5-turbo-0613', 16),
-    ('gpt-3.5-turbo-0301', 16),
-    ('gpt-3.5-turbo-16k', 16),
-    ('gpt-3.5-turbo-16k-0613', 16),
-    ('gpt-3.5-turbo-16k-0301', 16),
-    # GPT-3.5 models.
-    ('text-davinci-003', 8),  # GPT-3.5, trained with RHLF.
-    ('text-davinci-002', 4),  # Trained with SFT but no RHLF.
-    ('code-davinci-002', 4),
-    # GPT-3 instruction-tuned models.
-    ('text-curie-001', 4),
-    ('text-babbage-001', 4),
-    ('text-ada-001', 4),
-    ('davinci', 4),
-    ('curie', 4),
-    ('babbage', 4),
-    ('ada', 4),
-    # GPT-3 base models without instruction tuning.
-    ('babbage-002', 4),
-    ('davinci-002', 4),
-]
-
-
-# Model concurreny setting.
-_MODEL_CONCURRENCY = {m[0]: m[1] for m in SUPPORTED_MODELS_AND_SETTINGS}
+# From https://platform.openai.com/settings/organization/limits
+_DEFAULT_TPM = 250000
+_DEFAULT_RPM = 3000
+
+SUPPORTED_MODELS_AND_SETTINGS = {
+    # Models from https://platform.openai.com/docs/models
+    # RPM is from https://platform.openai.com/docs/guides/rate-limits
+    # GPT-4-Turbo models
+    'gpt-4-turbo': pg.Dict(rpm=10000, tpm=1500000),
+    'gpt-4-turbo-2024-04-09': pg.Dict(rpm=10000, tpm=1500000),
+    'gpt-4-turbo-preview': pg.Dict(rpm=10000, tpm=1500000),
+    'gpt-4-0125-preview': pg.Dict(rpm=10000, tpm=1500000),
+    'gpt-4-1106-preview': pg.Dict(rpm=10000, tpm=1500000),
+    'gpt-4-vision-preview': pg.Dict(rpm=10000, tpm=1500000),
+    'gpt-4-1106-vision-preview': pg.Dict(
+        rpm=10000, tpm=1500000
+    ),
+    # GPT-4 models
+    'gpt-4': pg.Dict(rpm=10000, tpm=300000),
+    'gpt-4-0613': pg.Dict(rpm=10000, tpm=300000),
+    'gpt-4-0314': pg.Dict(rpm=10000, tpm=300000),
+    'gpt-4-32k': pg.Dict(rpm=10000, tpm=300000),
+    'gpt-4-32k-0613': pg.Dict(rpm=10000, tpm=300000),
+    'gpt-4-32k-0314': pg.Dict(rpm=10000, tpm=300000),
+    # GPT-3.5-Turbo models
+    'gpt-3.5-turbo': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-3.5-turbo-0125': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-3.5-turbo-1106': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-3.5-turbo-0613': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-3.5-turbo-0301': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-3.5-turbo-16k': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-3.5-turbo-16k-0613': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-3.5-turbo-16k-0301': pg.Dict(rpm=10000, tpm=2000000),
+    # GPT-3.5 models
+    'text-davinci-003': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'text-davinci-002': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'code-davinci-002': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    # GPT-3 instruction-tuned models
+    'text-curie-001': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'text-babbage-001': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'text-ada-001': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'davinci': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'curie': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'babbage': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'ada': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    # GPT-3 base models
+    'babbage-002': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+    'davinci-002': pg.Dict(rpm=_DEFAULT_RPM, tpm=_DEFAULT_TPM),
+}
 
 
 @lf.use_init_args(['model'])
 class OpenAI(lf.LanguageModel):
   """OpenAI model."""
 
   model: pg.typing.Annotated[
       pg.typing.Enum(
-          pg.MISSING_VALUE, [m[0] for m in SUPPORTED_MODELS_AND_SETTINGS]
+          pg.MISSING_VALUE, list(SUPPORTED_MODELS_AND_SETTINGS.keys())
       ),
       'The name of the model to use.',
   ] = 'gpt-3.5-turbo'
 
   multimodal: Annotated[
       bool,
       'Whether this model has multimodal support.'
@@ -130,15 +131,19 @@
   @property
   def model_id(self) -> str:
     """Returns a string to identify the model."""
     return f'OpenAI({self.model})'
 
   @property
   def max_concurrency(self) -> int:
-    return _MODEL_CONCURRENCY[self.model]
+    rpm = SUPPORTED_MODELS_AND_SETTINGS[self.model].get('rpm', 0)
+    tpm = SUPPORTED_MODELS_AND_SETTINGS[self.model].get('tpm', 0)
+    return self.rate_to_max_concurrency(
+        requests_per_min=rpm, tokens_per_min=tpm
+    )
 
   @classmethod
   def dir(cls):
     return openai.Model.list()
 
   @property
   def is_chat_model(self):
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240423/langfun/core/llms/openai_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for openai models."""
+"""Tests for OpenAI models."""
 
 import unittest
 from unittest import mock
 
 import langfun.core as lf
 from langfun.core import modalities as lf_modalities
 from langfun.core.llms import openai
@@ -81,28 +81,28 @@
           prompt_tokens=100,
           completion_tokens=100,
           total_tokens=200,
       ),
   )
 
 
-class OpenaiTest(unittest.TestCase):
+class OpenAITest(unittest.TestCase):
   """Tests for OpenAI language model."""
 
   def test_model_id(self):
     self.assertEqual(
         openai.Gpt35(api_key='test_key').model_id, 'OpenAI(text-davinci-003)')
 
   def test_resource_id(self):
     self.assertEqual(
         openai.Gpt35(api_key='test_key').resource_id, 'OpenAI(text-davinci-003)'
     )
 
   def test_max_concurrency(self):
-    self.assertEqual(openai.Gpt35(api_key='test_key').max_concurrency, 8)
+    self.assertGreater(openai.Gpt35(api_key='test_key').max_concurrency, 0)
 
   def test_get_request_args(self):
     self.assertEqual(
         openai.Gpt35(api_key='test_key', timeout=90.0)._get_request_args(
             lf.LMSamplingOptions(
                 temperature=2.0,
                 n=2,
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240423/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240423/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/memory.py` & `langfun-0.0.2.dev20240423/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/message.py` & `langfun-0.0.2.dev20240423/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/message_test.py` & `langfun-0.0.2.dev20240423/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240423/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240423/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240423/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240423/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240423/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240423/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modality.py` & `langfun-0.0.2.dev20240423/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240423/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240423/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240423/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/sampling.py` & `langfun-0.0.2.dev20240423/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240423/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240423/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/subscription.py` & `langfun-0.0.2.dev20240423/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240423/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/template.py` & `langfun-0.0.2.dev20240423/langfun/core/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 NO_TEMPLATE_DOCSTR_SIGN = 'THIS IS NOT A TEMPLATE'
 
 # Keys for storing render stack in the
 # thread-local storage.
 _TLS_RENDER_STACK = '_template_render_stack'
 _TLS_RENDER_RESULT_CACHE = '_template_render_result_cache'
 
+# The prefix for fields or contextual attributes to be treated as additional
+# metadata for rendered message.
+_ADDITIONAL_METADATA_PREFIX = 'metadata_'
+
 
 class Template(
     natural_language.NaturalLanguageFormattable,
     component.Component,
     pg.typing.CustomTyping,
 ):
   """Langfun string template."""
@@ -299,27 +303,27 @@
             ):
               # Natural language formattable objects will be returned in natural
               # language when they are directly returned as rendering elements
               # in the template.
               with modality.format_modality_as_ref():
                 rendered_text = self._template.render(**inputs)
 
+            # Carry additional metadata.
+            metadata = self.additional_metadata()
+
         if self.clean:
           rendered_text = rendered_text.strip()
 
-        # Fill the variables for rendering the template as metadata.
-        message = message_cls(
-            text=rendered_text,
-            metadata={
-                k: pg.Ref(v)
-                for k, v in inputs.items()
-                if not inspect.ismethod(v)
-            },
+        metadata.update(
+            {k: pg.Ref(v) for k, v in inputs.items() if not inspect.ismethod(v)}
         )
 
+        # Fill the variables for rendering the template as metadata.
+        message = message_cls(text=rendered_text, metadata=metadata)
+
         # Tag input as rendered message.
         message.tag(message_lib.Message.TAG_RENDERED)
 
         # Adding result to cache.
         cache[id(self)] = message
 
         # Set last render output to message.
@@ -336,14 +340,28 @@
             )
         )
       return message
     finally:
       top = pg.object_utils.thread_local_pop(_TLS_RENDER_STACK)
       assert top is self, (top, self)
 
+  def additional_metadata(self) -> dict[str, Any]:
+    """Returns additional metadta to be carried in the rendered message."""
+    metadata = {}
+    # Carry metadata from `lf.context`.
+    for k, v in component.all_contextual_values().items():
+      if k.startswith(_ADDITIONAL_METADATA_PREFIX):
+        metadata[k.removeprefix(_ADDITIONAL_METADATA_PREFIX)] = v
+
+    # Carry metadata from fields.
+    for k, v in self.sym_init_args.items():
+      if k.startswith(_ADDITIONAL_METADATA_PREFIX):
+        metadata[k.removeprefix(_ADDITIONAL_METADATA_PREFIX)] = v
+    return metadata
+
   #
   # Implements `pg.typing.CustomTyping`.
   #
 
   def custom_apply(
       self,
       path: pg.KeyPath,
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/template_test.py` & `langfun-0.0.2.dev20240423/langfun/core/template_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Template test."""
 import inspect
 import unittest
 
 from langfun.core import component
+from langfun.core import message as message_lib
 from langfun.core import modality
 from langfun.core import subscription
 from langfun.core.template import Template
 from langfun.core.template import TemplateRenderEvent
 import pyglove as pg
 
 
@@ -423,14 +424,22 @@
             {{examples.key2}}: {{examples.value2}}
             """),
     )
 
     # Test len.
     self.assert_partial(Template('Hello {{len(x)}}'), 'Hello {{len(x)}}')
 
+  def test_additional_metadata(self):
+    t = Template('hi', metadata_weights=1.0, y=2)
+    self.assertEqual(t.render(), message_lib.UserMessage('hi', weights=1.0))
+
+    t = Template('hi')
+    with component.context(metadata_weights=1.0, y=2):
+      self.assertEqual(t.render(), message_lib.UserMessage('hi', weights=1.0))
+
 
 class TemplateRenderEventTest(unittest.TestCase):
 
   def test_render_event(self):
     l = Template(
         'Subject: {{subject}}', subject=Template('The science of {{name}}')
     )
```

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240423/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240423/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240423/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240423/langfun.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240422
+Version: 0.0.2.dev20240423
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240422/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240423/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240422/setup.py` & `langfun-0.0.2.dev20240423/setup.py`

 * *Files identical despite different names*


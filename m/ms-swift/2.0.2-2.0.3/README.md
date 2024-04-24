# Comparing `tmp/ms-swift-2.0.2.tar.gz` & `tmp/ms-swift-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms-swift-2.0.2.tar", last modified: Wed Apr 17 05:38:49 2024, max compression
+gzip compressed data, was "dist/ms-swift-2.0.3.tar", last modified: Tue Apr 23 14:36:17 2024, max compression
```

## Comparing `ms-swift-2.0.2.tar` & `ms-swift-2.0.3.tar`

### file list

```diff
@@ -1,227 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 05:38:46.000000 ms-swift-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55120 2024-04-17 05:38:49.000000 ms-swift-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-17 05:38:46.000000 ms-swift-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55120 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 05:38:49.000000 ms-swift-2.0.2/ms_swift.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 05:38:46.000000 ms-swift-2.0.2/requirements/aigc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 05:38:46.000000 ms-swift-2.0.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 05:38:46.000000 ms-swift-2.0.2/requirements/eval.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-17 05:38:46.000000 ms-swift-2.0.2/requirements/framework.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 05:38:46.000000 ms-swift-2.0.2/requirements/llm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 05:38:46.000000 ms-swift-2.0.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 05:38:49.000000 ms-swift-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-17 05:38:46.000000 ms-swift-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/aigc/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/animatediff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/animatediff_infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/aigc/diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    48449 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    54249 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    60203 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    58211 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    71598 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    46799 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    53924 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    57714 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image_sdxl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/aigc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/aigc/utils/argument.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/app_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/dpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/merge_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/cli/web_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/hub/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30552 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/file_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/push_to_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/snapshot_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/hub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/hub/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/llm/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/agent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/app_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/llm/data/
--rw-r--r--   0 runner    (1001) docker     (127)    27203 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/data/self_cognition.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/dpo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/llm/ds_config/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/ds_config/zero2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/ds_config/zero3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    20318 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/llm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51349 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52727 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   112933 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    53643 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17195 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/llm/utils/vllm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/torchacc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/dpo_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30575 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/trainers/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/trainers/optimizers/galore/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/optimizers/galore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11202 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/optimizers/galore/adafactor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/optimizers/galore/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/optimizers/galore/adamw8bit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5700 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/optimizers/galore/galore_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/optimizers/galore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/trainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    43987 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/llamapro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/tuners/longlora/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/longlora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/longlora/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/longlora/longlora.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    40224 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/module_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/neftune.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/peft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/restuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/restuning_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/tuners/rome/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/compute_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/compute_v.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/context_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/nethook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/repr_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/rome/rome_hparams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/tuners/scetuning/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/scetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/scetuning/scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/scetuning/scetuning_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/side.py
--rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/tuners/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/ui/llm_infer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_infer/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18467 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_infer/llm_infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_infer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_infer/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/ui/llm_train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/llm_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/self_cog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/ui/llm_train/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/swift/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/np_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/tb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-17 05:38:46.000000 ms-swift-2.0.2/swift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/hub/test_check_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/tests/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/llm/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20380 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/llm/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    27223 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/llm/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/llm/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/llm/test_vllm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/model_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/tests/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_extra_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_merged_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_neft.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    23706 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_swift_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_swift_device_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/tuners/test_swift_restuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:49.000000 ms-swift-2.0.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-17 05:38:46.000000 ms-swift-2.0.2/tests/utils/test_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 14:36:07.000000 ms-swift-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    59446 2024-04-23 14:36:17.000000 ms-swift-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    53550 2024-04-23 14:36:07.000000 ms-swift-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/ms_swift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    59446 2024-04-23 14:36:16.000000 ms-swift-2.0.3/ms_swift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-23 14:36:17.000000 ms-swift-2.0.3/ms_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:36:16.000000 ms-swift-2.0.3/ms_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 14:36:16.000000 ms-swift-2.0.3/ms_swift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:36:16.000000 ms-swift-2.0.3/ms_swift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 14:36:16.000000 ms-swift-2.0.3/ms_swift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 14:36:16.000000 ms-swift-2.0.3/ms_swift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 14:36:07.000000 ms-swift-2.0.3/requirements/aigc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-23 14:36:07.000000 ms-swift-2.0.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 14:36:07.000000 ms-swift-2.0.3/requirements/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-23 14:36:07.000000 ms-swift-2.0.3/requirements/framework.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 14:36:07.000000 ms-swift-2.0.3/requirements/llm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 14:36:07.000000 ms-swift-2.0.3/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-23 14:36:17.000000 ms-swift-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-23 14:36:07.000000 ms-swift-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/aigc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/animatediff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/animatediff_infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/aigc/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48449 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54249 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60203 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58211 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71598 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46799 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53924 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57714 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image_sdxl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/aigc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/aigc/utils/argument.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/app_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/dpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/merge_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/cli/web_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30552 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/file_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/push_to_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/snapshot_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/hub/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/llm/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/agent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/app_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/llm/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    27203 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/data/self_cognition.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    20582 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/dpo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/llm/ds_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/ds_config/zero2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/ds_config/zero3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/ds_config/zero3_offload.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19985 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13000 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/llm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53432 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59486 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135558 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60060 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31795 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/llm/utils/vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/torchacc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/dpo_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30575 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/trainers/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/trainers/optimizers/galore/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/optimizers/galore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11202 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/optimizers/galore/adafactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/optimizers/galore/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/optimizers/galore/adamw8bit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5700 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/optimizers/galore/galore_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/optimizers/galore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/trainers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43987 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/llamapro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/tuners/longlora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/longlora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/longlora/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/longlora/longlora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40224 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/module_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/neftune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/restuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/restuning_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/tuners/rome/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/compute_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/compute_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/context_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/nethook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/repr_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/rome/rome_hparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/tuners/scetuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/scetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/scetuning/scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/scetuning/scetuning_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/side.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/tuners/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/ui/llm_infer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_infer/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_infer/llm_infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_infer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_infer/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/ui/llm_train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/llm_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/self_cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/ui/llm_train/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/swift/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/np_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/tb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 14:36:07.000000 ms-swift-2.0.3/swift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/hub/test_check_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/tests/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/llm/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/llm/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27223 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/llm/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/llm/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/llm/test_vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/model_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/tests/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_extra_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_merged_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_neft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23592 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_swift_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_swift_device_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/tuners/test_swift_restuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:17.000000 ms-swift-2.0.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-23 14:36:07.000000 ms-swift-2.0.3/tests/utils/test_torch_utils.py
```

### Comparing `ms-swift-2.0.2/PKG-INFO` & `ms-swift-2.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-swift
-Version: 2.0.2
+Version: 2.0.3
 Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
 Home-page: https://github.com/modelscope/swift
 Author: DAMO ModelScope teams
 Author-email: contact@modelscope.cn
 License: Apache License 2.0
 Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
         
@@ -43,14 +43,22 @@
         SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
         
         To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
         
         Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
         
         ## 🎉 News
+        - 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series models. This includes：chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-13b along with their corresponding 16k and 64k long text versions.
+        - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-6b-128k, Openbuddy-Llama3.
+        - 2024.04.20: Support for inference, fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train.
+        - 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-best-practice.md).
+        - 2024.04.19: Support for inference, fine-tuning, and deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train.
+        - 2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided default zero3-offload configuration file for zero3+cpu offload usage.
+        - 2024.04.18: Supported compatibility with HuggingFace ecosystem using the environment variable `USE_HF`, switching to use models and datasets from HF. Please refer to the [HuggingFace ecosystem compatibility documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md).
+        - 2024.04.17: Support the evaluation for OpenAI standard interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-line-parameters.md#eval-parameters) for details.
         - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
         - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
         - 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
         - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train.
         - 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
@@ -60,25 +68,25 @@
         - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
         - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
         - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
         - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
         - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
         - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
         - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
+        <details><summary>More</summary>
+        
         - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
         - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
         - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
         - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
         - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
         - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
         - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
         - 🔥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start training.
         - 2024.02.25: Support `swift export` to quantize models using **AWQ/GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/source_en/LLM/LLM-quantization.md).
-        <details><summary>More</summary>
-        
         - 2024.02.22: Support gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct.
         - 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
         - 🔥2024.02.05: Support **Qwen1.5** series models, see [model list](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B) for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8).
         - 2024.02.05: Support training of diffusion models such as **SDXL**, **SD**, **ControlNet**, as well as **DreamBooth** training. See corresponding [training scripts](https://github.com/modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details.
         - 2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat.
         - 🔥2024.02.01: Support dataset mixing to reduce **catastrophic forgetting**. Use `--train_dataset_mix_ratio 2.0` to enable training! We also open sourced the general knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/iic/ms_bench/summary).
         - 🔥2024.02.01: Support Agent training! Agent training algorithm is derived from this [paper](https://arxiv.org/pdf/2309.00986.pdf). We also added [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/summary), a high-quality agent dataset. Use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/sft.sh) to start Agent training!
@@ -141,29 +149,29 @@
         
         SWIFT runs in the Python environment. Please ensure your Python version is higher than 3.8.
         
         - Method 1: Install SWIFT using pip command:
         
         ```shell
         # Full capabilities
-        pip install ms-swift[all] -U
+        pip install 'ms-swift[all]' -U
         # LLM only
-        pip install ms-swift[llm] -U
+        pip install 'ms-swift[llm]' -U
         # AIGC only
-        pip install ms-swift[aigc] -U
+        pip install 'ms-swift[aigc]' -U
         # Adapters only
         pip install ms-swift -U
         ```
         
         - Method 2: Install SWIFT through source code (convenient for running training and inference scripts), please run the following commands:
         
         ```shell
         git clone https://github.com/modelscope/swift.git
         cd swift
-        pip install -e .[llm]
+        pip install -e '.[llm]'
         ```
         
         SWIFT depends on torch>=1.13, recommend torch>=2.0.0.
         
         - Method 3: Use SWIFT in our Docker image
         
         ```shell
@@ -288,14 +296,15 @@
             --dataset blossom-math-zh \
             --num_train_epochs 5 \
             --sft_type lora \
             --output_dir output \
         ```
         
         #### Deepspeed Training
+        Deepspeed supports training of quantized GPTQ and AWQ models.
         
         ZeRO2:
         ```shell
         # Experimental Environment: 4 * A100
         # GPU Memory Requirement: 4 * 21GB
         # Runtime: 0.9 hours
         NPROC_PER_NODE=4 \
@@ -321,14 +330,61 @@
             --dataset blossom-math-zh \
             --num_train_epochs 5 \
             --sft_type lora \
             --output_dir output \
             --deepspeed default-zero3 \
         ```
         
+        ZeRO3-Offload:
+        ```shell
+        # Experimental Environment: 4 * A100
+        # GPU Memory Requirement: 4 * 12GB
+        # Runtime: 60 hours
+        NPROC_PER_NODE=4 \
+        CUDA_VISIBLE_DEVICES=0,1,2,3 \
+        swift sft \
+            --model_id_or_path AI-ModelScope/WizardLM-2-8x22B \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
+            --deepspeed zero3-offload \
+        ```
+        
+        
+        #### Multi-node Multi-GPU
+        ```shell
+        # node0
+        CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+        NNODES=2 \
+        NODE_RANK=0 \
+        MASTER_ADDR=127.0.0.1 \
+        NPROC_PER_NODE=8 \
+        swift sft \
+            --model_id_or_path qwen1half-32b-chat \
+            --sft_type full \
+            --dataset blossom-math-zh \
+            --output_dir output \
+            --deepspeed default-zero3 \
+        
+        # node1
+        CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+        NNODES=2 \
+        NODE_RANK=1 \
+        MASTER_ADDR=xxx.xxx.xxx.xxx \
+        NPROC_PER_NODE=8 \
+        swift sft \
+            --model_id_or_path qwen1half-32b-chat \
+            --sft_type full \
+            --dataset blossom-math-zh \
+            --output_dir output \
+            --deepspeed default-zero3 \
+        ```
+        
+        
         ### Inference
         Original model:
         ```shell
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
         # use VLLM
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
             --infer_backend vllm --max_model_len 8192
@@ -381,27 +437,29 @@
         # 使用VLLM加速
         CUDA_VISIBLE_DEVICES=0 swift deploy \
             --ckpt_dir xxx/checkpoint-xxx --merge_lora true \
             --infer_backend vllm --max_model_len 8192
         ```
         
         ### Supported Models
+        The complete list of supported models and datasets can be found at [Supported Models and Datasets List](https://idealab.alibaba-inc.com/docs/source/LLM/Supported-Models-and-Datasets.md).
         
         #### LLMs
         
         | Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
         |------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
         | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model<br>code model                      |
-        | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
+        | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model<br>long text model  |
         | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
         | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
         | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
         | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
+        | LLaMA3                   | [LLaMA3 series models](https://github.com/meta-llama/llama3)  | English       | 8B-70B<br>including quantized versions      | base model<br>chat model              |
         | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
-        | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
+        | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
         | InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
         | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
         | MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
         | Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
         | MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
         | OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
         | Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
@@ -416,15 +474,18 @@
         | CodeFuse-CodeLLaMA<br>CodeFuse-Codegeex2<br>CodeFuse-Qwen | [Ant CodeFuse series models](https://github.com/codefuse-ai)        | Chinese<br>English    | 6B-34B                                 | chat model<br>code model                      |
         | phi2                                           | Microsoft's PHI2 model                                                 | English            | 3B                                     | base model<br>code model                          |
         | Grok | [X-ai](https://github.com/xai-org/grok-1) | English | 300B | base model |
         | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat) | Chinese<br>English | 7B-12B | chat model |
         | dbrx | [databricks](https://github.com/databricks/dbrx) | English | 132B | base model<br>chat model  |
         | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) | Chinese<br>English | 13B | base model  |
         | c4ai-command-r | [c4ai](https://cohere.com/command) | Multilingual | 35B-104B | chat model  |
-        
+        | WizardLM2 | [WizardLM2 series models](https://github.com/nlpxucan/WizardLM) | English | 7B-8x22B<br>including quantized versions | chat model<br>MoE model |
+        | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) | Chinese | 7B| base model<br>chat model|
+        | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model<br>chat model<br>long text model |
+        | ModelScope-Agent | [ModelScope Agent series models](https://github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model |
         
         #### MLLMs
         
         | Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
         |------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
         | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
         | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
@@ -501,38 +562,41 @@
         
         ### User Guide
         
         | Document Name                                                |
         | ------------------------------------------------------------ |
         | [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
         | [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
-        | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
         | [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
+        | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
+        | [LLM Evaluation](docs/source_en/LLM/LLM-eval.md)     |
         | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
         | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
         | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
         | [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
         
         ### Reference Documentation
         | Document Name                                                |
         | ------------------------------------------------------------ |
         | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
-        | [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
         | [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
-        | [Runtime Speed and Memory Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) |
+        | [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
+        | [Runtime Speed and Memory Benchmark](docs/source_en/LLM/Benchmark.md) |
         
         
         ### Best Practices
         
         | Best Practices Name                                                |
         | ------------------------------------------------------------ |
-        | [Agent Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-        | [Self-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-        |  [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-        |  [Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/Multi-Modal/index.md) |
+        | [Agent Fine-Tuning Best Practice](docs/source_en/LLM/Agent-best-practice.md) |
+        | [Self-Cognition Fine-Tuning Best Practice](docs/source_en/LLM/Self-cognition-best-practice.md) |
+        |  [Qwen1.5 Best Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) |
+        |  [Multi-Modal Model Training Best Practice](docs/source_en/Multi-Modal/index.md) |
+        |  [NPU Best Practice](docs/source_en/LLM/NPU-best-practice.md) |
+        
         
         ### Deep Learning Tutorials
         
         | Tutorial Name                                                |
         |-------------------------------------------------------------- |
         | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md) |
         | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 2.0.2 Summary: Swift: Scalable
+Metadata-Version: 2.1 Name: ms-swift Version: 2.0.3 Summary: Swift: Scalable
 lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
 modelscope/swift Author: DAMO ModelScope teams Author-email:
 contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
 (Scalable lightWeight Infrastructure for Fine-Tuning)
 
                             [resources/banner.png]
                          _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
@@ -26,41 +26,67 @@
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
 support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- ð¥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B,
-CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://
-github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-codeqwen1half_7b_chat/lora/sft.sh) to train. - 2024.04.16: Supports inference
-and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to
-[here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
-Modal/llava-best-practice.md). - 2024.04.13: Support the fine-tuning and
-inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/
-modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/
-lora_ddp_ds/sft.sh) to start training! - 2024.04.13: Support the newly launched
-**MiniCPM** series: MiniCPM-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and
-MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start
-training! - ð¥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval
-datasets(also user custom eval datasets) with one command! Check [this
-documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we
-support a trick way to do multiple ablation experiments, check [this
-documentation](docs/source_en/LLM/LLM-exp.md) to use. - ð¥2024.04.11: Support
-**c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this
+- 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-
+llama-alpaca-2** series models. This includesï¼chinese-llama-2-1.3b, chinese-
+llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and
+chinese-alpaca-2-13b along with their corresponding 16k and 64k long text
+versions. - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-
+Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning
+of chatglm3-6b-128k, Openbuddy-Llama3. - 2024.04.20: Support for inference,
+fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B
+and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/
+main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train. -
+2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and
+inference with NPU, please refer to [NPU Inference and Fine-tuning Best
+Practices](docs/source_en/LLM/NPU-best-practice.md). - 2024.04.19: Support for
+inference, fine-tuning, and deployment of **Llama3** series models. This
+includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-
+Instruct. use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train. -
+2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-
+awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed
+zero3-offload` and provided default zero3-offload configuration file for
+zero3+cpu offload usage. - 2024.04.18: Supported compatibility with HuggingFace
+ecosystem using the environment variable `USE_HF`, switching to use models and
+datasets from HF. Please refer to the [HuggingFace ecosystem compatibility
+documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/
+LLM/Compat-HF.md). - 2024.04.17: Support the evaluation for OpenAI standard
+interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-
+line-parameters.md#eval-parameters) for details. - ð¥2024.04.17: Support
+**CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-
+Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train. -
+2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For
+best practice, you can refer to [here](https://github.com/modelscope/swift/
+tree/main/docs/source_en/Multi-Modal/llava-best-practice.md). - 2024.04.13:
+Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this
 script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
-scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. - 2024.04.10: Use SWIFT
-to fine-tune the qwen-7b-chat model to enhance its function call capabilities,
-and combine it with [Modelscope-Agent](https://github.com/modelscope/
-modelscope-agent) for best practices, which can be found [here](https://
-github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-
-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support ruozhiba
-dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training! -
+2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-
+2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
+(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
+Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
+with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
+for details. Meanwhile, we support a trick way to do multiple ablation
+experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
+- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
+command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. -
+2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
+function call capabilities, and combine it with [Modelscope-Agent](https://
+github.com/modelscope/modelscope-agent) for best practices, which can be found
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
+best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
+ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
 Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
 fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
 **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
 (https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
@@ -79,15 +105,15 @@
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
 github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
-practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
+practice.md). More - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -104,17 +130,17 @@
 2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/
 blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start
 training. - ð¥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/
 2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/
 blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start
 training. - 2024.02.25: Support `swift export` to quantize models using **AWQ/
 GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/
-source_en/LLM/LLM-quantization.md). More - 2024.02.22: Support gemma series:
-gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
+source_en/LLM/LLM-quantization.md). - 2024.02.22: Support gemma series: gemma-
+2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-
 instruct, deepseek-math-7b-chat. - ð¥2024.02.05: Support **Qwen1.5** series
 models, see [model list](https://github.com/modelscope/swift/blob/main/docs/
 source/LLM/
 %E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
 for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-
 7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
@@ -259,33 +285,33 @@
 qwen-14b-chat. - 2023.09.18: Support **internlm-20b** series: internlm-20b,
 internlm-20b-chat. - 2023.09.12: Support **MP+DDP** to accelerate full-
 parameter training. - 2023.09.05: Support **openbuddy-llama2-70b-chat**. -
 2023.09.03: Support **baichuan2** series: baichuan2-7b, baichuan2-7b-chat,
 baichuan2-13b, baichuan2-13b-chat. ## ð ï¸ Installation SWIFT runs in the
 Python environment. Please ensure your Python version is higher than 3.8. -
 Method 1: Install SWIFT using pip command: ```shell # Full capabilities pip
-install ms-swift[all] -U # LLM only pip install ms-swift[llm] -U # AIGC only
-pip install ms-swift[aigc] -U # Adapters only pip install ms-swift -U ``` -
-Method 2: Install SWIFT through source code (convenient for running training
-and inference scripts), please run the following commands: ```shell git clone
-https://github.com/modelscope/swift.git cd swift pip install -e .[llm] ```
-SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3: Use SWIFT in
-our Docker image ```shell # China-Hangzhou image docker pull registry.cn-
-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull registry.us-west-
-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This section introduces
-basic usage, see the [Documentation](#-documentation) section for more ways to
-use. ### Web-UI ```shell swift web-ui ``` ### Training #### Training Scripts
-You can refer to the following scripts to customize your own training script. -
-full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat]
+install 'ms-swift[all]' -U # LLM only pip install 'ms-swift[llm]' -U # AIGC
+only pip install 'ms-swift[aigc]' -U # Adapters only pip install ms-swift -
+U ``` - Method 2: Install SWIFT through source code (convenient for running
+training and inference scripts), please run the following commands: ```shell
+git clone https://github.com/modelscope/swift.git cd swift pip install -e '.
+[llm]' ``` SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3:
+Use SWIFT in our Docker image ```shell # China-Hangzhou image docker pull
+registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
+cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull
+registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
+cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This
+section introduces basic usage, see the [Documentation](#-documentation)
+section for more ways to use. ### Web-UI ```shell swift web-ui ``` ### Training
+#### Training Scripts You can refer to the following scripts to customize your
+own training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
+swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100),
+[qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/
+llm/scripts/qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat](https://
-github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
 //github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
 github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/
 lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/
 main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-
 34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
@@ -326,24 +352,37 @@
 NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
 sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
 Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
 Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
 CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
 dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ ``` #### Deepspeed Training ZeRO2: ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB # Runtime: 0.9 hours
+output \ ``` #### Deepspeed Training Deepspeed supports training of quantized
+GPTQ and AWQ models. ZeRO2: ```shell # Experimental Environment: 4 * A100 # GPU
+Memory Requirement: 4 * 21GB # Runtime: 0.9 hours NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
+output \ --deepspeed default-zero2 \ ``` ZeRO3: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 19GB # Runtime: 3.2 hours
 NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed default-zero2 \ ``` ZeRO3:
-```shell # Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 *
-19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \
-swift sft \ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
-num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
-default-zero3 \ ``` ### Inference Original model: ```shell
+sft_type lora \ --output_dir output \ --deepspeed default-zero3 \ ``` ZeRO3-
+Offload: ```shell # Experimental Environment: 4 * A100 # GPU Memory
+Requirement: 4 * 12GB # Runtime: 60 hours NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_id_or_path AI-ModelScope/
+WizardLM-2-8x22B \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ --deepspeed zero3-offload \ ``` ####
+Multi-node Multi-GPU ```shell # node0 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+NNODES=2 \ NODE_RANK=0 \ MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \
+--model_id_or_path qwen1half-32b-chat \ --sft_type full \ --dataset blossom-
+math-zh \ --output_dir output \ --deepspeed default-zero3 \ # node1
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=1 \
+MASTER_ADDR=xxx.xxx.xxx.xxx \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
+qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
+output \ --deepspeed default-zero3 \ ``` ### Inference Original model: ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
 infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
 load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
 ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
 infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
@@ -355,51 +394,58 @@
 --merge_lora true \ ``` ### Deployment Original model: ```shell
 CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
 ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
 chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
 CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
 ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
 checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
-``` ### Supported Models #### LLMs | Model Type | Model Introduction | Language
-| Model Size | Model Type | |------------------------------------------------|-
------------------------------------------------------------------------|-------
--------------|----------------------------------------|------------------------
-------------------- | | Qwen
+``` ### Supported Models The complete list of supported models and datasets can
+be found at [Supported Models and Datasets List](https://idealab.alibaba-
+inc.com/docs/source/LLM/Supported-Models-and-Datasets.md). #### LLMs | Model
+Type | Model Introduction | Language | Model Size | Model Type | |-------------
+-----------------------------------|-------------------------------------------
+-----------------------------|--------------------|----------------------------
+------------|------------------------------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-72B
 including quantized versions | base model
 chat model
 MoE model
 code model | | ChatGLM2
 ChatGLM3
 Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
 English | 6B | base model
 chat model
-code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
+code model
+long text model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
 github.com/baichuan-inc) | Chinese
 English | 7B-13B
 including quantized versions | base model
 chat model | | Yuan2 | [Langchao Yuan series models](https://github.com/IEIT-
 Yuan) | Chinese
 English | 2B-102B | instruct model | | XVerse | [XVerse series models](https://
 github.com/xverse-ai) | Chinese
 English | 7B-65B | base model
 chat model
 long text model
 MoE model | | LLaMA2 | [LLaMA2 series models](https://github.com/
 facebookresearch/llama) | English | 7B-70B
 including quantized versions | base model
+chat model | | LLaMA3 | [LLaMA3 series models](https://github.com/meta-llama/
+llama3) | English | 8B-70B
+including quantized versions | base model
 chat model | | Mistral
 Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
 English | 7B-22B | base model
 instruct model
 MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
 Chinese
-English | 6B-34B | base model
+English | 6B-34B
+including quantized | base model
 chat model
 long text model | | InternLM
 InternLM2
 InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
 InternLM/InternLM) | Chinese
 English | 1.8B-20B | base model
 chat model
@@ -456,19 +502,28 @@
 300B | base model | | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat)
 | Chinese
 English | 7B-12B | chat model | | dbrx | [databricks](https://github.com/
 databricks/dbrx) | English | 132B | base model
 chat model | | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) |
 Chinese
 English | 13B | base model | | c4ai-command-r | [c4ai](https://cohere.com/
-command) | Multilingual | 35B-104B | chat model | #### MLLMs | Model Type |
-Model Introduction | Language | Model Size | Model Type | |------------------|-
------------------------------------------------------------------------|-------
--------------|-------------------|------------------- | | Qwen-VL | [Tongyi
-Qwen vision model](https://github.com/QwenLM) | Chinese
+command) | Multilingual | 35B-104B | chat model | | WizardLM2 | [WizardLM2
+series models](https://github.com/nlpxucan/WizardLM) | English | 7B-8x22B
+including quantized versions | chat model
+MoE model | | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) |
+Chinese | 7B| base model
+chat model| | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://
+github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model
+chat model
+long text model | | ModelScope-Agent | [ModelScope Agent series models](https:/
+/github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model | ####
+MLLMs | Model Type | Model Introduction | Language | Model Size | Model Type |
+|------------------|-----------------------------------------------------------
+-------------|--------------------|-------------------|------------------- | |
+Qwen-VL | [Tongyi Qwen vision model](https://github.com/QwenLM) | Chinese
 English | 7B
 including quantized versions | base model
 chat model | | Qwen-Audio | [Tongyi Qwen speech model](https://github.com/
 QwenLM) | Chinese
 English | 7B | base model
 chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
 ai) | Chinese
@@ -543,41 +598,36 @@
 series, etc. | After 30 series, BF16 and FlashAttn can be used | | Computing
 cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing cards A10/
 A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð
 Documentation ### Documentation Compiling ```shell make docs # Check docs/
 build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
 --------------------------------------------------------- | | [Using Web-UI]
 (docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
-GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-
-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM
-Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
-(docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
-Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
-Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
-Documentation | Document Name | | ---------------------------------------------
---------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
-parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
-Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
-Supported-models-datasets.md) | | [Runtime Speed and Memory Benchmark](https://
-github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) | ### Best
-Practices | Best Practices Name | | -------------------------------------------
------------------ | | [Agent Fine-Tuning Best Practice](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/
-Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | | [Self-
-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/
-main/docs/source/LLM/
-%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md)
-| | [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/
-source/LLM/
-Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | |
-[Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/
-blob/main/docs/source/Multi-Modal/index.md) | ### Deep Learning Tutorials |
-Tutorial Name | |-------------------------------------------------------------
-- | | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-
-classroom/blob/main/LLM-tutorial/
+GetStarted/Tuners.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md)
+| | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM
+Evaluation](docs/source_en/LLM/LLM-eval.md) | | [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md) | | [LLM Deployment](docs/source_en/LLM/
+VLLM-inference-acceleration-and-deployment.md) | | [DPO Human Alignment
+Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff Training](docs/
+source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference Documentation |
+Document Name | | -----------------------------------------------------------
+- | | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
+| [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-
+datasets.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
+Customization.md) | | [Runtime Speed and Memory Benchmark](docs/source_en/LLM/
+Benchmark.md) | ### Best Practices | Best Practices Name | | ------------------
+------------------------------------------ | | [Agent Fine-Tuning Best
+Practice](docs/source_en/LLM/Agent-best-practice.md) | | [Self-Cognition Fine-
+Tuning Best Practice](docs/source_en/LLM/Self-cognition-best-practice.md) | |
+[Qwen1.5 Best Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) | |
+[Multi-Modal Model Training Best Practice](docs/source_en/Multi-Modal/index.md)
+| | [NPU Best Practice](docs/source_en/LLM/NPU-best-practice.md) | ### Deep
+Learning Tutorials | Tutorial Name | |-----------------------------------------
+--------------------- | | [Introduction to Deep Learning](https://github.com/
+modelscope/modelscope-classroom/blob/main/LLM-tutorial/
 A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
 | | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/
 B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
 | | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
 prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
```

### Comparing `ms-swift-2.0.2/README.md` & `ms-swift-2.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,22 @@
 SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
 
 To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
 
 Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
 
 ## 🎉 News
+- 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series models. This includes：chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-13b along with their corresponding 16k and 64k long text versions.
+- 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-6b-128k, Openbuddy-Llama3.
+- 2024.04.20: Support for inference, fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train.
+- 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-best-practice.md).
+- 2024.04.19: Support for inference, fine-tuning, and deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train.
+- 2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided default zero3-offload configuration file for zero3+cpu offload usage.
+- 2024.04.18: Supported compatibility with HuggingFace ecosystem using the environment variable `USE_HF`, switching to use models and datasets from HF. Please refer to the [HuggingFace ecosystem compatibility documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md).
+- 2024.04.17: Support the evaluation for OpenAI standard interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-line-parameters.md#eval-parameters) for details.
 - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
 - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
 - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
 - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
 - 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
 - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train.
 - 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
@@ -52,25 +60,25 @@
 - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
 - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
 - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
 - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
 - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
 - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
 - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
+<details><summary>More</summary>
+
 - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
 - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
 - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
 - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
 - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
 - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
 - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
 - 🔥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start training.
 - 2024.02.25: Support `swift export` to quantize models using **AWQ/GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/source_en/LLM/LLM-quantization.md).
-<details><summary>More</summary>
-
 - 2024.02.22: Support gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct.
 - 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
 - 🔥2024.02.05: Support **Qwen1.5** series models, see [model list](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B) for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8).
 - 2024.02.05: Support training of diffusion models such as **SDXL**, **SD**, **ControlNet**, as well as **DreamBooth** training. See corresponding [training scripts](https://github.com/modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details.
 - 2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat.
 - 🔥2024.02.01: Support dataset mixing to reduce **catastrophic forgetting**. Use `--train_dataset_mix_ratio 2.0` to enable training! We also open sourced the general knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/iic/ms_bench/summary).
 - 🔥2024.02.01: Support Agent training! Agent training algorithm is derived from this [paper](https://arxiv.org/pdf/2309.00986.pdf). We also added [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/summary), a high-quality agent dataset. Use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/sft.sh) to start Agent training!
@@ -133,29 +141,29 @@
 
 SWIFT runs in the Python environment. Please ensure your Python version is higher than 3.8.
 
 - Method 1: Install SWIFT using pip command:
 
 ```shell
 # Full capabilities
-pip install ms-swift[all] -U
+pip install 'ms-swift[all]' -U
 # LLM only
-pip install ms-swift[llm] -U
+pip install 'ms-swift[llm]' -U
 # AIGC only
-pip install ms-swift[aigc] -U
+pip install 'ms-swift[aigc]' -U
 # Adapters only
 pip install ms-swift -U
 ```
 
 - Method 2: Install SWIFT through source code (convenient for running training and inference scripts), please run the following commands:
 
 ```shell
 git clone https://github.com/modelscope/swift.git
 cd swift
-pip install -e .[llm]
+pip install -e '.[llm]'
 ```
 
 SWIFT depends on torch>=1.13, recommend torch>=2.0.0.
 
 - Method 3: Use SWIFT in our Docker image
 
 ```shell
@@ -280,14 +288,15 @@
     --dataset blossom-math-zh \
     --num_train_epochs 5 \
     --sft_type lora \
     --output_dir output \
 ```
 
 #### Deepspeed Training
+Deepspeed supports training of quantized GPTQ and AWQ models.
 
 ZeRO2:
 ```shell
 # Experimental Environment: 4 * A100
 # GPU Memory Requirement: 4 * 21GB
 # Runtime: 0.9 hours
 NPROC_PER_NODE=4 \
@@ -313,14 +322,61 @@
     --dataset blossom-math-zh \
     --num_train_epochs 5 \
     --sft_type lora \
     --output_dir output \
     --deepspeed default-zero3 \
 ```
 
+ZeRO3-Offload:
+```shell
+# Experimental Environment: 4 * A100
+# GPU Memory Requirement: 4 * 12GB
+# Runtime: 60 hours
+NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \
+swift sft \
+    --model_id_or_path AI-ModelScope/WizardLM-2-8x22B \
+    --dataset blossom-math-zh \
+    --num_train_epochs 5 \
+    --sft_type lora \
+    --output_dir output \
+    --deepspeed zero3-offload \
+```
+
+
+#### Multi-node Multi-GPU
+```shell
+# node0
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+NNODES=2 \
+NODE_RANK=0 \
+MASTER_ADDR=127.0.0.1 \
+NPROC_PER_NODE=8 \
+swift sft \
+    --model_id_or_path qwen1half-32b-chat \
+    --sft_type full \
+    --dataset blossom-math-zh \
+    --output_dir output \
+    --deepspeed default-zero3 \
+
+# node1
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+NNODES=2 \
+NODE_RANK=1 \
+MASTER_ADDR=xxx.xxx.xxx.xxx \
+NPROC_PER_NODE=8 \
+swift sft \
+    --model_id_or_path qwen1half-32b-chat \
+    --sft_type full \
+    --dataset blossom-math-zh \
+    --output_dir output \
+    --deepspeed default-zero3 \
+```
+
+
 ### Inference
 Original model:
 ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
 # use VLLM
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
     --infer_backend vllm --max_model_len 8192
@@ -373,27 +429,29 @@
 # 使用VLLM加速
 CUDA_VISIBLE_DEVICES=0 swift deploy \
     --ckpt_dir xxx/checkpoint-xxx --merge_lora true \
     --infer_backend vllm --max_model_len 8192
 ```
 
 ### Supported Models
+The complete list of supported models and datasets can be found at [Supported Models and Datasets List](https://idealab.alibaba-inc.com/docs/source/LLM/Supported-Models-and-Datasets.md).
 
 #### LLMs
 
 | Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
 |------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
 | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model<br>code model                      |
-| ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
+| ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model<br>long text model  |
 | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
 | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
 | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
 | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
+| LLaMA3                   | [LLaMA3 series models](https://github.com/meta-llama/llama3)  | English       | 8B-70B<br>including quantized versions      | base model<br>chat model              |
 | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
-| YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
+| YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
 | InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
 | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
 | MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
 | Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
 | MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
 | OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
 | Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
@@ -408,15 +466,18 @@
 | CodeFuse-CodeLLaMA<br>CodeFuse-Codegeex2<br>CodeFuse-Qwen | [Ant CodeFuse series models](https://github.com/codefuse-ai)        | Chinese<br>English    | 6B-34B                                 | chat model<br>code model                      |
 | phi2                                           | Microsoft's PHI2 model                                                 | English            | 3B                                     | base model<br>code model                          |
 | Grok | [X-ai](https://github.com/xai-org/grok-1) | English | 300B | base model |
 | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat) | Chinese<br>English | 7B-12B | chat model |
 | dbrx | [databricks](https://github.com/databricks/dbrx) | English | 132B | base model<br>chat model  |
 | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) | Chinese<br>English | 13B | base model  |
 | c4ai-command-r | [c4ai](https://cohere.com/command) | Multilingual | 35B-104B | chat model  |
-
+| WizardLM2 | [WizardLM2 series models](https://github.com/nlpxucan/WizardLM) | English | 7B-8x22B<br>including quantized versions | chat model<br>MoE model |
+| Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) | Chinese | 7B| base model<br>chat model|
+| Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model<br>chat model<br>long text model |
+| ModelScope-Agent | [ModelScope Agent series models](https://github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model |
 
 #### MLLMs
 
 | Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
 |------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
 | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
 | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
@@ -493,38 +554,41 @@
 
 ### User Guide
 
 | Document Name                                                |
 | ------------------------------------------------------------ |
 | [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
 | [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
-| [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
 | [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
+| [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
+| [LLM Evaluation](docs/source_en/LLM/LLM-eval.md)     |
 | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
 | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
 | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
 | [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
 
 ### Reference Documentation
 | Document Name                                                |
 | ------------------------------------------------------------ |
 | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
-| [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
 | [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
-| [Runtime Speed and Memory Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) |
+| [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
+| [Runtime Speed and Memory Benchmark](docs/source_en/LLM/Benchmark.md) |
 
 
 ### Best Practices
 
 | Best Practices Name                                                |
 | ------------------------------------------------------------ |
-| [Agent Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-| [Self-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-|  [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-|  [Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/Multi-Modal/index.md) |
+| [Agent Fine-Tuning Best Practice](docs/source_en/LLM/Agent-best-practice.md) |
+| [Self-Cognition Fine-Tuning Best Practice](docs/source_en/LLM/Self-cognition-best-practice.md) |
+|  [Qwen1.5 Best Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) |
+|  [Multi-Modal Model Training Best Practice](docs/source_en/Multi-Modal/index.md) |
+|  [NPU Best Practice](docs/source_en/LLM/NPU-best-practice.md) |
+
 
 ### Deep Learning Tutorials
 
 | Tutorial Name                                                |
 |-------------------------------------------------------------- |
 | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md) |
 | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md) |
```

#### html2text {}

```diff
@@ -22,41 +22,67 @@
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
 support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- ð¥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B,
-CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://
-github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-codeqwen1half_7b_chat/lora/sft.sh) to train. - 2024.04.16: Supports inference
-and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to
-[here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
-Modal/llava-best-practice.md). - 2024.04.13: Support the fine-tuning and
-inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/
-modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/
-lora_ddp_ds/sft.sh) to start training! - 2024.04.13: Support the newly launched
-**MiniCPM** series: MiniCPM-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and
-MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start
-training! - ð¥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval
-datasets(also user custom eval datasets) with one command! Check [this
-documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we
-support a trick way to do multiple ablation experiments, check [this
-documentation](docs/source_en/LLM/LLM-exp.md) to use. - ð¥2024.04.11: Support
-**c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this
+- 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-
+llama-alpaca-2** series models. This includesï¼chinese-llama-2-1.3b, chinese-
+llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and
+chinese-alpaca-2-13b along with their corresponding 16k and 64k long text
+versions. - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-
+Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning
+of chatglm3-6b-128k, Openbuddy-Llama3. - 2024.04.20: Support for inference,
+fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B
+and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/
+main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train. -
+2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and
+inference with NPU, please refer to [NPU Inference and Fine-tuning Best
+Practices](docs/source_en/LLM/NPU-best-practice.md). - 2024.04.19: Support for
+inference, fine-tuning, and deployment of **Llama3** series models. This
+includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-
+Instruct. use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train. -
+2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-
+awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed
+zero3-offload` and provided default zero3-offload configuration file for
+zero3+cpu offload usage. - 2024.04.18: Supported compatibility with HuggingFace
+ecosystem using the environment variable `USE_HF`, switching to use models and
+datasets from HF. Please refer to the [HuggingFace ecosystem compatibility
+documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/
+LLM/Compat-HF.md). - 2024.04.17: Support the evaluation for OpenAI standard
+interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-
+line-parameters.md#eval-parameters) for details. - ð¥2024.04.17: Support
+**CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-
+Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train. -
+2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For
+best practice, you can refer to [here](https://github.com/modelscope/swift/
+tree/main/docs/source_en/Multi-Modal/llava-best-practice.md). - 2024.04.13:
+Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this
 script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
-scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. - 2024.04.10: Use SWIFT
-to fine-tune the qwen-7b-chat model to enhance its function call capabilities,
-and combine it with [Modelscope-Agent](https://github.com/modelscope/
-modelscope-agent) for best practices, which can be found [here](https://
-github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-
-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support ruozhiba
-dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training! -
+2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-
+2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
+(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
+Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
+with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
+for details. Meanwhile, we support a trick way to do multiple ablation
+experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
+- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
+command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. -
+2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
+function call capabilities, and combine it with [Modelscope-Agent](https://
+github.com/modelscope/modelscope-agent) for best practices, which can be found
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
+best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
+ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
 Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
 fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
 **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
 (https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
@@ -75,15 +101,15 @@
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
 github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
-practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
+practice.md). More - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -100,17 +126,17 @@
 2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/
 blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start
 training. - ð¥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/
 2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/
 blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start
 training. - 2024.02.25: Support `swift export` to quantize models using **AWQ/
 GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/
-source_en/LLM/LLM-quantization.md). More - 2024.02.22: Support gemma series:
-gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
+source_en/LLM/LLM-quantization.md). - 2024.02.22: Support gemma series: gemma-
+2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-
 instruct, deepseek-math-7b-chat. - ð¥2024.02.05: Support **Qwen1.5** series
 models, see [model list](https://github.com/modelscope/swift/blob/main/docs/
 source/LLM/
 %E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
 for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-
 7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
@@ -255,33 +281,33 @@
 qwen-14b-chat. - 2023.09.18: Support **internlm-20b** series: internlm-20b,
 internlm-20b-chat. - 2023.09.12: Support **MP+DDP** to accelerate full-
 parameter training. - 2023.09.05: Support **openbuddy-llama2-70b-chat**. -
 2023.09.03: Support **baichuan2** series: baichuan2-7b, baichuan2-7b-chat,
 baichuan2-13b, baichuan2-13b-chat. ## ð ï¸ Installation SWIFT runs in the
 Python environment. Please ensure your Python version is higher than 3.8. -
 Method 1: Install SWIFT using pip command: ```shell # Full capabilities pip
-install ms-swift[all] -U # LLM only pip install ms-swift[llm] -U # AIGC only
-pip install ms-swift[aigc] -U # Adapters only pip install ms-swift -U ``` -
-Method 2: Install SWIFT through source code (convenient for running training
-and inference scripts), please run the following commands: ```shell git clone
-https://github.com/modelscope/swift.git cd swift pip install -e .[llm] ```
-SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3: Use SWIFT in
-our Docker image ```shell # China-Hangzhou image docker pull registry.cn-
-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull registry.us-west-
-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This section introduces
-basic usage, see the [Documentation](#-documentation) section for more ways to
-use. ### Web-UI ```shell swift web-ui ``` ### Training #### Training Scripts
-You can refer to the following scripts to customize your own training script. -
-full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat]
+install 'ms-swift[all]' -U # LLM only pip install 'ms-swift[llm]' -U # AIGC
+only pip install 'ms-swift[aigc]' -U # Adapters only pip install ms-swift -
+U ``` - Method 2: Install SWIFT through source code (convenient for running
+training and inference scripts), please run the following commands: ```shell
+git clone https://github.com/modelscope/swift.git cd swift pip install -e '.
+[llm]' ``` SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3:
+Use SWIFT in our Docker image ```shell # China-Hangzhou image docker pull
+registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
+cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull
+registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
+cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This
+section introduces basic usage, see the [Documentation](#-documentation)
+section for more ways to use. ### Web-UI ```shell swift web-ui ``` ### Training
+#### Training Scripts You can refer to the following scripts to customize your
+own training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
+swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100),
+[qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/
+llm/scripts/qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat](https://
-github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
 //github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
 github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/
 lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/
 main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-
 34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
@@ -322,24 +348,37 @@
 NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
 sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
 Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
 Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
 CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
 dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ ``` #### Deepspeed Training ZeRO2: ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB # Runtime: 0.9 hours
+output \ ``` #### Deepspeed Training Deepspeed supports training of quantized
+GPTQ and AWQ models. ZeRO2: ```shell # Experimental Environment: 4 * A100 # GPU
+Memory Requirement: 4 * 21GB # Runtime: 0.9 hours NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
+output \ --deepspeed default-zero2 \ ``` ZeRO3: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 19GB # Runtime: 3.2 hours
 NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed default-zero2 \ ``` ZeRO3:
-```shell # Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 *
-19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \
-swift sft \ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
-num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
-default-zero3 \ ``` ### Inference Original model: ```shell
+sft_type lora \ --output_dir output \ --deepspeed default-zero3 \ ``` ZeRO3-
+Offload: ```shell # Experimental Environment: 4 * A100 # GPU Memory
+Requirement: 4 * 12GB # Runtime: 60 hours NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_id_or_path AI-ModelScope/
+WizardLM-2-8x22B \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ --deepspeed zero3-offload \ ``` ####
+Multi-node Multi-GPU ```shell # node0 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+NNODES=2 \ NODE_RANK=0 \ MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \
+--model_id_or_path qwen1half-32b-chat \ --sft_type full \ --dataset blossom-
+math-zh \ --output_dir output \ --deepspeed default-zero3 \ # node1
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=1 \
+MASTER_ADDR=xxx.xxx.xxx.xxx \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
+qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
+output \ --deepspeed default-zero3 \ ``` ### Inference Original model: ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
 infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
 load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
 ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
 infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
@@ -351,51 +390,58 @@
 --merge_lora true \ ``` ### Deployment Original model: ```shell
 CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
 ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
 chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
 CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
 ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
 checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
-``` ### Supported Models #### LLMs | Model Type | Model Introduction | Language
-| Model Size | Model Type | |------------------------------------------------|-
------------------------------------------------------------------------|-------
--------------|----------------------------------------|------------------------
-------------------- | | Qwen
+``` ### Supported Models The complete list of supported models and datasets can
+be found at [Supported Models and Datasets List](https://idealab.alibaba-
+inc.com/docs/source/LLM/Supported-Models-and-Datasets.md). #### LLMs | Model
+Type | Model Introduction | Language | Model Size | Model Type | |-------------
+-----------------------------------|-------------------------------------------
+-----------------------------|--------------------|----------------------------
+------------|------------------------------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-72B
 including quantized versions | base model
 chat model
 MoE model
 code model | | ChatGLM2
 ChatGLM3
 Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
 English | 6B | base model
 chat model
-code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
+code model
+long text model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
 github.com/baichuan-inc) | Chinese
 English | 7B-13B
 including quantized versions | base model
 chat model | | Yuan2 | [Langchao Yuan series models](https://github.com/IEIT-
 Yuan) | Chinese
 English | 2B-102B | instruct model | | XVerse | [XVerse series models](https://
 github.com/xverse-ai) | Chinese
 English | 7B-65B | base model
 chat model
 long text model
 MoE model | | LLaMA2 | [LLaMA2 series models](https://github.com/
 facebookresearch/llama) | English | 7B-70B
 including quantized versions | base model
+chat model | | LLaMA3 | [LLaMA3 series models](https://github.com/meta-llama/
+llama3) | English | 8B-70B
+including quantized versions | base model
 chat model | | Mistral
 Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
 English | 7B-22B | base model
 instruct model
 MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
 Chinese
-English | 6B-34B | base model
+English | 6B-34B
+including quantized | base model
 chat model
 long text model | | InternLM
 InternLM2
 InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
 InternLM/InternLM) | Chinese
 English | 1.8B-20B | base model
 chat model
@@ -452,19 +498,28 @@
 300B | base model | | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat)
 | Chinese
 English | 7B-12B | chat model | | dbrx | [databricks](https://github.com/
 databricks/dbrx) | English | 132B | base model
 chat model | | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) |
 Chinese
 English | 13B | base model | | c4ai-command-r | [c4ai](https://cohere.com/
-command) | Multilingual | 35B-104B | chat model | #### MLLMs | Model Type |
-Model Introduction | Language | Model Size | Model Type | |------------------|-
------------------------------------------------------------------------|-------
--------------|-------------------|------------------- | | Qwen-VL | [Tongyi
-Qwen vision model](https://github.com/QwenLM) | Chinese
+command) | Multilingual | 35B-104B | chat model | | WizardLM2 | [WizardLM2
+series models](https://github.com/nlpxucan/WizardLM) | English | 7B-8x22B
+including quantized versions | chat model
+MoE model | | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) |
+Chinese | 7B| base model
+chat model| | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://
+github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model
+chat model
+long text model | | ModelScope-Agent | [ModelScope Agent series models](https:/
+/github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model | ####
+MLLMs | Model Type | Model Introduction | Language | Model Size | Model Type |
+|------------------|-----------------------------------------------------------
+-------------|--------------------|-------------------|------------------- | |
+Qwen-VL | [Tongyi Qwen vision model](https://github.com/QwenLM) | Chinese
 English | 7B
 including quantized versions | base model
 chat model | | Qwen-Audio | [Tongyi Qwen speech model](https://github.com/
 QwenLM) | Chinese
 English | 7B | base model
 chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
 ai) | Chinese
@@ -539,41 +594,36 @@
 series, etc. | After 30 series, BF16 and FlashAttn can be used | | Computing
 cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing cards A10/
 A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð
 Documentation ### Documentation Compiling ```shell make docs # Check docs/
 build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
 --------------------------------------------------------- | | [Using Web-UI]
 (docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
-GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-
-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM
-Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
-(docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
-Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
-Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
-Documentation | Document Name | | ---------------------------------------------
---------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
-parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
-Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
-Supported-models-datasets.md) | | [Runtime Speed and Memory Benchmark](https://
-github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) | ### Best
-Practices | Best Practices Name | | -------------------------------------------
------------------ | | [Agent Fine-Tuning Best Practice](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/
-Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | | [Self-
-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/
-main/docs/source/LLM/
-%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md)
-| | [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/
-source/LLM/
-Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | |
-[Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/
-blob/main/docs/source/Multi-Modal/index.md) | ### Deep Learning Tutorials |
-Tutorial Name | |-------------------------------------------------------------
-- | | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-
-classroom/blob/main/LLM-tutorial/
+GetStarted/Tuners.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md)
+| | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM
+Evaluation](docs/source_en/LLM/LLM-eval.md) | | [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md) | | [LLM Deployment](docs/source_en/LLM/
+VLLM-inference-acceleration-and-deployment.md) | | [DPO Human Alignment
+Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff Training](docs/
+source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference Documentation |
+Document Name | | -----------------------------------------------------------
+- | | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
+| [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-
+datasets.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
+Customization.md) | | [Runtime Speed and Memory Benchmark](docs/source_en/LLM/
+Benchmark.md) | ### Best Practices | Best Practices Name | | ------------------
+------------------------------------------ | | [Agent Fine-Tuning Best
+Practice](docs/source_en/LLM/Agent-best-practice.md) | | [Self-Cognition Fine-
+Tuning Best Practice](docs/source_en/LLM/Self-cognition-best-practice.md) | |
+[Qwen1.5 Best Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) | |
+[Multi-Modal Model Training Best Practice](docs/source_en/Multi-Modal/index.md)
+| | [NPU Best Practice](docs/source_en/LLM/NPU-best-practice.md) | ### Deep
+Learning Tutorials | Tutorial Name | |-----------------------------------------
+--------------------- | | [Introduction to Deep Learning](https://github.com/
+modelscope/modelscope-classroom/blob/main/LLM-tutorial/
 A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
 | | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/
 B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
 | | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
 prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
```

### Comparing `ms-swift-2.0.2/ms_swift.egg-info/PKG-INFO` & `ms-swift-2.0.3/ms_swift.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-swift
-Version: 2.0.2
+Version: 2.0.3
 Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
 Home-page: https://github.com/modelscope/swift
 Author: DAMO ModelScope teams
 Author-email: contact@modelscope.cn
 License: Apache License 2.0
 Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
         
@@ -43,14 +43,22 @@
         SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
         
         To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
         
         Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
         
         ## 🎉 News
+        - 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series models. This includes：chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-13b along with their corresponding 16k and 64k long text versions.
+        - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-6b-128k, Openbuddy-Llama3.
+        - 2024.04.20: Support for inference, fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train.
+        - 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-best-practice.md).
+        - 2024.04.19: Support for inference, fine-tuning, and deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train.
+        - 2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided default zero3-offload configuration file for zero3+cpu offload usage.
+        - 2024.04.18: Supported compatibility with HuggingFace ecosystem using the environment variable `USE_HF`, switching to use models and datasets from HF. Please refer to the [HuggingFace ecosystem compatibility documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md).
+        - 2024.04.17: Support the evaluation for OpenAI standard interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-line-parameters.md#eval-parameters) for details.
         - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
         - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
         - 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
         - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train.
         - 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
@@ -60,25 +68,25 @@
         - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
         - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
         - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
         - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
         - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
         - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
         - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
+        <details><summary>More</summary>
+        
         - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
         - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
         - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
         - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
         - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
         - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
         - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
         - 🔥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start training.
         - 2024.02.25: Support `swift export` to quantize models using **AWQ/GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/source_en/LLM/LLM-quantization.md).
-        <details><summary>More</summary>
-        
         - 2024.02.22: Support gemma series: gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct.
         - 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-instruct, deepseek-math-7b-chat.
         - 🔥2024.02.05: Support **Qwen1.5** series models, see [model list](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B) for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat), [qwen1half-7b-chat-int8](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_int8).
         - 2024.02.05: Support training of diffusion models such as **SDXL**, **SD**, **ControlNet**, as well as **DreamBooth** training. See corresponding [training scripts](https://github.com/modelscope/swift/tree/main/examples/pytorch/sdxl/scripts) for details.
         - 2024.02.01: Support minicpm series: [minicpm-2b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/minicpm_2b_sft_chat), minicpm-2b-chat.
         - 🔥2024.02.01: Support dataset mixing to reduce **catastrophic forgetting**. Use `--train_dataset_mix_ratio 2.0` to enable training! We also open sourced the general knowledge dataset [ms-bench](https://www.modelscope.cn/datasets/iic/ms_bench/summary).
         - 🔥2024.02.01: Support Agent training! Agent training algorithm is derived from this [paper](https://arxiv.org/pdf/2309.00986.pdf). We also added [ms-agent](https://www.modelscope.cn/datasets/iic/ms_agent/summary), a high-quality agent dataset. Use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen_7b_chat/lora/sft.sh) to start Agent training!
@@ -141,29 +149,29 @@
         
         SWIFT runs in the Python environment. Please ensure your Python version is higher than 3.8.
         
         - Method 1: Install SWIFT using pip command:
         
         ```shell
         # Full capabilities
-        pip install ms-swift[all] -U
+        pip install 'ms-swift[all]' -U
         # LLM only
-        pip install ms-swift[llm] -U
+        pip install 'ms-swift[llm]' -U
         # AIGC only
-        pip install ms-swift[aigc] -U
+        pip install 'ms-swift[aigc]' -U
         # Adapters only
         pip install ms-swift -U
         ```
         
         - Method 2: Install SWIFT through source code (convenient for running training and inference scripts), please run the following commands:
         
         ```shell
         git clone https://github.com/modelscope/swift.git
         cd swift
-        pip install -e .[llm]
+        pip install -e '.[llm]'
         ```
         
         SWIFT depends on torch>=1.13, recommend torch>=2.0.0.
         
         - Method 3: Use SWIFT in our Docker image
         
         ```shell
@@ -288,14 +296,15 @@
             --dataset blossom-math-zh \
             --num_train_epochs 5 \
             --sft_type lora \
             --output_dir output \
         ```
         
         #### Deepspeed Training
+        Deepspeed supports training of quantized GPTQ and AWQ models.
         
         ZeRO2:
         ```shell
         # Experimental Environment: 4 * A100
         # GPU Memory Requirement: 4 * 21GB
         # Runtime: 0.9 hours
         NPROC_PER_NODE=4 \
@@ -321,14 +330,61 @@
             --dataset blossom-math-zh \
             --num_train_epochs 5 \
             --sft_type lora \
             --output_dir output \
             --deepspeed default-zero3 \
         ```
         
+        ZeRO3-Offload:
+        ```shell
+        # Experimental Environment: 4 * A100
+        # GPU Memory Requirement: 4 * 12GB
+        # Runtime: 60 hours
+        NPROC_PER_NODE=4 \
+        CUDA_VISIBLE_DEVICES=0,1,2,3 \
+        swift sft \
+            --model_id_or_path AI-ModelScope/WizardLM-2-8x22B \
+            --dataset blossom-math-zh \
+            --num_train_epochs 5 \
+            --sft_type lora \
+            --output_dir output \
+            --deepspeed zero3-offload \
+        ```
+        
+        
+        #### Multi-node Multi-GPU
+        ```shell
+        # node0
+        CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+        NNODES=2 \
+        NODE_RANK=0 \
+        MASTER_ADDR=127.0.0.1 \
+        NPROC_PER_NODE=8 \
+        swift sft \
+            --model_id_or_path qwen1half-32b-chat \
+            --sft_type full \
+            --dataset blossom-math-zh \
+            --output_dir output \
+            --deepspeed default-zero3 \
+        
+        # node1
+        CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+        NNODES=2 \
+        NODE_RANK=1 \
+        MASTER_ADDR=xxx.xxx.xxx.xxx \
+        NPROC_PER_NODE=8 \
+        swift sft \
+            --model_id_or_path qwen1half-32b-chat \
+            --sft_type full \
+            --dataset blossom-math-zh \
+            --output_dir output \
+            --deepspeed default-zero3 \
+        ```
+        
+        
         ### Inference
         Original model:
         ```shell
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
         # use VLLM
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
             --infer_backend vllm --max_model_len 8192
@@ -381,27 +437,29 @@
         # 使用VLLM加速
         CUDA_VISIBLE_DEVICES=0 swift deploy \
             --ckpt_dir xxx/checkpoint-xxx --merge_lora true \
             --infer_backend vllm --max_model_len 8192
         ```
         
         ### Supported Models
+        The complete list of supported models and datasets can be found at [Supported Models and Datasets List](https://idealab.alibaba-inc.com/docs/source/LLM/Supported-Models-and-Datasets.md).
         
         #### LLMs
         
         | Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
         |------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
         | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model<br>code model                      |
-        | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
+        | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model<br>long text model  |
         | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
         | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
         | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
         | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
+        | LLaMA3                   | [LLaMA3 series models](https://github.com/meta-llama/llama3)  | English       | 8B-70B<br>including quantized versions      | base model<br>chat model              |
         | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
-        | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
+        | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
         | InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
         | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
         | MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
         | Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
         | MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
         | OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
         | Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
@@ -416,15 +474,18 @@
         | CodeFuse-CodeLLaMA<br>CodeFuse-Codegeex2<br>CodeFuse-Qwen | [Ant CodeFuse series models](https://github.com/codefuse-ai)        | Chinese<br>English    | 6B-34B                                 | chat model<br>code model                      |
         | phi2                                           | Microsoft's PHI2 model                                                 | English            | 3B                                     | base model<br>code model                          |
         | Grok | [X-ai](https://github.com/xai-org/grok-1) | English | 300B | base model |
         | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat) | Chinese<br>English | 7B-12B | chat model |
         | dbrx | [databricks](https://github.com/databricks/dbrx) | English | 132B | base model<br>chat model  |
         | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) | Chinese<br>English | 13B | base model  |
         | c4ai-command-r | [c4ai](https://cohere.com/command) | Multilingual | 35B-104B | chat model  |
-        
+        | WizardLM2 | [WizardLM2 series models](https://github.com/nlpxucan/WizardLM) | English | 7B-8x22B<br>including quantized versions | chat model<br>MoE model |
+        | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) | Chinese | 7B| base model<br>chat model|
+        | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model<br>chat model<br>long text model |
+        | ModelScope-Agent | [ModelScope Agent series models](https://github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model |
         
         #### MLLMs
         
         | Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
         |------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
         | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
         | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
@@ -501,38 +562,41 @@
         
         ### User Guide
         
         | Document Name                                                |
         | ------------------------------------------------------------ |
         | [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
         | [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
-        | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
         | [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
+        | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
+        | [LLM Evaluation](docs/source_en/LLM/LLM-eval.md)     |
         | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
         | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
         | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
         | [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
         
         ### Reference Documentation
         | Document Name                                                |
         | ------------------------------------------------------------ |
         | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
-        | [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
         | [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
-        | [Runtime Speed and Memory Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) |
+        | [Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) |
+        | [Runtime Speed and Memory Benchmark](docs/source_en/LLM/Benchmark.md) |
         
         
         ### Best Practices
         
         | Best Practices Name                                                |
         | ------------------------------------------------------------ |
-        | [Agent Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-        | [Self-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-        |  [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) |
-        |  [Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/blob/main/docs/source/Multi-Modal/index.md) |
+        | [Agent Fine-Tuning Best Practice](docs/source_en/LLM/Agent-best-practice.md) |
+        | [Self-Cognition Fine-Tuning Best Practice](docs/source_en/LLM/Self-cognition-best-practice.md) |
+        |  [Qwen1.5 Best Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) |
+        |  [Multi-Modal Model Training Best Practice](docs/source_en/Multi-Modal/index.md) |
+        |  [NPU Best Practice](docs/source_en/LLM/NPU-best-practice.md) |
+        
         
         ### Deep Learning Tutorials
         
         | Tutorial Name                                                |
         |-------------------------------------------------------------- |
         | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md) |
         | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/blob/main/LLM-tutorial/B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 2.0.2 Summary: Swift: Scalable
+Metadata-Version: 2.1 Name: ms-swift Version: 2.0.3 Summary: Swift: Scalable
 lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
 modelscope/swift Author: DAMO ModelScope teams Author-email:
 contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
 (Scalable lightWeight Infrastructure for Fine-Tuning)
 
                             [resources/banner.png]
                          _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
@@ -26,41 +26,67 @@
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
 support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- ð¥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B,
-CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://
-github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-codeqwen1half_7b_chat/lora/sft.sh) to train. - 2024.04.16: Supports inference
-and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to
-[here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
-Modal/llava-best-practice.md). - 2024.04.13: Support the fine-tuning and
-inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/
-modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/
-lora_ddp_ds/sft.sh) to start training! - 2024.04.13: Support the newly launched
-**MiniCPM** series: MiniCPM-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and
-MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start
-training! - ð¥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval
-datasets(also user custom eval datasets) with one command! Check [this
-documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we
-support a trick way to do multiple ablation experiments, check [this
-documentation](docs/source_en/LLM/LLM-exp.md) to use. - ð¥2024.04.11: Support
-**c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this
+- 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-
+llama-alpaca-2** series models. This includesï¼chinese-llama-2-1.3b, chinese-
+llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and
+chinese-alpaca-2-13b along with their corresponding 16k and 64k long text
+versions. - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-
+Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning
+of chatglm3-6b-128k, Openbuddy-Llama3. - 2024.04.20: Support for inference,
+fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B
+and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/
+main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train. -
+2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and
+inference with NPU, please refer to [NPU Inference and Fine-tuning Best
+Practices](docs/source_en/LLM/NPU-best-practice.md). - 2024.04.19: Support for
+inference, fine-tuning, and deployment of **Llama3** series models. This
+includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-
+Instruct. use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train. -
+2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-
+awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed
+zero3-offload` and provided default zero3-offload configuration file for
+zero3+cpu offload usage. - 2024.04.18: Supported compatibility with HuggingFace
+ecosystem using the environment variable `USE_HF`, switching to use models and
+datasets from HF. Please refer to the [HuggingFace ecosystem compatibility
+documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/
+LLM/Compat-HF.md). - 2024.04.17: Support the evaluation for OpenAI standard
+interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-
+line-parameters.md#eval-parameters) for details. - ð¥2024.04.17: Support
+**CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-
+Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train. -
+2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For
+best practice, you can refer to [here](https://github.com/modelscope/swift/
+tree/main/docs/source_en/Multi-Modal/llava-best-practice.md). - 2024.04.13:
+Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this
 script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
-scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. - 2024.04.10: Use SWIFT
-to fine-tune the qwen-7b-chat model to enhance its function call capabilities,
-and combine it with [Modelscope-Agent](https://github.com/modelscope/
-modelscope-agent) for best practices, which can be found [here](https://
-github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-
-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support ruozhiba
-dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training! -
+2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-
+2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
+(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
+Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
+with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
+for details. Meanwhile, we support a trick way to do multiple ablation
+experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
+- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
+command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. -
+2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
+function call capabilities, and combine it with [Modelscope-Agent](https://
+github.com/modelscope/modelscope-agent) for best practices, which can be found
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
+best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
+ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
 Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
 fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
 **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
 (https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
@@ -79,15 +105,15 @@
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
 github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
-practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
+practice.md). More - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -104,17 +130,17 @@
 2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/
 blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start
 training. - ð¥2024.02.29: Support [LoRA+](https://arxiv.org/pdf/
 2402.12354.pdf), simply use [this script](https://github.com/modelscope/swift/
 blob/main/examples/pytorch/llm/scripts/yi_6b_chat/lorap/sft.sh) to start
 training. - 2024.02.25: Support `swift export` to quantize models using **AWQ/
 GPTQ** and push to ModelScope Hub. See documentation: [LLM Quantization](docs/
-source_en/LLM/LLM-quantization.md). More - 2024.02.22: Support gemma series:
-gemma-2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
+source_en/LLM/LLM-quantization.md). - 2024.02.22: Support gemma series: gemma-
+2b, [gemma-2b-instruct](https://github.com/modelscope/swift/tree/main/examples/
+pytorch/llm/scripts/gemma_2b_instruct), gemma-7b, gemma-7b-instruct. -
 2024.02.16: Support deepseek-math series: deepseek-math-7b, deepseek-math-7b-
 instruct, deepseek-math-7b-chat. - ð¥2024.02.05: Support **Qwen1.5** series
 models, see [model list](https://github.com/modelscope/swift/blob/main/docs/
 source/LLM/
 %E6%94%AF%E6%8C%81%E7%9A%84%E6%A8%A1%E5%9E%8B%E5%92%8C%E6%95%B0%E6%8D%AE%E9%9B%86.md#%E6%A8%A1%E5%9E%8B)
 for all supported Qwen1.5 models. Provide fine-tuning scripts for [qwen1half-
 7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
@@ -259,33 +285,33 @@
 qwen-14b-chat. - 2023.09.18: Support **internlm-20b** series: internlm-20b,
 internlm-20b-chat. - 2023.09.12: Support **MP+DDP** to accelerate full-
 parameter training. - 2023.09.05: Support **openbuddy-llama2-70b-chat**. -
 2023.09.03: Support **baichuan2** series: baichuan2-7b, baichuan2-7b-chat,
 baichuan2-13b, baichuan2-13b-chat. ## ð ï¸ Installation SWIFT runs in the
 Python environment. Please ensure your Python version is higher than 3.8. -
 Method 1: Install SWIFT using pip command: ```shell # Full capabilities pip
-install ms-swift[all] -U # LLM only pip install ms-swift[llm] -U # AIGC only
-pip install ms-swift[aigc] -U # Adapters only pip install ms-swift -U ``` -
-Method 2: Install SWIFT through source code (convenient for running training
-and inference scripts), please run the following commands: ```shell git clone
-https://github.com/modelscope/swift.git cd swift pip install -e .[llm] ```
-SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3: Use SWIFT in
-our Docker image ```shell # China-Hangzhou image docker pull registry.cn-
-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull registry.us-west-
-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-cuda12.1.0-py310-
-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This section introduces
-basic usage, see the [Documentation](#-documentation) section for more ways to
-use. ### Web-UI ```shell swift web-ui ``` ### Training #### Training Scripts
-You can refer to the following scripts to customize your own training script. -
-full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/
-examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat]
+install 'ms-swift[all]' -U # LLM only pip install 'ms-swift[llm]' -U # AIGC
+only pip install 'ms-swift[aigc]' -U # Adapters only pip install ms-swift -
+U ``` - Method 2: Install SWIFT through source code (convenient for running
+training and inference scripts), please run the following commands: ```shell
+git clone https://github.com/modelscope/swift.git cd swift pip install -e '.
+[llm]' ``` SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3:
+Use SWIFT in our Docker image ```shell # China-Hangzhou image docker pull
+registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
+cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull
+registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
+cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This
+section introduces basic usage, see the [Documentation](#-documentation)
+section for more ways to use. ### Web-UI ```shell swift web-ui ``` ### Training
+#### Training Scripts You can refer to the following scripts to customize your
+own training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
+swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100),
+[qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/
+llm/scripts/qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat](https://
-github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
 //github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
 github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/chatglm3_6b/
 lora) (3090), [baichuan2-13b-chat](https://github.com/modelscope/swift/tree/
 main/examples/pytorch/llm/scripts/baichuan2_13b_chat/lora_mp) (2\*3090), [yi-
 34b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
@@ -326,24 +352,37 @@
 NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
 sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
 Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
 Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
 CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
 dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ ``` #### Deepspeed Training ZeRO2: ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB # Runtime: 0.9 hours
+output \ ``` #### Deepspeed Training Deepspeed supports training of quantized
+GPTQ and AWQ models. ZeRO2: ```shell # Experimental Environment: 4 * A100 # GPU
+Memory Requirement: 4 * 21GB # Runtime: 0.9 hours NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
+output \ --deepspeed default-zero2 \ ``` ZeRO3: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 19GB # Runtime: 3.2 hours
 NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed default-zero2 \ ``` ZeRO3:
-```shell # Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 *
-19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \
-swift sft \ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
-num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
-default-zero3 \ ``` ### Inference Original model: ```shell
+sft_type lora \ --output_dir output \ --deepspeed default-zero3 \ ``` ZeRO3-
+Offload: ```shell # Experimental Environment: 4 * A100 # GPU Memory
+Requirement: 4 * 12GB # Runtime: 60 hours NPROC_PER_NODE=4 \
+CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_id_or_path AI-ModelScope/
+WizardLM-2-8x22B \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ --deepspeed zero3-offload \ ``` ####
+Multi-node Multi-GPU ```shell # node0 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
+NNODES=2 \ NODE_RANK=0 \ MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \
+--model_id_or_path qwen1half-32b-chat \ --sft_type full \ --dataset blossom-
+math-zh \ --output_dir output \ --deepspeed default-zero3 \ # node1
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=1 \
+MASTER_ADDR=xxx.xxx.xxx.xxx \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
+qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
+output \ --deepspeed default-zero3 \ ``` ### Inference Original model: ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
 infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
 load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
 ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
 infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
@@ -355,51 +394,58 @@
 --merge_lora true \ ``` ### Deployment Original model: ```shell
 CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
 ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
 chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
 CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
 ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
 checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
-``` ### Supported Models #### LLMs | Model Type | Model Introduction | Language
-| Model Size | Model Type | |------------------------------------------------|-
------------------------------------------------------------------------|-------
--------------|----------------------------------------|------------------------
-------------------- | | Qwen
+``` ### Supported Models The complete list of supported models and datasets can
+be found at [Supported Models and Datasets List](https://idealab.alibaba-
+inc.com/docs/source/LLM/Supported-Models-and-Datasets.md). #### LLMs | Model
+Type | Model Introduction | Language | Model Size | Model Type | |-------------
+-----------------------------------|-------------------------------------------
+-----------------------------|--------------------|----------------------------
+------------|------------------------------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-72B
 including quantized versions | base model
 chat model
 MoE model
 code model | | ChatGLM2
 ChatGLM3
 Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
 English | 6B | base model
 chat model
-code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
+code model
+long text model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
 github.com/baichuan-inc) | Chinese
 English | 7B-13B
 including quantized versions | base model
 chat model | | Yuan2 | [Langchao Yuan series models](https://github.com/IEIT-
 Yuan) | Chinese
 English | 2B-102B | instruct model | | XVerse | [XVerse series models](https://
 github.com/xverse-ai) | Chinese
 English | 7B-65B | base model
 chat model
 long text model
 MoE model | | LLaMA2 | [LLaMA2 series models](https://github.com/
 facebookresearch/llama) | English | 7B-70B
 including quantized versions | base model
+chat model | | LLaMA3 | [LLaMA3 series models](https://github.com/meta-llama/
+llama3) | English | 8B-70B
+including quantized versions | base model
 chat model | | Mistral
 Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
 English | 7B-22B | base model
 instruct model
 MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
 Chinese
-English | 6B-34B | base model
+English | 6B-34B
+including quantized | base model
 chat model
 long text model | | InternLM
 InternLM2
 InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
 InternLM/InternLM) | Chinese
 English | 1.8B-20B | base model
 chat model
@@ -456,19 +502,28 @@
 300B | base model | | TeleChat | [Tele-AI](https://github.com/Tele-AI/Telechat)
 | Chinese
 English | 7B-12B | chat model | | dbrx | [databricks](https://github.com/
 databricks/dbrx) | English | 132B | base model
 chat model | | mengzi3 | [Langboat](https://github.com/Langboat/Mengzi3) |
 Chinese
 English | 13B | base model | | c4ai-command-r | [c4ai](https://cohere.com/
-command) | Multilingual | 35B-104B | chat model | #### MLLMs | Model Type |
-Model Introduction | Language | Model Size | Model Type | |------------------|-
------------------------------------------------------------------------|-------
--------------|-------------------|------------------- | | Qwen-VL | [Tongyi
-Qwen vision model](https://github.com/QwenLM) | Chinese
+command) | Multilingual | 35B-104B | chat model | | WizardLM2 | [WizardLM2
+series models](https://github.com/nlpxucan/WizardLM) | English | 7B-8x22B
+including quantized versions | chat model
+MoE model | | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) |
+Chinese | 7B| base model
+chat model| | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://
+github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model
+chat model
+long text model | | ModelScope-Agent | [ModelScope Agent series models](https:/
+/github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model | ####
+MLLMs | Model Type | Model Introduction | Language | Model Size | Model Type |
+|------------------|-----------------------------------------------------------
+-------------|--------------------|-------------------|------------------- | |
+Qwen-VL | [Tongyi Qwen vision model](https://github.com/QwenLM) | Chinese
 English | 7B
 including quantized versions | base model
 chat model | | Qwen-Audio | [Tongyi Qwen speech model](https://github.com/
 QwenLM) | Chinese
 English | 7B | base model
 chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
 ai) | Chinese
@@ -543,41 +598,36 @@
 series, etc. | After 30 series, BF16 and FlashAttn can be used | | Computing
 cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing cards A10/
 A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð
 Documentation ### Documentation Compiling ```shell make docs # Check docs/
 build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
 --------------------------------------------------------- | | [Using Web-UI]
 (docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
-GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-
-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM
-Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
-(docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
-Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
-Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
-Documentation | Document Name | | ---------------------------------------------
---------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
-parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
-Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
-Supported-models-datasets.md) | | [Runtime Speed and Memory Benchmark](https://
-github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) | ### Best
-Practices | Best Practices Name | | -------------------------------------------
------------------ | | [Agent Fine-Tuning Best Practice](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/
-Agent%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | | [Self-
-Cognition Fine-Tuning Best Practice](https://github.com/modelscope/swift/blob/
-main/docs/source/LLM/
-%E8%87%AA%E6%88%91%E8%AE%A4%E7%9F%A5%E5%BE%AE%E8%B0%83%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md)
-| | [Qwen1.5 Best Practice](https://github.com/modelscope/swift/blob/main/docs/
-source/LLM/
-Qwen1.5%E5%85%A8%E6%B5%81%E7%A8%8B%E6%9C%80%E4%BD%B3%E5%AE%9E%E8%B7%B5.md) | |
-[Multi-Modal Model Training Best Practice](https://github.com/modelscope/swift/
-blob/main/docs/source/Multi-Modal/index.md) | ### Deep Learning Tutorials |
-Tutorial Name | |-------------------------------------------------------------
-- | | [Introduction to Deep Learning](https://github.com/modelscope/modelscope-
-classroom/blob/main/LLM-tutorial/
+GetStarted/Tuners.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md)
+| | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM
+Evaluation](docs/source_en/LLM/LLM-eval.md) | | [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md) | | [LLM Deployment](docs/source_en/LLM/
+VLLM-inference-acceleration-and-deployment.md) | | [DPO Human Alignment
+Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff Training](docs/
+source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference Documentation |
+Document Name | | -----------------------------------------------------------
+- | | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
+| [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-
+datasets.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
+Customization.md) | | [Runtime Speed and Memory Benchmark](docs/source_en/LLM/
+Benchmark.md) | ### Best Practices | Best Practices Name | | ------------------
+------------------------------------------ | | [Agent Fine-Tuning Best
+Practice](docs/source_en/LLM/Agent-best-practice.md) | | [Self-Cognition Fine-
+Tuning Best Practice](docs/source_en/LLM/Self-cognition-best-practice.md) | |
+[Qwen1.5 Best Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) | |
+[Multi-Modal Model Training Best Practice](docs/source_en/Multi-Modal/index.md)
+| | [NPU Best Practice](docs/source_en/LLM/NPU-best-practice.md) | ### Deep
+Learning Tutorials | Tutorial Name | |-----------------------------------------
+--------------------- | | [Introduction to Deep Learning](https://github.com/
+modelscope/modelscope-classroom/blob/main/LLM-tutorial/
 A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
 | | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/
 B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
 | | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
 prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
```

### Comparing `ms-swift-2.0.2/ms_swift.egg-info/SOURCES.txt` & `ms-swift-2.0.3/ms_swift.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 swift/llm/sft.py
 swift/llm/tuner.py
 swift/llm/agent/__init__.py
 swift/llm/agent/utils.py
 swift/llm/data/self_cognition.jsonl
 swift/llm/ds_config/zero2.json
 swift/llm/ds_config/zero3.json
+swift/llm/ds_config/zero3_offload.json
 swift/llm/utils/__init__.py
 swift/llm/utils/argument.py
 swift/llm/utils/client_utils.py
 swift/llm/utils/dataset.py
 swift/llm/utils/model.py
 swift/llm/utils/preprocess.py
 swift/llm/utils/protocol.py
```

### Comparing `ms-swift-2.0.2/ms_swift.egg-info/requires.txt` & `ms-swift-2.0.3/ms_swift.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 accelerate
 dacite
-datasets
+datasets<=2.18
 jieba
 matplotlib
 modelscope>=1.13.3
 nltk
 numpy
 optimum>=1.17.0
 pandas
@@ -23,15 +23,15 @@
 diffusers==0.25.0
 einops
 torchvision
 
 [all]
 accelerate
 dacite
-datasets
+datasets<=2.18
 jieba
 matplotlib
 modelscope>=1.13.3
 nltk
 numpy
 optimum>=1.17.0
 pandas
```

### Comparing `ms-swift-2.0.2/setup.cfg` & `ms-swift-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/setup.py` & `ms-swift-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/__init__.py` & `ms-swift-2.0.3/swift/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/__init__.py` & `ms-swift-2.0.3/swift/aigc/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/animatediff.py` & `ms-swift-2.0.3/swift/aigc/animatediff.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/animatediff_infer.py` & `ms-swift-2.0.3/swift/aigc/animatediff_infer.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/__init__.py` & `ms-swift-2.0.3/swift/aigc/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_controlnet.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_controlnet.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_controlnet_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_controlnet_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_dreambooth.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_dreambooth_lora.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image_lora.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/infer_text_to_image_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/infer_text_to_image_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_controlnet.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_controlnet.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_controlnet_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_controlnet_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_dreambooth.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_dreambooth_lora.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image_lora.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/diffusers/train_text_to_image_sdxl.py` & `ms-swift-2.0.3/swift/aigc/diffusers/train_text_to_image_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/aigc/utils/argument.py` & `ms-swift-2.0.3/swift/aigc/utils/argument.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/cli/main.py` & `ms-swift-2.0.3/swift/cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,15 +48,24 @@
 def cli_main() -> None:
     argv = sys.argv[1:]
     method_name = argv[0]
     argv = argv[1:]
     file_path = importlib.util.find_spec(ROUTE_MAPPING[method_name]).origin
     torchrun_args = get_torchrun_args()
     if torchrun_args is None or method_name not in ('sft', 'dpo'):
-        args = ['python', file_path, *argv]
+        try:
+            python_cmd = 'python'
+            subprocess.run(
+                [python_cmd, '--version'],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+        except FileNotFoundError:
+            python_cmd = 'python3'
+        args = [python_cmd, file_path, *argv]
     else:
         args = ['torchrun', *torchrun_args, file_path, *argv]
     print(f"run sh: `{' '.join(args)}`", flush=True)
     subprocess.run(args)
 
 
 if __name__ == '__main__':
```

### Comparing `ms-swift-2.0.2/swift/hub/api.py` & `ms-swift-2.0.3/swift/hub/api.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/check_model.py` & `ms-swift-2.0.3/swift/hub/check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/constants.py` & `ms-swift-2.0.3/swift/hub/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/errors.py` & `ms-swift-2.0.3/swift/hub/errors.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/file_download.py` & `ms-swift-2.0.3/swift/hub/file_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/git.py` & `ms-swift-2.0.3/swift/hub/git.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/push_to_hub.py` & `ms-swift-2.0.3/swift/hub/push_to_hub.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/repository.py` & `ms-swift-2.0.3/swift/hub/repository.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/snapshot_download.py` & `ms-swift-2.0.3/swift/hub/snapshot_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/utils/caching.py` & `ms-swift-2.0.3/swift/hub/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/hub/utils/utils.py` & `ms-swift-2.0.3/swift/hub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/__init__.py` & `ms-swift-2.0.3/swift/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/accelerator.py` & `ms-swift-2.0.3/swift/llm/accelerator.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/agent/utils.py` & `ms-swift-2.0.3/swift/llm/agent/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,9 +51,28 @@
                 weights += [1.0]
             elif c['key'] in ('Observation:', ):
                 weights += [2.0]
                 weights += [0.0]
             agent_content.append(c['key'])
             agent_content.append(c['content'])
         return agent_content, weights
+    elif ('Action:' in response
+          or 'Next:' in response) and use_loss_scale:  # alpha-umi
+        agent_keyword = ['Next:', 'Action:', 'Action Input:']
+        agent_parts = split_str_parts_by(response, agent_keyword)
+        weights = []
+        agent_content = []
+        for c in agent_parts:
+            if c['key'] in ('Action:', 'Action Input:', 'Next:'):
+                weights += [2.0]
+                weights += [2.0]
+            elif c['key'] in ('Thought:', 'Final Answer:', ''):
+                weights += [1.0]
+                weights += [1.0]
+            elif c['key'] in ('Observation:', ):
+                weights += [2.0]
+                weights += [0.0]
+            agent_content.append(c['key'])
+            agent_content.append(c['content'])
+        return agent_content, weights
     else:
         return [response], [1.0]
```

### Comparing `ms-swift-2.0.2/swift/llm/app_ui.py` & `ms-swift-2.0.3/swift/llm/app_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 from typing import Iterator, Tuple
 
-from swift.utils import get_logger, get_main
+from swift.utils import get_logger, get_main, seed_everything
 from .infer import merge_lora, prepare_model_template
 from .utils import (AppUIArguments, History, inference_stream,
                     limit_history_length)
 
 logger = get_logger()
 
 
@@ -106,14 +106,15 @@
         share=share,
         server_name=server_name,
         server_port=server_port)
 
 
 def llm_app_ui(args: AppUIArguments) -> None:
     logger.info(f'args: {args}')
+    seed_everything(args.seed)
     args.eval_human = True
     if args.merge_lora:
         merge_lora(args, device_map=args.merge_device_map)
     if args.template_type.endswith('generation'):
         gradio_generation_demo(args)
     else:
         gradio_chat_demo(args)
```

### Comparing `ms-swift-2.0.2/swift/llm/data/self_cognition.jsonl` & `ms-swift-2.0.3/swift/llm/data/self_cognition.jsonl`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/deploy.py` & `ms-swift-2.0.3/swift/llm/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
                     ChatCompletionResponseStreamChoice,
                     ChatCompletionStreamResponse, ChatMessage,
                     CompletionRequest, CompletionResponse,
                     CompletionResponseChoice, CompletionResponseStreamChoice,
                     CompletionStreamResponse, DeltaMessage, DeployArguments,
                     Model, ModelList, UsageInfo, inference, inference_stream,
                     messages_to_history, random_uuid)
-from .utils.utils import _get_safe_print_idx
 
 logger = get_logger()
 
 app = FastAPI()
 _args = None
 model = None
 llm_engine = None
@@ -153,14 +152,18 @@
         raise ValueError(error_msg)
     tokenizer = template.tokenizer
     if tokenizer.eos_token is not None and tokenizer.eos_token not in generation_config.stop:
         generation_config.stop.append(tokenizer.eos_token)
     if isinstance(template.suffix[-1],
                   str) and template.suffix[-1] not in generation_config.stop:
         generation_config.stop.append(template.suffix[-1])
+    if isinstance(template.suffix[-1], list):
+        token_str = tokenizer.decode(template.suffix[-1])
+        if token_str not in generation_config.stop:
+            generation_config.stop.append(token_str)
     request_info['generation_config'] = generation_config
     request_info.update({'seed': request.seed, 'stream': request.stream})
     logger.info(request_info)
 
     created_time = int(time.time())
     generate_kwargs = {}
     if _args.vllm_enable_lora and request.model != _args.model_type:
@@ -188,93 +191,89 @@
         num_generated_tokens = sum(
             len(output.token_ids) for output in result.outputs)
         usage_info = UsageInfo(
             prompt_tokens=num_prompt_tokens,
             completion_tokens=num_generated_tokens,
             total_tokens=num_prompt_tokens + num_generated_tokens,
         )
+
         if isinstance(request, ChatCompletionRequest):
             choices = []
             for output in result.outputs:
+                response = template.generate_ids_to_response(output.token_ids)
                 choice = ChatCompletionResponseChoice(
                     index=output.index,
-                    message=ChatMessage(
-                        role='assistant',
-                        content=template.tokenizer.decode(
-                            output.token_ids, True)),
+                    message=ChatMessage(role='assistant', content=response),
                     finish_reason=output.finish_reason,
                 )
                 choices.append(choice)
             response = ChatCompletionResponse(
                 model=request.model,
                 choices=choices,
                 usage=usage_info,
                 id=request_id,
                 created=created_time)
         else:
             choices = []
             for output in result.outputs:
+                response = template.generate_ids_to_response(output.token_ids)
                 choice = CompletionResponseChoice(
                     index=output.index,
-                    text=template.tokenizer.decode(output.token_ids, True),
+                    text=response,
                     finish_reason=output.finish_reason,
                 )
                 choices.append(choice)
             response = CompletionResponse(
                 model=request.model,
                 choices=choices,
                 usage=usage_info,
                 id=request_id,
                 created=created_time)
         return response
 
     async def _generate_stream():
-        print_idx_list = [0] * request.n
+        print_idx_list = [[0] for _ in range(request.n)]
         async for result in result_generator:
             num_prompt_tokens = len(result.prompt_token_ids)
             num_generated_tokens = sum(
                 len(output.token_ids) for output in result.outputs)
             usage_info = UsageInfo(
                 prompt_tokens=num_prompt_tokens,
                 completion_tokens=num_generated_tokens,
                 total_tokens=num_prompt_tokens + num_generated_tokens,
             )
+
+            for output in result.outputs:
+                output.delta_text = template.generate_ids_to_response(
+                    output.token_ids,
+                    output.finished(),
+                    return_delta=True,
+                    print_idx=print_idx_list[output.index])
+
             if isinstance(request, ChatCompletionRequest):
                 choices = []
                 for output in result.outputs:
-                    text = template.tokenizer.decode(output.token_ids, True)
-                    new_print_idx = _get_safe_print_idx(
-                        text, print_idx_list[output.index], output.finished())
-                    delta_text = text[print_idx_list[output.
-                                                     index]:new_print_idx]
-                    print_idx_list[output.index] = new_print_idx
                     choice = ChatCompletionResponseStreamChoice(
                         index=output.index,
                         delta=DeltaMessage(
-                            role='assistant', content=delta_text),
+                            role='assistant', content=output.delta_text),
                         finish_reason=output.finish_reason)
                     choices.append(choice)
                 response = ChatCompletionStreamResponse(
                     model=request.model,
                     choices=choices,
                     usage=usage_info,
                     id=request_id,
                     created=created_time)
             else:
                 choices = []
                 for output in result.outputs:
-                    text = template.tokenizer.decode(output.token_ids, True)
-                    new_print_idx = _get_safe_print_idx(
-                        text, print_idx_list[output.index], output.finished())
-                    delta_text = text[print_idx_list[output.
-                                                     index]:new_print_idx]
-                    print_idx_list[output.index] = new_print_idx
                     choice = CompletionResponseStreamChoice(
                         index=output.index,
-                        text=delta_text,
+                        text=output.delta_text,
                         finish_reason=output.finish_reason)
                     choices.append(choice)
                 response = CompletionStreamResponse(
                     model=request.model,
                     choices=choices,
                     usage=usage_info,
                     id=request_id,
@@ -494,14 +493,15 @@
         return await inference_vllm_async(request, raw_request)
     else:
         return await inference_pt_async(request, raw_request)
 
 
 def llm_deploy(args: DeployArguments) -> None:
     logger.info(f'args: {args}')
+    seed_everything(args.seed)
     logger_format = logging.Formatter(
         '%(levelname)s: %(asctime)s %(filename)s:%(lineno)d] %(message)s')
     logger.handlers[0].setFormatter(logger_format)
     import uvicorn
     global llm_engine, model, template, _args
     _args = args
     if args.merge_lora:
```

### Comparing `ms-swift-2.0.2/swift/llm/dpo.py` & `ms-swift-2.0.3/swift/llm/dpo.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
                     get_template, get_time_info, set_generation_config)
 
 logger = get_logger()
 
 
 def llm_dpo(args: DPOArguments) -> str:
     logger.info(f'args: {args}')
+    seed_everything(args.seed)
     training_args = args.training_args
     print(f'device_count: {torch.cuda.device_count()}')
     rank, local_rank, world_size, local_world_size = get_dist_setting()
     print(f'rank: {rank}, local_rank: {local_rank}, '
           f'world_size: {world_size}, local_world_size: {local_world_size}')
-    seed_everything(args.seed)
 
     # Loading Model and Tokenizer
     if is_deepspeed_zero3_enabled():
         model_kwargs = {'device_map': None}
     else:
         model_kwargs = {'low_cpu_mem_usage': True}
         if is_dist() and not is_ddp_plus_mp():
@@ -51,21 +51,23 @@
     if args.use_flash_attn is not None:
         kwargs['use_flash_attn'] = args.use_flash_attn
     model, tokenizer = get_model_tokenizer(
         args.model_type,
         args.torch_dtype,
         model_kwargs,
         model_id_or_path=args.model_id_or_path,
+        revision=args.model_revision,
         **kwargs)
     if args.ref_model_type is not None:
         ref_model, _ = get_model_tokenizer(
             args.ref_model_type,
             args.torch_dtype,
             model_kwargs,
             model_id_or_path=args.ref_model_id_or_path,
+            revision=args.model_revision,
             **kwargs)
     else:
         ref_model = None
 
     logger.info(f'model_config: {model.config}')
     if hasattr(model, 'hf_device_map'):
         logger.info(f'model device_map {model.hf_device_map}')
```

### Comparing `ms-swift-2.0.2/swift/llm/ds_config/zero2.json` & `ms-swift-2.0.3/swift/llm/ds_config/zero2.json`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/ds_config/zero3.json` & `ms-swift-2.0.3/swift/llm/ds_config/zero3.json`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/eval.py` & `ms-swift-2.0.3/swift/llm/eval.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,45 +3,97 @@
 import time
 from typing import List
 
 import json
 from llmuses.models.custom import CustomModel
 from modelscope import GenerationConfig
 
-from swift.utils import get_logger, get_main
+from swift.utils import get_logger, get_main, seed_everything
 from . import EvalArguments, inference, merge_lora, prepare_model_template
 
 logger = get_logger()
 
 
 class EvalModel(CustomModel):
 
     def __init__(self, args: EvalArguments, model_name, config={}, **kwargs):
-        if args.merge_lora:
-            merge_lora(args, device_map=args.merge_device_map)
-        if args.infer_backend == 'vllm':
-            from .utils import prepare_vllm_engine_template
-            self.llm_engine, self.template = prepare_vllm_engine_template(args)
+        if args.eval_url is not None:
+            from openai import OpenAI
+            self.client = OpenAI(
+                api_key=args.eval_token,
+                base_url=args.eval_url,
+            )
         else:
-            self.model, self.template = prepare_model_template(args)
-            if args.overwrite_generation_config:
-                assert args.ckpt_dir is not None, 'args.ckpt_dir is not specified.'
-                self.model.generation_config.save_pretrained(args.ckpt_dir)
+            if args.merge_lora:
+                merge_lora(args, device_map=args.merge_device_map)
+            if args.infer_backend == 'vllm':
+                from .utils import prepare_vllm_engine_template
+                self.llm_engine, self.template = prepare_vllm_engine_template(
+                    args)
+            else:
+                self.model, self.template = prepare_model_template(args)
+                if args.overwrite_generation_config:
+                    assert args.ckpt_dir is not None, 'args.ckpt_dir is not specified.'
+                    self.model.generation_config.save_pretrained(args.ckpt_dir)
 
         self.args = args
         super(EvalModel, self).__init__(
             config={
                 'model_id': model_name,
                 **config
             }, **kwargs)
         self.model_name = model_name
         self.generation_info = {'time': 0, 'tokens': 0}
 
+    def call_openai_chat(self, query: str, history: List, **infer_args):
+        infer_args.pop('best_of', None)
+        history = history or []
+        messages = history
+        messages.append({'role': 'user', 'content': query})
+        resp = self.client.chat.completions.create(
+            model=self.args.model_type, messages=messages, **infer_args)
+        response = resp.choices[0].message.content
+        return response
+
+    def call_openai_base(self, query: str, **infer_args):
+        resp = self.client.completions.create(
+            model=self.args.model_type, prompt=query, **infer_args)
+        response = resp.choices[0].message.content
+        return response
+
     def predict(self, prompt: str, **kwargs):
-        if self.args.infer_backend == 'vllm':
+        if self.args.eval_url is not None:
+            assert self.args.eval_is_chat_model is not None
+            infer_cfg = kwargs['infer_cfg']
+            infer_cfg.pop('max_length', None)
+            if 'max_new_tokens' in infer_cfg:
+                infer_cfg['max_tokens'] = infer_cfg.pop('max_new_tokens')
+            if 'do_sample' in infer_cfg:
+                infer_cfg['temperature'] = infer_cfg[
+                    'temperature'] if infer_cfg['do_sample'] else 0.
+                infer_cfg.pop('do_sample', None)
+            if 'repetition_penalty' in infer_cfg:
+                infer_cfg['presence_penalty'] = infer_cfg.pop(
+                    'repetition_penalty')
+            if infer_cfg.get('limit') is not None:
+                infer_cfg['n'] = infer_cfg.pop('limit')
+            infer_cfg.pop('limit', None)
+            if 'top_k' in infer_cfg:
+                infer_cfg['best_of'] = infer_cfg.pop('top_k')
+            infer_cfg.pop('top_k', None)
+            infer_cfg.pop('num_beams', None)
+            if self.args.eval_is_chat_model:
+                system = kwargs.get('system')
+                history = kwargs.get('history') or []
+                if system:
+                    history.insert(0, {'role': 'system', 'content': 'system'})
+                response = self.call_openai_chat(prompt, history, **infer_cfg)
+            else:
+                response = self.call_openai_base(prompt, **infer_cfg)
+        elif self.args.infer_backend == 'vllm':
             from . import inference_vllm
             request_list = [{
                 'query': prompt,
                 'history': kwargs.get('history'),
                 'system': kwargs.get('system')
             }]
             if 'temperature' in kwargs['infer_cfg']:
@@ -140,14 +192,16 @@
         'generation_info': eval_model.generation_info,
     }
     print(f'Final report:{final_report}\n', flush=True)
     return final_report
 
 
 def llm_eval(args: EvalArguments) -> None:
+    logger.info(f'args: {args}')
+    seed_everything(args.seed)
     model_name = args.model_type
     if args.name:
         model_name += f'-{args.name}'
     run_eval_single_model(args, model_name)
 
 
 eval_main = get_main(EvalArguments, llm_eval)
```

### Comparing `ms-swift-2.0.2/swift/llm/export.py` & `ms-swift-2.0.3/swift/llm/export.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,19 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 import os
-from typing import List, Tuple, Union
 
 import torch
-from datasets import concatenate_datasets
-from modelscope import GenerationConfig
-from transformers import PreTrainedModel
 
 from swift.utils import (get_logger, get_main, get_model_info, push_to_ms_hub,
                          seed_everything, show_layers)
 from .infer import merge_lora, prepare_model_template, save_checkpoint
-from .utils import (ExportArguments, Template, get_dataset,
-                    get_model_tokenizer, get_template, set_generation_config,
-                    swift_to_peft_format)
+from .utils import ExportArguments, get_dataset, swift_to_peft_format
 
 logger = get_logger()
 
-
-def prepare_awq_model_template(
-        args: ExportArguments) -> Tuple[PreTrainedModel, Template]:
-    from awq import AutoAWQForCausalLM
-    logger.info(f'device_count: {torch.cuda.device_count()}')
-    seed_everything(args.seed)
-
-    # Loading Model and Tokenizer
-    model_kwargs = {
-        'low_cpu_mem_usage': True,
-        'device_map': args.quant_device_map
-    }
-    model_id_or_path = None
-    if args.sft_type == 'full' and args.ckpt_dir is not None:
-        model_id_or_path = args.ckpt_dir
-    elif args.model_id_or_path is not None:
-        model_id_or_path = args.model_id_or_path
-    model, tokenizer = get_model_tokenizer(
-        args.model_type,
-        args.torch_dtype,
-        model_kwargs,
-        model_id_or_path=model_id_or_path,
-        automodel_class=AutoAWQForCausalLM)
-    logger.info(f'model_config: {model.config}')
-    generation_config = GenerationConfig(
-        max_new_tokens=args.max_new_tokens,
-        temperature=args.temperature,
-        top_k=args.top_k,
-        top_p=args.top_p,
-        do_sample=args.do_sample,
-        repetition_penalty=args.repetition_penalty,
-        num_beams=args.num_beams,
-        pad_token_id=tokenizer.pad_token_id,
-        eos_token_id=tokenizer.eos_token_id)
-    logger.info(f'generation_config: {generation_config}')
-    set_generation_config(model, generation_config)
-
-    logger.info(get_model_info(model))
-    show_layers(model)
-
-    template: Template = get_template(
-        args.template_type,
-        tokenizer,
-        args.system,
-        args.max_length,
-        args.truncation_strategy,
-        model=model)
-    args.system = template.default_system
-    logger.info(f'system: {args.system}')
-    return model, template
-
-
 _args = None
 template = None
 
 
 def _get_dataset(*args, **kwargs):
     global _args, template
     assert _args is not None
@@ -156,14 +98,15 @@
     quantizer.get_dataset = _origin_get_dataset  # recover
     return gptq_quantizer
 
 
 def llm_export(args: ExportArguments) -> None:
     global _args, template
     logger.info(f'args: {args}')
+    seed_everything(args.seed)
     if args.to_peft_format:
         assert args.sft_type == 'lora'
         args.ckpt_dir = swift_to_peft_format(args.ckpt_dir)
     if args.merge_lora:
         merge_lora(args, device_map=args.merge_device_map)
     if args.quant_bits > 0:
         _args = args
@@ -176,39 +119,44 @@
             quant_path = f'{args.model_type}-{args.quant_method}-int{args.quant_bits}'
         else:
             ckpt_dir, ckpt_name = os.path.split(args.ckpt_dir)
             quant_path = os.path.join(
                 ckpt_dir,
                 f'{ckpt_name}-{args.quant_method}-int{args.quant_bits}')
         logger.info(f'Setting quant_path: {quant_path}')
-        assert not os.path.exists(quant_path)
+        assert not os.path.exists(quant_path), f'quant_path: {quant_path}'
         if args.quant_method == 'awq':
-            awq_model, template = prepare_awq_model_template(args)
-            awq_model_quantize(awq_model, template.tokenizer)
-            logger.info(get_model_info(awq_model))
-            show_layers(awq_model)
-            logger.info('Saving quantized weights...')
-            awq_model.save_quantized(quant_path)
-            model_cache_dir = awq_model.model_dir
+            from awq import AutoAWQForCausalLM
+            model, template = prepare_model_template(
+                args,
+                device_map=args.quant_device_map,
+                verbose=False,
+                automodel_class=AutoAWQForCausalLM)
+            awq_model_quantize(model, template.tokenizer)
+            model.save_quantized(quant_path)
         else:  # gptq
             model, template = prepare_model_template(
-                args, device_map=args.quant_device_map)
+                args, device_map=args.quant_device_map, verbose=False)
             gptq_quantizer = gptq_model_quantize(model, template.tokenizer)
-            logger.info(get_model_info(model))
-            show_layers(model)
-            logger.info('Saving quantized weights...')
+            model.config.quantization_config.pop('dataset', None)
             gptq_quantizer.save(model, quant_path)
-            model_cache_dir = model.model_dir
 
+        logger.info(get_model_info(model))
+        show_layers(model)
+        logger.info('Saving quantized weights...')
+        model_cache_dir = model.model_dir
         save_checkpoint(None, template.tokenizer, model_cache_dir,
                         args.ckpt_dir, quant_path)
         logger.info(
             f'Successfully quantized the model and saved in {quant_path}.')
         args.ckpt_dir = quant_path
 
     if args.push_to_hub:
-        assert args.ckpt_dir is not None, 'You need to specify `ckpt_dir`.'
-        push_to_ms_hub(args.ckpt_dir, args.hub_model_id, args.hub_token,
+        ckpt_dir = args.ckpt_dir
+        if ckpt_dir is None:
+            ckpt_dir = args.model_id_or_path
+        assert ckpt_dir is not None, 'You need to specify `ckpt_dir`.'
+        push_to_ms_hub(ckpt_dir, args.hub_model_id, args.hub_token,
                        args.hub_private_repo, args.commit_message)
 
 
 export_main = get_main(ExportArguments, llm_export)
```

### Comparing `ms-swift-2.0.2/swift/llm/infer.py` & `ms-swift-2.0.3/swift/llm/infer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 from tqdm import tqdm
 from transformers import PreTrainedModel, PreTrainedTokenizerBase
 from transformers.utils import is_torch_npu_available
 
 from swift.tuners import Swift
 from swift.utils import (append_to_jsonl, get_logger, get_main, get_model_info,
                          read_multi_line, seed_everything, show_layers)
-from .utils import (TEMPLATE_MAPPING, InferArguments, Template,
-                    get_additional_saved_files, get_dataset,
-                    get_model_tokenizer, get_template, inference,
+from .utils import (InferArguments, Template, get_additional_saved_files,
+                    get_dataset, get_model_tokenizer, get_template, inference,
                     inference_stream, is_adapter, set_generation_config)
 
 logger = get_logger()
 
 
 def save_checkpoint(model: Optional[PreTrainedModel],
                     tokenizer: PreTrainedTokenizerBase,
@@ -80,79 +79,56 @@
 def merge_lora(args: InferArguments,
                replace_if_exists=False,
                device_map: Optional[str] = None,
                **kwargs) -> Optional[str]:
     logger.info(f'replace_if_exists: {replace_if_exists}')
     assert args.ckpt_dir is not None, 'args.ckpt_dir is not specified.'
     assert args.sft_type == 'lora', "Only supports sft_type == 'lora'"
-    assert 'int4' not in args.model_type, 'int4 model is not supported'
-    assert 'int8' not in args.model_type, 'int8 model is not supported'
+    for s in ['int4', 'int8', 'awq']:
+        assert s not in args.model_type, f'{s} model is not supported'
     if args.quantization_bit != 0:
         logger.warning('It is not recommended to merge quantized models, '
                        'as this can result in performance degradation')
-    old_ckpt_dir = args.ckpt_dir
     ckpt_dir, ckpt_name = os.path.split(args.ckpt_dir)
     merged_lora_path = os.path.join(ckpt_dir, f'{ckpt_name}-merged')
     logger.info(f'merged_lora_path: `{merged_lora_path}`')
-    logger.info("Setting args.sft_type: 'full'")
-    logger.info(f'Setting args.ckpt_dir: {merged_lora_path}')
-    args.sft_type = 'full'
-    args.ckpt_dir = merged_lora_path
-    if os.path.exists(args.ckpt_dir) and not replace_if_exists:
+    if os.path.exists(merged_lora_path) and not replace_if_exists:
         logger.info(
             f'The weight directory for the merged LoRA already exists in {args.ckpt_dir}, '
             'skipping the saving process. '
             'you can pass `replace_if_exists=True` to overwrite it.')
-        return
-
-    model_kwargs = {}
-    if is_torch_npu_available():
-        logger.info(f'device_count: {torch.npu.device_count()}')
-        if device_map is None:
-            device_map = 'npu:0'
     else:
-        logger.info(f'device_count: {torch.cuda.device_count()}')
-        if device_map is None:
-            device_map = 'auto'
-    if device_map == 'auto':
-        model_kwargs['low_cpu_mem_usage'] = True
-    model_kwargs['device_map'] = device_map
-
-    # Loading Model and Tokenizer
-    model_id_or_path = None
-    if args.model_id_or_path is not None:
-        model_id_or_path = args.model_id_or_path
-    model, tokenizer = get_model_tokenizer(
-        args.model_type,
-        args.torch_dtype,
-        model_kwargs,
-        model_id_or_path=model_id_or_path)
-    logger.info(f'model_config: {model.config}')
-
-    # Preparing LoRA
-    model = Swift.from_pretrained(model, old_ckpt_dir, inference_mode=True)
-    Swift.merge_and_unload(model)
-    model = model.model
-    logger.info('Saving merged weights...')
-    save_checkpoint(
-        model,
-        tokenizer,
-        model.model_dir,
-        old_ckpt_dir,
-        merged_lora_path,
-        save_safetensors=args.save_safetensors)
-    logger.info(f'Successfully merged LoRA and saved in {merged_lora_path}.')
+        model, template = prepare_model_template(
+            args, device_map=args.merge_device_map, verbose=False)
+        logger.info('Merge LoRA...')
+        Swift.merge_and_unload(model)
+        model = model.model
+        logger.info('Saving merged weights...')
+        save_checkpoint(
+            model,
+            template.tokenizer,
+            model.model_dir,
+            args.ckpt_dir,
+            merged_lora_path,
+            save_safetensors=args.save_safetensors)
+        logger.info(
+            f'Successfully merged LoRA and saved in {merged_lora_path}.')
+    logger.info("Setting args.sft_type: 'full'")
+    logger.info(f'Setting args.ckpt_dir: {merged_lora_path}')
+    args.sft_type = 'full'
+    args.ckpt_dir = merged_lora_path
     return merged_lora_path
 
 
 def prepare_model_template(
         args: InferArguments,
-        device_map: Optional[str] = None) -> Tuple[PreTrainedModel, Template]:
-
-    seed_everything(args.seed)
+        *,
+        device_map: Optional[str] = None,
+        verbose: bool = True,
+        automodel_class=None) -> Tuple[PreTrainedModel, Template]:
 
     model_kwargs = {}
     if is_torch_npu_available():
         logger.info(f'device_count: {torch.npu.device_count()}')
         if device_map is None:
             device_map = 'npu:0'
     else:
@@ -179,22 +155,40 @@
     if args.use_flash_attn is not None:
         kwargs['use_flash_attn'] = args.use_flash_attn
     model_id_or_path = None
     if args.sft_type == 'full' and args.ckpt_dir is not None:
         model_id_or_path = args.ckpt_dir
     elif args.model_id_or_path is not None:
         model_id_or_path = args.model_id_or_path
+    if automodel_class is not None:
+        kwargs['automodel_class'] = automodel_class
 
     model, tokenizer = get_model_tokenizer(
         args.model_type,
         args.torch_dtype,
         model_kwargs,
         model_id_or_path=model_id_or_path,
+        revision=args.model_revision,
         **kwargs)
-    logger.info(f'model_config: {model.config}')
+    if verbose:
+        logger.info(f'model_config: {model.config}')
+
+    generation_config = GenerationConfig(
+        max_new_tokens=args.max_new_tokens,
+        temperature=args.temperature,
+        top_k=args.top_k,
+        top_p=args.top_p,
+        do_sample=args.do_sample,
+        repetition_penalty=args.repetition_penalty,
+        num_beams=args.num_beams,
+        pad_token_id=tokenizer.pad_token_id,
+        eos_token_id=tokenizer.eos_token_id)
+    logger.info(f'generation_config: {generation_config}')
+    set_generation_config(model, generation_config)
+
     if model.max_model_len is None:
         model.max_model_len = args.max_model_len
     elif args.max_model_len is not None:
         if args.max_model_len <= model.max_model_len:
             model.max_model_len = args.max_model_len
         else:
             raise ValueError(
@@ -204,29 +198,18 @@
     # Preparing LoRA
     if is_adapter(args.sft_type) and args.ckpt_dir is not None:
         model = Swift.from_pretrained(
             model, args.ckpt_dir, inference_mode=True)
         if args.sft_type == 'adalora':
             model = model.to(model.dtype)
 
+    if verbose:
+        show_layers(model)
+        logger.info(model)
     logger.info(get_model_info(model))
-    show_layers(model)
-
-    generation_config = GenerationConfig(
-        max_new_tokens=args.max_new_tokens,
-        temperature=args.temperature,
-        top_k=args.top_k,
-        top_p=args.top_p,
-        do_sample=args.do_sample,
-        repetition_penalty=args.repetition_penalty,
-        num_beams=args.num_beams,
-        pad_token_id=tokenizer.pad_token_id,
-        eos_token_id=tokenizer.eos_token_id)
-    logger.info(f'generation_config: {generation_config}')
-    set_generation_config(model, generation_config)
 
     template: Template = get_template(
         args.template_type,
         tokenizer,
         args.system,
         args.max_length,
         args.truncation_strategy,
@@ -249,14 +232,15 @@
             images += [image]
     if len(images) > 0:
         infer_kwargs['images'] = images
 
 
 def llm_infer(args: InferArguments) -> None:
     logger.info(f'args: {args}')
+    seed_everything(args.seed)
     if args.merge_lora:
         merge_lora(args, device_map=args.merge_device_map)
     if args.infer_backend == 'vllm':
         from .utils import prepare_vllm_engine_template, inference_stream_vllm, inference_vllm
         llm_engine, template = prepare_vllm_engine_template(args)
     else:
         model, template = prepare_model_template(args)
@@ -266,17 +250,23 @@
     lora_request = None
     if args.vllm_enable_lora:
         assert len(args.vllm_lora_request_list) == 1
         lora_request = args.vllm_lora_request_list[0]
     # Inference
     result = []
     jsonl_path = None
-    if args.save_result and args.ckpt_dir is not None:
-        time = dt.datetime.now().strftime('%Y%m%d-%H%M%S')
-        jsonl_path = os.path.join(args.ckpt_dir, f'infer_result_{time}.jsonl')
+    if args.save_result:
+        result_dir = args.ckpt_dir
+        if result_dir is None:
+            result_dir = model.model_dir
+        if result_dir is not None:
+            result_dir = os.path.join(result_dir, 'infer_result')
+            os.makedirs(result_dir, exist_ok=True)
+            time = dt.datetime.now().strftime('%Y%m%d-%H%M%S')
+            jsonl_path = os.path.join(result_dir, f'{time}.jsonl')
     if args.eval_human:
         input_mode: Literal['S', 'M'] = 'S'
         logger.info('Input `exit` or `quit` to exit the conversation.')
         logger.info('Input `multi-line` to switch to multi-line input mode.')
         logger.info(
             'Input `reset-system` to reset the system and clear the history.')
         if template.support_multi_round:
@@ -478,15 +468,15 @@
                 result.append(obj)
                 if args.verbose:
                     print()
                     print(f'[LABELS]{label}')
                     if images is not None:
                         print(f'[IMAGES]{images}')
                     print('-' * 50)
-    if args.save_result and args.ckpt_dir is not None:
+    if jsonl_path is not None:
         logger.info(f'save_result_path: {jsonl_path}')
     if args.val_dataset_sample == 10:  # is default
         logger.info(
             'You can set `--val_dataset_sample -1` to perform inference on the entire dataset.'
         )
     return {'result': result}
```

### Comparing `ms-swift-2.0.2/swift/llm/rome.py` & `ms-swift-2.0.3/swift/llm/rome.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
                     get_template, inference, set_generation_config)
 
 logger = get_logger()
 
 
 def rome_infer(args: RomeArguments) -> None:
     logger.info(f'args: {args}')
+    seed_everything(args.seed)
     logger.info(
         'Rome does not support quantization for now, all quantization args will be ignored.'
     )
     logger.info(f'device_count: {torch.cuda.device_count()}')
-    seed_everything(args.seed)
 
     # Loading Model and Tokenizer
     model_kwargs = {'low_cpu_mem_usage': True, 'device_map': 'auto'}
     kwargs = {'use_flash_attn': args.use_flash_attn}
     model, tokenizer = get_model_tokenizer(args.model_type, args.torch_dtype,
                                            model_kwargs, **kwargs)
     logger.info(f'model_config: {model.config}')
```

### Comparing `ms-swift-2.0.2/swift/llm/sft.py` & `ms-swift-2.0.3/swift/llm/sft.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,42 +21,41 @@
 from .accelerator import ta_accelerate
 from .tuner import prepare_model
 from .utils import (TEMPLATE_MAPPING, LazyLLMDataset, SftArguments, Template,
                     add_self_cognition_dataset, dataset_map, get_dataset,
                     get_model_tokenizer, get_template, get_time_info,
                     print_example, set_generation_config, sort_by_max_length,
                     stat_dataset)
-from .utils.argument import handle_dataset_mixture
 
 logger = get_logger()
 
 
 def llm_sft(args: SftArguments) -> Dict[str, Union[str, Any]]:
     logger.info(f'args: {args}')
+    seed_everything(args.seed)
     training_args = args.training_args
     if is_torch_npu_available():
         print(f'device_count: {torch.npu.device_count()}')
     else:
         print(f'device_count: {torch.cuda.device_count()}')
     rank, local_rank, world_size, local_world_size = get_dist_setting()
     print(f'rank: {rank}, local_rank: {local_rank}, '
           f'world_size: {world_size}, local_world_size: {local_world_size}')
-    seed_everything(args.seed)
 
     if args.gpu_memory_fraction is not None:
         for device_id in range(torch.cuda.device_count()):
             torch.cuda.set_per_process_memory_fraction(
                 max(min(args.gpu_memory_fraction, 1.0), 0.01),
                 device=device_id)
 
     # Loading Model and Tokenizer
-    if is_torch_npu_available():
-        model_kwargs = {'device_map': local_rank if local_rank >= 0 else 0}
-    elif is_deepspeed_zero3_enabled():
+    if is_deepspeed_zero3_enabled():
         model_kwargs = {'device_map': None}
+    elif is_torch_npu_available():
+        model_kwargs = {'device_map': local_rank if local_rank >= 0 else 0}
     else:
         model_kwargs = {'low_cpu_mem_usage': True}
         if is_dist() and not is_ddp_plus_mp():
             model_kwargs['device_map'] = {'': local_rank}
         elif not use_torchacc():
             model_kwargs['device_map'] = 'auto'
 
@@ -74,14 +73,15 @@
     if args.use_flash_attn is not None:
         kwargs['use_flash_attn'] = args.use_flash_attn
     model, tokenizer = get_model_tokenizer(
         args.model_type,
         args.torch_dtype,
         model_kwargs,
         model_id_or_path=args.model_id_or_path,
+        revision=args.model_revision,
         is_training=True,
         **kwargs)
     logger.info(f'model_config: {model.config}')
     generation_config = GenerationConfig(
         max_new_tokens=args.max_new_tokens,
         temperature=args.temperature,
         top_k=args.top_k,
@@ -102,19 +102,19 @@
         label_names = find_labels(model)
         return_loss = can_return_loss(model)
         model = ta.patch_qwen_model(model)
     # Preparing LoRA
     model, callbacks = prepare_model(model, args)
 
     show_layers(model)
+    logger.info(model)
     model_info = None
     if not is_deepspeed_zero3_enabled():
         model_info = get_model_info(model)
         logger.info(model_info)
-    logger.info(model)
 
     if args.gradient_checkpointing:
         model.config.use_cache = False  # fix transformers==4.36
         logger.info('Setting model.config.use_cache: False')
         model.enable_input_require_grads()
 
     if use_torchacc():
@@ -149,25 +149,22 @@
                 int(train_dataset_sample * args.dataset_test_ratio), 1)
     if val_dataset is not None and val_dataset_sample is not None and val_dataset_sample >= 0:
         if val_dataset.shape[0] > val_dataset_sample:
             logger.info(f'val_dataset_sample: {val_dataset_sample}')
             val_idxs = random_state.permutation(val_dataset_sample)
             val_dataset = val_dataset.select(val_idxs)
 
-    train_dataset = handle_dataset_mixture(args, train_dataset)
+    train_dataset = args.handle_dataset_mixture(train_dataset)
 
     # add self-cognition dataset
     if args.self_cognition_sample > 0:
         train_dataset = add_self_cognition_dataset(train_dataset,
                                                    args.self_cognition_sample,
                                                    args.model_name,
                                                    args.model_author)
-    if val_dataset is None:
-        training_args.evaluation_strategy = IntervalStrategy.NO
-        training_args.do_eval = False
     logger.info(f'train_dataset: {train_dataset}')
     logger.info(f'val_dataset: {val_dataset}')
     template_kwargs = {}
     template_info = TEMPLATE_MAPPING[args.template_type]
     use_model = template_info.get('use_model', False)
     if use_model:
         template_kwargs['model'] = model
@@ -198,14 +195,17 @@
     else:
         dataset_info = None
         td0, tkwargs0 = template.encode(train_dataset[0])
         print_example(td0, tokenizer, tkwargs0)
         train_dataset = LazyLLMDataset(train_dataset, template)
         if val_dataset is not None:
             val_dataset = LazyLLMDataset(val_dataset, template)
+    if val_dataset is None:
+        training_args.evaluation_strategy = IntervalStrategy.NO
+        training_args.do_eval = False
 
     padding_to = args.max_length if args.sft_type == 'longlora' else None
     data_collator = partial(template.data_collator, padding_to=padding_to)
 
     trian_batch_size = args.batch_size
     eval_batch_size = args.eval_batch_size
     if use_torchacc():
@@ -263,17 +263,18 @@
                                     None)
     logger.info(f'last_model_checkpoint: {last_model_checkpoint}')
     logger.info(
         f'best_model_checkpoint: {trainer.state.best_model_checkpoint}')
     train_time = get_time_info(trainer.state.log_history, len(train_dataset))
     # Visualization
     if is_master() and not use_torchacc():
-        images_dir = os.path.join(args.output_dir, 'images')
-        logger.info(f'images_dir: {images_dir}')
-        plot_images(images_dir, args.logging_dir, ['train/loss'], 0.9)
+        if 'tensorboard' in args.training_args.report_to:
+            images_dir = os.path.join(args.output_dir, 'images')
+            logger.info(f'images_dir: {images_dir}')
+            plot_images(images_dir, args.logging_dir, ['train/loss'], 0.9)
         if args.push_to_hub:
             trainer._add_patterns_to_gitignore(['images/'])
             trainer.push_to_hub()
     run_info = {
         'memory': trainer.perf['memory'],
         'gen_time': trainer.perf['gen_time'],
         'gen_len': trainer.perf['gen_len'],
```

### Comparing `ms-swift-2.0.2/swift/llm/tuner.py` & `ms-swift-2.0.3/swift/llm/tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import torch
 import transformers
 from packaging import version
 
 from swift.torchacc_utils import consolidate_checkpoint
 from swift.trainers import TrainerCallback
 from swift.tuners import (AdaLoraConfig, AdapterConfig, IA3Config,
-                          LongLoRAConfig, LongLoRAModelType, LoraConfig,
-                          LoRAConfig, NEFTuneConfig, Swift)
+                          LongLoRAModelType, LoraConfig, LoRAConfig,
+                          NEFTuneConfig, Swift)
 from swift.tuners.llamapro import LLaMAProConfig
 from swift.tuners.module_mapping import MODEL_KEYS_MAPPING
 from swift.utils import (activate_model_parameters, freeze_model_parameters,
                          get_logger, use_torchacc)
 from .utils import (SftArguments, find_all_linears, find_embedding, find_ln,
                     is_adapter)
 
@@ -74,14 +74,16 @@
                 'bias': args.lora_bias_trainable,
                 'modules_to_save': args.lora_modules_to_save,
                 'use_rslora': args.use_rslora,
                 'use_dora': args.use_dora,
                 'lorap_lr_ratio': args.lora_lr_ratio,
             }
             if args.sft_type in ('lora', 'longlora'):
+                if args.lora_dtype == 'AUTO':
+                    args.lora_dtype = None
                 if args.tuner_backend == 'swift':
                     lora_config = LoRAConfig(
                         lora_dtype=args.lora_dtype, **lora_kwargs)
                 elif args.tuner_backend == 'peft':
                     lora_config = LoraConfig(
                         task_type='CAUSAL_LM',
                         lora_dtype=args.lora_dtype,
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/__init__.py` & `ms-swift-2.0.3/swift/llm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/utils/argument.py` & `ms-swift-2.0.3/swift/llm/utils/argument.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import transformers
 from datasets import Dataset as HfDataset
 from datasets import concatenate_datasets
 from packaging import version
 from torch import dtype as Dtype
 from transformers.utils import (is_torch_bf16_gpu_available,
                                 is_torch_cuda_available,
-                                is_torch_npu_available)
+                                is_torch_npu_available, strtobool)
 from transformers.utils.versions import require_version
 
 from swift.hub import HubApi, ModelScopeConfig
 from swift.trainers import Seq2SeqTrainingArguments
 from swift.tuners import Swift
 from swift.utils import (add_version_to_work_dir, get_dist_setting, get_logger,
                          get_pai_tensorboard_dir, is_dist, is_mp,
@@ -35,16 +35,258 @@
 
 def is_adapter(sft_type: str) -> bool:
     return sft_type in {
         'lora', 'longlora', 'adalora', 'ia3', 'llamapro', 'adapter'
     }
 
 
+class ArgumentsBase:
+
+    def register_custom_dataset(
+            self: Union['SftArguments', 'InferArguments']) -> None:
+        dataset = []
+        for d in self.dataset:
+            if os.path.exists(d):
+                self.custom_train_dataset_path.append(d)
+            else:
+                dataset.append(d)
+        self.dataset = dataset
+
+        for key in ['custom_train_dataset_path', 'custom_val_dataset_path']:
+            value = getattr(self, key)
+            if isinstance(value, str):
+                setattr(self, key, [value])
+        if len(self.custom_train_dataset_path) == 0 and len(
+                self.custom_val_dataset_path) == 0:
+            return
+
+        dataset_name = '_custom_dataset'
+        _register_local_dataset(dataset_name, self.custom_train_dataset_path,
+                                self.custom_val_dataset_path)
+        self.dataset.append(dataset_name)
+
+    def handle_path(self: Union['SftArguments', 'InferArguments']) -> None:
+        check_exist_path = [
+            'ckpt_dir', 'resume_from_checkpoint', 'custom_train_dataset_path',
+            'custom_val_dataset_path'
+        ]
+        if self.model_id_or_path is not None and (
+                self.model_id_or_path.startswith('~')
+                or self.model_id_or_path.startswith('/')):
+            check_exist_path.append('model_id_or_path')
+        check_exist_path_set = set(check_exist_path)
+        other_path = ['output_dir', 'logging_dir']
+        for k in check_exist_path + other_path:
+            value = getattr(self, k, None)
+            if value is None:
+                continue
+            value = _check_path(k, value, check_exist_path_set)
+            setattr(self, k, value)
+
+    def check_flash_attn(
+            self: Union['SftArguments', 'InferArguments']) -> None:
+        model_info = MODEL_MAPPING[self.model_type]
+        support_flash_attn = model_info.get('support_flash_attn', False)
+        if self.use_flash_attn and not support_flash_attn:
+            logger.warning(f'use_flash_attn: {self.use_flash_attn}, '
+                           f'but support_flash_attn: {support_flash_attn}')
+
+    def handle_generation_config(
+            self: Union['SftArguments', 'InferArguments']) -> None:
+        if self.do_sample is False:
+            # fix warning
+            self.temperature = 1.
+            self.top_p = 1.
+            self.top_k = 50
+            logger.info(
+                'Due to do_sample=False, the following settings are applied: args.temperature: '
+                f'{self.temperature}, args.top_p: {self.top_p}, args.top_k: {self.top_k}.'
+            )
+
+    def select_dtype(
+        self: Union['SftArguments', 'InferArguments']
+    ) -> Tuple[Optional[Dtype], bool, bool]:
+        if not is_torch_cuda_available() and not is_torch_npu_available():
+            # cpu
+            if self.dtype == 'AUTO':
+                self.dtype = 'fp32'
+                logger.info(f'Setting args.dtype: {self.dtype}')
+            assert self.dtype != 'fp16', 'The CPU does not support matrix multiplication with FP16.'
+            if self.dtype == 'fp32':
+                return torch.float32, False, False
+            elif self.dtype == 'bf16':
+                return torch.bfloat16, False, True
+            else:
+                raise ValueError(f'args.dtype: {self.dtype}')
+        # cuda, npu
+        if self.dtype == 'AUTO':
+            if not is_torch_bf16_gpu_available():
+                self.dtype = 'fp16'
+            else:
+                model_torch_dtype = MODEL_MAPPING[self.model_type].get(
+                    'torch_dtype')
+                if model_torch_dtype is not None:
+                    self.dtype = dtype_mapping[model_torch_dtype]
+                elif isinstance(self, SftArguments):
+                    self.dtype = 'bf16'
+                else:
+                    return None, False, False
+
+        torch_dtype = dtype_mapping_reversed[self.dtype]
+
+        assert torch_dtype in {torch.float16, torch.bfloat16, torch.float32}
+        if torch_dtype == torch.float16:
+            if isinstance(self, SftArguments) and self.sft_type == 'full':
+                self.dtype = 'fp32'
+                torch_dtype = torch.float32
+                logger.warning(
+                    'Fine-tuning with full parameters does not support fp16, and is prone to NaN. '
+                    'We will use the fp32 & AMP approach, which consumes approximately twice the memory of bf16.'
+                )
+                logger.info(f'Setting torch_dtype: {torch_dtype}')
+            fp16, bf16 = True, False
+        elif torch_dtype == torch.bfloat16:
+            support_bf16 = is_torch_bf16_gpu_available()
+            if not support_bf16:
+                logger.warning(f'support_bf16: {support_bf16}')
+            fp16, bf16 = False, True
+        else:
+            fp16, bf16 = False, False
+        return torch_dtype, fp16, bf16
+
+    def select_bnb(
+        self: Union['SftArguments', 'InferArguments']
+    ) -> Tuple[Optional[Dtype], bool, bool]:
+        if self.bnb_4bit_comp_dtype == 'AUTO':
+            self.bnb_4bit_comp_dtype = self.dtype
+
+        if self.bnb_4bit_comp_dtype != 'AUTO':
+            bnb_4bit_compute_dtype = dtype_mapping_reversed[
+                self.bnb_4bit_comp_dtype]
+            assert bnb_4bit_compute_dtype in {
+                torch.float16, torch.bfloat16, torch.float32
+            }
+        else:
+            bnb_4bit_compute_dtype = None
+        quantization_bit = self.quantization_bit
+        if quantization_bit == 4:
+            require_version('bitsandbytes')
+            load_in_4bit, load_in_8bit = True, False
+        elif quantization_bit == 8:
+            require_version('bitsandbytes')
+            load_in_4bit, load_in_8bit = False, True
+        else:
+            load_in_4bit, load_in_8bit = False, False
+
+        return bnb_4bit_compute_dtype, load_in_4bit, load_in_8bit
+
+    def handle_compatibility(
+            self: Union['SftArguments', 'InferArguments']) -> None:
+        template_type_mapping = {
+            'chatglm2-generation': 'chatglm-generation',
+            'chatml': 'qwen'
+        }
+        model_type_mapping = {
+            'openbmb-minicpm-2b-sft-chat': 'minicpm-2b-sft-chat',
+            'openbmb-minicpm-2b-chat': 'minicpm-2b-chat',
+        }
+        for k, v in template_type_mapping.items():
+            if k == self.template_type:
+                self.template_type = v
+                break
+        for k, v in model_type_mapping.items():
+            if k == self.model_type:
+                self.model_type = v
+                break
+        if self.dataset is not None and len(
+                self.dataset) == 1 and ',' in self.dataset[0]:
+            self.dataset = self.dataset[0].split(',')
+        if self.truncation_strategy == 'ignore':
+            self.truncation_strategy = 'delete'
+        if isinstance(self, InferArguments):
+            if self.show_dataset_sample != 10 and self.val_dataset_sample == 10:
+                # args.val_dataset_sample is the default value and args.show_dataset_sample is not the default value.
+                self.val_dataset_sample = self.show_dataset_sample
+            if self.safe_serialization is not None:
+                self.save_safetensors = self.safe_serialization
+            if self.merge_lora_and_save is not None:
+                self.merge_lora = self.merge_lora_and_save
+        if isinstance(self, SftArguments):
+            if self.only_save_model is not None:
+                self.save_only_model = self.only_save_model
+            if self.neftune_alpha is not None:
+                self.neftune_noise_alpha = self.neftune_alpha
+            if self.per_device_train_batch_size is not None:
+                self.batch_size = self.per_device_train_batch_size
+            if self.per_device_eval_batch_size is not None:
+                self.eval_batch_size = self.per_device_eval_batch_size
+            if self.deepspeed_config_path is not None:
+                self.deepspeed = self.deepspeed_config_path
+
+    def set_model_type(self: Union['SftArguments', 'InferArguments']) -> None:
+        # compat with swift<1.7
+        if self.model_cache_dir is not None and self.model_id_or_path is None:
+            self.model_id_or_path = self.model_cache_dir
+            self.model_cache_dir = None
+
+        if self.model_id_or_path is not None:
+            model_mapping_reversed = {
+                v['model_id_or_path'].lower(): k
+                for k, v in MODEL_MAPPING.items()
+            }
+            model_id_or_path = self.model_id_or_path
+            model_id_or_path_lower = model_id_or_path.lower()
+            if model_id_or_path_lower not in model_mapping_reversed:
+                if (isinstance(self, InferArguments)
+                        and 'checkpoint' in model_id_or_path
+                        and 'merged' not in model_id_or_path
+                        and self.ckpt_dir is None):
+                    raise ValueError(
+                        'Please use `--ckpt_dir vx-xxx/checkpoint-xxx` to use the checkpoint.'
+                    )
+                if self.model_type is None:
+                    raise ValueError(
+                        f"model_id_or_path: '{model_id_or_path}' is not registered. "
+                        'Please set `--model_type <model_type>` additionally.')
+                assert self.model_cache_dir is None
+            else:
+                model_type = model_mapping_reversed[model_id_or_path_lower]
+                assert self.model_type is None or self.model_type == model_type
+                self.model_type = model_type
+                logger.info(f'Setting args.model_type: {model_type}')
+                if self.model_cache_dir is not None:
+                    self.model_id_or_path = self.model_cache_dir
+
+        error_msg = f'The model_type you can choose: {list(MODEL_MAPPING.keys())}'
+        if self.model_type is None:
+            raise ValueError('please setting `--model_type <model_type>`. '
+                             + error_msg)
+        elif self.model_type not in MODEL_MAPPING:
+            raise ValueError(
+                f"model_type: '{self.model_type}' is not registered. "
+                + error_msg)
+        model_info = MODEL_MAPPING[self.model_type]
+        use_hf = strtobool(os.environ.get('USE_HF', 'False'))
+        if self.model_revision is not None:
+            model_info['revision'] = self.model_revision
+            logger.info(
+                f"Setting model_info['revision']: {self.model_revision}")
+        elif use_hf:
+            model_info['revision'] = 'main'
+        self.model_revision = model_info['revision']
+        if self.model_id_or_path is None:
+            self.model_id_or_path = model_info[
+                'hf_model_id'] if use_hf else model_info['model_id_or_path']
+        requires = model_info['requires']
+        for require in requires:
+            require_version(require)
+
+
 @dataclass
-class SftArguments:
+class SftArguments(ArgumentsBase):
     # You can specify the model by either using the model_type or model_id_or_path.
     model_type: Optional[str] = field(
         default=None,
         metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
     model_id_or_path: Optional[str] = None
     model_revision: Optional[str] = None
     model_layer_cls_name: Optional[str] = field(
@@ -63,15 +305,15 @@
         default='AUTO',
         metadata={
             'help':
             f"template_type choices: {list(TEMPLATE_MAPPING.keys()) + ['AUTO']}"
         })
     output_dir: str = 'output'
     add_output_dir_suffix: Optional[bool] = None
-    ddp_backend: Literal['nccl', 'gloo', 'mpi', 'ccl'] = None
+    ddp_backend: Optional[Literal['nccl', 'gloo', 'mpi', 'ccl']] = None
     ddp_find_unused_parameters: Optional[bool] = None
     ddp_broadcast_buffers: Optional[bool] = None
 
     seed: int = 42
     resume_from_checkpoint: Optional[str] = None
     dtype: Literal['bf16', 'fp16', 'fp32', 'AUTO'] = 'AUTO'
 
@@ -113,15 +355,15 @@
     lora_target_modules: List[str] = field(default_factory=lambda: ['DEFAULT'])
     lora_rank: int = 8
     lora_alpha: int = 32
     lora_dropout_p: float = 0.05
     lora_bias_trainable: Literal['none', 'all'] = 'none'
     # e.g. ['wte', 'ln_1', 'ln_2', 'ln_f', 'lm_head']
     lora_modules_to_save: List[str] = field(default_factory=list)
-    lora_dtype: Literal['fp16', 'bf16', 'fp32'] = 'fp32'
+    lora_dtype: Literal['fp16', 'bf16', 'fp32', 'AUTO'] = 'fp32'
     lora_lr_ratio: float = None
     use_rslora: bool = False
     use_dora: bool = False
 
     # adapter
     adapter_act: str = 'gelu'
     adapter_length: int = 128
@@ -154,15 +396,15 @@
     llamapro_num_groups: Optional[int] = None
 
     # neftune
     neftune_noise_alpha: Optional[float] = None  # e.g. 5, 10, 15
     neftune_backend: Literal['swift', 'transformers'] = None
 
     gradient_checkpointing: Optional[bool] = None
-    # e.g. 'default-zero3', 'default-zero2', 'ds_config/zero2.json'
+    # e.g. 'default-zero3', 'default-zero2', 'ds_config/zero2.json', 'zero3-offload'
     deepspeed: Optional[str] = None
     batch_size: int = 1
     eval_batch_size: Optional[int] = None
     num_train_epochs: int = 1
     # if max_steps >= 0, override num_train_epochs
     max_steps: int = -1
     optim: str = 'adamw_torch'
@@ -241,14 +483,74 @@
     model_cache_dir: Optional[str] = None
 
     # fsdp option
     fsdp: Optional[str] = ''
     # fsdp config file
     fsdp_config: Optional[str] = None
 
+    def handle_dataset_mixture(self, train_dataset: HfDataset) -> None:
+        if train_dataset is None:
+            return train_dataset
+        if self.train_dataset_mix_ratio <= 0 or len(
+                self.train_dataset_mix_ds) == 0:
+            return train_dataset
+
+        random_state = np.random.RandomState(self.dataset_seed)
+        train_dataset_mix_ds = []
+        custom_mix_ds = []
+        for mix_ds in self.train_dataset_mix_ds:
+            if os.path.exists(mix_ds):
+                custom_mix_ds.append(mix_ds)
+            else:
+                train_dataset_mix_ds.append(mix_ds)
+
+        if len(custom_mix_ds) > 0:
+            dataset_name = '_custom_mixture'
+            _register_local_dataset(dataset_name, custom_mix_ds, [])
+            train_dataset_mix_ds.append(dataset_name)
+        mix_dataset_sample = int(
+            len(train_dataset) * self.train_dataset_mix_ratio)
+        logger.info(f'train_dataset_mix_ds: {train_dataset_mix_ds}')
+        logger.info(
+            f'len(train_dataset): {len(train_dataset)}, mix_dataset_sample: {mix_dataset_sample}'
+        )
+        mixed_dataset = get_dataset(
+            train_dataset_mix_ds,
+            0.0,
+            random_state,
+            check_dataset_strategy=self.check_dataset_strategy)[0]
+        if len(mixed_dataset) < mix_dataset_sample:
+            logger.warn(
+                f'The length of dataset used for mixin: {train_dataset_mix_ds} are '
+                'lesser than the ratio required by the `train_dataset_mix_ratio` '
+                f'argument: {self.train_dataset_mix_ratio}. '
+                f'the actual ratio is: {len(mixed_dataset) / len(train_dataset):.6}.'
+            )
+        else:
+            train_idxs = random_state.permutation(mix_dataset_sample)
+            mixed_dataset = mixed_dataset.select(train_idxs)
+        return concatenate_datasets([train_dataset, mixed_dataset])
+
+    def prepare_push_ms_hub(self) -> None:
+        if not self.push_to_hub:
+            return
+        if self.hub_model_id is None:
+            self.hub_model_id = f'{self.model_type}-{self.sft_type}'
+            logger.info(f'Setting hub_model_id: {self.hub_model_id}')
+
+        api = HubApi()
+        if self.hub_token is None:
+            self.hub_token = os.environ.get('MODELSCOPE_API_TOKEN')
+        if self.hub_token is not None:
+            api.login(self.hub_token)
+        else:
+            assert ModelScopeConfig.get_token(
+            ) is not None, 'Please enter hub_token'
+        logger.info('hub login successful!')
+
     def _prepare_target_modules(self, target_modules) -> List[str]:
         if isinstance(target_modules, str):
             target_modules = [target_modules]
         if len(target_modules) == 0:
             return target_modules
         elif len(target_modules) == 1:
             if ',' in target_modules[0]:
@@ -277,34 +579,38 @@
             self.lora_m2s_use_embedding = True
         if 'LN' in modules_to_save:
             modules_to_save.remove('LN')
             self.lora_m2s_use_ln = True
         return modules_to_save
 
     def __post_init__(self) -> None:
-        handle_compatibility(self)
+        self.handle_compatibility()
         if is_pai_training_job():
             self._handle_pai_compat()
         ds_config_folder = os.path.join(__file__, '..', '..', 'ds_config')
-        if self.deepspeed == 'default-zero2':
-            self.deepspeed = os.path.abspath(
-                os.path.join(ds_config_folder, 'zero2.json'))
-        elif self.deepspeed == 'default-zero3':
-            self.deepspeed = os.path.abspath(
-                os.path.join(ds_config_folder, 'zero3.json'))
+        deepspeed_mapping = {
+            'default-zero2': 'zero2.json',
+            'default-zero3': 'zero3.json',
+            'zero3-offload': 'zero3_offload.json'
+        }
+        for ds_name, ds_config in deepspeed_mapping.items():
+            if self.deepspeed == ds_name:
+                self.deepspeed = os.path.abspath(
+                    os.path.join(ds_config_folder, ds_config))
+                break
 
-        handle_path(self)
-        set_model_type(self)
+        self.handle_path()
+        self.set_model_type()
         if isinstance(self.dataset, str):
             self.dataset = [self.dataset]
         if isinstance(self.train_dataset_mix_ds, str):
             self.train_dataset_mix_ds = [self.train_dataset_mix_ds]
-        register_custom_dataset(self)
-        check_flash_attn(self)
-        handle_generation_config(self)
+        self.register_custom_dataset()
+        self.check_flash_attn()
+        self.handle_generation_config()
 
         self.lora_use_embedding = False
         self.lora_use_all = False
         self.lora_m2s_use_embedding = False
         self.lora_m2s_use_ln = False
         if self.sft_type == 'ia3':
             self.ia3_feedforward_modules = self._prepare_target_modules(
@@ -339,32 +645,37 @@
             if self.sft_type == 'lora' and not self.lora_use_all:
                 logger.warning(
                     'Due to knowledge editing involved, it is recommended to add LoRA on MLP. '
                     'For example: `--lora_target_modules ALL`. '
                     'If you have already added LoRA on MLP, please ignore this warning.'
                 )
 
-        self.torch_dtype, self.fp16, self.bf16 = select_dtype(self)
+        self.torch_dtype, self.fp16, self.bf16 = self.select_dtype()
         world_size = 1
         if is_dist():
             rank, local_rank, world_size, _ = get_dist_setting()
-            torch.cuda.set_device(local_rank)
+            if is_torch_npu_available():
+                torch.npu.set_device(local_rank)
+            else:
+                torch.cuda.set_device(local_rank)
             self.seed += rank  # Avoid the same dropout
+            if self.ddp_backend is None:
+                self.ddp_backend = 'nccl'
             if self.ddp_backend == 'gloo' and self.quantization_bit != 0:
                 raise ValueError('not supported, please use `nccl`')
 
         if is_adapter(self.sft_type):
             assert self.freeze_parameters == 0., (
                 'lora does not support `freeze_parameters`, please set `--sft_type full`'
             )
             assert len(self.additional_trainable_parameters) == 0, (
                 'lora does not support `additional_trainable_parameters`, please set `--sft_type full`'
             )
-            if 'int4' in self.model_type or 'int8' in self.model_type:
-                assert self.quantization_bit == 0, 'int4 and int8 models do not need to be quantized again.'
+            if 'int4' in self.model_type or 'int8' in self.model_type or 'awq' in self.model_type:
+                assert self.quantization_bit == 0, 'int4, int8 or awq models do not need to be quantized again.'
             if self.learning_rate is None:
                 self.learning_rate = 1e-4
             if self.save_only_model is None:
                 if self.deepspeed is None:
                     self.save_only_model = False
                 else:
                     self.save_only_model = True
@@ -395,22 +706,22 @@
                                        and self.self_cognition_sample == 0):
             raise ValueError(
                 f'self.dataset: {self.dataset}, Please input the training dataset.'
             )
 
         if self.save_steps is None:
             self.save_steps = self.eval_steps
-        self.bnb_4bit_compute_dtype, self.load_in_4bit, self.load_in_8bit = select_bnb(
-            self)
+        self.bnb_4bit_compute_dtype, self.load_in_4bit, self.load_in_8bit = self.select_bnb(
+        )
 
         if self.neftune_backend is None:
             self.neftune_backend = 'swift' if version.parse(transformers.__version__) < version.parse('4.35') \
                 else 'transformers'
 
-        prepare_push_ms_hub(self)
+        self.prepare_push_ms_hub()
         self.train_sampler_random = not self.test_oom_error
         if self.eval_batch_size is None:
             if self.predict_with_generate:
                 self.eval_batch_size = 1
             else:
                 self.eval_batch_size = self.batch_size
         if self.save_total_limit == -1:
@@ -567,15 +878,15 @@
             self.add_output_dir_suffix = False
             logger.info(
                 f'Setting args.add_output_dir_suffix: {self.add_output_dir_suffix}'
             )
 
 
 @dataclass
-class InferArguments:
+class InferArguments(ArgumentsBase):
     # You can specify the model by either using the model_type or model_id_or_path.
     model_type: Optional[str] = field(
         default=None,
         metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
     model_id_or_path: Optional[str] = None
     model_revision: Optional[str] = None
 
@@ -650,65 +961,73 @@
 
     def __post_init__(self) -> None:
         if self.ckpt_dir is not None and not self.check_ckpt_dir_correct(
                 self.ckpt_dir):
             logger.warning(
                 f'The checkpoint dir {self.ckpt_dir} passed in is invalid, please make sure'
                 'the dir contains a `configuration.json` file.')
-        handle_compatibility(self)
-        handle_path(self)
+        self.handle_compatibility()
+        self.handle_path()
         logger.info(f'ckpt_dir: {self.ckpt_dir}')
         if self.ckpt_dir is None and self.load_args_from_ckpt_dir:
             self.load_args_from_ckpt_dir = False
             logger.info(
                 'Due to `ckpt_dir` being `None`, `load_args_from_ckpt_dir` is set to `False`.'
             )
         if self.load_args_from_ckpt_dir:
-            load_from_ckpt_dir(self)
+            self.load_from_ckpt_dir()
         else:
             assert self.load_dataset_config is False, 'You need to first set `--load_args_from_ckpt_dir true`.'
-        set_model_type(self)
+        self.set_model_type()
         if isinstance(self.dataset, str):
             self.dataset = [self.dataset]
-        register_custom_dataset(self)
-        check_flash_attn(self)
-        handle_generation_config(self)
+        self.register_custom_dataset()
+        self.check_flash_attn()
+        self.handle_generation_config()
 
-        self.torch_dtype, _, _ = select_dtype(self)
-        if self.template_type == 'AUTO':
-            self.template_type = get_default_template_type(self.model_type)
-            logger.info(f'Setting template_type: {self.template_type}')
+        self.torch_dtype, _, _ = self.select_dtype()
+        self.prepare_template()
         has_dataset = (
             len(self.dataset) > 0 or len(self.custom_train_dataset_path) > 0
             or len(self.custom_val_dataset_path) > 0)
         if self.eval_human is None:
             if not has_dataset:
                 self.eval_human = True
             else:
                 self.eval_human = False
             logger.info(f'Setting self.eval_human: {self.eval_human}')
         elif self.eval_human is False and not has_dataset:
             raise ValueError(
                 'Please provide the dataset or set `--load_dataset_config true`.'
             )
-        self.bnb_4bit_compute_dtype, self.load_in_4bit, self.load_in_8bit = select_bnb(
-            self)
+
+        self.bnb_4bit_compute_dtype, self.load_in_4bit, self.load_in_8bit = self.select_bnb(
+        )
 
         if self.max_length == -1:
             self.max_length = None
         if self.overwrite_generation_config is None:
             if self.ckpt_dir is None:
                 self.overwrite_generation_config = False
             else:
                 self.overwrite_generation_config = True
             logger.info(
                 f'Setting overwrite_generation_config: {self.overwrite_generation_config}'
             )
         if self.ckpt_dir is None:
             self.sft_type = 'full'
+
+        self.prepare_vllm()
+
+    def prepare_template(self):
+        if self.template_type == 'AUTO':
+            self.template_type = get_default_template_type(self.model_type)
+            logger.info(f'Setting template_type: {self.template_type}')
+
+    def prepare_vllm(self):
         model_info = MODEL_MAPPING[self.model_type]
         support_vllm = model_info.get('support_vllm', False)
         self.vllm_lora_request_list = None
         if self.infer_backend == 'AUTO':
             self.infer_backend = 'pt'
             if is_vllm_available() and support_vllm:
                 if ((self.sft_type == 'full'
@@ -737,14 +1056,43 @@
         if self.num_beams != 1:
             self.stream = False
             logger.info('Setting self.stream: False')
         self.infer_media_type = template_info.get('infer_media_type', 'none')
         if self.merge_device_map is None:
             self.merge_device_map = 'cpu'
 
+    def load_from_ckpt_dir(self) -> None:
+        sft_args_path = os.path.join(self.ckpt_dir, 'sft_args.json')
+        if not os.path.exists(sft_args_path):
+            logger.info(f'{sft_args_path} not found')
+            return
+        with open(sft_args_path, 'r', encoding='utf-8') as f:
+            sft_args = json.load(f)
+        imported_keys = [
+            'model_type', 'model_revision', 'sft_type', 'template_type',
+            'system', 'quantization_bit', 'bnb_4bit_comp_dtype',
+            'bnb_4bit_quant_type', 'bnb_4bit_use_double_quant'
+        ]
+        if self.load_dataset_config:
+            imported_keys += [
+                'dataset', 'dataset_seed', 'dataset_test_ratio',
+                'check_dataset_strategy', 'custom_train_dataset_path',
+                'custom_val_dataset_path'
+            ]
+        for key in imported_keys:
+            if (key in {
+                    'dataset', 'custom_train_dataset_path',
+                    'custom_val_dataset_path'
+            } and len(getattr(self, key)) > 0):
+                continue
+            setattr(self, key, sft_args.get(key))
+
+        if self.model_id_or_path is None:
+            self.model_id_or_path = sft_args.get('model_id_or_path')
+
     @staticmethod
     def check_ckpt_dir_correct(ckpt_dir) -> bool:
         """Check the checkpoint dir is correct, which means it must contains a `configuration.json` file.
         Args:
             ckpt_dir: The checkpoint dir
         Returns:
             A bool value represents the dir is valid or not.
@@ -778,36 +1126,58 @@
 
 
 @dataclass
 class EvalArguments(InferArguments):
 
     name: Optional[str] = None
 
+    eval_url: Optional[str] = None
+
+    eval_token: Optional[str] = 'EMPTY'
+
+    eval_is_chat_model: bool = None
+
     eval_dataset: List[str] = field(
         default_factory=lambda: ['ceval', 'gsm8k', 'arc'])
 
     eval_few_shot: Optional[int] = None
 
     eval_limit: Optional[int] = None
 
     custom_eval_config: Optional[str] = None
 
     eval_use_cache: Optional[bool] = False
 
+    def set_model_type(self) -> None:
+        if self.eval_url is None:
+            super().set_model_type()
+
+    def check_flash_attn(self) -> None:
+        if self.eval_url is None:
+            super().check_flash_attn()
+
+    def prepare_template(self) -> None:
+        if self.eval_url is None:
+            super().prepare_template()
+
+    def prepare_vllm(self) -> None:
+        if self.eval_url is None:
+            super().prepare_vllm()
+
 
 @dataclass
 class ExportArguments(InferArguments):
     to_peft_format: bool = False
     # The parameter has been defined in InferArguments.
     # merge_lora: bool = False
 
     # awq: 4; gptq: 2, 3, 4, 8
     quant_bits: int = 0  # e.g. 4
     quant_method: Literal['awq', 'gptq'] = 'awq'
-    quant_n_samples: Optional[int] = None
+    quant_n_samples: int = 256
     quant_seqlen: int = 2048
     quant_device_map: str = 'cpu'  # e.g. 'cpu', 'auto'
 
     # push to ms hub
     push_to_hub: bool = False
     # 'user_name/repo_name' or 'repo_name'
     hub_model_id: Optional[str] = None
@@ -824,22 +1194,14 @@
     def __post_init__(self):
         if self.merge_device_map is None:
             self.merge_device_map = 'cpu' if self.quant_bits != 0 else 'auto'
         super().__post_init__()
         if len(self.dataset) == 0:
             self.dataset = ['ms-bench-mini']
             logger.info(f'Setting args.dataset: {self.dataset}')
-        if self.quant_n_samples is None:
-            if self.quant_method == 'awq':
-                self.quant_n_samples = 256
-            elif self.quant_method == 'gptq':
-                self.quant_n_samples = 1024
-            else:
-                raise ValueError(
-                    f'args.quant_n_samples: {self.quant_n_samples}')
 
 
 @dataclass
 class DPOArguments(SftArguments):
 
     ref_model_type: Optional[str] = field(
         default=None,
@@ -861,225 +1223,31 @@
         metadata={
             'help':
             'The rome request file, please check the documentation '
             'to get the format'
         })
 
     def __post_init__(self) -> None:
-        handle_compatibility(self)
-        handle_path(self)
-        set_model_type(self)
-        check_flash_attn(self)
+        self.handle_compatibility()
+        self.handle_path()
+        self.set_model_type()
+        self.check_flash_attn()
 
-        self.torch_dtype, _, _ = select_dtype(self)
+        self.torch_dtype, _, _ = self.select_dtype()
         if self.template_type == 'AUTO':
             self.template_type = get_default_template_type(self.model_type)
             logger.info(f'Setting template_type: {self.template_type}')
 
         if self.max_length == -1:
             self.max_length = None
 
 
 dtype_mapping_reversed = {v: k for k, v in dtype_mapping.items()}
 
 
-def select_dtype(
-    args: Union[SftArguments, InferArguments]
-) -> Tuple[Optional[Dtype], bool, bool]:
-    if not is_torch_cuda_available() and not is_torch_npu_available():
-        # cpu
-        if args.dtype == 'AUTO':
-            args.dtype = 'fp32'
-            logger.info(f'Setting args.dtype: {args.dtype}')
-        assert args.dtype != 'fp16', 'The CPU does not support matrix multiplication with FP16.'
-        if args.dtype == 'fp32':
-            return torch.float32, False, False
-        elif args.dtype == 'bf16':
-            return torch.bfloat16, False, True
-        else:
-            raise ValueError(f'args.dtype: {args.dtype}')
-    # cuda, npu
-    if args.dtype == 'AUTO' and not is_torch_bf16_gpu_available():
-        args.dtype = 'fp16'
-    if args.dtype == 'AUTO' and ('int4' in args.model_type
-                                 or 'int8' in args.model_type):
-        model_torch_dtype = MODEL_MAPPING[args.model_type]['torch_dtype']
-        if model_torch_dtype is not None:
-            args.dtype = dtype_mapping[model_torch_dtype]
-    if args.dtype == 'AUTO':
-        if isinstance(args, SftArguments):
-            args.dtype = 'bf16'
-        else:
-            return None, False, False
-
-    torch_dtype = dtype_mapping_reversed[args.dtype]
-
-    assert torch_dtype in {torch.float16, torch.bfloat16, torch.float32}
-    if torch_dtype == torch.float16:
-        if isinstance(args, SftArguments) and args.sft_type == 'full':
-            args.dtype = 'fp32'
-            torch_dtype = torch.float32
-            logger.warning(
-                'Fine-tuning with full parameters does not support fp16, and is prone to NaN. '
-                'We will use the fp32 & AMP approach, which consumes approximately twice the memory of bf16.'
-            )
-            logger.info(f'Setting torch_dtype: {torch_dtype}')
-        fp16, bf16 = True, False
-    elif torch_dtype == torch.bfloat16:
-        support_bf16 = is_torch_bf16_gpu_available()
-        if not support_bf16:
-            logger.warning(f'support_bf16: {support_bf16}')
-        fp16, bf16 = False, True
-    else:
-        fp16, bf16 = False, False
-    return torch_dtype, fp16, bf16
-
-
-def select_bnb(
-    args: Union[SftArguments, InferArguments]
-) -> Tuple[Optional[Dtype], bool, bool]:
-    if args.bnb_4bit_comp_dtype == 'AUTO':
-        args.bnb_4bit_comp_dtype = args.dtype
-
-    if args.bnb_4bit_comp_dtype != 'AUTO':
-        bnb_4bit_compute_dtype = dtype_mapping_reversed[
-            args.bnb_4bit_comp_dtype]
-        assert bnb_4bit_compute_dtype in {
-            torch.float16, torch.bfloat16, torch.float32
-        }
-    else:
-        bnb_4bit_compute_dtype = None
-    quantization_bit = args.quantization_bit
-    if quantization_bit == 4:
-        require_version('bitsandbytes')
-        load_in_4bit, load_in_8bit = True, False
-    elif quantization_bit == 8:
-        require_version('bitsandbytes')
-        load_in_4bit, load_in_8bit = False, True
-    else:
-        load_in_4bit, load_in_8bit = False, False
-
-    return bnb_4bit_compute_dtype, load_in_4bit, load_in_8bit
-
-
-def handle_compatibility(args: Union[SftArguments, InferArguments]) -> None:
-    template_type_mapping = {
-        'chatglm2-generation': 'chatglm-generation',
-        'chatml': 'qwen'
-    }
-    model_type_mapping = {
-        'openbmb-minicpm-2b-sft-chat': 'minicpm-2b-sft-chat',
-        'openbmb-minicpm-2b-chat': 'minicpm-2b-chat',
-    }
-    for k, v in template_type_mapping.items():
-        if k == args.template_type:
-            args.template_type = v
-            break
-    for k, v in model_type_mapping.items():
-        if k == args.model_type:
-            args.model_type = v
-            break
-    if args.dataset is not None and len(
-            args.dataset) == 1 and ',' in args.dataset[0]:
-        args.dataset = args.dataset[0].split(',')
-    if args.truncation_strategy == 'ignore':
-        args.truncation_strategy = 'delete'
-    if isinstance(args, InferArguments):
-        if args.show_dataset_sample != 10 and args.val_dataset_sample == 10:
-            # args.val_dataset_sample is the default value and args.show_dataset_sample is not the default value.
-            args.val_dataset_sample = args.show_dataset_sample
-        if args.safe_serialization is not None:
-            args.save_safetensors = args.safe_serialization
-        if args.merge_lora_and_save is not None:
-            args.merge_lora = args.merge_lora_and_save
-    if isinstance(args, SftArguments):
-        if args.only_save_model is not None:
-            args.save_only_model = args.only_save_model
-        if args.neftune_alpha is not None:
-            args.neftune_noise_alpha = args.neftune_alpha
-        if args.per_device_train_batch_size is not None:
-            args.batch_size = args.per_device_train_batch_size
-        if args.per_device_eval_batch_size is not None:
-            args.eval_batch_size = args.per_device_eval_batch_size
-        if args.deepspeed_config_path is not None:
-            args.deepspeed = args.deepspeed_config_path
-
-
-def set_model_type(args: Union[SftArguments, InferArguments]) -> None:
-    # compat with swift<1.7
-    if args.model_cache_dir is not None and args.model_id_or_path is None:
-        args.model_id_or_path = args.model_cache_dir
-        args.model_cache_dir = None
-
-    if args.model_id_or_path is not None:
-        model_mapping_reversed = {
-            v['model_id_or_path'].lower(): k
-            for k, v in MODEL_MAPPING.items()
-        }
-        model_id_or_path = args.model_id_or_path
-        model_id_or_path_lower = model_id_or_path.lower()
-        if model_id_or_path_lower not in model_mapping_reversed:
-            if (isinstance(args, InferArguments)
-                    and 'checkpoint' in model_id_or_path
-                    and 'merged' not in model_id_or_path
-                    and args.ckpt_dir is None):
-                raise ValueError(
-                    'Please use `--ckpt_dir vx-xxx/checkpoint-xxx` to use the checkpoint.'
-                )
-            if args.model_type is None:
-                raise ValueError(
-                    f"model_id_or_path: '{model_id_or_path}' is not registered. "
-                    'Please set `--model_type <model_type>` additionally.')
-            assert args.model_cache_dir is None
-        else:
-            model_type = model_mapping_reversed[model_id_or_path_lower]
-            assert args.model_type is None or args.model_type == model_type
-            args.model_type = model_type
-            logger.info(f'Setting args.model_type: {model_type}')
-            if args.model_cache_dir is not None:
-                args.model_id_or_path = args.model_cache_dir
-
-    error_msg = f'The model_type you can choose: {list(MODEL_MAPPING.keys())}'
-    if args.model_type is None:
-        raise ValueError('please setting `--model_type <model_type>`. '
-                         + error_msg)
-    elif args.model_type not in MODEL_MAPPING:
-        raise ValueError(f"model_type: '{args.model_type}' is not registered. "
-                         + error_msg)
-    model_info = MODEL_MAPPING[args.model_type]
-    if args.model_revision is None:
-        args.model_revision = model_info['revision']
-    else:
-        model_info['revision'] = args.model_revision
-        logger.info(f"Setting model_info['revision']: {args.model_revision}")
-    if args.model_id_or_path is None:
-        args.model_id_or_path = model_info['model_id_or_path']
-    requires = model_info['requires']
-    for require in requires:
-        require_version(require)
-
-
-def prepare_push_ms_hub(args: SftArguments) -> None:
-    if not args.push_to_hub:
-        return
-    if args.hub_model_id is None:
-        args.hub_model_id = f'{args.model_type}-{args.sft_type}'
-        logger.info(f'Setting hub_model_id: {args.hub_model_id}')
-
-    api = HubApi()
-    if args.hub_token is None:
-        args.hub_token = os.environ.get('MODELSCOPE_API_TOKEN')
-    if args.hub_token is not None:
-        api.login(args.hub_token)
-    else:
-        assert ModelScopeConfig.get_token(
-        ) is not None, 'Please enter hub_token'
-    logger.info('hub login successful!')
-
-
 def _check_path(
         k: str, value: Union[str, List[str]],
         check_exist_path_set: Optional[Set[str]]) -> Union[str, List[str]]:
     if isinstance(value, str):
         value = os.path.expanduser(value)
         value = os.path.abspath(value)
         if k in check_exist_path_set and not os.path.exists(value):
@@ -1088,162 +1256,25 @@
         res = []
         for v in value:
             res.append(_check_path(k, v, check_exist_path_set))
         value = res
     return value
 
 
-def handle_path(args: Union[SftArguments, InferArguments]) -> None:
-    check_exist_path = [
-        'ckpt_dir', 'resume_from_checkpoint', 'custom_train_dataset_path',
-        'custom_val_dataset_path'
-    ]
-    if args.model_id_or_path is not None and (
-            args.model_id_or_path.startswith('~')
-            or args.model_id_or_path.startswith('/')):
-        check_exist_path.append('model_id_or_path')
-    check_exist_path_set = set(check_exist_path)
-    other_path = ['output_dir', 'logging_dir']
-    for k in check_exist_path + other_path:
-        value = getattr(args, k, None)
-        if value is None:
-            continue
-        value = _check_path(k, value, check_exist_path_set)
-        setattr(args, k, value)
-
-
 def _register_local_dataset(dataset_name: str, train_dataset_path: List[str],
                             val_dataset_path: List[str]) -> None:
     register_dataset(
         dataset_name,
         '_',
         train_dataset_path,
         val_dataset_path,
         get_function=get_custom_dataset,
         exists_ok=True)
 
 
-def register_custom_dataset(args: Union[SftArguments, InferArguments]) -> None:
-    dataset = []
-    for d in args.dataset:
-        if os.path.exists(d):
-            args.custom_train_dataset_path.append(d)
-        else:
-            dataset.append(d)
-    args.dataset = dataset
-
-    for key in ['custom_train_dataset_path', 'custom_val_dataset_path']:
-        value = getattr(args, key)
-        if isinstance(value, str):
-            setattr(args, key, [value])
-    if len(args.custom_train_dataset_path) == 0 and len(
-            args.custom_val_dataset_path) == 0:
-        return
-
-    dataset_name = '_custom_dataset'
-    _register_local_dataset(dataset_name, args.custom_train_dataset_path,
-                            args.custom_val_dataset_path)
-    args.dataset.append(dataset_name)
-
-
-def load_from_ckpt_dir(args: InferArguments) -> None:
-    sft_args_path = os.path.join(args.ckpt_dir, 'sft_args.json')
-    if not os.path.exists(sft_args_path):
-        logger.info(f'{sft_args_path} not found')
-        return
-    with open(sft_args_path, 'r', encoding='utf-8') as f:
-        sft_args = json.load(f)
-    imported_keys = [
-        'model_type', 'model_revision', 'sft_type', 'template_type', 'system',
-        'quantization_bit', 'bnb_4bit_comp_dtype', 'bnb_4bit_quant_type',
-        'bnb_4bit_use_double_quant'
-    ]
-    if args.load_dataset_config:
-        imported_keys += [
-            'dataset', 'dataset_seed', 'dataset_test_ratio',
-            'check_dataset_strategy', 'custom_train_dataset_path',
-            'custom_val_dataset_path'
-        ]
-    for key in imported_keys:
-        if (key in {
-                'dataset', 'custom_train_dataset_path',
-                'custom_val_dataset_path'
-        } and len(getattr(args, key)) > 0):
-            continue
-        setattr(args, key, sft_args.get(key))
-
-    if args.model_id_or_path is None:
-        args.model_id_or_path = sft_args.get('model_id_or_path')
-
-
-def check_flash_attn(args: Union[SftArguments, InferArguments]) -> None:
-    model_info = MODEL_MAPPING[args.model_type]
-    support_flash_attn = model_info.get('support_flash_attn', False)
-    if args.use_flash_attn and not support_flash_attn:
-        logger.warning(f'use_flash_attn: {args.use_flash_attn}, '
-                       f'but support_flash_attn: {support_flash_attn}')
-
-
-def handle_generation_config(
-        args: Union[SftArguments, InferArguments]) -> None:
-    if args.do_sample is False:
-        # fix warning
-        args.temperature = 1.
-        args.top_p = 1.
-        args.top_k = 50
-        logger.info(
-            'Due to do_sample=False, the following settings are applied: args.temperature: '
-            f'{args.temperature}, args.top_p: {args.top_p}, args.top_k: {args.top_k}.'
-        )
-
-
-def handle_dataset_mixture(args: SftArguments,
-                           train_dataset: HfDataset) -> None:
-    if train_dataset is None:
-        return train_dataset
-    if args.train_dataset_mix_ratio <= 0 or len(
-            args.train_dataset_mix_ds) == 0:
-        return train_dataset
-
-    random_state = np.random.RandomState(args.dataset_seed)
-    train_dataset_mix_ds = []
-    custom_mix_ds = []
-    for mix_ds in args.train_dataset_mix_ds:
-        if os.path.exists(mix_ds):
-            custom_mix_ds.append(mix_ds)
-        else:
-            train_dataset_mix_ds.append(mix_ds)
-
-    if len(custom_mix_ds) > 0:
-        dataset_name = '_custom_mixture'
-        _register_local_dataset(dataset_name, custom_mix_ds, [])
-        train_dataset_mix_ds.append(dataset_name)
-    mix_dataset_sample = int(len(train_dataset) * args.train_dataset_mix_ratio)
-    logger.info(f'train_dataset_mix_ds: {train_dataset_mix_ds}')
-    logger.info(
-        f'len(train_dataset): {len(train_dataset)}, mix_dataset_sample: {mix_dataset_sample}'
-    )
-    mixed_dataset = get_dataset(
-        train_dataset_mix_ds,
-        0.0,
-        random_state,
-        check_dataset_strategy=args.check_dataset_strategy)[0]
-    if len(mixed_dataset) < mix_dataset_sample:
-        logger.warn(
-            f'The length of dataset used for mixin: {train_dataset_mix_ds} are '
-            'lesser than the ratio required by the `train_dataset_mix_ratio` '
-            f'argument: {args.train_dataset_mix_ratio}. '
-            f'the actual ratio is: {len(mixed_dataset)/len(train_dataset):.6}.'
-        )
-    else:
-        train_idxs = random_state.permutation(mix_dataset_sample)
-        mixed_dataset = mixed_dataset.select(train_idxs)
-    return concatenate_datasets([train_dataset, mixed_dataset])
-
-
 def swift_to_peft_format(lora_checkpoint_path: str) -> str:
     if 'default' in os.listdir(lora_checkpoint_path):  # swift_backend
         new_lora_checkpoint_path = f'{lora_checkpoint_path}-peft'
         Swift.save_to_peft_format(lora_checkpoint_path,
                                   new_lora_checkpoint_path)
         lora_checkpoint_path = new_lora_checkpoint_path
         logger.info('Converting the swift format checkpoint to peft format, '
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/client_utils.py` & `ms-swift-2.0.3/swift/llm/utils/client_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/llm/utils/dataset.py` & `ms-swift-2.0.3/swift/llm/utils/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from functools import partial
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import json
 import numpy as np
 import pandas as pd
 from datasets import Dataset as HfDataset
-from datasets import concatenate_datasets
-from modelscope import MsDataset
+from datasets import concatenate_datasets, load_dataset
 from numpy.random import RandomState
 from pandas import DataFrame
 from tqdm.auto import tqdm
+from transformers.utils import strtobool
 
 from swift.utils import (get_logger, get_seed, read_from_jsonl,
                          transform_jsonl_to_df)
 from .preprocess import (AlpacaPreprocessor, ClsPreprocessor,
                          ComposePreprocessor, ConversationsPreprocessor,
                          PreprocessFunc, RenameColumnsPreprocessor,
                          SmartPreprocessor, TextGenerationPreprocessor)
@@ -63,21 +63,28 @@
     sharegpt_zh = 'sharegpt-zh'
     tulu_v2_sft_mixture = 'tulu-v2-sft-mixture'
     wikipedia_zh = 'wikipedia-zh'
     open_orca = 'open-orca'
     open_orca_gpt4 = 'open-orca-gpt4'
     sharegpt_gpt4 = 'sharegpt-gpt4'
     sharegpt_gpt4_mini = 'sharegpt-gpt4-mini'
+    deepctrl_sft_zh = 'deepctrl-sft-zh'
+    deepctrl_sft_en = 'deepctrl-sft-en'
     # agent
     ms_agent = 'ms-agent'
     ms_agent_for_agentfabric_default = 'ms-agent-for-agentfabric-default'
     ms_agent_for_agentfabric_addition = 'ms-agent-for-agentfabric-addition'
+    ms_agent_multirole = 'ms-agent-multirole'
     damo_agent_zh = 'damo-agent-zh'
     damo_agent_mini_zh = 'damo-agent-mini-zh'
     agent_instruct_all_en = 'agent-instruct-all-en'
+    toolbench_for_alpha_umi_backbone = 'toolbench-for-alpha-umi-backbone'
+    toolbench_for_alpha_umi_caller = 'toolbench-for-alpha-umi-caller'
+    toolbench_for_alpha_umi_planner = 'toolbench-for-alpha-umi-planner'
+    toolbench_for_alpha_umi_summarizer = 'toolbench-for-alpha-umi-summarizer'
     # coding
     code_alpaca_en = 'code-alpaca-en'
     leetcode_python_en = 'leetcode-python-en'
     codefuse_python_en = 'codefuse-python-en'
     codefuse_evol_instruction_zh = 'codefuse-evol-instruction-zh'
     # medical
     medical_en = 'medical-en'
@@ -175,14 +182,15 @@
         dataset_name: str,
         dataset_id_or_path: str,
         train_subset_split_list: Optional[List[SubsetSplit]] = None,
         val_subset_split_list: Optional[List[SubsetSplit]] = None,
         preprocess_func: Optional[PreprocessFunc] = None,
         get_function: Optional[GetDatasetFunction] = None,
         *,
+        hf_dataset_id: Optional[str] = None,
         function_kwargs: Optional[Dict[str, Any]] = None,
         exists_ok: bool = False,
         **kwargs
 ) -> Optional[Callable[[GetDatasetFunction], GetDatasetFunction]]:
     if preprocess_func is None:
         preprocess_func = SmartPreprocessor()
     if not exists_ok and dataset_name in DATASET_MAPPING:
@@ -197,14 +205,15 @@
         function_kwargs = {}
 
     dataset_info = {
         'dataset_id_or_path': dataset_id_or_path,
         'train_subset_split_list': train_subset_split_list,
         'val_subset_split_list': val_subset_split_list,
         'preprocess_func': preprocess_func,
+        'hf_dataset_id': hf_dataset_id,
         **kwargs
     }
     if get_function is not None:
         if len(function_kwargs) > 0:
             get_function = partial(get_function, **function_kwargs)
         dataset_info['get_function'] = get_function
         DATASET_MAPPING[dataset_name] = dataset_info
@@ -221,38 +230,63 @@
 
     return _register_dataset
 
 
 def load_ms_dataset(
         dataset_id: str,
         subset_split_list: Optional[List[SubsetSplit]]) -> Optional[HfDataset]:
+    from modelscope import MsDataset
     if subset_split_list is None or len(subset_split_list) == 0:
         return None
     dataset_list = []
     for subset_split in subset_split_list:
         if isinstance(subset_split, str):
             subset_split = ('default', subset_split)
         assert len(subset_split) == 2
         subset_name, split = subset_split
+        force_redownload = strtobool(
+            os.environ.get('FORCE_REDOWNLOAD', 'False'))
+        download_mode = 'force_redownload' if force_redownload else 'reuse_dataset_if_exists'
         dataset = MsDataset.load(
-            dataset_id, subset_name=subset_name, split=split)
+            dataset_id,
+            subset_name=subset_name,
+            split=split,
+            download_mode=download_mode)
         if hasattr(dataset, 'to_hf_dataset'):
             dataset = dataset.to_hf_dataset()
         dataset_list.append(dataset)
     return concatenate_datasets(dataset_list)
 
 
+def load_hf_dataset(
+        dataset_id: str,
+        subset_split_list: Optional[List[SubsetSplit]]) -> Optional[HfDataset]:
+    if subset_split_list is None or len(subset_split_list) == 0:
+        return None
+    dataset_list = []
+    for subset_split in subset_split_list:
+        if isinstance(subset_split, str):
+            subset_split = (None, subset_split)
+        assert len(subset_split) == 2
+        subset_name, split = subset_split
+        dataset = load_dataset(dataset_id, name=subset_name, split=split)
+        dataset_list.append(dataset)
+    return concatenate_datasets(dataset_list)
+
+
 @register_dataset(
     DatasetName.text2sql_en,
     'AI-ModelScope/texttosqlv2_25000_v2', ['train'],
-    tags=['chat', 'sql'])
+    tags=['chat', 'sql'],
+    hf_dataset_id='Clinton/texttosqlv2_25000_v2')
 @register_dataset(
     DatasetName.school_math_zh,
     'AI-ModelScope/school_math_0.25M', ['train'],
-    tags=['chat', 'math'])
+    tags=['chat', 'math'],
+    hf_dataset_id='BelleGroup/school_math_0.25M')
 @register_dataset(
     DatasetName.gpt4all_en,
     'wyj123456/GPT4all', ['train'],
     tags=['chat', 'general'])
 @register_dataset(
     DatasetName.cot_zh, 'YorickHe/CoT_zh', ['train'], tags=['chat', 'general'])
 @register_dataset(
@@ -264,23 +298,26 @@
 @register_dataset(
     DatasetName.instinwild_zh,
     'wyj123456/instinwild', ['train'],
     tags=['chat', 'general'])
 @register_dataset(
     DatasetName.code_alpaca_en,
     'wyj123456/code_alpaca_en', ['train'],
-    tags=['chat', 'coding'])
+    tags=['chat', 'coding'],
+    hf_dataset_id='sahil2801/CodeAlpaca-20k')
 @register_dataset(
     DatasetName.finance_en,
     'wyj123456/finance_en', ['train'],
-    tags=['chat', 'financial'])
+    tags=['chat', 'financial'],
+    hf_dataset_id='ssbuild/alpaca_finance_en')
 @register_dataset(
     DatasetName.alpaca_en,
     'AI-ModelScope/alpaca-gpt4-data-en', ['train'],
-    tags=['chat', 'general', '🔥'])
+    tags=['chat', 'general', '🔥'],
+    hf_dataset_id='vicgalle/alpaca-gpt4')
 @register_dataset(
     DatasetName.coig_cqia_chinese_traditional,
     'AI-ModelScope/COIG-CQIA', [('chinese_traditional', 'train')],
     tags=['general', '🔥'])
 @register_dataset(
     DatasetName.coig_cqia_coig_pc,
     'AI-ModelScope/COIG-CQIA', [('coig_pc', 'train')],
@@ -340,20 +377,24 @@
 def get_dataset_from_repo(
         dataset_id: str,
         train_subset_split_list: List[SubsetSplit],
         val_subset_split_list: Optional[List[SubsetSplit]],
         preprocess_func: PreprocessFunc,
         remove_useless_columns: bool = True,
         train_dataset_sample: int = -1,
-        val_dataset_sample: int = -1) -> Tuple[HfDataset, Optional[HfDataset]]:
+        val_dataset_sample: int = -1,
+        use_hf: bool = False) -> Tuple[HfDataset, Optional[HfDataset]]:
     dataset_list = []
     _iter = zip([train_subset_split_list, val_subset_split_list],
                 [train_dataset_sample, val_dataset_sample])
     for subset_split_list, dataset_sample in _iter:
-        dataset = load_ms_dataset(dataset_id, subset_split_list)
+        if use_hf:
+            dataset = load_hf_dataset(dataset_id, subset_split_list)
+        else:
+            dataset = load_ms_dataset(dataset_id, subset_split_list)
         if dataset is not None:
             if dataset_sample > 0 and len(dataset) > dataset_sample:
                 random_state = np.random.RandomState(42)
                 idxs = random_state.permutation(dataset_sample)
                 dataset = dataset.select(idxs)
             dataset = preprocess_func(dataset)
             if remove_useless_columns:
@@ -398,15 +439,16 @@
 
 register_dataset(
     DatasetName.alpaca_zh,
     'AI-ModelScope/alpaca-gpt4-data-zh', ['train'],
     None,
     AlpacaPreprocessor(concat_inst_inp=_concat_inst_inp_alpaca_zh),
     get_dataset_from_repo,
-    tags=['chat', 'general', '🔥'])
+    tags=['chat', 'general', '🔥'],
+    hf_dataset_id='c-s-ale/alpaca-gpt4-data-zh')
 
 
 def _preprocess_vision_dataset(dataset: HfDataset) -> HfDataset:
     prompt = 'please describe the image.'
     image_key = 'image'
     response_key = 'caption'
 
@@ -505,35 +547,37 @@
     _preprocess_aishell1_dataset,
     get_dataset_from_repo,
     function_kwargs={'val_dataset_sample': 200},
     tags=['chat', 'multi-modal', 'audio', '🔥'])
 
 
 def _repair_agent_conversations(conversations: str,
-                                use_mini: bool) -> Dict[str, str]:
+                                use_mini: bool) -> List[Dict[str, str]]:
     if use_mini:
         pattern = r'\d\. {"plugin_name": "(.+?)"'
     else:
         pattern = r'\d\. {"(?:plugin_)?name": "(.+?)"'
 
     idx = conversations.find(r"'from': 'user")
     if idx == -1:
         return
     # remove dirty data
     find_list = re.findall(pattern, conversations[:idx])
     if len(set(find_list)) <= 1:
         return
-    conversations = ast.literal_eval(conversations)
+    if isinstance(conversations, str):
+        conversations = ast.literal_eval(conversations)
     if len(conversations) == 1:
         return
     return conversations
 
 
-def _repair_ms_bench(conversations: str) -> Dict[str, str]:
-    conversations = ast.literal_eval(conversations)
+def _repair_ms_bench(conversations: str) -> List[Dict[str, str]]:
+    if isinstance(conversations, str):
+        conversations = ast.literal_eval(conversations)
     default_system = 'You are a helpful assistant.'
     if conversations[0]['from'] == 'system' and conversations[0][
             'value'] == default_system:
         conversations.pop(0)
     # skip MOSS
     for c in conversations:
         value = c['value'].lower()
@@ -555,15 +599,16 @@
 
 
 register_dataset(
     DatasetName.long_alpaca_12k,
     'AI-ModelScope/LongAlpaca-12k', ['train'], [],
     long_alpaca_preprocessor,
     get_dataset_from_repo,
-    tags=['longlora', 'QA'])
+    tags=['longlora', 'QA'],
+    hf_dataset_id='Yukang/LongAlpaca-12k')
 
 
 def _preprocess_ruozhiba(dataset: HfDataset):
 
     def map_row(row):
         title = row['title'] if 'title' in row else row['content']
         abs = row['abs'] if 'abs' in row else None
@@ -623,35 +668,55 @@
     tags=['chat', 'agent', 'multi-round', '🔥'])
 
 register_dataset(
     DatasetName.damo_agent_mini_zh,
     'damo/MSAgent-Bench', ['train'], ['validation'],
     ConversationsPreprocessor(
         repair_conversations=partial(
-            _repair_agent_conversations, use_mini=True)),
+            _repair_agent_conversations, use_mini=True),
+        error_strategy='delete'),
     get_dataset_from_repo,
     tags=['chat', 'agent', 'multi-round'])
 register_dataset(
     DatasetName.damo_agent_zh,
     'damo/MSAgent-Bench', ['train'], ['validation'],
     ConversationsPreprocessor(
         repair_conversations=partial(
-            _repair_agent_conversations, use_mini=False)),
+            _repair_agent_conversations,
+            use_mini=False,
+            error_strategy='delete')),
     get_dataset_from_repo,
     tags=['chat', 'agent', 'multi-round'])
 
+register_dataset(
+    DatasetName.deepctrl_sft_zh,
+    'AI-ModelScope/deepctrl-sft-data', [['default', 'train']],
+    None,
+    SmartPreprocessor(),
+    get_dataset_from_repo,
+    tags=['chat', 'general', 'sft', 'multi-round'])
+
+register_dataset(
+    DatasetName.deepctrl_sft_en,
+    'AI-ModelScope/deepctrl-sft-data', [['en', 'train']],
+    None,
+    SmartPreprocessor(),
+    get_dataset_from_repo,
+    tags=['chat', 'general', 'sft', 'multi-round'])
+
 advertise_gen_prompt = """Task: Generating advertisements based on keywords.
 Keywords: {query}
 Advertisements:"""
 register_dataset(
     DatasetName.advertise_gen_zh,
     'lvjianjin/AdvertiseGen', ['train'], ['validation'],
     TextGenerationPreprocessor(advertise_gen_prompt, 'content', 'summary'),
     get_dataset_from_repo,
-    tags=['text-generation', '🔥'])
+    tags=['text-generation', '🔥'],
+    hf_dataset_id='shibing624/AdvertiseGen')
 
 _firefly_kind_list = [
     'ProseGeneration', 'MRC', 'JinYongGeneration', 'TextCorrection',
     'ClassicalChinese', 'BELLE', 'StoryGeneration', 'Couplet', 'Cot',
     'Dictionary', 'Translation', 'Program', 'SentimentAnalyze', 'OpenQA',
     'AncientPoem', 'TextMatching', 'NLI', 'Summary', 'KeywordRecognition',
     'ProductDesc', 'LyricGeneration', 'Composition', 'MusicComment', 'NER'
@@ -714,27 +779,29 @@
 
 register_dataset(
     DatasetName.cmnli_zh,
     'clue', [('cmnli', 'train')], [('cmnli', 'validation')],
     ClsPreprocessor(['neutral', 'entailment', 'contradiction'],
                     'Natural Language Inference', True),
     get_dataset_from_repo,
-    tags=['text-generation', 'classification'])
+    tags=['text-generation', 'classification'],
+    hf_dataset_id='clue')
 
 register_dataset(
     DatasetName.cmnli_mini_zh,
     'clue', [('cmnli', 'train')], [('cmnli', 'validation')],
     ClsPreprocessor(['neutral', 'entailment', 'contradiction'],
                     'Natural Language Inference', True),
     get_dataset_from_repo,
     function_kwargs={
         'train_dataset_sample': 20000,
         'val_dataset_sample': 200
     },
-    tags=['text-generation', 'classification', '🔥'])
+    tags=['text-generation', 'classification', '🔥'],
+    hf_dataset_id='clue')
 
 register_dataset(
     DatasetName.jd_sentiment_zh,
     'DAMO_NLP/jd', ['train'], ['validation'],
     ClsPreprocessor(['negative', 'positive'], 'Sentiment Classification',
                     False),
     get_dataset_from_repo,
@@ -1014,15 +1081,16 @@
 
 
 def _preprocess_sharegpt(dataset: HfDataset) -> HfDataset:
     query = []
     response = []
     history: List[History] = []
     for d in tqdm(dataset):
-        conversation = ast.literal_eval(d['conversation'])
+        if isinstance(d['conversation'], str):
+            conversation = ast.literal_eval(d['conversation'])
         query.append(conversation[-1]['human'])
         response.append(conversation[-1]['assistant'])
         h = []
         for c in conversation[:-1]:
             h.append([c['human'], c['assistant']])
         history.append(h)
     return HfDataset.from_dict({
@@ -1070,14 +1138,22 @@
         'response': response,
         'images': images
     })
     dataset._info.features._column_requires_decoding['images'] = True
     return dataset
 
 
+def _repair_planner(conversations: list) -> list:
+    if isinstance(conversations, str):
+        conversations = ast.literal_eval(conversations)
+    if len(conversations) == 2 and conversations[0]['from'] != 'user':
+        conversations[0]['from'] = 'user'
+    return conversations
+
+
 register_dataset(
     DatasetName.capcha_images,
     'AI-ModelScope/captcha-images', [('default', 'train')],
     [('default', 'validation')],
     _preprocess_capcha_images,
     get_dataset_from_repo,
     tags=['chat', 'multi-modal', 'vision'])
@@ -1113,14 +1189,47 @@
         'bot',
         conversations_key='chat_rounds',
         from_key='role',
         value_key='content'),
     get_dataset_from_repo,
     tags=['chat', 'coding', '🔥'])
 
+register_dataset(
+    DatasetName.toolbench_for_alpha_umi_backbone,
+    'shenweizhou/alpha-umi-toolbench-processed-v2', [('backbone', 'train')],
+    None,
+    ConversationsPreprocessor('system', system_role=None),
+    get_dataset_from_repo,
+    tags=['chat', 'agent'])
+
+register_dataset(
+    DatasetName.toolbench_for_alpha_umi_caller,
+    'shenweizhou/alpha-umi-toolbench-processed-v2', [('caller', 'train')],
+    None,
+    ConversationsPreprocessor('system', 'caller', None),
+    get_dataset_from_repo,
+    tags=['chat', 'agent'])
+
+register_dataset(
+    DatasetName.toolbench_for_alpha_umi_planner,
+    'shenweizhou/alpha-umi-toolbench-processed-v2', [('planner', 'train')],
+    None,
+    ConversationsPreprocessor(
+        repair_conversations=_repair_planner, error_strategy='delete'),
+    get_dataset_from_repo,
+    tags=['chat', 'agent'])
+
+register_dataset(
+    DatasetName.toolbench_for_alpha_umi_summarizer,
+    'shenweizhou/alpha-umi-toolbench-processed-v2', [('summarizer', 'train')],
+    None,
+    ConversationsPreprocessor('system', 'conclusion', None),
+    get_dataset_from_repo,
+    tags=['chat', 'agent'])
+
 
 def _preprocess_blossom_math(dataset: HfDataset) -> HfDataset:
     response = []
     for d in tqdm(dataset):
         output, answer = d['output'], d['answer']
         response.append(f'{output}\n\nAnswer: {answer}')
     return HfDataset.from_dict({
@@ -1131,42 +1240,45 @@
 
 register_dataset(
     DatasetName.blossom_math_zh,
     'AI-ModelScope/blossom-math-v2', ['train'],
     None,
     _preprocess_blossom_math,
     get_dataset_from_repo,
-    tags=['chat', 'math', '🔥'])
+    tags=['chat', 'math', '🔥'],
+    hf_dataset_id='Azure99/blossom-math-v2')
 
 register_dataset(
     DatasetName.sql_create_context_en,
     'AI-ModelScope/sql-create-context', ['train'],
     None,
     ComposePreprocessor([
         RenameColumnsPreprocessor({
             'question': 'instruction',
             'context': 'input',
             'answer': 'output'
         }),
         AlpacaPreprocessor(),
     ]),
     get_dataset_from_repo,
-    tags=['chat', 'sql', '🔥'])
+    tags=['chat', 'sql', '🔥'],
+    hf_dataset_id='b-mc2/sql-create-context')
 
 register_dataset(
     DatasetName.lawyer_llama_zh,
     'AI-ModelScope/lawyer_llama_data', ['train'],
     None,
     RenameColumnsPreprocessor({
         'instruction': 'query',
         'output': 'response',
         'history': '_'
     }),
     get_dataset_from_repo,
-    tags=['chat', 'law'])
+    tags=['chat', 'law'],
+    hf_dataset_id='Skepsun/lawyer_llama_data')
 
 
 def _preprocess_tigerbot_law(dataset: HfDataset) -> HfDataset:
     prompt = """{type}
 {title}
 """
     response = []
@@ -1185,15 +1297,16 @@
 
 register_dataset(
     DatasetName.tigerbot_law_zh,
     'AI-ModelScope/tigerbot-law-plugin', ['train'],
     None,
     _preprocess_tigerbot_law,
     get_dataset_from_repo,
-    tags=['text-generation', 'law', 'pretrained'])
+    tags=['text-generation', 'law', 'pretrained'],
+    hf_dataset_id='TigerResearch/tigerbot-law-plugin')
 
 
 def _preprocess_leetcode_python(dataset: HfDataset) -> HfDataset:
     query = []
     response = []
     for d in dataset:
         code_with_problem = d['code_with_problem']
@@ -1219,31 +1332,64 @@
     tags=['chat', 'coding', '🔥'])
 
 _agent_instruct_subset_list = [
     'alfworld', 'db', 'kg', 'mind2web', 'os', 'webshop'
 ]
 
 
-def _repair_conversations_agent_instruct(s: str) -> str:
+def _repair_conversations_agent_instruct(s: str) -> List[Dict[str, Any]]:
     s = s.replace('}\n {', '},\n {')
-    return ast.literal_eval(s)
+    if isinstance(s, str):
+        s = ast.literal_eval(s)
+    return s
 
 
 register_dataset(
     DatasetName.agent_instruct_all_en,
     'huangjintao/AgentInstruct_copy',
     [(subset, 'train') for subset in _agent_instruct_subset_list],
     None,
     ConversationsPreprocessor(
         'human',
         'gpt',
         repair_conversations=_repair_conversations_agent_instruct),
     get_dataset_from_repo,
     tags=['chat', 'agent', 'multi-round'])
 
+
+def _preprocess_msagent_multirole_dataset(dataset: HfDataset) -> HfDataset:
+    res_prompt = """\n\n【注意事项】\n1. 这是聊天室，不要发送私信给任何人\n2. 仅代表你个人说话,不要扮演其他人，
+    只根据对话历史进行回复\n3. 长话短说，不要说太多话，不要超过50字 """
+    history_prompt = '\n\n【chat history】'
+    conv_prompt = '\n {name}:{content}'
+    query = []
+    response = []
+
+    for d in dataset:
+        conv = d['conversations']
+        system = conv[0]['value']
+        if '【注意事项】' not in system:
+            system += res_prompt
+        system += history_prompt
+        response.append(conv[-1]['value'])
+        for i in range(1, len(conv) - 1):
+            system += conv_prompt.format(
+                name=conv[i]['from'], content=conv[i]['value'])
+        query.append(system)
+    return HfDataset.from_dict({'query': query, 'response': response})
+
+
+register_dataset(
+    DatasetName.ms_agent_multirole,
+    'iic/MSAgent-MultiRole', [('default', 'train')],
+    None,
+    _preprocess_msagent_multirole_dataset,
+    get_dataset_from_repo,
+    tags=['chat', 'agent', 'multi-round', 'role-play', 'multi-agent'])
+
 register_dataset(
     DatasetName.codefuse_evol_instruction_zh,
     'codefuse-ai/Evol-instruction-66k', ['train'],
     None,
     RenameColumnsPreprocessor({
         'instruction': 'query',
         'output': 'response'
@@ -1278,56 +1424,63 @@
 
 register_dataset(
     DatasetName.hc3_zh,
     'simpleai/HC3-Chinese',
     [[subset, 'train'] for subset in hc3_chinese_subset], [],
     _preprocess_hc3,
     get_dataset_from_repo,
-    tags=['text-generation', 'classification', '🔥'])
+    tags=['text-generation', 'classification', '🔥'],
+    hf_dataset_id='Hello-SimpleAI/HC3-Chinese')
 
 register_dataset(
     DatasetName.hc3_en,
     'simpleai/HC3', [[subset, 'train'] for subset in ['finance', 'medicine']],
     [],
     _preprocess_hc3,
     get_dataset_from_repo,
-    tags=['text-generation', 'classification', '🔥'])
+    tags=['text-generation', 'classification', '🔥'],
+    hf_dataset_id='Hello-SimpleAI/HC3')
 
 register_dataset(
     DatasetName.tulu_v2_sft_mixture,
     'AI-ModelScope/tulu-v2-sft-mixture', ['train'], [],
     None,
     get_dataset_from_repo,
-    tags=['chat', 'multilingual', 'general', 'multi-round'])
+    tags=['chat', 'multilingual', 'general', 'multi-round'],
+    hf_dataset_id='allenai/tulu-v2-sft-mixture')
 register_dataset(
     DatasetName.webnovel_zh,
     'AI-ModelScope/webnovel_cn', ['train'], [],
     None,
     get_dataset_from_repo,
-    tags=['chat', 'novel'])
+    tags=['chat', 'novel'],
+    hf_dataset_id='zxbsmk/webnovel_cn')
 register_dataset(
     DatasetName.generated_chat_zh,
     'AI-ModelScope/generated_chat_0.4M', ['train'], [],
     None,
     get_dataset_from_repo,
-    tags=['chat', 'character-dialogue'])
+    tags=['chat', 'character-dialogue'],
+    hf_dataset_id='BelleGroup/generated_chat_0.4M')
 register_dataset(
     DatasetName.wikipedia_zh,
     'AI-ModelScope/wikipedia-cn-20230720-filtered', ['train'],
     None,
     RenameColumnsPreprocessor({'completion': 'response'}),
     get_dataset_from_repo,
-    tags=['text-generation', 'general', 'pretrained'])
+    tags=['text-generation', 'general', 'pretrained'],
+    hf_dataset_id='pleisto/wikipedia-cn-20230720-filtered')
 register_dataset(
     DatasetName.open_platypus_en,
     'AI-ModelScope/Open-Platypus', ['train'],
     None,
     None,
     get_dataset_from_repo,
-    tags=['chat', 'math'])
+    tags=['chat', 'math'],
+    hf_dataset_id='garage-bAInd/Open-Platypus')
 register_dataset(
     DatasetName.open_orca_gpt4,
     'AI-ModelScope/OpenOrca', ['train'],
     None,
     RenameColumnsPreprocessor({'question': 'query'}),
     get_dataset_from_repo,
     tags=['chat', 'multilingual', 'general'])
@@ -1362,36 +1515,39 @@
     None,
     ConversationsPreprocessor(
         conversations_key='conversation',
         from_key='role',
         value_key='content',
         error_strategy='delete'),
     get_dataset_from_repo,
-    tags=['chat', 'medical', '🔥'])
+    tags=['chat', 'medical', '🔥'],
+    hf_dataset_id='Flmc/DISC-Med-SFT')
 
 register_dataset(
     DatasetName.disc_law_sft_zh,
     'AI-ModelScope/DISC-Law-SFT', ['train'],
     None,
     RenameColumnsPreprocessor({
         'input': 'query',
         'output': 'response'
     }),
     get_dataset_from_repo,
-    tags=['chat', 'law', '🔥'])
+    tags=['chat', 'law', '🔥'],
+    hf_dataset_id='ShengbinYue/DISC-Law-SFT')
 
 register_dataset(
     DatasetName.pileval,
-    'huangjintao/pile-val-backup', ['train'],
+    'huangjintao/pile-val-backup', ['validation'],
     None,
     RenameColumnsPreprocessor({
         'text': 'response',
     }),
     get_dataset_from_repo,
-    tags=['text-generation', 'awq'])
+    tags=['text-generation', 'awq'],
+    hf_dataset_id='mit-han-lab/pile-val-backup')
 
 
 def add_self_cognition_dataset(
         train_dataset: HfDataset, dataset_sample: int,
         model_name: Tuple[str, Optional[str]],
         model_author: Tuple[str, Optional[str]]) -> HfDataset:
     assert model_name[0] is not None
@@ -1490,32 +1646,47 @@
 
 
 def get_dataset(
     dataset_name_list: Union[List[str], str],
     dataset_test_ratio: float = 0.,
     dataset_seed: Union[RandomState, int] = 42,
     check_dataset_strategy: Literal['none', 'discard', 'error',
-                                    'warning'] = 'none'
+                                    'warning'] = 'none',
 ) -> Tuple[HfDataset, Optional[HfDataset]]:
     """Returns train_dataset and val_dataset"""
     if isinstance(dataset_name_list, str):
         dataset_name_list = [dataset_name_list]
     train_dataset_list: List[HfDataset] = []
     val_dataset_list: List[HfDataset] = []
     random_state = dataset_seed
     if isinstance(dataset_seed, int):
         random_state = RandomState(dataset_seed)
     for dataset_name in dataset_name_list:
         dataset_info = DATASET_MAPPING[dataset_name]
+        use_hf = strtobool(os.environ.get('USE_HF', 'False'))
+        dataset_str_f = 'Downloading the dataset from {hub}, dataset_id: {dataset_id}'
+        if use_hf:
+            dataset_id_or_path = dataset_info['hf_dataset_id']
+            dataset_str = dataset_str_f.format(
+                hub='HuggingFace', dataset_id=dataset_id_or_path)
+        else:
+            dataset_id_or_path = dataset_info['dataset_id_or_path']
+            dataset_str = dataset_str_f.format(
+                hub='ModelScope', dataset_id=dataset_id_or_path)
+        logger.info(dataset_str)
+        assert dataset_id_or_path is not None, (
+            f'dataset_name: {dataset_name}, use_hf: {use_hf}, '
+            f'dataset_id_or_path: {dataset_id_or_path}.')
         get_function: GetDatasetFunction = dataset_info['get_function']
         dataset = get_function(
-            dataset_info['dataset_id_or_path'],
+            dataset_id_or_path,
             train_subset_split_list=dataset_info['train_subset_split_list'],
             val_subset_split_list=dataset_info['val_subset_split_list'],
-            preprocess_func=dataset_info['preprocess_func'])
+            preprocess_func=dataset_info['preprocess_func'],
+            use_hf=use_hf)
         train_d: HfDataset
         if isinstance(dataset, (list, tuple)):
             train_d, val_d = dataset
         else:
             train_d, val_d = dataset, None
         assert train_d is not None or val_d is not None
         if val_d is None and dataset_test_ratio > 0:
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/model.py` & `ms-swift-2.0.3/swift/llm/utils/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 from packaging import version
 from torch import Tensor
 from torch import dtype as Dtype
 from transformers import (PretrainedConfig, PreTrainedModel,
                           PreTrainedTokenizerBase)
 from transformers.dynamic_module_utils import get_class_from_dynamic_module
 from transformers.models.auto.tokenization_auto import get_tokenizer_config
+from transformers.utils import strtobool
 from transformers.utils.versions import require_version
 
 from swift import get_logger
 from swift.utils import (get_dist_setting, is_dist, is_local_master,
-                         use_torchacc)
+                         subprocess_run, use_torchacc)
 from .template import TemplateType
 from .utils import get_max_model_len
 
 logger = get_logger()
 
 # Model Home: 'https://modelscope.cn/models/{model_id_or_path}/summary'
 MODEL_MAPPING: Dict[str, Dict[str, Any]] = {}
@@ -51,14 +52,16 @@
     qwen_14b_chat = 'qwen-14b-chat'
     qwen_14b_chat_int4 = 'qwen-14b-chat-int4'
     qwen_14b_chat_int8 = 'qwen-14b-chat-int8'
     qwen_72b = 'qwen-72b'
     qwen_72b_chat = 'qwen-72b-chat'
     qwen_72b_chat_int4 = 'qwen-72b-chat-int4'
     qwen_72b_chat_int8 = 'qwen-72b-chat-int8'
+    modelscope_agent_7b = 'modelscope-agent-7b'
+    modelscope_agent_14b = 'modelscope-agent-14b'
     # qwen1.5
     qwen1half_0_5b = 'qwen1half-0_5b'
     qwen1half_1_8b = 'qwen1half-1_8b'
     qwen1half_4b = 'qwen1half-4b'
     qwen1half_7b = 'qwen1half-7b'
     qwen1half_14b = 'qwen1half-14b'
     qwen1half_32b = 'qwen1half-32b'
@@ -110,35 +113,67 @@
     qwen_audio_chat = 'qwen-audio-chat'
     # chatglm
     chatglm2_6b = 'chatglm2-6b'
     chatglm2_6b_32k = 'chatglm2-6b-32k'
     chatglm3_6b_base = 'chatglm3-6b-base'
     chatglm3_6b = 'chatglm3-6b'
     chatglm3_6b_32k = 'chatglm3-6b-32k'
+    chatglm3_6b_128k = 'chatglm3-6b-128k'
     codegeex2_6b = 'codegeex2-6b'
     # llama2
     llama2_7b = 'llama2-7b'
     llama2_7b_chat = 'llama2-7b-chat'
     llama2_13b = 'llama2-13b'
     llama2_13b_chat = 'llama2-13b-chat'
     llama2_70b = 'llama2-70b'
     llama2_70b_chat = 'llama2-70b-chat'
     llama2_7b_aqlm_2bit_1x16 = 'llama2-7b-aqlm-2bit-1x16'  # aqlm
+    # llama3
+    llama3_8b = 'llama3-8b'
+    llama3_8b_instruct = 'llama3-8b-instruct'
+    llama3_8b_instruct_int4 = 'llama3-8b-instruct-int4'
+    llama3_8b_instruct_int8 = 'llama3-8b-instruct-int8'
+    llama3_8b_instruct_awq = 'llama3-8b-instruct-awq'
+    llama3_70b = 'llama3-70b'
+    llama3_70b_instruct = 'llama3-70b-instruct'
+    llama3_70b_instruct_int4 = 'llama3-70b-instruct-int4'
+    llama3_70b_instruct_int8 = 'llama3-70b-instruct-int8'
+    llama3_70b_instruct_awq = 'llama3-70b-instruct-awq'
+    # chinese-llama-alpaca-2
+    chinese_llama_2_1_3b = 'chinese-llama-2-1_3b'
+    chinese_llama_2_7b = 'chinese-llama-2-7b'
+    chinese_llama_2_7b_16k = 'chinese-llama-2-7b-16k'
+    chinese_llama_2_7b_64k = 'chinese-llama-2-7b-64k'
+    chinese_llama_2_13b = 'chinese-llama-2-13b'
+    chinese_llama_2_13b_16k = 'chinese-llama-2-13b-16k'
+    chinese_alpaca_2_1_3b = 'chinese-alpaca-2-1_3b'
+    chinese_alpaca_2_7b = 'chinese-alpaca-2-7b'
+    chinese_alpaca_2_7b_16k = 'chinese-alpaca-2-7b-16k'
+    chinese_alpaca_2_7b_64k = 'chinese-alpaca-2-7b-64k'
+    chinese_alpaca_2_13b = 'chinese-alpaca-2-13b'
+    chinese_alpaca_2_13b_16k = 'chinese-alpaca-2-13b-16k'
+    # atom
+    atom_7b = 'atom-7b'
+    atom_7b_chat = 'atom-7b-chat'
     # llava
     llava1d6_mistral_7b_instruct = 'llava1d6-mistral-7b-instruct'
     llava1d6_yi_34b_instruct = 'llava1d6-yi-34b-instruct'
     # yi
     yi_6b = 'yi-6b'
     yi_6b_200k = 'yi-6b-200k'
     yi_6b_chat = 'yi-6b-chat'
+    yi_6b_chat_awq = 'yi-6b-chat-awq'
+    yi_6b_chat_int8 = 'yi-6b-chat-int8'
     yi_9b = 'yi-9b'
     yi_9b_200k = 'yi-9b-200k'
     yi_34b = 'yi-34b'
     yi_34b_200k = 'yi-34b-200k'
     yi_34b_chat = 'yi-34b-chat'
+    yi_34b_chat_awq = 'yi-34b-chat-awq'
+    yi_34b_chat_int8 = 'yi-34b-chat-int8'
     # yi-vl
     yi_vl_6b_chat = 'yi-vl-6b-chat'
     yi_vl_34b_chat = 'yi-vl-34b-chat'
     # internlm
     internlm_7b = 'internlm-7b'
     internlm_7b_chat = 'internlm-7b-chat'
     internlm_7b_chat_8k = 'internlm-7b-chat-8k'
@@ -196,14 +231,15 @@
     minicpm_2b_128k = 'minicpm-2b-128k'
     minicpm_moe_8x2b = 'minicpm-moe-8x2b'
     # minicpm-v
     minicpm_v_3b_chat = 'minicpm-v-3b-chat'
     minicpm_v_v2 = 'minicpm-v-v2'
     # openbuddy
     openbuddy_llama2_13b_chat = 'openbuddy-llama2-13b-chat'
+    openbuddy_llama3_8b_chat = 'openbuddy-llama3-8b-chat'
     openbuddy_llama2_65b_chat = 'openbuddy-llama-65b-chat'
     openbuddy_llama2_70b_chat = 'openbuddy-llama2-70b-chat'
     openbuddy_mistral_7b_chat = 'openbuddy-mistral-7b-chat'
     openbuddy_zephyr_7b_chat = 'openbuddy-zephyr-7b-chat'
     openbuddy_deepseek_67b_chat = 'openbuddy-deepseek-67b-chat'
     openbuddy_mixtral_moe_7b_chat = 'openbuddy-mixtral-moe-7b-chat'
     # mistral
@@ -211,14 +247,17 @@
     mistral_7b_v2 = 'mistral-7b-v2'
     mistral_7b_instruct = 'mistral-7b-instruct'
     mistral_7b_instruct_v2 = 'mistral-7b-instruct-v2'
     mixtral_moe_7b = 'mixtral-moe-7b'
     mixtral_moe_7b_instruct = 'mixtral-moe-7b-instruct'
     mixtral_moe_7b_aqlm_2bit_1x16 = 'mixtral-moe-7b-aqlm-2bit-1x16'  # aqlm
     mixtral_moe_8x22b_v1 = 'mixtral-moe-8x22b-v1'
+    # wizardlm
+    wizardlm2_7b_awq = 'wizardlm2-7b-awq'
+    wizardlm2_8x22b = 'wizardlm2-8x22b'
     # baichuan
     baichuan_7b = 'baichuan-7b'
     baichuan_13b = 'baichuan-13b'
     baichuan_13b_chat = 'baichuan-13b-chat'
     # baichuan2
     baichuan2_7b = 'baichuan2-7b'
     baichuan2_7b_chat = 'baichuan2-7b-chat'
@@ -356,16 +395,16 @@
     model_id_or_path: Optional[str],
     lora_target_modules: Optional[List[str]] = None,
     template: str = TemplateType.default,
     get_function: Optional[GetModelTokenizerFunction] = None,
     *,
     requires: Optional[List[str]] = None,
     torch_dtype: Optional[Dtype] = None,
-    use_hf: bool = False,
-    revision: Optional[str] = None,
+    hf_model_id: Optional[str] = None,
+    revision: Optional[str] = None,  # only modelscope
     ignore_file_pattern: Optional[List[str]] = None,
     function_kwargs: Optional[Dict[str, Any]] = None,
     exists_ok: bool = False,
     eos_token: Optional[str] = None,
     **kwargs
 ) -> Optional[Callable[[GetModelTokenizerFunction],
                        GetModelTokenizerFunction]]:
@@ -374,23 +413,23 @@
             f'The `{model_type}` has already been registered in the MODEL_MAPPING.'
         )
     if requires is None:
         requires = []
     if function_kwargs is None:
         function_kwargs = {}
     if revision is None:
-        revision = 'main' if use_hf else 'master'
+        revision = 'master'
     model_info = {
         'model_id_or_path': model_id_or_path,
         'lora_target_modules': lora_target_modules,
         'template': template,
         'requires': requires,
         'torch_dtype': torch_dtype,
         'ignore_file_pattern': ignore_file_pattern,
-        'use_hf': use_hf,
+        'hf_model_id': hf_model_id,
         'revision': revision,
         'eos_token': eos_token,
         **kwargs
     }
 
     if get_function is not None:
         if len(function_kwargs) > 0:
@@ -408,139 +447,373 @@
         model_info['get_function'] = get_function
         MODEL_MAPPING[model_type] = model_info
         return _old_get_function
 
     return _register_model
 
 
+def _check_awq_ext() -> None:
+    try:
+        from awq.utils.packing_utils import dequantize_gemm
+        import awq_ext  # with CUDA kernels (AutoAWQ_kernels)
+    except ImportError as e:
+        raise ImportError(
+            'You are training awq models, remember installing awq_ext by '
+            '`git clone https://github.com/casper-hansen/AutoAWQ_kernels '
+            '&& cd AutoAWQ_kernels && pip install -e .`') from e
+
+
+def _check_gptq_model(bits: int, model_kwargs: Dict[str, Any]) -> None:
+    assert model_kwargs.get('quantization_config') is None
+    if version.parse(transformers.__version__) >= version.parse('4.35'):
+        model_kwargs['quantization_config'] = GPTQConfig(
+            bits=bits, use_exllama=False)
+    else:
+        model_kwargs['quantization_config'] = GPTQConfig(
+            bits=bits, disable_exllama=True)
+
+    # fix quantlinear bug
+    from auto_gptq.nn_modules.qlinear.qlinear_cuda_old import QuantLinear
+    __old_forward = QuantLinear.forward
+
+    def _new_forward(self, x):
+        if not self.training or not self.autogptq_cuda_available:
+            return self.__old_forward(x)
+        # fix sft no grad
+        self.autogptq_cuda_available = False
+        res = self.__old_forward(x)
+        self.autogptq_cuda_available = True
+        return res
+
+    if not hasattr(QuantLinear, '__old_forward'):  # avoid double patching
+        QuantLinear.__old_forward = __old_forward
+        QuantLinear.forward = _new_forward
+
+
+@register_model(
+    ModelType.atom_7b,
+    'FlagAlpha/Atom-7B',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='FlagAlpha/Atom-7B')
+@register_model(
+    ModelType.atom_7b_chat,
+    'FlagAlpha/Atom-7B-Chat',
+    LoRATM.llama2,
+    TemplateType.atom,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='FlagAlpha/Atom-7B-Chat')
 @register_model(
     ModelType.internlm_20b,
     'Shanghai_AI_Laboratory/internlm-20b',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-20b')
 @register_model(
     ModelType.internlm_7b,
     'Shanghai_AI_Laboratory/internlm-7b',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
-    support_vllm=True)
-@register_model(ModelType.bluelm_7b_chat_32k, 'vivo-ai/BlueLM-7B-Chat-32K',
-                LoRATM.llama2, TemplateType.bluelm)
-@register_model(ModelType.bluelm_7b_chat, 'vivo-ai/BlueLM-7B-Chat',
-                LoRATM.llama2, TemplateType.bluelm)
-@register_model(ModelType.bluelm_7b_32k, 'vivo-ai/BlueLM-7B-Base-32K',
-                LoRATM.llama2, TemplateType.default_generation_bos)
-@register_model(ModelType.bluelm_7b, 'vivo-ai/BlueLM-7B-Base', LoRATM.llama2,
-                TemplateType.default_generation_bos)
+    support_vllm=True,
+    hf_model_id='internlm/internlm-7b')
+@register_model(
+    ModelType.bluelm_7b_chat_32k,
+    'vivo-ai/BlueLM-7B-Chat-32K',
+    LoRATM.llama2,
+    TemplateType.bluelm,
+    hf_model_id='vivo-ai/BlueLM-7B-Chat-32K')
+@register_model(
+    ModelType.bluelm_7b_chat,
+    'vivo-ai/BlueLM-7B-Chat',
+    LoRATM.llama2,
+    TemplateType.bluelm,
+    hf_model_id='vivo-ai/BlueLM-7B-Chat')
+@register_model(
+    ModelType.bluelm_7b_32k,
+    'vivo-ai/BlueLM-7B-Base-32K',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    hf_model_id='vivo-ai/BlueLM-7B-Base-32K')
+@register_model(
+    ModelType.bluelm_7b,
+    'vivo-ai/BlueLM-7B-Base',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    hf_model_id='vivo-ai/BlueLM-7B-Base')
 @register_model(
     ModelType.seqgpt_560m,
     'damo/nlp_seqgpt-560m',
     LoRATM.bloom,
     TemplateType.default_generation,
-    support_vllm=True)
-@register_model(ModelType.xverse_13b_chat, 'xverse/XVERSE-13B-Chat',
-                LoRATM.llama2, TemplateType.xverse)
-@register_model(ModelType.xverse_13b, 'xverse/XVERSE-13B', LoRATM.llama2,
-                TemplateType.default_generation)
-@register_model(ModelType.xverse_65b, 'xverse/XVERSE-65B', LoRATM.llama2,
-                TemplateType.default_generation)
-@register_model(ModelType.xverse_65b_v2, 'xverse/XVERSE-65B-2', LoRATM.llama2,
-                TemplateType.default_generation)
-@register_model(ModelType.xverse_65b_chat, 'xverse/XVERSE-65B-Chat',
-                LoRATM.llama2, TemplateType.xverse)
+    support_vllm=True,
+    hf_model_id='DAMO-NLP/SeqGPT-560M')
+@register_model(
+    ModelType.xverse_13b_chat,
+    'xverse/XVERSE-13B-Chat',
+    LoRATM.llama2,
+    TemplateType.xverse,
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-13B-Chat')
+@register_model(
+    ModelType.xverse_13b,
+    'xverse/XVERSE-13B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-13B')
+@register_model(
+    ModelType.xverse_65b,
+    'xverse/XVERSE-65B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-65B')
+@register_model(
+    ModelType.xverse_65b_v2,
+    'xverse/XVERSE-65B-2',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-65B-2')
+@register_model(
+    ModelType.xverse_65b_chat,
+    'xverse/XVERSE-65B-Chat',
+    LoRATM.llama2,
+    TemplateType.xverse,
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-65B-Chat')
 @register_model(
     ModelType.xverse_13b_256k,
     'xverse/XVERSE-13B-256K',
     LoRATM.llama2,
     TemplateType.default_generation,
-    revision='v1.0.0')
-@register_model(ModelType.xverse_7b_chat, 'xverse/XVERSE-7B-Chat',
-                LoRATM.llama2, TemplateType.xverse)
-@register_model(ModelType.xverse_7b, 'xverse/XVERSE-7B', LoRATM.llama2,
-                TemplateType.default_generation)
-@register_model(ModelType.xverse_moe_a4_2b, 'xverse/XVERSE-MoE-A4.2B',
-                LoRATM.llama2, TemplateType.default_generation)
+    revision='v1.0.0',
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-13B-256K')
+@register_model(
+    ModelType.xverse_7b_chat,
+    'xverse/XVERSE-7B-Chat',
+    LoRATM.llama2,
+    TemplateType.xverse,
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-7B-Chat')
+@register_model(
+    ModelType.xverse_7b,
+    'xverse/XVERSE-7B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    hf_model_id='xverse/XVERSE-7B')
+@register_model(
+    ModelType.xverse_moe_a4_2b,
+    'xverse/XVERSE-MoE-A4.2B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    hf_model_id='xverse/XVERSE-MoE-A4.2B')
 @register_model(
     ModelType.baichuan_13b_chat,
     'baichuan-inc/Baichuan-13B-Chat',
     LoRATM.baichuan,
     TemplateType.baichuan,
     requires=['transformers<4.34'],
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='baichuan-inc/Baichuan-13B-Chat')
 @register_model(
     ModelType.baichuan_7b,
     'baichuan-inc/baichuan-7B',
     LoRATM.baichuan,
     TemplateType.default_generation,
     requires=['transformers<4.34'],
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='baichuan-inc/Baichuan-7B')
 @register_model(
     ModelType.mengzi3_13b_base,
     'langboat/Mengzi3-13B-Base',
     LoRATM.llama2,
     TemplateType.mengzi,
     support_vllm=True,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='Langboat/Mengzi3-13B-Base')
 @register_model(
     ModelType.c4ai_command_r_v01,
     'AI-ModelScope/c4ai-command-r-v01',
     LoRATM.llama2,
     TemplateType.c4ai,
     requires=['transformers>=4.39.1'],
     support_vllm=False,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='CohereForAI/c4ai-command-r-v01')
 @register_model(
     ModelType.c4ai_command_r_plus,
     'AI-ModelScope/c4ai-command-r-plus',
     LoRATM.llama2,
     TemplateType.c4ai,
     requires=['transformers>4.39'],
     support_vllm=False,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='CohereForAI/c4ai-command-r-plus')
+@register_model(
+    ModelType.chinese_llama_2_1_3b,
+    'AI-ModelScope/chinese-llama-2-1.3b',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-llama-2-1.3b')
+@register_model(
+    ModelType.chinese_llama_2_7b,
+    'AI-ModelScope/chinese-llama-2-7b',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-llama-2-7b')
+@register_model(
+    ModelType.chinese_llama_2_7b_16k,
+    'AI-ModelScope/chinese-llama-2-7b-16k',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-llama-2-7b-16k')
+@register_model(
+    ModelType.chinese_llama_2_7b_64k,
+    'AI-ModelScope/chinese-llama-2-7b-64k',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-llama-2-7b-64k')
+@register_model(
+    ModelType.chinese_llama_2_13b,
+    'AI-ModelScope/chinese-llama-2-13b',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-llama-2-13b')
+@register_model(
+    ModelType.chinese_llama_2_13b_16k,
+    'AI-ModelScope/chinese-llama-2-13b-16k',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-llama-2-13b-16k')
+@register_model(
+    ModelType.chinese_alpaca_2_1_3b,
+    'AI-ModelScope/chinese-alpaca-2-1.3b',
+    LoRATM.llama2,
+    TemplateType.llama,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-alpaca-2-1.3b')
+@register_model(
+    ModelType.chinese_alpaca_2_7b,
+    'AI-ModelScope/chinese-alpaca-2-7b',
+    LoRATM.llama2,
+    TemplateType.llama,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-alpaca-2-7b')
+@register_model(
+    ModelType.chinese_alpaca_2_7b_16k,
+    'AI-ModelScope/chinese-alpaca-2-7b-16k',
+    LoRATM.llama2,
+    TemplateType.llama,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-alpaca-2-7b-16k')
+@register_model(
+    ModelType.chinese_alpaca_2_7b_64k,
+    'AI-ModelScope/chinese-alpaca-2-7b-64k',
+    LoRATM.llama2,
+    TemplateType.llama,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-alpaca-2-7b-64k')
+@register_model(
+    ModelType.chinese_alpaca_2_13b,
+    'AI-ModelScope/chinese-alpaca-2-13b',
+    LoRATM.llama2,
+    TemplateType.llama,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-alpaca-2-13b')
+@register_model(
+    ModelType.chinese_alpaca_2_13b_16k,
+    'AI-ModelScope/chinese-alpaca-2-13b-16k',
+    LoRATM.llama2,
+    TemplateType.llama,
+    support_vllm=True,
+    support_flash_attn=True,
+    hf_model_id='hfl/chinese-alpaca-2-13b-16k')
 def get_model_tokenizer_from_repo(model_dir: str,
                                   torch_dtype: Optional[Dtype],
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   model_config=None,
                                   tokenizer=None,
                                   automodel_class=AutoModelForCausalLM,
                                   **kwargs):
     """load from an independent repository"""
+    is_awq = kwargs.pop('is_awq', False)
+    is_aqlm = kwargs.pop('is_aqlm', False)
+    gptq_bits = kwargs.pop('gptq_bits', 0)
+    is_training = kwargs.pop('is_training', False)
+    if is_awq and is_training:
+        _check_awq_ext()
+    if gptq_bits > 0 and is_training:
+        _check_gptq_model(gptq_bits, model_kwargs)
+    context = kwargs.get('context', None)
+    if is_aqlm and is_training:
+        require_version('transformers>=4.39')
+        import aqlm
+        context = aqlm.optimize_for_training()
+    if context is None:
+        context = nullcontext()
     if model_config is None:
         model_config = AutoConfig.from_pretrained(
             model_dir, trust_remote_code=True)
     if torch_dtype is not None:
         model_config.torch_dtype = torch_dtype
     if tokenizer is None:
         tokenizer = AutoTokenizer.from_pretrained(
             model_dir, trust_remote_code=True)
     eos_token = kwargs.get('eos_token')
     if eos_token is not None:
         tokenizer.eos_token = eos_token
     model = None
-    context = kwargs.get('context', nullcontext())
     if load_model:
         with context:
             model = automodel_class.from_pretrained(
                 model_dir,
                 config=model_config,
                 torch_dtype=torch_dtype,
                 trust_remote_code=True,
                 **model_kwargs)
+    if load_model and is_awq:
+        model.is_awq = is_awq
+    if load_model and gptq_bits > 0:
+        model.gptq_bits = gptq_bits
     return model, tokenizer
 
 
 @register_model(
     ModelType.grok_1,
     'colossalai/grok-1-pytorch',
     LoRATM.grok_1,
     TemplateType.default_generation,
     support_vllm=False,
-    support_flash_attn=False)
+    support_flash_attn=False,
+    hf_model_id='hpcai-tech/grok-1')
 def get_model_tokenizer_grok(model_dir: str,
                              torch_dtype: Optional[Dtype],
                              model_kwargs: Dict[str, Any],
                              load_model: bool = True,
                              model_config=None,
                              tokenizer=None,
                              automodel_class=AutoModelForCausalLM,
@@ -569,50 +842,56 @@
 
 @register_model(
     ModelType.mamba_130m,
     'AI-ModelScope/mamba-130m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
     requires=['transformers>=4.39.0'],
-    support_vllm=False)
+    support_vllm=False,
+    hf_model_id='state-spaces/mamba-130m-hf')
 @register_model(
     ModelType.mamba_370m,
     'AI-ModelScope/mamba-370m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
     requires=['transformers>=4.39.0'],
-    support_vllm=False)
+    support_vllm=False,
+    hf_model_id='state-spaces/mamba-370m-hf')
 @register_model(
     ModelType.mamba_390m,
     'AI-ModelScope/mamba-390m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
     requires=['transformers>=4.39.0'],
-    support_vllm=False)
+    support_vllm=False,
+    hf_model_id='state-spaces/mamba-390m-hf')
 @register_model(
     ModelType.mamba_790m,
     'AI-ModelScope/mamba-790m-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
     requires=['transformers>=4.39.0'],
-    support_vllm=False)
+    support_vllm=False,
+    hf_model_id='state-spaces/mamba-790m-hf')
 @register_model(
     ModelType.mamba_1_4b,
     'AI-ModelScope/mamba-1.4b-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
     requires=['transformers>=4.39.0'],
-    support_vllm=False)
+    support_vllm=False,
+    hf_model_id='state-spaces/mamba-1.4b-hf')
 @register_model(
     ModelType.mamba_2_8b,
     'AI-ModelScope/mamba-2.8b-hf',
     LoRATM.mamba,
     TemplateType.default_generation,
     requires=['transformers>=4.39.0'],
-    support_vllm=False)
+    support_vllm=False,
+    hf_model_id='state-spaces/mamba-2.8b-hf')
 def get_model_tokenizer_mamba(model_dir: str,
                               torch_dtype: Optional[Dtype],
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
     logger.info(
         '[IMPORTANT] Remember installing causal-conv1d>=1.2.0 and mamba-ssm, or you training and inference will'
@@ -623,29 +902,32 @@
 
 @register_model(
     ModelType.cogvlm_17b_instruct,
     'ZhipuAI/cogvlm-chat',
     LoRATM.cogvlm,
     TemplateType.cogvlm_instruct,
     support_gradient_checkpointing=False,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='THUDM/cogvlm-chat-hf')
 @register_model(
     ModelType.cogagent_18b_chat,
     'ZhipuAI/cogagent-chat',
     LoRATM.cogagent,
     TemplateType.cogagent_chat,
     support_gradient_checkpointing=False,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='THUDM/cogagent-chat-hf')
 @register_model(
     ModelType.cogagent_18b_instruct,
     'ZhipuAI/cogagent-vqa',
     LoRATM.cogagent,
     TemplateType.cogagent_instruct,
     support_gradient_checkpointing=False,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='THUDM/cogagent-vqa-hf')
 def get_model_tokenizer_cogagent(model_dir: str,
                                  torch_dtype: Dtype,
                                  model_kwargs: Dict[str, Any],
                                  load_model: bool = True,
                                  **kwargs):
     tokenizer = AutoTokenizer.from_pretrained(
         'AI-ModelScope/vicuna-7b-v1.5',
@@ -667,27 +949,29 @@
 
 
 @register_model(
     ModelType.internlm_20b_chat,
     'Shanghai_AI_Laboratory/internlm-chat-20b',
     LoRATM.llama2,
     TemplateType.internlm,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-chat-20b')
 @register_model(
     ModelType.internlm_7b_chat_8k,
     'Shanghai_AI_Laboratory/internlm-chat-7b-8k',
     LoRATM.llama2,
     TemplateType.internlm,
     support_vllm=True)
 @register_model(
     ModelType.internlm_7b_chat,
-    'Shanghai_AI_Laboratory/internlm-chat-7b-v1_1',
+    'Shanghai_AI_Laboratory/internlm-chat-7b',
     LoRATM.llama2,
     TemplateType.internlm,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm-chat-7b')
 def get_model_tokenizer_internlm_chat(model_dir: str,
                                       torch_dtype: Dtype,
                                       model_kwargs: Dict[str, Any],
                                       load_model: bool = True,
                                       **kwargs):
     model, tokenizer = get_model_tokenizer_from_repo(model_dir, torch_dtype,
                                                      model_kwargs, load_model,
@@ -700,15 +984,16 @@
 
 @register_model(
     ModelType.baichuan_13b,
     'baichuan-inc/Baichuan-13B-Base',
     LoRATM.baichuan,
     TemplateType.default_generation,
     requires=['transformers<4.34'],
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='baichuan-inc/Baichuan-13B-Base')
 def get_model_tokenizer_baichuan_13b(model_dir: str,
                                      torch_dtype: Dtype,
                                      model_kwargs: Dict[str, Any],
                                      load_model: bool = True,
                                      **kwargs):
     model, tokenizer = get_model_tokenizer_from_repo(model_dir, torch_dtype,
                                                      model_kwargs, load_model,
@@ -723,21 +1008,23 @@
 
 
 @register_model(
     ModelType.baichuan2_13b_chat,
     'baichuan-inc/Baichuan2-13B-Chat',
     LoRATM.baichuan,
     TemplateType.baichuan,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='baichuan-inc/Baichuan2-13B-Chat')
 @register_model(
     ModelType.baichuan2_13b,
     'baichuan-inc/Baichuan2-13B-Base',
     LoRATM.baichuan,
     TemplateType.default_generation,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='baichuan-inc/Baichuan2-13B-Base')
 def get_model_tokenizer_baichuan2_13b(model_dir: str,
                                       torch_dtype: Dtype,
                                       model_kwargs: Dict[str, Any],
                                       load_model: bool = True,
                                       **kwargs):
     # patch: baichuan2_13b configuration_baichuan.py bug
     model_config = AutoConfig.from_pretrained(
@@ -768,21 +1055,23 @@
 
 
 @register_model(
     ModelType.baichuan2_7b_chat,
     'baichuan-inc/Baichuan2-7B-Chat',
     LoRATM.baichuan,
     TemplateType.baichuan,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='baichuan-inc/Baichuan2-7B-Chat')
 @register_model(
     ModelType.baichuan2_7b,
     'baichuan-inc/Baichuan2-7B-Base',
     LoRATM.baichuan,
     TemplateType.default_generation,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='baichuan-inc/Baichuan2-7B-Base')
 def get_model_tokenizer_baichuan2(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   model_config=None,
                                   **kwargs):
     if model_config is None:
@@ -812,22 +1101,24 @@
     'baichuan-inc/Baichuan2-13B-Chat-4bits',
     LoRATM.baichuan,
     TemplateType.baichuan,
     function_kwargs={
         'get_baichuan2_function': get_model_tokenizer_baichuan2_13b
     },
     torch_dtype=torch.bfloat16,
-    requires=['bitsandbytes<0.41.2', 'accelerate<0.26'])
+    requires=['bitsandbytes<0.41.2', 'accelerate<0.26'],
+    hf_model_id='baichuan-inc/Baichuan2-13B-Chat-4bits')
 @register_model(
     ModelType.baichuan2_7b_chat_int4,
     'baichuan-inc/Baichuan2-7B-Chat-4bits',
     LoRATM.baichuan,
     TemplateType.baichuan,
     torch_dtype=torch.bfloat16,
-    requires=['bitsandbytes<0.41.2', 'accelerate<0.26'])
+    requires=['bitsandbytes<0.41.2', 'accelerate<0.26'],
+    hf_model_id='baichuan-inc/Baichuan2-7B-Chat-4bits')
 def get_model_tokenizer_baichuan2_int4(model_dir: str,
                                        torch_dtype: Dtype,
                                        model_kwargs: Dict[str, Any],
                                        load_model: bool = True,
                                        **kwargs):
     logger.info('use `model_config.quantization_config`, ignore bnb arguments')
     model_kwargs.pop('quantization_config', None)
@@ -865,53 +1156,67 @@
 @register_model(
     ModelType.codefuse_codegeex2_6b_chat,
     'codefuse-ai/CodeFuse-CodeGeeX2-6B',
     LoRATM.chatglm,
     TemplateType.codefuse,
     requires=['transformers<4.34'],
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='codefuse-ai/CodeFuse-CodeGeeX2-6B')
 @register_model(
     ModelType.chatglm3_6b_32k,
     'ZhipuAI/chatglm3-6b-32k',
     LoRATM.chatglm,
     TemplateType.chatglm3,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='THUDM/chatglm3-6b-32k')
+@register_model(
+    ModelType.chatglm3_6b_128k,
+    'ZhipuAI/chatglm3-6b-128k',
+    LoRATM.chatglm,
+    TemplateType.chatglm3,
+    support_vllm=True,
+    hf_model_id='THUDM/chatglm3-6b-128k')
 @register_model(
     ModelType.chatglm3_6b,
     'ZhipuAI/chatglm3-6b',
     LoRATM.chatglm,
     TemplateType.chatglm3,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='THUDM/chatglm3-6b')
 @register_model(
     ModelType.chatglm3_6b_base,
     'ZhipuAI/chatglm3-6b-base',
     LoRATM.chatglm,
     TemplateType.chatglm_generation,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='THUDM/chatglm3-6b-base')
 @register_model(
     ModelType.chatglm2_6b_32k,
     'ZhipuAI/chatglm2-6b-32k',
     LoRATM.chatglm,
     TemplateType.chatglm2,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='THUDM/chatglm2-6b-32k')
 @register_model(
     ModelType.chatglm2_6b,
     'ZhipuAI/chatglm2-6b',
     LoRATM.chatglm,
     TemplateType.chatglm2,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='THUDM/chatglm2-6b')
 @register_model(
     ModelType.codegeex2_6b,
     'ZhipuAI/codegeex2-6b',
     LoRATM.chatglm,
     TemplateType.chatglm_generation,
     requires=['transformers<4.34'],
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='THUDM/codegeex2-6b')
 def get_model_tokenizer_chatglm(model_dir: str,
                                 torch_dtype: Dtype,
                                 model_kwargs: Dict[str, Any],
                                 load_model: bool = True,
                                 **kwargs):
     if model_kwargs.get('quantization_config') is not None:
         model_kwargs['quantization_config'].llm_int8_skip_modules = [
@@ -939,440 +1244,572 @@
             return __old_forward(self, inputs, target)
 
         CrossEntropyLoss.forward = cross_entropy_forward
     return model, tokenizer
 
 
 @register_model(
+    ModelType.wizardlm2_8x22b,
+    'AI-ModelScope/WizardLM-2-8x22B',
+    LoRATM.llama2,
+    TemplateType.wizardlm2,
+    requires=['transformers>=4.36'],
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='alpindale/WizardLM-2-8x22B')
+@register_model(
+    ModelType.wizardlm2_7b_awq,
+    'AI-ModelScope/WizardLM-2-7B-AWQ',
+    LoRATM.llama2,
+    TemplateType.wizardlm2_awq,
+    requires=['transformers>=4.34'],
+    torch_dtype=torch.float16,
+    support_flash_attn=True,
+    support_vllm=True,
+    function_kwargs={'is_awq': True},
+    hf_model_id='MaziyarPanahi/WizardLM-2-7B-AWQ')
+@register_model(
     ModelType.gemma_2b,
     'AI-ModelScope/gemma-2b',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.38'],
     ignore_file_pattern=[r'.+\.gguf$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='google/gemma-2b')
 @register_model(
     ModelType.gemma_7b,
     'AI-ModelScope/gemma-7b',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.38'],
     ignore_file_pattern=[r'.+\.gguf$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='google/gemma-7b')
 @register_model(
     ModelType.gemma_2b_instruct,
     'AI-ModelScope/gemma-2b-it',
     LoRATM.llama2,
     TemplateType.gemma,
     requires=['transformers>=4.38'],
     ignore_file_pattern=[r'.+\.gguf$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='google/gemma-2b-it')
 @register_model(
     ModelType.gemma_7b_instruct,
     'AI-ModelScope/gemma-7b-it',
     LoRATM.llama2,
     TemplateType.gemma,
     requires=['transformers>=4.38'],
     ignore_file_pattern=[r'.+\.gguf$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='google/gemma-7b-it')
 @register_model(
     ModelType.deepseek_math_7b_instruct,
     'deepseek-ai/deepseek-math-7b-instruct',
     LoRATM.llama2,
     TemplateType.deepseek,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['math'])
+    tags=['math'],
+    hf_model_id='deepseek-ai/deepseek-math-7b-instruct')
 @register_model(
     ModelType.deepseek_math_7b_chat,
     'deepseek-ai/deepseek-math-7b-rl',
     LoRATM.llama2,
     TemplateType.deepseek,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['math'])
+    tags=['math'],
+    hf_model_id='deepseek-ai/deepseek-math-7b-rl')
 @register_model(
     ModelType.deepseek_math_7b,
     'deepseek-ai/deepseek-math-7b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['math'])
+    tags=['math'],
+    hf_model_id='deepseek-ai/deepseek-math-7b-base')
 @register_model(
     ModelType.qwen1half_0_5b,
     'qwen/Qwen1.5-0.5B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-0.5B')
 @register_model(
     ModelType.qwen1half_1_8b,
     'qwen/Qwen1.5-1.8B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-1.8B')
 @register_model(
     ModelType.qwen1half_4b,
     'qwen/Qwen1.5-4B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-4B')
 @register_model(
     ModelType.qwen1half_7b,
     'qwen/Qwen1.5-7B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-7B')
 @register_model(
     ModelType.qwen1half_14b,
     'qwen/Qwen1.5-14B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-14B')
 @register_model(
     ModelType.qwen1half_32b,
     'qwen/Qwen1.5-32B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-32B')
 @register_model(
     ModelType.qwen1half_72b,
     'qwen/Qwen1.5-72B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-72B')
 @register_model(
     ModelType.codeqwen1half_7b,
     'qwen/CodeQwen1.5-7B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/CodeQwen1.5-7B')
 @register_model(
     ModelType.qwen1half_moe_a2_7b,
     'qwen/Qwen1.5-MoE-A2.7B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.40'],
+    hf_model_id='Qwen/Qwen1.5-MoE-A2.7B')
 @register_model(
     ModelType.deepseek_coder_1_3b,
     'deepseek-ai/deepseek-coder-1.3b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='deepseek-ai/deepseek-coder-1.3b-base')
 @register_model(
     ModelType.deepseek_coder_6_7b,
     'deepseek-ai/deepseek-coder-6.7b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='deepseek-ai/deepseek-coder-6.7b-base')
 @register_model(
     ModelType.deepseek_coder_33b,
     'deepseek-ai/deepseek-coder-33b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='deepseek-ai/deepseek-coder-33b-base')
 @register_model(
     ModelType.deepseek_coder_1_3b_instruct,
     'deepseek-ai/deepseek-coder-1.3b-instruct',
     LoRATM.llama2,
     TemplateType.deepseek_coder,
     eos_token='<|EOT|>',
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='deepseek-ai/deepseek-coder-1.3b-instruct')
 @register_model(
     ModelType.deepseek_coder_6_7b_instruct,
     'deepseek-ai/deepseek-coder-6.7b-instruct',
     LoRATM.llama2,
     TemplateType.deepseek_coder,
     eos_token='<|EOT|>',
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='deepseek-ai/deepseek-coder-6.7b-instruct')
 @register_model(
     ModelType.deepseek_coder_33b_instruct,
     'deepseek-ai/deepseek-coder-33b-instruct',
     LoRATM.llama2,
     TemplateType.deepseek_coder,
     eos_token='<|EOT|>',
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='deepseek-ai/deepseek-coder-33b-instruct')
 @register_model(
     ModelType.openbuddy_deepseek_67b_chat,
     'OpenBuddy/openbuddy-deepseek-67b-v15.2',
     LoRATM.llama2,
     TemplateType.openbuddy,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='OpenBuddy/openbuddy-deepseek-67b-v15.2')
 @register_model(
     ModelType.deepseek_67b_chat,
     'deepseek-ai/deepseek-llm-67b-chat',
     LoRATM.llama2,
     TemplateType.deepseek,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='deepseek-ai/deepseek-llm-67b-chat')
 @register_model(
     ModelType.deepseek_67b,
     'deepseek-ai/deepseek-llm-67b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='deepseek-ai/deepseek-llm-67b-base')
 @register_model(
     ModelType.deepseek_7b_chat,
     'deepseek-ai/deepseek-llm-7b-chat',
     LoRATM.llama2,
     TemplateType.deepseek,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='deepseek-ai/deepseek-llm-7b-chat')
 @register_model(
     ModelType.deepseek_7b,
     'deepseek-ai/deepseek-llm-7b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='deepseek-ai/deepseek-llm-7b-base')
 @register_model(
     ModelType.sus_34b_chat,
     'SUSTC/SUS-Chat-34B',
     LoRATM.llama2,
     TemplateType.sus,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='SUSTech/SUS-Chat-34B')
 @register_model(
     ModelType.openbuddy_zephyr_7b_chat,
     'OpenBuddy/openbuddy-zephyr-7b-v14.1',
     LoRATM.llama2,
     TemplateType.openbuddy,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='OpenBuddy/openbuddy-zephyr-7b-v14.1')
 @register_model(
     ModelType.zephyr_7b_beta_chat,
     'modelscope/zephyr-7b-beta',
     LoRATM.llama2,
     TemplateType.zephyr,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='HuggingFaceH4/zephyr-7b-beta')
 @register_model(
     ModelType.yi_6b_chat,
     '01ai/Yi-6B-Chat',
     LoRATM.llama2,
     TemplateType.yi,
     eos_token='<|im_end|>',
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-6B-Chat')
+@register_model(
+    ModelType.yi_6b_chat_awq,
+    '01ai/Yi-6B-Chat-4bits',
+    LoRATM.llama2,
+    TemplateType.yi,
+    eos_token='<|im_end|>',
+    requires=['autoawq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'is_awq': True},
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-6B-Chat-4bits')
+@register_model(
+    ModelType.yi_6b_chat_int8,
+    '01ai/Yi-6B-Chat-8bits',
+    LoRATM.llama2,
+    TemplateType.yi,
+    eos_token='<|im_end|>',
+    requires=['auto_gptq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-6B-Chat-8bits')
 @register_model(
     ModelType.yi_34b_chat,
     '01ai/Yi-34B-Chat',
     LoRATM.llama2,
     TemplateType.yi,
     eos_token='<|im_end|>',
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-34B-Chat')
+@register_model(
+    ModelType.yi_34b_chat_awq,
+    '01ai/Yi-34B-Chat-4bits',
+    LoRATM.llama2,
+    TemplateType.yi,
+    eos_token='<|im_end|>',
+    requires=['autoawq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'is_awq': True},
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-34B-Chat-4bits')
+@register_model(
+    ModelType.yi_34b_chat_int8,
+    '01ai/Yi-34B-Chat-8bits',
+    LoRATM.llama2,
+    TemplateType.yi,
+    eos_token='<|im_end|>',
+    requires=['auto_gptq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-34B-Chat-8bits')
 @register_model(
     ModelType.yi_34b_200k,
     '01ai/Yi-34B-200K',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-34B-200K')
 @register_model(
     ModelType.yi_34b,
     '01ai/Yi-34B',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-34B')
 @register_model(
     ModelType.yi_6b_200k,
     '01ai/Yi-6B-200K',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-6B-200K')
 @register_model(
     ModelType.yi_9b,
     '01ai/Yi-9B',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-9B')
 @register_model(
     ModelType.yi_9b_200k,
     '01ai/Yi-9B-200K',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-9B-200K')
 @register_model(
     ModelType.yi_6b,
     '01ai/Yi-6B',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-6B')
 @register_model(
     ModelType.ziya2_13b_chat,
     'Fengshenbang/Ziya2-13B-Chat',
     LoRATM.llama2,
     TemplateType.ziya,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='IDEA-CCNL/Ziya2-13B-Chat')
 @register_model(
     ModelType.ziya2_13b,
     'Fengshenbang/Ziya2-13B-Base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='IDEA-CCNL/Ziya2-13B-Base')
 @register_model(
     ModelType.openbuddy_mixtral_moe_7b_chat,
     'OpenBuddy/openbuddy-mixtral-7bx8-v18.1-32k',
     LoRATM.llama2,
     TemplateType.openbuddy,
     requires=['transformers>=4.36'],
     support_flash_attn=True,
     support_vllm=True,
-    support_gradient_checkpointing=False)
+    support_gradient_checkpointing=False,
+    hf_model_id='OpenBuddy/openbuddy-mixtral-7bx8-v18.1-32k')
 @register_model(
     ModelType.openbuddy_mistral_7b_chat,
     'OpenBuddy/openbuddy-mistral-7b-v17.1-32k',
     LoRATM.llama2,
     TemplateType.openbuddy,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='OpenBuddy/openbuddy-mistral-7b-v17.1-32k')
 @register_model(
     ModelType.openbuddy_llama2_70b_chat,
     'OpenBuddy/openbuddy-llama2-70b-v10.1-bf16',
     LoRATM.llama2,
     TemplateType.openbuddy,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='OpenBuddy/openbuddy-llama2-70b-v10.1-bf16')
 @register_model(
     ModelType.openbuddy_llama2_65b_chat,
     'OpenBuddy/openbuddy-llama-65b-v8-bf16',
     LoRATM.llama2,
     TemplateType.openbuddy,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='OpenBuddy/openbuddy-llama-65b-v8-bf16')
+@register_model(
+    ModelType.openbuddy_llama3_8b_chat,
+    'OpenBuddy/openbuddy-llama3-8b-v21.1-8k',
+    LoRATM.llama2,
+    TemplateType.openbuddy2,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='OpenBuddy/openbuddy-llama3-8b-v21.1-8k')
 @register_model(
     ModelType.openbuddy_llama2_13b_chat,
     'OpenBuddy/openbuddy-llama2-13b-v8.1-fp16',
     LoRATM.llama2,
     TemplateType.openbuddy,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='OpenBuddy/openbuddy-llama2-13b-v8.1-fp16')
 @register_model(
     ModelType.mistral_7b_instruct,
     'AI-ModelScope/Mistral-7B-Instruct-v0.1',
     LoRATM.llama2,
     TemplateType.llama,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='mistralai/Mistral-7B-Instruct-v0.1')
 @register_model(
     ModelType.mistral_7b_instruct_v2,
     'AI-ModelScope/Mistral-7B-Instruct-v0.2',
     LoRATM.llama2,
     TemplateType.llama,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='mistralai/Mistral-7B-Instruct-v0.2')
 @register_model(
     ModelType.mistral_7b,
     'AI-ModelScope/Mistral-7B-v0.1',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='mistralai/Mistral-7B-v0.1')
 @register_model(
     ModelType.mistral_7b_v2,
     'AI-ModelScope/Mistral-7B-v0.2-hf',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='alpindale/Mistral-7B-v0.2-hf')
 @register_model(
     ModelType.mixtral_moe_7b,
     'AI-ModelScope/Mixtral-8x7B-v0.1',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.36'],
+    ignore_file_pattern=[r'.+\.pt$'],
     support_flash_attn=True,
     support_vllm=True,
-    support_gradient_checkpointing=False)
+    support_gradient_checkpointing=False,
+    hf_model_id='mistralai/Mixtral-8x7B-v0.1')
 @register_model(
     ModelType.mixtral_moe_7b_instruct,
     'AI-ModelScope/Mixtral-8x7B-Instruct-v0.1',
     LoRATM.llama2,
     TemplateType.llama,
     requires=['transformers>=4.36'],
+    ignore_file_pattern=[r'.+\.pt$'],
     support_flash_attn=True,
     support_vllm=True,
-    support_gradient_checkpointing=False)
+    support_gradient_checkpointing=False,
+    hf_model_id='mistralai/Mixtral-8x7B-Instruct-v0.1')
 @register_model(
     ModelType.mixtral_moe_8x22b_v1,
     'AI-ModelScope/Mixtral-8x22B-v0.1',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     requires=['transformers>=4.36'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='mistral-community/Mixtral-8x22B-v0.1')
 @register_model(
     ModelType.dbrx_base,
     'AI-ModelScope/dbrx-base',
     LoRATM.dbrx,
     TemplateType.dbrx,
     requires=['transformers>=4.36'],
     support_flash_attn=True,
     support_vllm=True,
-    support_gradient_checkpointing=False)
+    support_gradient_checkpointing=False,
+    hf_model_id='databricks/dbrx-base')
 @register_model(
     ModelType.dbrx_instruct,
     'AI-ModelScope/dbrx-instruct',
     LoRATM.dbrx,
     TemplateType.dbrx,
     requires=['transformers>=4.36'],
     support_flash_attn=True,
     support_vllm=True,
-    support_gradient_checkpointing=False)
+    support_gradient_checkpointing=False,
+    hf_model_id='databricks/dbrx-instruct')
 def get_model_tokenizer_with_flash_attn(model_dir: str,
                                         torch_dtype: Dtype,
                                         model_kwargs: Dict[str, Any],
                                         load_model: bool = True,
                                         model_config=None,
                                         **kwargs):
     if model_config is None:
@@ -1390,346 +1827,340 @@
         model_kwargs,
         load_model,
         model_config=model_config,
         **kwargs)
 
 
 @register_model(
-    ModelType.llama2_7b_aqlm_2bit_1x16,
-    'AI-ModelScope/Llama-2-7b-AQLM-2Bit-1x16-hf',
-    LoRATM.llama2,
-    TemplateType.default_generation_bos,
-    ignore_file_pattern=[r'.+\.bin$'],
-    support_flash_attn=True,
-    requires=['transformers>=4.38', 'aqlm', 'torch>=2.2.0'],
-    support_vllm=False)
-@register_model(
-    ModelType.mixtral_moe_7b_aqlm_2bit_1x16,
-    'AI-ModelScope/Mixtral-8x7b-AQLM-2Bit-1x16-hf',
-    LoRATM.llama2,
-    TemplateType.default_generation_bos,
-    requires=['transformers>=4.38', 'aqlm', 'torch>=2.2.0'],
-    support_flash_attn=True,
-    support_vllm=False,
-    support_gradient_checkpointing=False)
-def get_model_tokenizer_aqlm(model_dir: str,
-                             torch_dtype: Dtype,
-                             model_kwargs: Dict[str, Any],
-                             load_model: bool = True,
-                             **kwargs):
-    import aqlm
-    context = aqlm.optimize_for_training()
-    return get_model_tokenizer_llama2(
-        model_dir,
-        torch_dtype,
-        model_kwargs,
-        load_model,
-        context=context,
-        **kwargs)
-
-
-@register_model(
     ModelType.qwen1half_0_5b_chat_awq,
     'qwen/Qwen1.5-0.5B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/Qwen1.5-0.5B-Chat-AWQ')
 @register_model(
     ModelType.qwen1half_1_8b_chat_awq,
     'qwen/Qwen1.5-1.8B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/Qwen1.5-1.8B-Chat-AWQ')
 @register_model(
     ModelType.qwen1half_4b_chat_awq,
     'qwen/Qwen1.5-4B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/Qwen1.5-4B-Chat-AWQ')
 @register_model(
     ModelType.qwen1half_7b_chat_awq,
     'qwen/Qwen1.5-7B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/Qwen1.5-7B-Chat-AWQ')
 @register_model(
     ModelType.qwen1half_14b_chat_awq,
     'qwen/Qwen1.5-14B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/Qwen1.5-14B-Chat-AWQ')
 @register_model(
     ModelType.qwen1half_32b_chat_awq,
     'qwen/Qwen1.5-32B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/Qwen1.5-32B-Chat-AWQ')
 @register_model(
     ModelType.qwen1half_72b_chat_awq,
     'qwen/Qwen1.5-72B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/Qwen1.5-72B-Chat-AWQ')
 @register_model(
     ModelType.codeqwen1half_7b_chat_awq,
     'qwen/CodeQwen1.5-7B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
-    requires=['transformers>=4.37', 'autoawq'])
+    requires=['transformers>=4.37', 'autoawq'],
+    torch_dtype=torch.float16,
+    hf_model_id='Qwen/CodeQwen1.5-7B-Chat-AWQ')
 @register_model(
     ModelType.qwen1half_0_5b_chat,
     'qwen/Qwen1.5-0.5B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-0.5B-Chat')
 @register_model(
     ModelType.qwen1half_1_8b_chat,
     'qwen/Qwen1.5-1.8B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-1.8B-Chat')
 @register_model(
     ModelType.qwen1half_4b_chat,
     'qwen/Qwen1.5-4B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-4B-Chat')
 @register_model(
     ModelType.qwen1half_7b_chat,
     'qwen/Qwen1.5-7B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-7B-Chat')
 @register_model(
     ModelType.qwen1half_14b_chat,
     'qwen/Qwen1.5-14B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-14B-Chat')
 @register_model(
     ModelType.qwen1half_32b_chat,
     'qwen/Qwen1.5-32B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-32B-Chat')
 @register_model(
     ModelType.qwen1half_72b_chat,
     'qwen/Qwen1.5-72B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/Qwen1.5-72B-Chat')
 @register_model(
     ModelType.qwen1half_moe_a2_7b_chat,
     'qwen/Qwen1.5-MoE-A2.7B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.40'],
+    hf_model_id='Qwen/Qwen1.5-MoE-A2.7B-Chat')
 @register_model(
     ModelType.codeqwen1half_7b_chat,
     'qwen/CodeQwen1.5-7B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    requires=['transformers>=4.37'])
+    requires=['transformers>=4.37'],
+    hf_model_id='Qwen/CodeQwen1.5-7B-Chat')
 def get_model_tokenizer_qwen1half(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
-    is_awq = kwargs.pop('is_awq', False)
-    is_training = kwargs.pop('is_training', False)
     kwargs['eos_token'] = '<|im_end|>'
-    if is_awq and is_training:
-        try:
-            from awq.utils.packing_utils import dequantize_gemm
-            import awq_ext  # with CUDA kernels (AutoAWQ_kernels)
-        except ImportError as e:
-            raise ImportError(
-                'You are training awq models, remember installing awq_ext by '
-                '`git clone https://github.com/casper-hansen/AutoAWQ_kernels '
-                '&& cd AutoAWQ_kernels && pip install -e .`') from e
     return get_model_tokenizer_with_flash_attn(model_dir, torch_dtype,
                                                model_kwargs, load_model,
                                                **kwargs)
 
 
 @register_model(
     ModelType.qwen1half_0_5b_chat_int4,
     'qwen/Qwen1.5-0.5B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-0.5B-Chat-GPTQ-Int4')
 @register_model(
     ModelType.qwen1half_0_5b_chat_int8,
     'qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_1_8b_chat_int4,
     'qwen/Qwen1.5-1.8B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-1.8B-Chat-GPTQ-Int4')
 @register_model(
     ModelType.qwen1half_1_8b_chat_int8,
     'qwen/Qwen1.5-1.8B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen1.5-1.8B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_4b_chat_int4,
     'qwen/Qwen1.5-4B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-4B-Chat-GPTQ-Int4')
 @register_model(
     ModelType.qwen1half_4b_chat_int8,
     'qwen/Qwen1.5-4B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen1.5-4B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_7b_chat_int4,
     'qwen/Qwen1.5-7B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-7B-Chat-GPTQ-Int4')
 @register_model(
     ModelType.qwen1half_7b_chat_int8,
     'qwen/Qwen1.5-7B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen1.5-7B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_14b_chat_int4,
     'qwen/Qwen1.5-14B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-14B-Chat-GPTQ-Int4')
 @register_model(
     ModelType.qwen1half_14b_chat_int8,
     'qwen/Qwen1.5-14B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen1.5-14B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_32b_chat_int4,
     'qwen/Qwen1.5-32B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-32B-Chat-GPTQ-Int4')
 @register_model(
     ModelType.qwen1half_72b_chat_int4,
     'qwen/Qwen1.5-72B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-72B-Chat-GPTQ-Int4')
 @register_model(
     ModelType.qwen1half_72b_chat_int8,
     'qwen/Qwen1.5-72B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen1.5-72B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_moe_a2_7b_chat_int4,
     'qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
-    requires=['auto_gptq>=0.5', 'transformers>=4.37'],
+    requires=['auto_gptq>=0.5', 'transformers>=4.40'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 4},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4')
 def get_model_tokenizer_qwen1half_intx(model_dir: str,
                                        torch_dtype: Dtype,
                                        model_kwargs: Dict[str, Any],
                                        load_model: bool = True,
                                        **kwargs):
     kwargs['get_qwen_function'] = get_model_tokenizer_qwen1half
     return get_model_tokenizer_qwen_intx(model_dir, torch_dtype, model_kwargs,
@@ -1737,126 +2168,156 @@
 
 
 @register_model(
     ModelType.internlm2_1_8b,
     'Shanghai_AI_Laboratory/internlm2-1_8b',
     LoRATM.internlm2,
     TemplateType.default_generation_bos,
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-1_8b')
 @register_model(
     ModelType.internlm2_1_8b_sft_chat,
     'Shanghai_AI_Laboratory/internlm2-chat-1_8b-sft',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-chat-1_8b-sft')
 @register_model(
     ModelType.internlm2_1_8b_chat,
     'Shanghai_AI_Laboratory/internlm2-chat-1_8b',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-chat-1_8b')
 @register_model(
     ModelType.internlm2_math_7b,
     'Shanghai_AI_Laboratory/internlm2-math-base-7b',
     LoRATM.internlm2,
     TemplateType.default_generation_bos,
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
     support_vllm=True,
-    tags=['math'])
+    tags=['math'],
+    hf_model_id='internlm/internlm2-math-base-7b')
 @register_model(
     ModelType.internlm2_math_20b,
     'Shanghai_AI_Laboratory/internlm2-math-base-20b',
     LoRATM.internlm2,
     TemplateType.default_generation_bos,
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
     support_vllm=True,
-    tags=['math'])
+    tags=['math'],
+    hf_model_id='internlm/internlm2-math-base-20b')
 @register_model(
     ModelType.internlm2_math_7b_chat,
     'Shanghai_AI_Laboratory/internlm2-math-7b',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
     support_vllm=True,
-    tags=['math'])
+    tags=['math'],
+    hf_model_id='internlm/internlm2-math-7b')
 @register_model(
     ModelType.internlm2_math_20b_chat,
     'Shanghai_AI_Laboratory/internlm2-math-20b',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
     support_vllm=True,
-    tags=['math'])
+    tags=['math'],
+    hf_model_id='internlm/internlm2-math-20b')
 @register_model(
     ModelType.internlm2_7b_sft_chat,
     'Shanghai_AI_Laboratory/internlm2-chat-7b-sft',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-chat-7b-sft')
 @register_model(
     ModelType.internlm2_7b_chat,
     'Shanghai_AI_Laboratory/internlm2-chat-7b',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-chat-7b')
 @register_model(
     ModelType.internlm2_20b_sft_chat,
     'Shanghai_AI_Laboratory/internlm2-chat-20b-sft',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-chat-20b-sft')
 @register_model(
     ModelType.internlm2_20b_chat,
     'Shanghai_AI_Laboratory/internlm2-chat-20b',
     LoRATM.internlm2,
     TemplateType.internlm2,
     eos_token='<|im_end|>',
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-chat-20b')
 @register_model(
     ModelType.internlm2_7b,
     'Shanghai_AI_Laboratory/internlm2-7b',
     LoRATM.internlm2,
     TemplateType.default_generation_bos,
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-7b')
 @register_model(
     ModelType.internlm2_7b_base,
     'Shanghai_AI_Laboratory/internlm2-base-7b',
     LoRATM.internlm2,
     TemplateType.default_generation_bos,
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-base-7b')
 @register_model(
     ModelType.internlm2_20b,
     'Shanghai_AI_Laboratory/internlm2-20b',
     LoRATM.internlm2,
     TemplateType.default_generation_bos,
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-20b')
 @register_model(
     ModelType.internlm2_20b_base,
     'Shanghai_AI_Laboratory/internlm2-base-20b',
     LoRATM.internlm2,
     TemplateType.default_generation_bos,
+    requires=['transformers>=4.35'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='internlm/internlm2-base-20b')
 def get_model_tokenizer_internlm2(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -1883,15 +2344,16 @@
 @register_model(
     ModelType.internlm_xcomposer2_7b_chat,
     'Shanghai_AI_Laboratory/internlm-xcomposer2-7b',
     LoRATM.internlm2,
     TemplateType.internlm_xcomposer2,
     eos_token='[UNUSED_TOKEN_145]',
     support_flash_attn=True,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='internlm/internlm-xcomposer2-7b')
 def get_model_tokenizer_internlm_xcomposer2(model_dir: str,
                                             torch_dtype: Dtype,
                                             model_kwargs: Dict[str, Any],
                                             load_model: bool = True,
                                             **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -1923,17 +2385,21 @@
     if local_repo_name is None:
         github_url = github_url.rstrip('/')
         local_repo_name = github_url.rsplit('/', 1)[1]
     local_repo_path = os.path.join(git_cache_dir, local_repo_name)
     if not os.path.exists(local_repo_path):
         if not github_url.endswith('.git'):
             github_url = f'{github_url}.git'
-        command = f'git -C {git_cache_dir} clone {github_url} {local_repo_name}'
-        logger.info(f'Run the command: `{command}`')
-        os.system(command)
+        command = [
+            'git', '-C', git_cache_dir, 'clone', github_url, local_repo_name
+        ]
+        command_str = f"git -C '{git_cache_dir}' clone '{github_url}' {local_repo_name}"
+        logger.info(f'Run the command: `{command_str}`')
+        subprocess_run(command)
+    logger.info(f'local_repo_path: {local_repo_path}')
     return local_repo_path
 
 
 def __prepare_inputs_embeds(
     self,
     input_ids: torch.LongTensor,
     pixel_values: torch.FloatTensor,
@@ -1993,22 +2459,24 @@
 
 @register_model(
     ModelType.deepseek_vl_7b_chat,
     'deepseek-ai/deepseek-vl-7b-chat',
     LoRATM.llama2,
     TemplateType.deepseek_vl,
     support_flash_attn=True,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='deepseek-ai/deepseek-vl-7b-chat')
 @register_model(
     ModelType.deepseek_vl_1_3b_chat,
     'deepseek-ai/deepseek-vl-1.3b-chat',
     LoRATM.llama2,
     TemplateType.deepseek_vl,
     support_flash_attn=True,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='deepseek-ai/deepseek-vl-1.3b-chat')
 def get_model_tokenizer_deepseek_vl(model_dir: str,
                                     torch_dtype: Dtype,
                                     model_kwargs: Dict[str, Any],
                                     load_model: bool = True,
                                     **kwargs):
     # compat with python==3.10
     if sys.version_info.minor >= 10:
@@ -2043,61 +2511,181 @@
     tokenizer.vl_chat_processor = vl_chat_processor
     if load_model:
         _patch_deepseek_vl(model)
     return model, tokenizer
 
 
 @register_model(
+    ModelType.llama3_70b_instruct_awq,
+    'huangjintao/Meta-Llama-3-70B-Instruct-AWQ',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    requires=['autoawq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'is_awq': True},
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.llama3_70b_instruct_int8,
+    'huangjintao/Meta-Llama-3-70b-Instruct-GPTQ-Int8',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    requires=['auto_gptq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.llama3_70b_instruct_int4,
+    'huangjintao/Meta-Llama-3-70B-Instruct-GPTQ-Int4',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    requires=['auto_gptq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'gptq_bits': 4},
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.llama3_8b_instruct_awq,
+    'huangjintao/Meta-Llama-3-8B-Instruct-AWQ',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    requires=['autoawq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'is_awq': True},
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.llama3_8b_instruct_int8,
+    'huangjintao/Meta-Llama-3-8B-Instruct-GPTQ-Int8',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    requires=['auto_gptq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.llama3_8b_instruct_int4,
+    'huangjintao/Meta-Llama-3-8B-Instruct-GPTQ-Int4',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    requires=['auto_gptq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'gptq_bits': 4},
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
+    ModelType.llama3_70b_instruct,
+    'LLM-Research/Meta-Llama-3-70B-Instruct',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='meta-llama/Meta-Llama-3-70B-Instruct')
+@register_model(
+    ModelType.llama3_70b,
+    'LLM-Research/Meta-Llama-3-70B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='meta-llama/Meta-Llama-3-70B')
+@register_model(
+    ModelType.llama3_8b_instruct,
+    'LLM-Research/Meta-Llama-3-8B-Instruct',
+    LoRATM.llama2,
+    TemplateType.llama3,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='meta-llama/Meta-Llama-3-8B-Instruct')
+@register_model(
+    ModelType.llama3_8b,
+    'LLM-Research/Meta-Llama-3-8B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='meta-llama/Meta-Llama-3-8B')
+@register_model(
+    ModelType.llama2_7b_aqlm_2bit_1x16,
+    'AI-ModelScope/Llama-2-7b-AQLM-2Bit-1x16-hf',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    ignore_file_pattern=[r'.+\.bin$'],
+    support_flash_attn=True,
+    requires=['transformers>=4.38', 'aqlm', 'torch>=2.2.0'],
+    support_vllm=False,
+    function_kwargs={'is_aqlm': True},
+    hf_model_id='ISTA-DASLab/Llama-2-7b-AQLM-2Bit-1x16-hf')
+@register_model(
+    ModelType.mixtral_moe_7b_aqlm_2bit_1x16,
+    'AI-ModelScope/Mixtral-8x7b-AQLM-2Bit-1x16-hf',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    requires=['transformers>=4.38', 'aqlm', 'torch>=2.2.0'],
+    support_flash_attn=True,
+    support_vllm=False,
+    support_gradient_checkpointing=False,
+    function_kwargs={'is_aqlm': True},
+    hf_model_id='ISTA-DASLab/Mixtral-8x7b-AQLM-2Bit-1x16-hf')
+@register_model(
     ModelType.llama2_7b,
     'modelscope/Llama-2-7b-ms',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     ignore_file_pattern=[r'.+\.bin$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='meta-llama/Llama-2-7b-hf')
 @register_model(
     ModelType.llama2_13b,
     'modelscope/Llama-2-13b-ms',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     ignore_file_pattern=[r'.+\.bin$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='meta-llama/Llama-2-13b-hf')
 @register_model(
     ModelType.llama2_70b,
     'modelscope/Llama-2-70b-ms',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     ignore_file_pattern=[r'.+\.bin$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='meta-llama/Llama-2-70b-hf')
 @register_model(
     ModelType.llama2_7b_chat,
     'modelscope/Llama-2-7b-chat-ms',
     LoRATM.llama2,
     TemplateType.llama,
     ignore_file_pattern=[r'.+\.bin$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='meta-llama/Llama-2-7b-chat-hf')
 @register_model(
     ModelType.llama2_13b_chat,
     'modelscope/Llama-2-13b-chat-ms',
     LoRATM.llama2,
     TemplateType.llama,
     ignore_file_pattern=[r'.+\.bin$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='meta-llama/Llama-2-13b-chat-hf')
 @register_model(
     ModelType.llama2_70b_chat,
     'modelscope/Llama-2-70b-chat-ms',
     LoRATM.llama2,
     TemplateType.llama,
     ignore_file_pattern=[r'.+\.bin$'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='meta-llama/Llama-2-70b-chat-hf')
 def get_model_tokenizer_llama2(model_dir: str,
                                torch_dtype: Dtype,
                                model_kwargs: Dict[str, Any],
                                load_model: bool = True,
                                **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -2107,16 +2695,20 @@
         torch_dtype,
         model_kwargs,
         load_model,
         model_config=model_config,
         **kwargs)
 
 
-@register_model(ModelType.polylm_13b, 'damo/nlp_polylm_13b_text_generation',
-                LoRATM.polylm, TemplateType.default_generation)
+@register_model(
+    ModelType.polylm_13b,
+    'damo/nlp_polylm_13b_text_generation',
+    LoRATM.polylm,
+    TemplateType.default_generation,
+    hf_model_id='DAMO-NLP-MT/polylm-13b')
 def get_model_tokenizer_polylm(model_dir: str,
                                torch_dtype: Dtype,
                                model_kwargs: Dict[str, Any],
                                load_model: bool = True,
                                **kwargs):
     tokenizer = AutoTokenizer.from_pretrained(
         model_dir, trust_remote_code=True, use_fast=False, legacy=True)
@@ -2175,99 +2767,123 @@
         logger.info('registered_causal_mask to cuda')
     except AttributeError:
         pass
     return model, tokenizer
 
 
 @register_model(
+    ModelType.modelscope_agent_7b,
+    'iic/ModelScope-Agent-7B',
+    LoRATM.qwen,
+    TemplateType.modelscope_agent,
+    support_flash_attn=True,
+    support_vllm=False)
+@register_model(
+    ModelType.modelscope_agent_14b,
+    'iic/ModelScope-Agent-14B',
+    LoRATM.qwen,
+    TemplateType.modelscope_agent,
+    support_flash_attn=True,
+    support_vllm=False)
+@register_model(
     ModelType.codefuse_qwen_14b_chat,
     'codefuse-ai/CodeFuse-QWen-14B',
     LoRATM.qwen,
     TemplateType.codefuse,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='codefuse-ai/CodeFuse-QWen-14B')
 @register_model(
     ModelType.qwen_1_8b,
     'qwen/Qwen-1_8B',
     LoRATM.qwen,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen1.5-1.8B')
 @register_model(
     ModelType.qwen_72b,
     'qwen/Qwen-72B',
     LoRATM.qwen,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-72B')
 @register_model(
     ModelType.tongyi_finance_14b,
     'TongyiFinance/Tongyi-Finance-14B',
     LoRATM.qwen,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     tags=['financial'])
 @register_model(
     ModelType.qwen_14b,
     'qwen/Qwen-14B',
     LoRATM.qwen,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-14B')
 @register_model(
     ModelType.qwen_7b,
     'qwen/Qwen-7B',
     LoRATM.qwen,
     TemplateType.default_generation,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-7B')
 def get_model_tokenizer_qwen_base(*args, **kwargs):
     model, tokenizer = get_model_tokenizer_qwen(*args, **kwargs)
     tokenizer.eos_token_id = tokenizer.eod_id
     return model, tokenizer
 
 
 @register_model(
     ModelType.qwen_1_8b_chat,
     'qwen/Qwen-1_8B-Chat',
     LoRATM.qwen,
     TemplateType.qwen,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-1_8B-Chat')
 @register_model(
     ModelType.qwen_72b_chat,
     'qwen/Qwen-72B-Chat',
     LoRATM.qwen,
     TemplateType.qwen,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-72B-Chat')
 @register_model(
     ModelType.tongyi_finance_14b_chat,
     'TongyiFinance/Tongyi-Finance-14B-Chat',
     LoRATM.qwen,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['financial'])
+    tags=['financial'],
+    hf_model_id='jxy/Tongyi-Finance-14B-Chat')
 @register_model(
     ModelType.qwen_14b_chat,
     'qwen/Qwen-14B-Chat',
     LoRATM.qwen,
     TemplateType.qwen,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-14B-Chat')
 @register_model(
     ModelType.qwen_7b_chat,
     'qwen/Qwen-7B-Chat',
     LoRATM.qwen,
     TemplateType.qwen,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-7B-Chat')
 def get_model_tokenizer_qwen_chat(*args, **kwargs):
     model, tokenizer = get_model_tokenizer_qwen(*args, **kwargs)
     tokenizer.eos_token_id = tokenizer.im_end_id
     return model, tokenizer
 
 
 def _qwen_vl_visual_block_forward(
@@ -2321,23 +2937,25 @@
 
 @register_model(
     ModelType.qwen_vl_chat,
     'qwen/Qwen-VL-Chat',
     LoRATM.qwen,
     TemplateType.qwen,
     support_flash_attn=True,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='Qwen/Qwen-VL-Chat')
 @register_model(
     ModelType.qwen_vl,
     'qwen/Qwen-VL',
     LoRATM.qwen,
     TemplateType.default_generation,
     function_kwargs={'get_qwen_function': get_model_tokenizer_qwen_base},
     support_flash_attn=True,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='Qwen/Qwen-VL')
 def get_model_tokenizer_qwen_vl(model_dir: str,
                                 torch_dtype: Dtype,
                                 model_kwargs: Dict[str, Any],
                                 load_model: bool = True,
                                 **kwargs):
     if (model_kwargs.get('quantization_config') is not None and isinstance(
             model_kwargs['quantization_config'], BitsAndBytesConfig)):
@@ -2381,34 +2999,45 @@
                                          load_model, **kwargs)
     if model is not None:
         fix_qwen_inplace_bug(model)
         # fix device_map is 4
         if n_gpu // local_world_size >= 4:
             model.transformer.visual.proj.data = model.transformer.visual.proj.to(
                 model.transformer.visual.ln_post.bias.device)
+        # fix images cuda:1 bug
+        vision_transformer = model.transformer.visual
+        if not hasattr(vision_transformer, '__old_forward'):
+            _old_forward = vision_transformer.forward
+
+            def _new_forward(x: torch.Tensor):
+                return _old_forward(x).to(device=f'{x.device.type}:0')
 
+            vision_transformer.__old_forward = _old_forward
+            vision_transformer.forward = _new_forward
     return model, tokenizer
 
 
 @register_model(
     ModelType.qwen_audio_chat,
     'qwen/Qwen-Audio-Chat',
     LoRATM.qwen,
     TemplateType.qwen_audio,
     support_flash_attn=True,
     function_kwargs={'get_qwen_function': get_model_tokenizer_qwen_chat},
-    tags=['multi-modal', 'audio'])
+    tags=['multi-modal', 'audio'],
+    hf_model_id='Qwen/Qwen-Audio-Chat')
 @register_model(
     ModelType.qwen_audio,
     'qwen/Qwen-Audio',
     LoRATM.qwen,
     TemplateType.qwen_audio_generation,
     support_flash_attn=True,
     function_kwargs={'get_qwen_function': get_model_tokenizer_qwen_base},
-    tags=['multi-modal', 'audio'])
+    tags=['multi-modal', 'audio'],
+    hf_model_id='Qwen/Qwen-Audio')
 def get_model_tokenizer_qwen_audio(model_dir: str,
                                    torch_dtype: Dtype,
                                    model_kwargs: Dict[str, Any],
                                    load_model: bool = True,
                                    **kwargs):
     get_qwen_function = kwargs.pop('get_qwen_function')
     tokenizer_config = get_tokenizer_config(model_dir)
@@ -2432,147 +3061,136 @@
 @register_model(
     ModelType.qwen_1_8b_chat_int8,
     'qwen/Qwen-1_8B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen-1_8B-Chat-Int8')
 @register_model(
     ModelType.qwen_1_8b_chat_int4,
     'qwen/Qwen-1_8B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-1_8B-Chat-Int4')
 @register_model(
     ModelType.qwen_72b_chat_int8,
     'qwen/Qwen-72B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen-72B-Chat-Int8')
 @register_model(
     ModelType.qwen_72b_chat_int4,
     'qwen/Qwen-72B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-72B-Chat-Int4')
 @register_model(
     ModelType.tongyi_finance_14b_chat_int4,
     'TongyiFinance/Tongyi-Finance-14B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
     support_vllm=True,
-    tags=['financial'])
+    tags=['financial'],
+    hf_model_id='jxy/Tongyi-Finance-14B-Chat-Int4')
 @register_model(
     ModelType.qwen_vl_chat_int4,
     'qwen/Qwen-VL-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
     function_kwargs={
         'get_qwen_function': get_model_tokenizer_qwen_vl,
-        'bits': 4
+        'gptq_bits': 4
     },
     support_flash_attn=True,
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='Qwen/Qwen-VL-Chat-Int4')
 @register_model(
     ModelType.qwen_14b_chat_int8,
     'qwen/Qwen-14B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen-14B-Chat-Int8')
 @register_model(
     ModelType.qwen_7b_chat_int8,
     'qwen/Qwen-7B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 8},
-    support_flash_attn=True)
+    function_kwargs={'gptq_bits': 8},
+    support_flash_attn=True,
+    hf_model_id='Qwen/Qwen-7B-Chat-Int8')
 @register_model(
     ModelType.qwen_14b_chat_int4,
     'qwen/Qwen-14B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-14B-Chat-Int4')
 @register_model(
     ModelType.qwen_7b_chat_int4,
     'qwen/Qwen-7B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
-    function_kwargs={'bits': 4},
+    function_kwargs={'gptq_bits': 4},
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='Qwen/Qwen-7B-Chat-Int4')
 def get_model_tokenizer_qwen_intx(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
-    logger.info('use gptq, ignore bnb arguments')
-    bits = kwargs.pop('bits')
-    if version.parse(transformers.__version__) >= version.parse('4.35'):
-        model_kwargs['quantization_config'] = GPTQConfig(
-            bits=bits, use_exllama=False)
-    else:
-        model_kwargs['quantization_config'] = GPTQConfig(
-            bits=bits, disable_exllama=True)
-
-    # fix quantlinear bug
-    from auto_gptq.nn_modules.qlinear.qlinear_cuda_old import QuantLinear
-    __old_forward = QuantLinear.forward
-
-    def _new_forward(self, x):
-        if not self.training or not self.autogptq_cuda_available:
-            return self.__old_forward(x)
-        # fix sft no grad
-        self.autogptq_cuda_available = False
-        res = self.__old_forward(x)
-        self.autogptq_cuda_available = True
-        return res
-
-    if not hasattr(QuantLinear, '__old_forward'):  # avoid double patching
-        QuantLinear.__old_forward = __old_forward
-        QuantLinear.forward = _new_forward
     get_qwen_function = kwargs.pop('get_qwen_function',
                                    get_model_tokenizer_qwen_chat)
     model, tokenizer = get_qwen_function(model_dir, torch_dtype, model_kwargs,
                                          load_model, **kwargs)
     return model, tokenizer
 
 
-register_model(ModelType.skywork_13b, 'skywork/Skywork-13B-base',
-               LoRATM.llama2, TemplateType.default_generation_bos,
-               get_model_tokenizer_from_repo)
+register_model(
+    ModelType.skywork_13b,
+    'skywork/Skywork-13B-base',
+    LoRATM.llama2,
+    TemplateType.default_generation_bos,
+    get_model_tokenizer_from_repo,
+    hf_model_id='Skywork/Skywork-13B-base')
 
 
 @register_model(ModelType.skywork_13b_chat, 'skywork/Skywork-13B-chat',
                 LoRATM.llama2, TemplateType.skywork)
 def get_skywork_model_tokenizer(model_dir: str,
                                 torch_dtype: Dtype,
                                 model_kwargs: Dict[str, Any],
@@ -2590,15 +3208,16 @@
 @register_model(
     ModelType.codefuse_codellama_34b_chat,
     'codefuse-ai/CodeFuse-CodeLlama-34B',
     LoRATM.llama2,
     TemplateType.codefuse_codellama,
     support_flash_attn=True,
     support_vllm=True,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='codefuse-ai/CodeFuse-CodeLlama-34B')
 def get_model_tokenizer_codellama(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
     tokenizer = AutoTokenizer.from_pretrained(
         model_dir, trust_remote_code=True, use_fast=False, legacy=False)
@@ -2615,21 +3234,23 @@
     ModelType.phi2_3b,
     'AI-ModelScope/phi-2',
     LoRATM.phi,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     support_gradient_checkpointing=False,
-    tags=['coding'])
+    tags=['coding'],
+    hf_model_id='microsoft/phi-2')
 @register_model(
     ModelType.telechat_12b,
     'TeleAI/TeleChat-12B',
     LoRATM.telechat,
     TemplateType.telechat,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='Tele-AI/TeleChat-12B')
 def get_model_tokenizer_phi(model_dir: str,
                             torch_dtype: Dtype,
                             model_kwargs: Dict[str, Any],
                             load_model: bool = True,
                             **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -2645,23 +3266,24 @@
 
 
 @register_model(
     ModelType.telechat_7b,
     'TeleAI/TeleChat-7B',
     LoRATM.telechat,
     TemplateType.telechat,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='Tele-AI/telechat-7B')
 def get_model_tokenizer_telechat(model_dir: str,
                                  torch_dtype: Dtype,
                                  model_kwargs: Dict[str, Any],
                                  load_model: bool = True,
                                  **kwargs):
     if torch_dtype == torch.bfloat16:
         logger.info(
-            'telechat-7b does not support the bfl16 dtype; the dtype is converted to fp16.'
+            'telechat-7b does not support the bf16 dtype; the dtype is converted to fp16.'
         )
         torch_dtype = torch.float16
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
     use_flash_attn = kwargs.pop('use_flash_attn', False)
     model_config.flash_attn = use_flash_attn
     return get_model_tokenizer_from_repo(
@@ -2675,30 +3297,33 @@
 
 @register_model(
     ModelType.deepseek_moe_16b_chat,
     'deepseek-ai/deepseek-moe-16b-chat',
     LoRATM.llama2,
     TemplateType.deepseek,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='deepseek-ai/deepseek-moe-16b-chat')
 @register_model(
     ModelType.deepseek_moe_16b,
     'deepseek-ai/deepseek-moe-16b-base',
     LoRATM.llama2,
     TemplateType.default_generation_bos,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='deepseek-ai/deepseek-moe-16b-base')
 @register_model(
     ModelType.minicpm_moe_8x2b,
     'OpenBMB/MiniCPM-MoE-8x2B',
     LoRATM.llama2,
     TemplateType.minicpm,
     requires=['transformers>=4.36.0'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='openbmb/MiniCPM-MoE-8x2B')
 def get_model_tokenizer_deepseek_moe(model_dir: str,
                                      torch_dtype: Dtype,
                                      model_kwargs: Dict[str, Any],
                                      load_model: bool = True,
                                      **kwargs):
     model, tokenizer = get_model_tokenizer_with_flash_attn(
         model_dir, torch_dtype, model_kwargs, load_model, **kwargs)
@@ -2728,33 +3353,37 @@
 
 
 @register_model(
     ModelType.yuan2_2b_instruct,
     'YuanLLM/Yuan2.0-2B-hf',
     LoRATM.llama2,
     TemplateType.yuan,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='IEITYuan/Yuan2-2B-hf')
 @register_model(
     ModelType.yuan2_51b_instruct,
     'YuanLLM/Yuan2.0-51B-hf',
     LoRATM.llama2,
     TemplateType.yuan,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='IEITYuan/Yuan2-51B-hf')
 @register_model(
     ModelType.yuan2_102b_instruct,
     'YuanLLM/Yuan2.0-102B-hf',
     LoRATM.llama2,
     TemplateType.yuan,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='IEITYuan/Yuan2-102B-hf')
 @register_model(
     ModelType.yuan2_2b_janus_instruct,
     'YuanLLM/Yuan2-2B-Janus-hf',
     LoRATM.llama2,
     TemplateType.yuan,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='IEITYuan/Yuan2-2B-Janus-hf')
 def get_model_tokenizer_yuan(model_dir: str,
                              torch_dtype: Dtype,
                              model_kwargs: Dict[str, Any],
                              load_model: bool = True,
                              **kwargs):
     model_folder, model_name = os.path.split(model_dir)
     need_rename = '.' in model_name
@@ -2794,21 +3423,23 @@
 
 
 @register_model(
     ModelType.orion_14b,
     'OrionStarAI/Orion-14B-Base',
     LoRATM.llama2,
     TemplateType.default_generation,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='OrionStarAI/Orion-14B-Base')
 @register_model(
     ModelType.orion_14b_chat,
     'OrionStarAI/Orion-14B-Chat',
     LoRATM.llama2,
     TemplateType.orion,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='OrionStarAI/Orion-14B-Chat')
 def get_model_tokenizer_orion(model_dir: str,
                               torch_dtype: Dtype,
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -2825,23 +3456,25 @@
 @register_model(
     ModelType.yi_vl_34b_chat,
     '01ai/Yi-VL-34B',
     LoRATM.llama2,
     TemplateType.yi_vl,
     support_flash_attn=True,
     requires=['transformers>=4.34'],
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='01-ai/Yi-VL-34B')
 @register_model(
     ModelType.yi_vl_6b_chat,
     '01ai/Yi-VL-6B',
     LoRATM.llama2,
     TemplateType.yi_vl,
     support_flash_attn=True,
     requires=['transformers>=4.34'],
-    tags=['multi-modal', 'vision'])
+    tags=['multi-modal', 'vision'],
+    hf_model_id='01-ai/Yi-VL-6B')
 def get_model_tokenizer_yi_vl(model_dir: str,
                               torch_dtype: Dtype,
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
     local_repo_path = _git_clone_github('https://github.com/01-ai/Yi')
     sys.path.append(os.path.join(local_repo_path, 'VL'))
@@ -2864,50 +3497,54 @@
         automodel_class=LlavaLlamaForCausalLM,
         **kwargs)
     logger.info('Please ignore the above warning.')
     logger.info('Loading the parameters of vision_tower...')
     model.resize_token_embeddings(len(tokenizer))
     vision_tower = model.get_vision_tower()
     vision_tower.load_model()
-    vision_tower.to(device='cuda', dtype=torch_dtype)
+    vision_tower.to(device=model.device, dtype=torch_dtype)
     if not hasattr(model.config, 'max_sequence_length'):
         model.config.max_sequence_length = 2048
     return model, tokenizer
 
 
 @register_model(
     ModelType.minicpm_2b_sft_chat,
     'OpenBMB/MiniCPM-2B-sft-fp32',
     LoRATM.llama2,
     TemplateType.minicpm,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='openbmb/MiniCPM-2B-sft-fp32')
 @register_model(
     ModelType.minicpm_2b_chat,
     'OpenBMB/MiniCPM-2B-dpo-fp32',
     LoRATM.llama2,
     TemplateType.minicpm,
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='openbmb/MiniCPM-2B-dpo-fp32')
 @register_model(
     ModelType.minicpm_1b_sft_chat,
     'OpenBMB/MiniCPM-1B-sft-bf16',
     LoRATM.llama2,
     TemplateType.minicpm,
     requires=['transformers>=4.36.0'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='openbmb/MiniCPM-1B-sft-bf16')
 @register_model(
     ModelType.minicpm_2b_128k,
     'OpenBMB/MiniCPM-2B-128k',
     LoRATM.llama2,
     TemplateType.chatml,
     requires=['transformers>=4.36.0'],
     support_flash_attn=True,
-    support_vllm=True)
+    support_vllm=True,
+    hf_model_id='openbmb/MiniCPM-2B-128k')
 def get_model_tokenizer_minicpm(model_dir: str,
                                 torch_dtype: Dtype,
                                 model_kwargs: Dict[str, Any],
                                 load_model: bool = True,
                                 **kwargs):
     model_config = AutoConfig.from_pretrained(
         model_dir, trust_remote_code=True)
@@ -2924,21 +3561,23 @@
 
 
 @register_model(
     ModelType.minicpm_v_3b_chat,
     'OpenBMB/MiniCPM-V',
     LoRATM.llama2,
     TemplateType.minicpm_v,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='openbmb/MiniCPM-V')
 @register_model(
     ModelType.minicpm_v_v2,
     'OpenBMB/MiniCPM-V-2',
     LoRATM.llama2,
     TemplateType.minicpm_v,
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='openbmb/MiniCPM-V-2')
 def get_model_tokenizer_minicpm_v(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
     model, tokenizer = get_model_tokenizer_minicpm(model_dir, torch_dtype,
                                                    model_kwargs, load_model,
@@ -3022,48 +3661,51 @@
         torch_dtype,
         model_kwargs,
         load_model,
         model_config=model_config,
         automodel_class=automodel_class,
         **kwargs)
 
-    model.resize_token_embeddings(len(tokenizer))
-    vision_tower = model.get_vision_tower()
-    device_map = str(model_kwargs.get('device_map', str(model.device)))
-    if not vision_tower.is_loaded:
-        vision_tower.load_model(device_map=device_map)
-    if not hasattr(model.config, 'max_sequence_length'):
-        model.config.max_sequence_length = 2048
-    _patch_llava(model)
+    if model is not None:
+        model.resize_token_embeddings(len(tokenizer))
+        vision_tower = model.get_vision_tower()
+        device_map = str(model_kwargs.get('device_map', str(model.device)))
+        if not vision_tower.is_loaded:
+            vision_tower.load_model(device_map=device_map)
+        if not hasattr(model.config, 'max_sequence_length'):
+            model.config.max_sequence_length = 2048
+        _patch_llava(model)
     return model, tokenizer
 
 
 @register_model(
     ModelType.mplug_owl2_chat,
     'iic/mPLUG-Owl2',
     LoRATM.mplug_owl2,
     TemplateType.mplug_owl2,
     requires=['transformers<4.35', 'icecream'],
     eos_token='</s>',
     function_kwargs={
         'get_model_tokenizer_function': get_model_tokenizer_with_flash_attn
     },
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='MAGAer13/mplug-owl2-llama2-7b')
 @register_model(
     ModelType.mplug_owl2d1_chat,
     'iic/mPLUG-Owl2.1',
     LoRATM.mplug_owl2d1,
     TemplateType.mplug_owl2,
     requires=['transformers<4.35', 'icecream'],
     eos_token='<|endoftext|>',
     function_kwargs={
         'vocab_size': 151851,
         'get_model_tokenizer_function': get_model_tokenizer_qwen
     },
-    support_flash_attn=True)
+    support_flash_attn=True,
+    hf_model_id='Mizukiluke/mplug_owl_2_1')
 def get_model_tokenizer_mplug_owl2(model_dir: str,
                                    torch_dtype: Dtype,
                                    model_kwargs: Dict[str, Any],
                                    load_model: bool = True,
                                    **kwargs):
     local_repo_path = _git_clone_github('https://github.com/X-PLUG/mPLUG-Owl')
     local_repo_path = os.path.join(local_repo_path, 'mPLUG-Owl2')
@@ -3127,51 +3769,61 @@
                 _old_checkpoint(*args, use_reentrant=use_reentrant, **kwargs))
     except ImportError:
         pass
 
 
 def safe_snapshot_download(model_type: str,
                            model_id_or_path: Optional[str] = None,
+                           revision: Optional[str] = None,
                            **kwargs) -> str:
     # Perform snapshot_download (ms or hf) based on model_type and model_id_or_path.
     model_info = MODEL_MAPPING[model_type]
+    use_hf = strtobool(os.environ.get('USE_HF', 'False'))
     if model_id_or_path is None:
         model_dir = kwargs.pop('model_dir', None)  # compat with swift<1.7
         if model_dir is not None:
             model_id_or_path = model_dir
         else:
-            model_id_or_path = model_info['model_id_or_path']
+            model_id_or_path = model_info[
+                'hf_model_id' if use_hf else 'model_id_or_path']
 
     if is_dist() and not is_local_master():
         dist.barrier()
     if model_id_or_path is not None and not os.path.exists(model_id_or_path):
-        revision = model_info['revision']
-        use_hf = model_info['use_hf']
         ignore_file_pattern = model_info['ignore_file_pattern']
         if use_hf:
+            if revision is None:
+                revision = 'main'
             logger.info(
                 f'Downloading the model from HuggingFace Hub, model_id: {model_id_or_path}'
             )
+            use_hf_transfer = strtobool(
+                os.environ.get('USE_HF_TRANSFER', 'False'))
+            if use_hf_transfer:
+                import huggingface_hub._snapshot_download as hf_s
+                hf_s.HF_HUB_ENABLE_HF_TRANSFER = True
             from huggingface_hub import snapshot_download as hf_snapshot_download
             model_dir = hf_snapshot_download(
                 model_id_or_path,
                 repo_type='model',
                 revision=revision,
                 ignore_patterns=ignore_file_pattern)
         else:
+            if revision is None:
+                revision = model_info['revision']
             logger.info(
                 f'Downloading the model from ModelScope Hub, model_id: {model_id_or_path}'
             )
             model_dir = snapshot_download(
                 model_id_or_path,
                 revision,
                 ignore_file_pattern=ignore_file_pattern)
     else:
         model_dir = model_id_or_path
-        logger.info(f'Loading the model using model_dir: {model_dir}')
+    logger.info(f'Loading the model using model_dir: {model_dir}')
     if is_dist() and is_local_master():
         dist.barrier()
 
     model_dir = os.path.expanduser(model_dir)
     assert os.path.isdir(model_dir), f'model_dir: {model_dir}'
     return model_dir
 
@@ -3189,22 +3841,23 @@
 def get_model_tokenizer(
         model_type: str,
         torch_dtype: Optional[Dtype] = None,
         model_kwargs: Optional[Dict[str, Any]] = None,
         load_model: bool = True,
         *,
         model_id_or_path: Optional[str] = None,
+        revision: Optional[str] = None,
         **kwargs) -> Tuple[Optional[PreTrainedModel], PreTrainedTokenizerBase]:
     """
     torch_dtype: If you use None, it will retrieve the torch_dtype from the config.json file.
         However, if torch.float32 is retrieved, torch.float16 will be used.
     """
     model_dir = kwargs.pop('model_dir', None)  # compat with swift<1.7
     model_dir = safe_snapshot_download(
-        model_type, model_id_or_path, model_dir=model_dir)
+        model_type, model_id_or_path, revision=revision, model_dir=model_dir)
 
     model_info = MODEL_MAPPING[model_type]
     requires = model_info['requires']
     for require in requires:
         require_version(require)
     get_function = model_info['get_function']
     if model_kwargs is None:
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/preprocess.py` & `ms-swift-2.0.3/swift/llm/utils/preprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,28 +35,44 @@
     def __init__(self,
                  concat_inst_inp: Optional[Callable[[str, str], str]] = None):
         self.concat_inst_inp = concat_inst_inp
 
     def __call__(self, dataset: HfDataset) -> HfDataset:
         query: List[str] = []
         response = []
-        for d in tqdm(dataset):
-            inst, inp, output = d['instruction'], d.get('input',
-                                                        None), d['output']
+        system = None
+        history = None
+        for i, d in tqdm(enumerate(dataset)):
+            inst, inp = d['instruction'], d.get('input', None)
+            h, output = d.pop('history', None), d['output']
+            sys = d.pop('system', None)
+            if history is None and h is not None:
+                history = [None for _ in range(i - 1)]
+            if system is None and sys is not None:
+                system = [None for _ in range(i - 1)]
             if output is None:
                 continue
             if inp is None or len(inp) == 0:
                 q = inst
             elif self.concat_inst_inp is not None:
                 q = self.concat_inst_inp(inst, inp)
             else:
                 q = f'{inst}\n{inp}'
             query.append(q)
             response.append(output)
-        dataset = HfDataset.from_dict({'query': query, 'response': response})
+            if history is not None:
+                history.append(h)
+            if system is not None:
+                system.append(sys)
+        d_dict = {'query': query, 'response': response}
+        if history is not None:
+            d_dict['history'] = history
+        if system is not None:
+            d_dict['system'] = system
+        dataset = HfDataset.from_dict(d_dict)
         return dataset
 
 
 def _default_repair_conversations(s: Union[str, Any]) -> Any:
     if isinstance(s, str):
         return ast.literal_eval(s)
     return s
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/protocol.py` & `ms-swift-2.0.3/swift/llm/utils/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     Default values for OpenAI:
         temperature = 1.
         top_k = -1
         top_p = 1.
         repetition_penalty = 1.
     """
     max_tokens: Optional[int] = None  # None: max_model_len - num_tokens
-    temperature: Optional[float] = None  # None: use deploy_args
+    # None: use deploy_args
+    temperature: Optional[float] = None
     top_p: Optional[float] = None
     repetition_penalty: Optional[float] = None
 
     n: int = 1
     seed: Optional[int] = None
     stop: List[str] = field(default_factory=list)
     stream: bool = False
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/template.py` & `ms-swift-2.0.3/swift/llm/utils/template.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
+import re
 from copy import deepcopy
 from io import BytesIO
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import requests
 import torch
@@ -25,21 +26,24 @@
     default_generation_bos = 'default-generation-bos'
     chatglm_generation = 'chatglm-generation'
     qwen_audio_generation = 'qwen-audio-generation'
     # chat
     default = 'default'
     qwen = 'qwen'
     qwen_audio = 'qwen-audio'
+    modelscope_agent = 'modelscope-agent'
     baichuan = 'baichuan'
     chatglm2 = 'chatglm2'
     chatglm3 = 'chatglm3'
-    llama = 'llama'
+    llama = 'llama'  # llama2
+    llama3 = 'llama3'
     llava_mistral_instruct = 'llava-mistral-instruct'
     llava_yi_instruct = 'llava-yi-instruct'
     openbuddy = 'openbuddy'
+    openbuddy2 = 'openbuddy2'
     internlm = 'internlm'
     internlm2 = 'internlm2'
     internlm_xcomposer2 = 'internlm-xcomposer2'
     yi = 'yi'
     yi_vl = 'yi-vl'
     yuan = 'yuan'
     xverse = 'xverse'
@@ -57,14 +61,17 @@
     cogagent_chat = 'cogagent-chat'
     cogagent_instruct = 'cogagent-instruct'
     orion = 'orion'
     minicpm = 'minicpm'
     minicpm_v = 'minicpm-v'
     gemma = 'gemma'
     mplug_owl2 = 'mplug-owl2'
+    wizardlm2_awq = 'wizardlm2-awq'
+    wizardlm2 = 'wizardlm2'
+    atom = 'atom'
     # compatibility. (Deprecated)
     chatml = 'chatml'
     telechat = 'telechat'
     dbrx = 'dbrx'
     mengzi = 'mengzi'
     c4ai = 'c4ai'
 
@@ -300,17 +307,17 @@
         input_ids: List[int] = []
         labels: List[int] = []
         loss_scale: List[float] = []
         tokenizer_kwargs = {}
         for i, (context,
                 loss_weight) in enumerate(zip(context_list, compute_loss_idx)):
             if isinstance(context, str):
-                curr_tokenizer_kwargs = self.get_tokenizer_kwargs(context)
-                self.concat_tokenizer_kwargs(tokenizer_kwargs,
-                                             curr_tokenizer_kwargs)
+                curr_tokenizer_kwargs = self._get_tokenizer_kwargs(context)
+                self._concat_tokenizer_kwargs(tokenizer_kwargs,
+                                              curr_tokenizer_kwargs)
                 token_list = tokenizer(
                     context,
                     return_attention_mask=False,
                     add_special_tokens=False,
                     **curr_tokenizer_kwargs)['input_ids']
             else:
                 token_list = context
@@ -378,19 +385,19 @@
             'input_ids': input_ids,
             'labels': labels,
         }
         if self.use_loss_scale:
             inputs['loss_scale'] = loss_scale
         return inputs, tokenizer_kwargs
 
-    def get_tokenizer_kwargs(self, context: str) -> Dict[str, Any]:
+    def _get_tokenizer_kwargs(self, context: str) -> Dict[str, Any]:
         """return: curr_tokenizer_kwargs"""
         return {}
 
-    def concat_tokenizer_kwargs(
+    def _concat_tokenizer_kwargs(
             self, old_tokenizer_kwargs: Dict[str, Any],
             curr_tokenizer_kwargs: Dict[str, Any]) -> Dict[str, Any]:
         assert len(old_tokenizer_kwargs) == 0
         return curr_tokenizer_kwargs
 
     def data_collator(self,
                       batch: List[Dict[str, Any]],
@@ -451,14 +458,93 @@
         return res
 
     @staticmethod
     def get_generate_ids(generate_ids: Tensor,
                          input_token_len: int) -> List[int]:
         return generate_ids[0, input_token_len:].tolist()
 
+    @staticmethod
+    def _is_chinese_char(cp: int) -> bool:
+        """Checks whether CP is the codepoint of a CJK character."""
+        # copy from transformers.generation.streamers.TextStreamer
+        if ((cp >= 0x4E00 and cp <= 0x9FFF) or (cp >= 0x3400 and cp <= 0x4DBF)
+                or (cp >= 0x20000 and cp <= 0x2A6DF)
+                or (cp >= 0x2A700 and cp <= 0x2B73F)
+                or (cp >= 0x2B740 and cp <= 0x2B81F)
+                or (cp >= 0x2B820 and cp <= 0x2CEAF)
+                or (cp >= 0xF900 and cp <= 0xFAFF)
+                or (cp >= 0x2F800 and cp <= 0x2FA1F)):
+            return True
+
+        return False
+
+    @classmethod
+    def _get_safe_print_idx(cls,
+                            response: str,
+                            print_idx: int,
+                            is_finished: bool = False) -> int:
+        if is_finished:
+            return len(response)
+        if response.endswith(
+                '\n') or len(response) > 0 and cls._is_chinese_char(
+                    ord(response[-1])):
+            print_idx = len(response)
+        else:
+            print_idx = max(response.rfind(' ') + 1, print_idx)
+        return print_idx
+
+    def generate_ids_to_response(
+        self,
+        generate_ids: List[int],
+        is_finished: bool = True,
+        *,
+        tokenizer_kwargs: Optional[Dict[str, Any]] = None,
+        # only stream=True
+        return_delta: bool = False,
+        print_idx: Optional[List[int]] = None,
+        first_num_space: Optional[List[int]] = None,
+    ):
+        if tokenizer_kwargs is None:
+            tokenizer_kwargs = {}
+        tokenizer = self.tokenizer
+        # avoid printing template.suffix[-1])
+        if isinstance(self.suffix[-1], list) and (
+                not is_finished or is_finished
+                and generate_ids[-len(self.suffix[-1]):] == self.suffix[-1]):
+            generate_ids = generate_ids[:-len(self.suffix[-1])]
+        response = tokenizer.decode(generate_ids, **tokenizer_kwargs)
+        if first_num_space is not None:
+            # Avoid the occurrence of repeated words in sentence.
+            res_fns = first_num_space  # res_first_num_space
+            first_num_space = first_num_space[0]
+            cur_num_space = len(response) - len(response.lstrip(' '))
+            if not is_finished and first_num_space == -1:
+                first_num_space = cur_num_space
+                res_fns[0] = first_num_space
+            if cur_num_space < first_num_space:
+                response = ' ' * (first_num_space - cur_num_space) + response
+            elif cur_num_space > first_num_space:
+                response = response[cur_num_space - first_num_space:]
+        if isinstance(self.suffix[-1], str) and (
+                not is_finished or is_finished
+                and response[-len(self.suffix[-1]):] == self.suffix[-1]):
+            response = response[:-len(self.suffix[-1])]
+
+        if print_idx is not None:
+            old_print_idx = print_idx[0]
+            if not is_finished:
+                # avoid printing incomplete words
+                print_idx[0] = self._get_safe_print_idx(response, print_idx[0])
+                response = response[:print_idx[0]]
+            if return_delta:
+                response = response[old_print_idx:]
+        else:
+            assert is_finished and not return_delta
+        return response
+
 
 TEMPLATE_MAPPING: Dict[str, Dict[str, Any]] = {}
 
 
 def register_template(template_type: str,
                       template: Template,
                       *,
@@ -500,30 +586,36 @@
             ['<|im_end|>\n'], ['<|im_end|>'], DEFAULT_SYSTEM,
             ['<|im_start|>system\n{{SYSTEM}}<|im_end|>\n'])
 
 
 register_template(TemplateType.qwen, QwenTemplate())
 register_template(TemplateType.chatml, QwenTemplate())
 
+register_template(
+    TemplateType.modelscope_agent,
+    Template([], [' \n\n<|user|>:{{QUERY}} \n\n<|assistant|>:'], [],
+             [' \n\n</s>'], DEFAULT_SYSTEM, [' \n\n<|system|>:{{SYSTEM}}']))
+
 
 class _QwenAudioTemplateMixin:
 
     def encode(
             self, example: Dict[str,
                                 Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         inputs, tokenizer_kwargs = super().encode(example)
         inputs.pop('loss_scale', None)
         inputs.update(tokenizer_kwargs)
         return inputs, tokenizer_kwargs
 
-    def get_tokenizer_kwargs(self, context: str) -> Dict[str, Any]:
+    def _get_tokenizer_kwargs(self, context: str) -> Dict[str, Any]:
         return {'audio_info': self.tokenizer.process_audio(context)}
 
-    def concat_tokenizer_kwargs(self, tokenizer_kwargs: Dict[str, Any],
-                                curr_tokenizer_kwargs: Dict[str, Any]) -> None:
+    def _concat_tokenizer_kwargs(
+            self, tokenizer_kwargs: Dict[str, Any],
+            curr_tokenizer_kwargs: Dict[str, Any]) -> None:
         audio_info = curr_tokenizer_kwargs.get('audio_info')
         old_audio_info = tokenizer_kwargs.get('audio_info')
         if old_audio_info is None:
             tokenizer_kwargs['audio_info'] = audio_info
         elif audio_info is not None:
             for k in ['input_audios', 'input_audio_lengths']:
                 old_audio_info[k] = torch.concat(
@@ -642,16 +734,15 @@
 register_template(
     TemplateType.chatglm_generation,
     Template([[64790, 64792]], ['{{QUERY}}'], None, [['eos_token_id']]))
 
 register_template(
     TemplateType.chatglm3,
     Template([[64790, 64792]], [[64795], '\n {{QUERY}}', [64796], '\n'], [],
-             [['eos_token_id']], None,
-             [[64790, 64792, 64794], '\n {{SYSTEM}}']))
+             [[64795]], None, [[64790, 64792, 64794], '\n {{SYSTEM}}']))
 
 register_template(
     TemplateType.deepseek,
     Template([['bos_token_id']], ['User: {{QUERY}}\n\nAssistant:'],
              [['eos_token_id']], [['eos_token_id']], None,
              [['bos_token_id'], '{{SYSTEM}}\n\n']))
 
@@ -666,14 +757,24 @@
     "If you don't know the answer to a question, please don't share false information."
 )
 register_template(
     TemplateType.llama,
     Template(['<s>[INST] '], ['{{QUERY}} [/INST]'], ['</s><s>[INST] '],
              ['</s>'], LLAMA_DEFAULT_SYSTEM,
              ['<s>[INST] <<SYS>>\n{{SYSTEM}}\n<</SYS>>\n\n']))
+
+register_template(
+    TemplateType.llama3,
+    Template(['<|begin_of_text|>'], [
+        '<|start_header_id|>user<|end_header_id|>\n\n{{QUERY}}<|eot_id|>'
+        '<|start_header_id|>assistant<|end_header_id|>\n\n'
+    ], ['<|eot_id|>'], ['<|eot_id|>'], None, [
+        '<|begin_of_text|><|start_header_id|>system<|end_header_id|>\n\n{{SYSTEM}}<|eot_id|>'
+    ]))
+
 OPENBUDDY_DEFAULT_SYSTEM = (
     'You are a helpful, respectful and honest INTP-T AI Assistant named Buddy. You are talking to a human User.\n'
     'Always answer as helpfully and logically as possible, while being safe. '
     'Your answers should not include any '
     'harmful, political, religious, unethical, racist, sexist, toxic, dangerous, or illegal content. '
     'Please ensure that your responses are socially unbiased and positive in nature.\n'
     'If a question does not make any sense, or is not factually coherent, '
@@ -687,14 +788,32 @@
 )
 register_template(
     TemplateType.openbuddy,
     Template([['bos_token_id']], ['User: {{QUERY}}\nAssistant:'], ['\n'],
              [['eos_token_id']], OPENBUDDY_DEFAULT_SYSTEM,
              [['bos_token_id'], '{{SYSTEM}}\n\n']))
 
+OPENBUDDY2_DEFAULT_SYSTEM = (
+    'You(assistant) are a helpful, respectful and honest INTP-T AI Assistant named Buddy. '
+    'You are talking to a human(user).\nAlways answer as helpfully and logically as possible, while being safe. '
+    'Your answers should not include any harmful, political, religious, unethical, racist, '
+    'sexist, toxic, dangerous, or illegal content. '
+    'Please ensure that your responses are socially unbiased and positive in nature.\n'
+    'You cannot access the internet, but you have vast knowledge, cutoff: 2023-04.\n'
+    'You are trained by OpenBuddy team, (https://openbuddy.ai, https://github.com/OpenBuddy/OpenBuddy), '
+    'not related to GPT or OpenAI')
+
+register_template(
+    TemplateType.openbuddy2,
+    Template(
+        [],
+        ['<|role|>user<|says|>{{QUERY}}<|end|>\n<|role|>assistant<|says|>'],
+        ['<|end|>\n'], ['<|end|>'], OPENBUDDY2_DEFAULT_SYSTEM,
+        ['<|role|>system<|says|>{{SYSTEM}}<|end|>\n']))
+
 INTERNLM_SYSTEM = (
     'You are an AI assistant whose name is InternLM (书生·浦语).\n'
     '- InternLM (书生·浦语) is a conversational language model that is developed by Shanghai AI Laboratory (上海人工智能实验室). '
     'It is designed to be helpful, honest, and harmless.\n'
     '- InternLM (书生·浦语) can understand and communicate fluently in the language chosen '
     'by the user such as English and 中文.')
 
@@ -707,14 +826,27 @@
     Template(
         ['<s>'],
         ['<|im_start|>user\n{{QUERY}}<|im_end|>\n<|im_start|>assistant\n'],
         ['<|im_end|>\n'], ['<|im_end|>'], INTERNLM_SYSTEM,
         ['<s><|im_start|>system\n{{SYSTEM}}<|im_end|>\n']))
 
 
+def replace_img_tab(query: str, history: History,
+                    replace_token: str) -> Tuple[str, History, List[str]]:
+    images_path = []
+    pattern = r'<img>(.+?)</img>'
+    new_history = []
+    for i, h in enumerate(history):
+        images_path += re.findall(pattern, h[0])
+        new_history.append([re.sub(pattern, replace_token, h[0]), h[1]])
+    images_path += re.findall(pattern, query)
+    new_query = re.sub(pattern, replace_token, query)
+    return new_query, new_history, images_path
+
+
 class InternLMXComposer2(Template):
     INTERNLM_XCOMPOSER2_SYSTEM = (
         'You are an AI assistant whose name is InternLM-XComposer (浦语·灵笔).\n'
         '- InternLM-XComposer (浦语·灵笔) is a conversational language model that is developed by '
         'Shanghai AI Laboratory (上海人工智能实验室). '
         'It is designed to be helpful, honest, and harmless.\n'
         '- InternLM-XComposer (浦语·灵笔) can understand and communicate fluently in the language chosen '
@@ -732,34 +864,27 @@
         ]
         super().__init__(prefix, prompt, chat_sep, suffix,
                          self.INTERNLM_XCOMPOSER2_SYSTEM, prefix_has_system)
 
     def encode(
             self, example: Dict[str,
                                 Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
-        import re
-        images_path = []
         example = example.copy()
-        history = example.pop('history', [])
-        pattern = r'<img>(.+?)</img>'
-        replace_token = '</s>'
-        new_history = []
-        for i, h in enumerate(history):
-            images_path += re.findall(pattern, h[0])
-            new_history.append([re.sub(pattern, replace_token, h[0]), h[1]])
-        history = new_history
-        images_path += re.findall(pattern, example['query'])
-        example['query'] = re.sub(pattern, replace_token, example['query'])
+        history = example.pop('history', None)
+        if history is None:
+            history = []
+        example['query'], example['history'], images_path = replace_img_tab(
+            example['query'], history, '</s>')
+
         images = []
         dtype = self.model.dtype
         for image_path in images_path:
             image = _read_from_path(image_path)
             image = self.model.vis_processor(image)
             images.append(image.to(dtype))
-        example['history'] = history
         inputs, _ = super().encode(example)
         inputs.pop('loss_scale', None)
         input_ids = inputs['input_ids']
         labels = inputs['labels']
         if len(images) > 0:  # # ignore <s>
             input_ids = input_ids[1:]
             if labels is not None:
@@ -974,25 +1099,36 @@
 class DeepseekVLTemplate(Template):
     DEEPSEEK_VL_SYSTEM = (
         'You are a helpful language and vision assistant. '
         'You are able to understand the visual content that the user provides, '
         'and assist the user with a variety of tasks using natural language.')
 
     def __init__(self):
-        return super().__init__(
-            ['<｜begin▁of▁sentence｜>{{SYSTEM}}\n\n'],
-            ['User: <image_placeholder>{{QUERY}}\n\nAssistant:'],
-            ['<｜end▁of▁sentence｜>'], ['<｜end▁of▁sentence｜>'],
-            self.DEEPSEEK_VL_SYSTEM)
+        return super().__init__(['<｜begin▁of▁sentence｜>{{SYSTEM}}\n\n'],
+                                ['User: {{QUERY}}\n\nAssistant:'],
+                                ['<｜end▁of▁sentence｜>'],
+                                ['<｜end▁of▁sentence｜>'],
+                                self.DEEPSEEK_VL_SYSTEM)
 
     def encode(
             self, example: Dict[str,
                                 Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        images = example.pop('images', None)
+        assert images is None, (
+            'Please read the best practices: https://github.com/modelscope/swift/blob/main/'
+            'docs/source/Multi-Modal/deepseek-vl最佳实践.md')
+
+        example = example.copy()
+        history = example.pop('history', None)
+        if history is None:
+            history = []
+        example['query'], example['history'], images_path = replace_img_tab(
+            example['query'], history, '<image_placeholder>')
+
         inputs, _ = super().encode(example)
-        images_path = example['images']
         images = []
         for image_path in images_path:
             image = _read_from_path(image_path)
             images.append(image)
 
         vl_chat_processor = self.tokenizer.vl_chat_processor
         input_ids, labels = inputs['input_ids'], inputs['labels']
@@ -1061,15 +1197,14 @@
 
 
 register_template(
     TemplateType.deepseek_vl,
     DeepseekVLTemplate(),
     use_model=True,
     lazy_tokenize=True,
-    infer_media_type='round',
     dataloader_num_workers=0,
     dataloader_pin_memory=False)  # only 'cpu' can pin_memory
 
 register_template(
     TemplateType.zephyr,
     Template([], ['<|user|>\n{{QUERY}}</s>\n<|assistant|>\n'], ['</s>\n'],
              ['</s>'], None, ['<|system|>\n{{SYSTEM}}</s>\n']))
@@ -1359,14 +1494,33 @@
 register_template(
     TemplateType.mplug_owl2,
     mPlugOwl2Template(),
     infer_media_type='round',
     use_model=True,
     lazy_tokenize=True)
 
+register_template(
+    TemplateType.wizardlm2_awq,
+    Template(['{{SYSTEM}}'], ['User:\n{{QUERY}}\n\nAssistant:\n'], ['\n\n'],
+             ['</s>']))
+
+_wizardlm2_system = (
+    'A chat between a curious user and an artificial intelligence assistant. '
+    'The assistant gives helpful, detailed, and polite answers to the user\'s questions. '
+)
+register_template(
+    TemplateType.wizardlm2,
+    Template(['{{SYSTEM}}'], ['USER: {{QUERY}} ASSISTANT:'], ['</s>'],
+             ['</s>'], _wizardlm2_system))
+
+register_template(
+    TemplateType.atom,
+    Template(['{{SYSTEM}}'], ['<s>Human: {{QUERY}}\n</s><s>Assistant: '],
+             ['</s>'], ['</s>']))
+
 
 def get_template(
     template_type: str,
     tokenizer: PreTrainedTokenizerBase,
     default_system: Optional[str] = None,
     max_length: Optional[int] = None,
     truncation_strategy: Literal['delete', 'truncation_left'] = 'delete',
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/utils.py` & `ms-swift-2.0.3/swift/llm/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,36 +16,35 @@
 
 import accelerate
 import multiprocess
 import numpy as np
 import requests
 import torch
 import torch.distributed as dist
-import torch.nn.functional as F
 import transformers
 from accelerate.utils.modeling import (get_balanced_memory,
                                        infer_auto_device_map)
 from datasets import Dataset as HfDataset
-from modelscope import MsDataset
 from modelscope.utils.config_ds import MS_CACHE_HOME
 from modelscope.utils.logger import get_logger as get_ms_logger
 from torch import device as Device
 from torch.nn import Linear, Module
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.utils.data import Dataset
 from tqdm.auto import tqdm
 from transformers import (GenerationConfig, PretrainedConfig, PreTrainedModel,
                           PreTrainedTokenizerBase, StoppingCriteriaList,
                           TextStreamer, trainer)
 from transformers.generation.streamers import BaseStreamer
+from transformers.utils import is_torch_npu_available, strtobool
 
 from swift.hub import ModelScopeConfig
 from swift.tuners.module_mapping import MODEL_KEYS_MAPPING
 from swift.utils import (get_dist_setting, get_logger, is_ddp_plus_mp, is_dist,
-                         is_local_master, is_master, stat_array, upper_bound,
+                         is_local_master, stat_array, upper_bound,
                          use_torchacc)
 from .template import History, StopWords, StopWordsCriteria, Template
 
 logger = get_logger()
 ms_logger = get_ms_logger()
 
 logger_format = logging.Formatter('[%(levelname)s:%(name)s] %(message)s')
@@ -88,28 +87,33 @@
                 continue
             download_files(url, temp_fpath, cookies)
             shutil.copy2(temp_fpath, local_fpath)
 
     return local_dir
 
 
-_old_msdataset_load = MsDataset.load
+use_hf = strtobool(os.environ.get('USE_HF', 'False'))
+if not use_hf:
+    from modelscope import MsDataset
+    _old_msdataset_load = MsDataset.load
+
+    @wraps(_old_msdataset_load)
+    def _msdataset_ddp_load(*args, **kwargs):
+        if is_dist() and not is_local_master():
+            dist.barrier()
+        dataset = _old_msdataset_load(*args, **kwargs)
+        if is_dist() and is_local_master():
+            dist.barrier()
+
+        if is_dist():
+            dist.barrier()
+        return dataset
 
-
-@wraps(_old_msdataset_load)
-def _msdataset_ddp_load(*args, **kwargs):
-    if is_dist() and not is_local_master():
-        dist.barrier()
-    dataset = _old_msdataset_load(*args, **kwargs)
-    if is_dist() and is_local_master():
-        dist.barrier()
-
-    if is_dist():
-        dist.barrier()
-    return dataset
+    # monkey patching
+    MsDataset.load = _msdataset_ddp_load
 
 
 def _get_max_memory(device_ids: List[int]) -> Dict[Union[int, str], int]:
     """add feat in accelerate to support DDP + MP"""
     import psutil
     # Make sure CUDA is initialized on each GPU to have the right memory info.
     for i in device_ids:
@@ -423,46 +427,18 @@
     logger.info('sort by max length...')
     dataset_len = [len(d['input_ids']) for d in llm_dataset]
     idx = heapq.nlargest(
         num_dataset, range(len(dataset_len)), key=lambda i: dataset_len[i])
     return llm_dataset.select(idx)
 
 
-def _is_chinese_char(cp):
-    """Checks whether CP is the codepoint of a CJK character."""
-    # copy from transformers.generation.streamers.TextStreamer
-    if ((cp >= 0x4E00 and cp <= 0x9FFF) or (cp >= 0x3400 and cp <= 0x4DBF)
-            or (cp >= 0x20000 and cp <= 0x2A6DF)
-            or (cp >= 0x2A700 and cp <= 0x2B73F)
-            or (cp >= 0x2B740 and cp <= 0x2B81F)
-            or (cp >= 0x2B820 and cp <= 0x2CEAF)
-            or (cp >= 0xF900 and cp <= 0xFAFF)
-            or (cp >= 0x2F800 and cp <= 0x2FA1F)):
-        return True
-
-    return False
-
-
-def _get_safe_print_idx(response: str,
-                        print_idx: int,
-                        is_finished: bool = False) -> int:
-    if is_finished:
-        return len(response)
-    if response.endswith('\n') or len(response) > 0 and _is_chinese_char(
-            ord(response[-1])):
-        print_idx = len(response)
-    else:
-        print_idx = max(response.rfind(' ') + 1, print_idx)
-    return print_idx
-
-
 def to_device(inputs: Any, device: Device) -> Any:
     if callable(getattr(inputs, 'to', None)):
         return inputs.to(device=device)
-    #
+
     if isinstance(inputs, Mapping):
         res = {}
         for k, v in inputs.items():
             res[k] = to_device(v, device)
     elif isinstance(inputs, Sequence) and not isinstance(inputs, str):
         res = []
         for b in inputs:
@@ -591,71 +567,53 @@
     streamer = TokenListIteratorStreamer()
     generation_kwargs = {
         'streamer': streamer,
         'generation_config': generation_config,
         'stopping_criteria': stopping_criteria,
         **inputs
     }
-    thread = Thread(target=model.generate, kwargs=generation_kwargs)
+    _model_generate = model.generate
+    if is_torch_npu_available():
+
+        def _model_generate(*args, **kwargs):
+            torch.npu.set_device(model.device)
+            return model.generate(*args, **kwargs)
+
+    thread = Thread(target=_model_generate, kwargs=generation_kwargs)
     thread.start()
     raw_generate_ids, generate_ids = [], []
-    response, safe_response = '', ''
-    print_idx = 0
+
     if not is_observation:
         history.append(None)  # dummy
-    # Avoid the occurrence of repeated words in sentence.
-    first_num_space = -1
-    for token in streamer:
-        raw_generate_ids.append(token)
+
+    print_idx = [0]
+    first_num_space = [-1]
+
+    is_finished = False
+    while not is_finished:
+        try:
+            token = next(streamer)
+            raw_generate_ids.append(token)
+        except StopIteration:
+            is_finished = True
         generate_ids = template.get_generate_ids(
             torch.tensor(raw_generate_ids)[None], token_len)
         if generation_info is not None:
             generation_info['num_generated_tokens'] = len(generate_ids)
-        # avoid printing template.suffix[-1])
-        if isinstance(template.suffix[-1], list):
-            generate_ids = generate_ids[:-len(template.suffix[-1])]
-        response = tokenizer.decode(generate_ids, **tokenizer_kwargs)
-        cur_num_space = len(response) - len(response.lstrip(' '))
-        if first_num_space == -1:
-            first_num_space = cur_num_space
-        if cur_num_space < first_num_space:
-            response = ' ' * (first_num_space - cur_num_space) + response
-        elif cur_num_space > first_num_space:
-            response = response[cur_num_space - first_num_space:]
-        if isinstance(template.suffix[-1], str):
-            response = response[:-len(template.suffix[-1])]
-        print_idx = _get_safe_print_idx(response, print_idx)
-        # avoid printing incomplete words
-        if safe_response != response[:print_idx]:
-            safe_response = response[:print_idx]
-            if not is_observation:
-                history[-1] = [query, safe_response]
-            else:
-                history[-1][-1] = history[-1][-1][:act_length] + safe_response
-            yield safe_response, history
-    # avoid printing template.suffix[-1])
-    if (isinstance(template.suffix[-1], list) and
-            generate_ids[-len(template.suffix[-1]):] == template.suffix[-1]):
-        generate_ids = generate_ids[:-len(template.suffix[-1])]
-    response = tokenizer.decode(generate_ids, **tokenizer_kwargs)
-    if first_num_space > -1:
-        cur_num_space = len(response) - len(response.lstrip(' '))
-        if cur_num_space < first_num_space:
-            response = ' ' * (first_num_space - cur_num_space) + response
-        elif cur_num_space > first_num_space:
-            response = response[cur_num_space - first_num_space:]
-    if isinstance(
-            template.suffix[-1], str
-    ) and response[-len(template.suffix[-1]):] == template.suffix[-1]:
-        response = response[:-len(template.suffix[-1])]
-    if not is_observation:
-        history[-1] = [query, response]
-    else:
-        history[-1][-1] = history[-1][-1][:act_length] + response
-    yield response, history
+        response = template.generate_ids_to_response(
+            generate_ids,
+            is_finished,
+            tokenizer_kwargs=tokenizer_kwargs,
+            print_idx=print_idx,
+            first_num_space=first_num_space)
+        if not is_observation:
+            history[-1] = [query, response]
+        else:
+            history[-1][-1] = history[-1][-1][:act_length] + response
+        yield response, history
 
 
 def inference(model: PreTrainedModel,
               template: Template,
               query: str,
               history: Optional[History] = None,
               system: Optional[str] = None,
@@ -763,25 +721,16 @@
     generate_ids = template.get_generate_ids(generate_ids, token_len)
     if generation_info is not None:
         generation_info['num_generated_tokens'] = len(generate_ids)
     response = None
     if verbose and stream is False:
         response = tokenizer.decode(generate_ids, **tokenizer_kwargs)
         print(response)
-    # avoid printing template.suffix[-1])
-    if (isinstance(template.suffix[-1], list) and
-            generate_ids[-len(template.suffix[-1]):] == template.suffix[-1]):
-        generate_ids = generate_ids[:-len(template.suffix[-1])]
-        response = None
-    if response is None:
-        response = tokenizer.decode(generate_ids, **tokenizer_kwargs)
-    if isinstance(
-            template.suffix[-1], str
-    ) and response[-len(template.suffix[-1]):] == template.suffix[-1]:
-        response = response[:-len(template.suffix[-1])]
+    response = template.generate_ids_to_response(
+        generate_ids, tokenizer_kwargs=tokenizer_kwargs)
     if not is_observation:
         history.append([query, response])
     else:
         history[-1][-1] = history[-1][-1] + response
     return response, history
 
 
@@ -895,16 +844,14 @@
         if max_len_key is not None:
             max_model_len = min(max_model_len, max_len_key)
     if max_model_len == INF:
         max_model_len = None
     return max_model_len
 
 
-# monkey patching
-MsDataset.load = _msdataset_ddp_load
 if is_ddp_plus_mp():
     _old_ddp_init = DDP.__init__
     accelerate.accelerator.torch.nn.parallel.DistributedDataParallel.__init__ = (
         lambda self, model, device_ids, output_device, *args, **kwargs:
         _old_ddp_init(self, model, *args, **kwargs))
     transformers.modeling_utils.get_balanced_memory = lambda *args, **kwargs: None
     transformers.modeling_utils.infer_auto_device_map = _infer_auto_device_map_patch
```

### Comparing `ms-swift-2.0.2/swift/llm/utils/vllm_utils.py` & `ms-swift-2.0.3/swift/llm/utils/vllm_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 from packaging import version
 from torch import dtype as Dtype
 from tqdm import tqdm
 from transformers import PreTrainedTokenizerBase
 from vllm import (AsyncEngineArgs, AsyncLLMEngine, EngineArgs, LLMEngine,
                   SamplingParams)
 
-from swift.tuners import Swift
-from swift.utils import get_logger, seed_everything
+from swift.utils import get_logger
 from .argument import InferArguments
 from .model import get_model_tokenizer
 from .template import Template, get_template
-from .utils import _get_safe_print_idx
 
 try:
     from vllm.lora.request import LoRARequest
 except ImportError:
     pass
 
 logger = get_logger()
 
 
 def get_vllm_engine(model_type: str,
                     torch_dtype: Optional[Dtype] = None,
                     *,
                     model_id_or_path: Optional[str] = None,
+                    revision: Optional[str] = None,
                     gpu_memory_utilization: float = 0.9,
                     tensor_parallel_size: int = 1,
                     max_model_len: Optional[int] = None,
                     engine_kwargs: Optional[Dict[str, Any]] = None,
                     use_async: bool = False,
                     enable_lora: bool = False,
                     max_loras: int = 1,
                     max_lora_rank: int = 16,
                     **kwargs) -> LLMEngine:
     model_dir = kwargs.pop('model_dir', None)  # compat with swift<1.7
     tokenizer = get_model_tokenizer(
         model_type,
         load_model=False,
         model_id_or_path=model_id_or_path,
-        model_dir=model_dir)[1]
+        model_dir=model_dir,
+        revision=revision)[1]
     model_dir = tokenizer.model_dir
 
     if engine_kwargs is None:
         engine_kwargs = {}
     dtype_mapping = {
         torch.float16: 'float16',
         torch.bfloat16: 'bfloat16',
@@ -66,15 +66,15 @@
         llm_engine_cls = AsyncLLMEngine
         engine_kwargs['disable_log_requests'] = True
     else:
         engine_args_cls = EngineArgs
         llm_engine_cls = LLMEngine
 
     parameters = inspect.signature(engine_args_cls.__init__).parameters
-    if 'enable_lora' in parameters:
+    if 'enable_lora' in parameters and enable_lora:
         engine_kwargs['enable_lora'] = enable_lora
         engine_kwargs['max_loras'] = max_loras
         engine_kwargs['max_lora_rank'] = max_lora_rank
     else:
         assert not enable_lora, (
             'The current version of VLLM does not support `enable_lora`. Please upgrade VLLM.'
         )
@@ -226,14 +226,18 @@
 
     tokenizer = template.tokenizer
     if tokenizer.eos_token is not None and tokenizer.eos_token not in generation_config.stop:
         generation_config.stop.append(tokenizer.eos_token)
     if isinstance(template.suffix[-1],
                   str) and template.suffix[-1] not in generation_config.stop:
         generation_config.stop.append(template.suffix[-1])
+    if isinstance(template.suffix[-1], list):
+        token_str = tokenizer.decode(template.suffix[-1])
+        if token_str not in generation_config.stop:
+            generation_config.stop.append(token_str)
 
     parameters = inspect.signature(llm_engine.add_request).parameters
     add_request_kwargs = {}
     if 'lora_request' in parameters:
         add_request_kwargs['lora_request'] = lora_request
     else:
         assert lora_request is None, (
@@ -261,29 +265,26 @@
             raise ValueError(
                 'input_ids exceeds `max_length`. Please increase the value of `max_length`.'
             )
         input_ids = inputs['input_ids']
         llm_engine.add_request(
             str(i), None, generation_config, input_ids, **add_request_kwargs)
 
-    batch_size = len(request_list)
-    resp_list = [None] * batch_size
-    print_idx_list = [0] * batch_size
-    prog_bar = tqdm(total=batch_size, dynamic_ncols=True, disable=not use_tqdm)
+    resp_list = [None] * len(request_list)
+    print_idx_list = [[0] for _ in range(len(request_list))]
+    prog_bar = tqdm(
+        total=len(request_list), dynamic_ncols=True, disable=not use_tqdm)
     while llm_engine.has_unfinished_requests():
         step_outputs = llm_engine.step()
         for output in step_outputs:
             i = int(output.request_id)
             request = request_list[i]
-            response = tokenizer.decode(output.outputs[0].token_ids, True)
-            print_idx_list[i] = _get_safe_print_idx(response,
-                                                    print_idx_list[i],
-                                                    output.finished)
-            # avoid printing incomplete words
-            safe_response = response[:print_idx_list[i]]
+            generate_ids = output.outputs[0].token_ids
+            safe_response = template.generate_ids_to_response(
+                generate_ids, output.finished, print_idx=print_idx_list[i])
             query = request['query']
             history = request['history']
             if resp_list[i] is None and not request_temp[i][0]:
                 history.append(None)
             if not request_temp[i][0]:
                 history[-1] = [query, safe_response]
             else:
@@ -322,14 +323,18 @@
 
     tokenizer = template.tokenizer
     if tokenizer.eos_token is not None and tokenizer.eos_token not in generation_config.stop:
         generation_config.stop.append(tokenizer.eos_token)
     if isinstance(template.suffix[-1],
                   str) and template.suffix[-1] not in generation_config.stop:
         generation_config.stop.append(template.suffix[-1])
+    if isinstance(template.suffix[-1], list):
+        token_str = tokenizer.decode(template.suffix[-1])
+        if token_str not in generation_config.stop:
+            generation_config.stop.append(token_str)
 
     parameters = inspect.signature(llm_engine.add_request).parameters
     add_request_kwargs = {}
     if 'lora_request' in parameters:
         add_request_kwargs['lora_request'] = lora_request
     else:
         assert lora_request is None, (
@@ -352,31 +357,32 @@
             raise ValueError(
                 'input_ids exceeds `max_length`. Please increase the value of `max_length`.'
             )
         input_ids = inputs['input_ids']
         llm_engine.add_request(
             str(i), None, generation_config, input_ids, **add_request_kwargs)
 
-    batch_size = len(request_list)
     if use_tqdm is True:
         assert verbose is False
-    prog_bar = tqdm(total=batch_size, dynamic_ncols=True, disable=not use_tqdm)
+    prog_bar = tqdm(
+        total=len(request_list), dynamic_ncols=True, disable=not use_tqdm)
     outputs = []
     while llm_engine.has_unfinished_requests():
         step_outputs = llm_engine.step()
         for output in step_outputs:
             if output.finished:
                 outputs.append(output)
                 prog_bar.update()
 
-    resp_list = [None] * batch_size
+    resp_list = [None] * len(request_list)
     for output in outputs:
         i = int(output.request_id)
         request = request_list[i]
-        response = tokenizer.decode(output.outputs[0].token_ids, True)
+        generate_ids = output.outputs[0].token_ids
+        response = template.generate_ids_to_response(generate_ids)
         query = request['query']
         history = request['history']
         if not is_observation:
             history.append([query, response])
         else:
             history[-1][-1] = history[-1][-1] + response
         resp_list[i] = {'response': response, 'history': history}
@@ -388,15 +394,14 @@
     return resp_list
 
 
 def prepare_vllm_engine_template(
         args: InferArguments,
         use_async: bool = False) -> Tuple[LLMEngine, Template]:
     logger.info(f'device_count: {torch.cuda.device_count()}')
-    seed_everything(args.seed)
 
     assert args.quantization_bit == 0, 'not support bnb'
     assert not (args.sft_type == 'lora'
                 and not args.vllm_enable_lora), 'you need to merge lora'
     # Loading Model and Tokenizer
     model_id_or_path = None
     if args.sft_type == 'full' and args.ckpt_dir is not None:
@@ -408,15 +413,15 @@
         args.torch_dtype,
         gpu_memory_utilization=args.gpu_memory_utilization,
         tensor_parallel_size=args.tensor_parallel_size,
         max_model_len=args.max_model_len,
         use_async=use_async,
         model_id_or_path=model_id_or_path,
         enable_lora=args.vllm_enable_lora,
-        max_loras=len(args.vllm_lora_modules),
+        max_loras=min(len(args.vllm_lora_modules), 1),
         max_lora_rank=args.vllm_max_lora_rank)
     tokenizer = llm_engine.hf_tokenizer
     if use_async:
         model_config = asyncio.run(llm_engine.get_model_config())
         llm_engine.model_config = model_config
     else:
         model_config = llm_engine.model_config
```

### Comparing `ms-swift-2.0.2/swift/torchacc_utils.py` & `ms-swift-2.0.3/swift/torchacc_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/__init__.py` & `ms-swift-2.0.3/swift/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/arguments.py` & `ms-swift-2.0.3/swift/trainers/arguments.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/callback.py` & `ms-swift-2.0.3/swift/trainers/callback.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/dpo_trainers.py` & `ms-swift-2.0.3/swift/trainers/dpo_trainers.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/mixin.py` & `ms-swift-2.0.3/swift/trainers/mixin.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/optimizers/galore/__init__.py` & `ms-swift-2.0.3/swift/trainers/optimizers/galore/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/optimizers/galore/adafactor.py` & `ms-swift-2.0.3/swift/trainers/optimizers/galore/adafactor.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/optimizers/galore/adamw.py` & `ms-swift-2.0.3/swift/trainers/optimizers/galore/adamw.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/optimizers/galore/adamw8bit.py` & `ms-swift-2.0.3/swift/trainers/optimizers/galore/adamw8bit.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/optimizers/galore/galore_projector.py` & `ms-swift-2.0.3/swift/trainers/optimizers/galore/galore_projector.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/optimizers/galore/utils.py` & `ms-swift-2.0.3/swift/trainers/optimizers/galore/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/trainers/trainers.py` & `ms-swift-2.0.3/swift/trainers/trainers.py`

 * *Files 12% similar despite different names*

```diff
@@ -264,48 +264,17 @@
                 self._custom_metrics['acc'] = self._acc
             self._custom_metrics['acc'] = self._custom_metrics[
                 'acc'] + acc / self.args.gradient_accumulation_steps
         return (loss, outputs) if return_outputs else loss
 
     def get_train_dataloader(self):
 
-        def __iter__(self):
-            self._num_yielded = 0
-            if self._iterator is None:
-                self._iterator = self.__original_iter__()
-            return self
-
-        def __next__(self):
-            if self._num_yielded >= len(self):
-                raise StopIteration
-            self._num_yielded += 1
-            try:
-                return next(self._iterator)
-            except StopIteration:
-                self._iterator = self.__original_iter__()
-            return next(self._iterator)
-
         if not use_torchacc():
-            origin_loader = super().get_train_dataloader()
-            grad_acc_steps = self.args.gradient_accumulation_steps
-            if grad_acc_steps is None or grad_acc_steps <= 1:
-                return origin_loader
+            return super().get_train_dataloader()
 
-            length = len(origin_loader) // grad_acc_steps * grad_acc_steps
-            origin_loader_type = type(origin_loader)
-            loader = type(
-                origin_loader_type.__name__, (origin_loader_type, ), {
-                    '__len__': lambda _: length,
-                    '__iter__': __iter__,
-                    '__next__': __next__
-                })(
-                    origin_loader.dataset)
-            loader.__dict__.update(origin_loader.__dict__)
-            loader.__original_iter__ = origin_loader.__iter__
-            return loader
         else:
             if trainer.is_datasets_available():
                 import datasets
 
             if self.train_dataset is None:
                 raise ValueError('Trainer: training requires a train_dataset.')
```

### Comparing `ms-swift-2.0.2/swift/trainers/utils.py` & `ms-swift-2.0.3/swift/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/__init__.py` & `ms-swift-2.0.3/swift/tuners/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/adapter.py` & `ms-swift-2.0.3/swift/tuners/adapter.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/base.py` & `ms-swift-2.0.3/swift/tuners/base.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/llamapro.py` & `ms-swift-2.0.3/swift/tuners/llamapro.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/longlora/llama.py` & `ms-swift-2.0.3/swift/tuners/longlora/llama.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/longlora/longlora.py` & `ms-swift-2.0.3/swift/tuners/longlora/longlora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/lora.py` & `ms-swift-2.0.3/swift/tuners/lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/lora_layers.py` & `ms-swift-2.0.3/swift/tuners/lora_layers.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/mapping.py` & `ms-swift-2.0.3/swift/tuners/mapping.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/module_mapping.py` & `ms-swift-2.0.3/swift/tuners/module_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,26 @@
 OPENBUDDY_KEYS = LLAMA_KEYS
 XVERSE_KEYS = LLAMA_KEYS
 ORION_KEYS = LLAMA_KEYS
 BLUELM_KEYS = LLAMA_KEYS
 ZIYA_KEYS = LLAMA_KEYS
 SKYWORK_KEYS = LLAMA_KEYS
 
+INTERNLM2_KEYS = ModelKeys(
+    **{
+        'module_list': 'model.layers',
+        'mlp': 'model.layers.{}.feed_forward',
+        'down_proj': 'model.layers.{}.feed_forward.w2',
+        'attention': 'model.layers.{}.attention',
+        'o_proj': 'model.layers.{}.attention.wo',
+        'qkv_proj': 'model.layers.{}.attention.wqkv',
+        'embedding': 'model.tok_embeddings',
+        'output': 'output',
+    })
+
 CHATGLM_KEYS = ModelKeys(
     **{
         'module_list': 'transformer.encoder.layers',
         'mlp': 'transformer.encoder.layers.{}.mlp',
         'down_proj': 'transformer.encoder.layers.{}.mlp.dense_4h_to_h',
         'attention': 'transformer.encoder.layers.{}.self_attention',
         'o_proj': 'transformer.encoder.layers.{}.self_attention.dense',
@@ -136,14 +148,15 @@
 
 MODEL_KEYS_MAPPING = OrderedDict([
     ('llama', LLAMA_KEYS),
     ('mistral', MISTRAL_KEYS),
     ('qwen1half', QWEN2_KEYS),
     ('yi', YI_KEYS),
     ('gemma', GEMMA_KEYS),
+    ('internlm2', INTERNLM2_KEYS),
     ('internlm', INTERNLM_KEYS),
     ('deepseek', DEEPSEEK_KEYS),
     ('openbuddy', OPENBUDDY_KEYS),
     ('xverse', XVERSE_KEYS),
     ('orion', ORION_KEYS),
     ('bluelm', BLUELM_KEYS),
     ('ziya', ZIYA_KEYS),
```

### Comparing `ms-swift-2.0.2/swift/tuners/neftune.py` & `ms-swift-2.0.3/swift/tuners/neftune.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/peft.py` & `ms-swift-2.0.3/swift/tuners/peft.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/prompt.py` & `ms-swift-2.0.3/swift/tuners/prompt.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/restuning.py` & `ms-swift-2.0.3/swift/tuners/restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/restuning_components.py` & `ms-swift-2.0.3/swift/tuners/restuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/rome/compute_u.py` & `ms-swift-2.0.3/swift/tuners/rome/compute_u.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/rome/compute_v.py` & `ms-swift-2.0.3/swift/tuners/rome/compute_v.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/rome/context_template.py` & `ms-swift-2.0.3/swift/tuners/rome/context_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/rome/nethook.py` & `ms-swift-2.0.3/swift/tuners/rome/nethook.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/rome/repr_tools.py` & `ms-swift-2.0.3/swift/tuners/rome/repr_tools.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/rome/rome.py` & `ms-swift-2.0.3/swift/tuners/rome/rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/rome/rome_hparams.py` & `ms-swift-2.0.3/swift/tuners/rome/rome_hparams.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/scetuning/scetuning.py` & `ms-swift-2.0.3/swift/tuners/scetuning/scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/scetuning/scetuning_components.py` & `ms-swift-2.0.3/swift/tuners/scetuning/scetuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/side.py` & `ms-swift-2.0.3/swift/tuners/side.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/tuners/utils.py` & `ms-swift-2.0.3/swift/tuners/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/app.py` & `ms-swift-2.0.3/swift/ui/app.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/base.py` & `ms-swift-2.0.3/swift/ui/base.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_infer/generate.py` & `ms-swift-2.0.3/swift/ui/llm_infer/generate.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_infer/llm_infer.py` & `ms-swift-2.0.3/swift/ui/llm_infer/llm_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
     @classmethod
     def send_message(cls, running_task, model_and_template, template_type,
                      prompt: str, history, system, max_new_tokens, temperature,
                      top_k, top_p, repetition_penalty):
         if not model_and_template:
             gr.Warning(cls.locale('generate_alert', cls.lang)['value'])
             return '', None
-        args = Runtime.parse_info_from_cmdline(running_task)
+        _, args = Runtime.parse_info_from_cmdline(running_task)
         model_type, template = model_and_template
         old_history, history = history, []
         request_config = XRequestConfig(
             temperature=temperature,
             top_k=top_k,
             top_p=top_p,
             repetition_penalty=repetition_penalty)
```

### Comparing `ms-swift-2.0.2/swift/ui/llm_infer/model.py` & `ms-swift-2.0.3/swift/ui/llm_infer/model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_infer/runtime.py` & `ms-swift-2.0.3/swift/ui/llm_infer/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections
 import os.path
+import sys
 import time
 from datetime import datetime
 from typing import Dict, List, Tuple, Type
 
 import gradio as gr
 import psutil
 from gradio import Accordion, Tab
@@ -121,15 +122,15 @@
     def update_log(cls):
         return gr.update(visible=True)
 
     @classmethod
     def wait(cls, task):
         if not task:
             return [None]
-        args = cls.parse_info_from_cmdline(task)
+        _, args = cls.parse_info_from_cmdline(task)
         log_file = args['log_file']
         offset = 0
         latest_data = ''
         lines = collections.deque(
             maxlen=int(os.environ.get('MAX_LOG_LINES', 50)))
         try:
             with open(log_file, 'r') as input:
@@ -173,36 +174,40 @@
             if any([process_name in cmdline
                     for cmdline in cmdlines]) and any(  # noqa
                         [cmd_name == cmdline for cmdline in cmdlines]):  # noqa
                 try:
                     ports.add(
                         int(
                             Runtime.parse_info_from_cmdline(
-                                Runtime.construct_running_task(proc)).get(
+                                Runtime.construct_running_task(proc))[1].get(
                                     'port', 8000)))
                 except IndexError:
                     pass
         return ports
 
     @staticmethod
     def refresh_tasks(running_task=None):
         log_file = running_task if not running_task or 'pid:' not in running_task else None
         process_name = 'swift'
+        negative_name = 'swift.exe'
         cmd_name = 'deploy'
         process = []
         selected = None
         for proc in psutil.process_iter():
             try:
                 cmdlines = proc.cmdline()
             except (psutil.ZombieProcess, psutil.AccessDenied,
                     psutil.NoSuchProcess):
                 cmdlines = []
-            if any([process_name in cmdline
-                    for cmdline in cmdlines]) and any(  # noqa
-                        [cmd_name == cmdline for cmdline in cmdlines]):  # noqa
+            if any([
+                    process_name in cmdline for cmdline in cmdlines
+            ]) and not any([negative_name in cmdline
+                            for cmdline in cmdlines]) and any(  # noqa
+                                [cmd_name == cmdline
+                                 for cmdline in cmdlines]):  # noqa
                 process.append(Runtime.construct_running_task(proc))
                 if log_file is not None and any(  # noqa
                     [log_file == cmdline for cmdline in cmdlines]):  # noqa
                     selected = Runtime.construct_running_task(proc)
         if not selected:
             if running_task and running_task in process:
                 selected = running_task
@@ -236,38 +241,44 @@
             return time_str
 
         return f'pid:{pid}/create:{create_time_formatted}' \
                f'/running:{format_time(ts - create_time)}/cmd:{" ".join(proc.cmdline())}'
 
     @staticmethod
     def parse_info_from_cmdline(task):
+        pid = None
         for i in range(3):
             slash = task.find('/')
+            if i == 0:
+                pid = task[:slash].split(':')[1]
             task = task[slash + 1:]
         args = task.split('swift deploy')[1]
         args = [arg.strip() for arg in args.split('--') if arg.strip()]
         all_args = {}
         for i in range(len(args)):
             space = args[i].find(' ')
             splits = args[i][:space], args[i][space + 1:]
             all_args[splits[0]] = splits[1]
-        return all_args
+        return pid, all_args
 
     @staticmethod
     def kill_task(task):
-        all_args = Runtime.parse_info_from_cmdline(task)
+        pid, all_args = Runtime.parse_info_from_cmdline(task)
         log_file = all_args['log_file']
-        os.system(f'pkill -9 -f {log_file}')
+        if sys.platform == 'win32':
+            os.system(f'taskkill /f /t /pid "{pid}"')
+        else:
+            os.system(f'pkill -9 -f {log_file}')
         time.sleep(1)
         return [Runtime.refresh_tasks()] + [gr.update(value=None)]
 
     @staticmethod
     def task_changed(task, base_tab):
         if task:
-            all_args = Runtime.parse_info_from_cmdline(task)
+            _, all_args = Runtime.parse_info_from_cmdline(task)
         else:
             all_args = {}
         elements = [
             value for value in base_tab.elements().values()
             if not isinstance(value, (Tab, Accordion))
         ]
         ret = []
```

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/advanced.py` & `ms-swift-2.0.3/swift/ui/llm_train/advanced.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/dataset.py` & `ms-swift-2.0.3/swift/ui/llm_train/dataset.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/hyper.py` & `ms-swift-2.0.3/swift/ui/llm_train/hyper.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/llm_train.py` & `ms-swift-2.0.3/swift/ui/llm_train/llm_train.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/lora.py` & `ms-swift-2.0.3/swift/ui/llm_train/lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/model.py` & `ms-swift-2.0.3/swift/ui/llm_train/model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/quantization.py` & `ms-swift-2.0.3/swift/ui/llm_train/quantization.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/runtime.py` & `ms-swift-2.0.3/swift/ui/llm_train/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections
 import os.path
+import sys
 import time
 import webbrowser
 from datetime import datetime
 from typing import Dict, List, Tuple, Type
 
 import gradio as gr
 import json
@@ -326,26 +327,30 @@
             close_loop(Runtime.handlers[logging_dir][0])
             Runtime.handlers.pop(logging_dir)
 
     @staticmethod
     def refresh_tasks(running_task=None):
         output_dir = running_task if not running_task or 'pid:' not in running_task else None
         process_name = 'swift'
+        negative_name = 'swift.exe'
         cmd_name = 'sft'
         process = []
         selected = None
         for proc in psutil.process_iter():
             try:
                 cmdlines = proc.cmdline()
             except (psutil.ZombieProcess, psutil.AccessDenied,
                     psutil.NoSuchProcess):
                 cmdlines = []
-            if any([process_name in cmdline
-                    for cmdline in cmdlines]) and any(  # noqa
-                        [cmd_name == cmdline for cmdline in cmdlines]):  # noqa
+            if any([
+                    process_name in cmdline for cmdline in cmdlines
+            ]) and not any([negative_name in cmdline
+                            for cmdline in cmdlines]) and any(  # noqa
+                                [cmd_name == cmdline
+                                 for cmdline in cmdlines]):  # noqa
                 process.append(Runtime.construct_running_task(proc))
                 if output_dir is not None and any(  # noqa
                     [output_dir == cmdline for cmdline in cmdlines]):  # noqa
                     selected = Runtime.construct_running_task(proc)
         if not selected:
             if running_task and running_task in process:
                 selected = running_task
@@ -379,16 +384,19 @@
             return time_str
 
         return f'pid:{pid}/create:{create_time_formatted}' \
                f'/running:{format_time(ts-create_time)}/cmd:{" ".join(proc.cmdline())}'
 
     @staticmethod
     def parse_info_from_cmdline(task):
+        pid = None
         for i in range(3):
             slash = task.find('/')
+            if i == 0:
+                pid = task[:slash].split(':')[1]
             task = task[slash + 1:]
         args = task.split('swift sft')[1]
         args = [arg.strip() for arg in args.split('--') if arg.strip()]
         all_args = {}
         for i in range(len(args)):
             space = args[i].find(' ')
             splits = args[i][:space], args[i][space + 1:]
@@ -402,33 +410,36 @@
                 all_args[key] = _json[key]
                 if isinstance(all_args[key], list):
                     if any([' ' in value for value in all_args[key]]):
                         all_args[key] = [
                             f'"{value}"' for value in all_args[key]
                         ]
                     all_args[key] = ' '.join(all_args[key])
-        return all_args
+        return pid, all_args
 
     @staticmethod
     def kill_task(task):
-        all_args = Runtime.parse_info_from_cmdline(task)
+        pid, all_args = Runtime.parse_info_from_cmdline(task)
         output_dir = all_args['output_dir']
-        os.system(f'pkill -9 -f {output_dir}')
+        if sys.platform == 'win32':
+            os.system(f'taskkill /f /t /pid "{pid}"')
+        else:
+            os.system(f'pkill -9 -f {output_dir}')
         time.sleep(1)
         return [Runtime.refresh_tasks()] + [gr.update(value=None)] * (
             len(Runtime.sft_plot) + 1)
 
     @staticmethod
     def reset():
         return None, 'output'
 
     @staticmethod
     def task_changed(task, base_tab):
         if task:
-            all_args = Runtime.parse_info_from_cmdline(task)
+            _, all_args = Runtime.parse_info_from_cmdline(task)
         else:
             all_args = {}
         elements = [
             value for value in base_tab.elements().values()
             if not isinstance(value, (Tab, Accordion))
         ]
         ret = []
@@ -443,15 +454,15 @@
                 ret.append(gr.update())
         return ret + [gr.update(value=None)] * (len(Runtime.sft_plot) + 1)
 
     @staticmethod
     def plot(task):
         if not task:
             return [None] * len(Runtime.sft_plot)
-        all_args = Runtime.parse_info_from_cmdline(task)
+        _, all_args = Runtime.parse_info_from_cmdline(task)
         tb_dir = all_args['logging_dir']
         fname = [
             fname for fname in os.listdir(tb_dir)
             if os.path.isfile(os.path.join(tb_dir, fname))
             and fname.startswith('events.out')
         ]
         if fname:
```

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/save.py` & `ms-swift-2.0.3/swift/ui/llm_train/save.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/self_cog.py` & `ms-swift-2.0.3/swift/ui/llm_train/self_cog.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/ui/llm_train/utils.py` & `ms-swift-2.0.3/swift/ui/llm_train/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/__init__.py` & `ms-swift-2.0.3/swift/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/constants.py` & `ms-swift-2.0.3/swift/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/hub.py` & `ms-swift-2.0.3/swift/utils/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import shutil
 import subprocess
+import tempfile
 import time
 from typing import Optional
 
 from requests.exceptions import HTTPError
 
 from swift.hub import HubApi, ModelScopeConfig
 from swift.hub.constants import ModelVisibility
@@ -42,23 +43,24 @@
 
 def push_to_ms_hub(ckpt_dir: str,
                    hub_model_id: str,
                    hub_token: Optional[str] = None,
                    hub_private_repo: bool = False,
                    commit_message: str = 'update files'):
     logger.info(f'Starting push to hub. ckpt_dir: {ckpt_dir}.')
+    tmp_file_name = tempfile.TemporaryDirectory().name
     subprocess_run(['git', 'lfs', 'env'],
                    stdout=subprocess.PIPE)  # check git-lfs install
 
     hub_model_id = create_ms_repo(hub_model_id, hub_token, hub_private_repo)
     git_token = ModelScopeConfig.get_token()
     ms_url = f'https://oauth2:{git_token}@www.modelscope.cn/{hub_model_id}.git'
-    subprocess_run(['git', '-C', ckpt_dir, 'clone', ms_url, 'tmp'],
+    subprocess_run(['git', '-C', ckpt_dir, 'clone', ms_url, tmp_file_name],
                    env={'GIT_LFS_SKIP_SMUDGE': '1'})
-    tmp_dir = os.path.join(ckpt_dir, 'tmp')
+    tmp_dir = os.path.join(ckpt_dir, tmp_file_name)
     subprocess_run(['git', '-C', tmp_dir, 'lfs', 'pull'])
     logger.info('Git clone the repo successfully.')
     # mv .git
     dst_git_path = os.path.join(ckpt_dir, '.git')
     if os.path.exists(dst_git_path):
         shutil.rmtree(dst_git_path)
     shutil.copytree(os.path.join(tmp_dir, '.git'), dst_git_path)
```

### Comparing `ms-swift-2.0.2/swift/utils/import_utils.py` & `ms-swift-2.0.3/swift/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/io_utils.py` & `ms-swift-2.0.3/swift/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/logger.py` & `ms-swift-2.0.3/swift/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/metric.py` & `ms-swift-2.0.3/swift/utils/metric.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/np_utils.py` & `ms-swift-2.0.3/swift/utils/np_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/run_utils.py` & `ms-swift-2.0.3/swift/utils/run_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/tb_utils.py` & `ms-swift-2.0.3/swift/utils/tb_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/swift/utils/torch_utils.py` & `ms-swift-2.0.3/swift/utils/torch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bisect import bisect_right
 from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
 import torch.distributed as dist
 from torch.nn import Module
+from transformers.utils import is_torch_npu_available
 
 from .logger import get_logger, is_master
 
 logger = get_logger()
 
 
 def is_on_same_device(model: torch.nn.Module) -> bool:
@@ -148,23 +149,25 @@
     """String broadcasting in case of DDP
     string: main rank: str
         other rank: None or str(not use)
     return: all rank: str
     """
     assert dist.is_initialized()
     rank, local_rank, _, _ = get_dist_setting()
+    device = f'npu:{local_rank}' if is_torch_npu_available(
+    ) else f'cuda:{local_rank}'
     assert rank >= 0
     if rank == 0:
         assert string is not None
         tensor = torch.tensor(
             [ord(c) for c in string] + [0] * (buffer_size - len(string)),
             dtype=torch.int64,
-            device=local_rank)
+            device=device)
     else:
-        tensor = torch.zeros(buffer_size, dtype=torch.int64, device=local_rank)
+        tensor = torch.zeros(buffer_size, dtype=torch.int64, device=device)
     dist.broadcast(tensor, 0)
     first_zero = (tensor == 0).nonzero()[0].item()
     res = tensor.tolist()[:first_zero]
     return ''.join([chr(x) for x in res])
 
 
 def time_synchronize() -> float:
```

### Comparing `ms-swift-2.0.2/swift/utils/utils.py` & `ms-swift-2.0.3/swift/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 def get_pai_tensorboard_dir() -> Optional[str]:
     return os.environ.get('PAI_OUTPUT_TENSORBOARD')
 
 
 def subprocess_run(command: List[str],
                    env: Optional[Dict[str, str]] = None,
                    stdout=None,
-                   stderr=None) -> None:
+                   stderr=None):
     # stdoutm stderr: e.g. subprocess.PIPE.
     resp = subprocess.run(command, env=env, stdout=stdout, stderr=stderr)
     resp.check_returncode()
     return resp
 
 
 def split_str_parts_by(text: str, delimiters: List[str]):
```

### Comparing `ms-swift-2.0.2/tests/hub/test_check_model.py` & `ms-swift-2.0.3/tests/hub/test_check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/llm/test_dataset.py` & `ms-swift-2.0.3/tests/llm/test_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datasets import Dataset as HfDataset
 
 from swift.llm import DatasetName, get_dataset
 
 
 class TestDataset(unittest.TestCase):
 
+    @unittest.skip('fix citest')
     def test_dataset(self):
         train_dataset, val_dataset = get_dataset(
             [DatasetName.leetcode_python_en, DatasetName.blossom_math_zh])
         assert isinstance(train_dataset, HfDataset) and val_dataset is None
         totol_len = 12359
         assert len(train_dataset) == totol_len
```

### Comparing `ms-swift-2.0.2/tests/llm/test_run.py` & `ms-swift-2.0.3/tests/llm/test_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
             SftArguments(
                 model_type=ModelType.deepseek_vl_1_3b_chat,
                 #   dataset=DatasetName.capcha_images,
                 lora_target_modules='ALL',
                 train_dataset_sample=100,
                 eval_steps=5,
                 custom_train_dataset_path=[
-                    os.path.join(folder, 'multi_modal.jsonl')
+                    os.path.join(folder, 'multi_modal2.jsonl')
                 ],
                 lazy_tokenize=False))
 
 
 def data_collate_fn(batch: List[Dict[str, Any]],
                     tokenizer) -> Dict[str, Tensor]:
     # text-classification
```

### Comparing `ms-swift-2.0.2/tests/llm/test_template.py` & `ms-swift-2.0.3/tests/llm/test_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/llm/test_utils.py` & `ms-swift-2.0.3/tests/llm/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/llm/test_vllm_utils.py` & `ms-swift-2.0.3/tests/llm/test_vllm_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/model_tag.py` & `ms-swift-2.0.3/tests/model_tag.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/run.py` & `ms-swift-2.0.3/tests/run.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/test_utils.py` & `ms-swift-2.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/tuners/test_extra_state_dict.py` & `ms-swift-2.0.3/tests/tuners/test_extra_state_dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import os.path
 import shutil
 import tempfile
 import unittest
 
-import peft
 import torch
 from modelscope import Model
-from packaging import version
 
 from swift import LoRAConfig, Swift
 from swift.tuners.utils import ModulesToSaveWrapper
 
 
-@unittest.skipIf(
-    version.parse(peft.__version__) >= version.parse('0.10.0'),
-    reason='version not match')
 class TestExtraStateDict(unittest.TestCase):
 
     def setUp(self):
         print(('Testing %s.%s' % (type(self).__name__, self._testMethodName)))
         self.tmp_dir = tempfile.TemporaryDirectory().name
         if not os.path.exists(self.tmp_dir):
             os.makedirs(self.tmp_dir)
```

### Comparing `ms-swift-2.0.2/tests/tuners/test_merged_linear.py` & `ms-swift-2.0.3/tests/tuners/test_merged_linear.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import math
 import unittest
 
-import peft
 import torch
 from modelscope import Model, Preprocessor
-from packaging import version
 from torch import nn
 
 from swift import LoRAConfig, Swift
 
 
-@unittest.skipIf(
-    version.parse(peft.__version__) >= version.parse('0.10.0'),
-    reason='version not match')
 class TestMergedLinear(unittest.TestCase):
 
     def test_swift_lora_forward(self):
 
         from swift.tuners.lora import MergedLinear
 
         def reset_parameters(self):
```

### Comparing `ms-swift-2.0.2/tests/tuners/test_neft.py` & `ms-swift-2.0.3/tests/tuners/test_neft.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import os
 import shutil
 import tempfile
 import unittest
 
-import peft
 import torch
-from modelscope import AutoModel, AutoTokenizer, Preprocessor
-from packaging import version
+from modelscope import AutoModel, Preprocessor
 from peft.utils import WEIGHTS_NAME
 from transformers import PreTrainedModel
 
-from swift import LoraConfig, Swift
+from swift import LoRAConfig, Swift
 from swift.tuners import NEFTuneConfig
 
 
 class TestNEFT(unittest.TestCase):
 
     def setUp(self):
         print(('Testing %s.%s' % (type(self).__name__, self._testMethodName)))
@@ -73,24 +71,21 @@
             self.assertTrue(key in state_dict2)
             self.assertTrue(
                 all(
                     torch.isclose(state_dict[key],
                                   state_dict2[key]).flatten().detach().cpu()))
         PreTrainedModel.save_pretrained = PreTrainedModel.origin_save_pretrained
 
-    @unittest.skipIf(
-        version.parse(peft.__version__) >= version.parse('0.10.0'),
-        reason='version not match')
     def test_neft_lora(self):
         model = AutoModel.from_pretrained('AI-ModelScope/bert-base-uncased')
         preprocessor = Preprocessor.from_pretrained(
             'damo/nlp_structbert_sentence-similarity_chinese-base')
         inputs = preprocessor('how are you')
         config = NEFTuneConfig()
-        config2 = LoraConfig(target_modules=['query', 'key', 'value'])
+        config2 = LoRAConfig(target_modules=['query', 'key', 'value'])
 
         t1 = model.embeddings.word_embeddings(inputs['input_ids'])
         model = Swift.prepare_model(model, {'c1': config, 'c2': config2})
         model.train()
         t2 = model.embeddings.word_embeddings(inputs['input_ids'])
         model.deactivate_adapter('c1')
         t3 = model.embeddings.word_embeddings(inputs['input_ids'])
```

### Comparing `ms-swift-2.0.2/tests/tuners/test_peft.py` & `ms-swift-2.0.3/tests/tuners/test_peft.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import unittest
 
 import peft
 import torch
 from modelscope import Preprocessor
 from modelscope.models.nlp.structbert import (SbertConfig,
                                               SbertForSequenceClassification)
-from packaging import version
 from peft import PeftModel, inject_adapter_in_model
 from peft.config import PeftConfigMixin
 from peft.tuners.lora import Linear
 from peft.utils import WEIGHTS_NAME
 from torch import nn
 
 from swift import AdaLoraConfig, LoraConfig, LoRAConfig, Swift, get_peft_model
@@ -118,17 +117,14 @@
         for key in state_dict:
             self.assertTrue(key in state_dict3)
             self.assertTrue(
                 all(
                     torch.isclose(state_dict[key],
                                   state_dict3[key]).flatten().detach().cpu()))
 
-    @unittest.skipIf(
-        version.parse(peft.__version__) >= version.parse('0.10.0'),
-        reason='version not match')
     def test_lora_reload_by_peft(self):
         lora_config = LoRAConfig(target_modules=['query', 'key', 'value'])
         model = SbertForSequenceClassification(SbertConfig())
         model2 = copy.deepcopy(model)
         model = Swift.prepare_model(model, lora_config)
         model.save_pretrained(self.tmp_dir, peft_format=True)
         model2 = PeftModel.from_pretrained(model2, self.tmp_dir)
@@ -162,14 +158,15 @@
         for key in state_dict:
             self.assertTrue(key in state_dict2)
             self.assertTrue(
                 all(
                     torch.isclose(state_dict[key],
                                   state_dict2[key]).flatten().detach().cpu()))
 
+    @unittest.skip
     def test_peft_lora_dtype(self):
         model = SbertForSequenceClassification(SbertConfig())
         model2 = copy.deepcopy(model)
         model3 = copy.deepcopy(model)
         lora_config = LoraConfig(
             target_modules=['query', 'key', 'value'], lora_dtype='fp16')
         model = Swift.prepare_model(model, lora_config)
@@ -187,12 +184,12 @@
             self.assertTrue(key in state_dict2)
             self.assertTrue(
                 all(
                     torch.isclose(state_dict[key],
                                   state_dict2[key]).flatten().detach().cpu()))
 
         PeftConfigMixin.from_pretrained = PeftConfigMixin.from_pretrained_origin
-        model3 = peft.PeftModel.from_pretrained(model3, self.tmp_dir)
+        model3 = Swift.from_pretrained(model3, self.tmp_dir)
         self.assertTrue(model3.base_model.model.bert.encoder.layer[0].attention
                         .self.key.lora_A.default.weight.dtype == torch.float32)
         self.assertTrue(
             isinstance(model3.peft_config['default'], peft.LoraConfig))
```

### Comparing `ms-swift-2.0.2/tests/tuners/test_rome.py` & `ms-swift-2.0.3/tests/tuners/test_rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/tuners/test_scetuning.py` & `ms-swift-2.0.3/tests/tuners/test_scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/tuners/test_swift_base.py` & `ms-swift-2.0.3/tests/tuners/test_swift_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 from peft.utils import WEIGHTS_NAME
 from torch import nn
 
 from swift import (AdapterConfig, LoRAConfig, PromptConfig, ResTuningConfig,
                    SideConfig, Swift, SwiftModel)
 
 
-@unittest.skipIf(
-    version.parse(peft.__version__) >= version.parse('0.10.0'),
-    reason='version not match')
 class TestSwift(unittest.TestCase):
 
     def setUp(self):
         print(('Testing %s.%s' % (type(self).__name__, self._testMethodName)))
         self.tmp_dir = tempfile.TemporaryDirectory().name
         if not os.path.exists(self.tmp_dir):
             os.makedirs(self.tmp_dir)
```

### Comparing `ms-swift-2.0.2/tests/tuners/test_swift_device_map.py` & `ms-swift-2.0.3/tests/tuners/test_swift_device_map.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/tuners/test_swift_restuning.py` & `ms-swift-2.0.3/tests/tuners/test_swift_restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.2/tests/utils/test_io_utils.py` & `ms-swift-2.0.3/tests/utils/test_io_utils.py`

 * *Files identical despite different names*


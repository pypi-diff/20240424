# Comparing `tmp/llm_optimized_inference-0.1.4-py3-none-any.whl.zip` & `tmp/llm_optimized_inference-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,38 @@
-Zip file size: 66366 bytes, number of entries: 36
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-19 00:42 llm/__init__.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-19 00:42 llm/optimized/__init__.py
--rw-rw-r--  2.0 unx      703 b- defN 24-Apr-19 00:42 llm/optimized/inference/__init__.py
--rw-rw-r--  2.0 unx      204 b- defN 24-Apr-19 00:42 llm/optimized/inference/_version.py
--rw-rw-r--  2.0 unx    28243 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server.py
--rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-19 00:42 llm/optimized/inference/configs.py
--rw-rw-r--  2.0 unx     5469 b- defN 24-Apr-19 00:42 llm/optimized/inference/constants.py
--rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-19 00:42 llm/optimized/inference/conversation.py
--rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-19 00:42 llm/optimized/inference/fm_score.py
--rw-rw-r--  2.0 unx      664 b- defN 24-Apr-19 00:42 llm/optimized/inference/logging_config.py
--rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-19 00:42 llm/optimized/inference/managed_inference.py
--rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-19 00:42 llm/optimized/inference/model_config_factory.py
--rw-rw-r--  2.0 unx     6638 b- defN 24-Apr-19 00:42 llm/optimized/inference/model_utils.py
--rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-19 00:42 llm/optimized/inference/prompt_formatter.py
--rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-19 00:42 llm/optimized/inference/replica_manager.py
--rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-19 00:42 llm/optimized/inference/score.py
--rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-19 00:42 llm/optimized/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server_setup/__init__.py
--rw-rw-r--  2.0 unx     9502 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server_setup/openapi.json
--rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server_setup/protocol.py
--rw-rw-r--  2.0 unx      131 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/__init__.py
--rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
--rw-rw-r--  2.0 unx     8806 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
--rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/schema_output.py
--rw-rw-r--  2.0 unx      259 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/__init__.py
--rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/_hf_predictors.py
--rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/engine.py
--rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/hf_engine.py
--rw-rw-r--  2.0 unx    10797 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/mii_engine.py
--rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/mii_engine_v2.py
--rw-rw-r--  2.0 unx    14278 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/vllm_engine.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3113 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3599 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/RECORD
-36 files, 218567 bytes uncompressed, 60382 bytes compressed:  72.4%
+Zip file size: 66390 bytes, number of entries: 36
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-24 00:40 llm/__init__.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-24 00:40 llm/optimized/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 24-Apr-24 00:40 llm/optimized/inference/__init__.py
+-rw-rw-r--  2.0 unx      204 b- defN 24-Apr-24 00:40 llm/optimized/inference/_version.py
+-rw-rw-r--  2.0 unx    28243 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server.py
+-rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-24 00:40 llm/optimized/inference/configs.py
+-rw-rw-r--  2.0 unx     5548 b- defN 24-Apr-24 00:40 llm/optimized/inference/constants.py
+-rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-24 00:40 llm/optimized/inference/conversation.py
+-rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-24 00:40 llm/optimized/inference/fm_score.py
+-rw-rw-r--  2.0 unx      664 b- defN 24-Apr-24 00:40 llm/optimized/inference/logging_config.py
+-rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-24 00:40 llm/optimized/inference/managed_inference.py
+-rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-24 00:40 llm/optimized/inference/model_config_factory.py
+-rw-rw-r--  2.0 unx     6638 b- defN 24-Apr-24 00:40 llm/optimized/inference/model_utils.py
+-rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-24 00:40 llm/optimized/inference/prompt_formatter.py
+-rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-24 00:40 llm/optimized/inference/replica_manager.py
+-rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-24 00:40 llm/optimized/inference/score.py
+-rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-24 00:40 llm/optimized/inference/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server_setup/__init__.py
+-rw-rw-r--  2.0 unx     9502 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server_setup/openapi.json
+-rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server_setup/protocol.py
+-rw-rw-r--  2.0 unx      131 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/__init__.py
+-rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
+-rw-rw-r--  2.0 unx     8806 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/schema_output.py
+-rw-rw-r--  2.0 unx      259 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/__init__.py
+-rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/_hf_predictors.py
+-rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/engine.py
+-rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/hf_engine.py
+-rw-rw-r--  2.0 unx    10797 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/mii_engine.py
+-rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/mii_engine_v2.py
+-rw-rw-r--  2.0 unx    14278 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/vllm_engine.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3113 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3599 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/RECORD
+36 files, 218646 bytes uncompressed, 60406 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -87,23 +87,23 @@
 
 Filename: llm/optimized/inference/engine/mii_engine_v2.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/vllm_engine.py
 Comment: 
 
-Filename: llm_optimized_inference-0.1.4.dist-info/LICENSE
+Filename: llm_optimized_inference-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: llm_optimized_inference-0.1.4.dist-info/METADATA
+Filename: llm_optimized_inference-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: llm_optimized_inference-0.1.4.dist-info/WHEEL
+Filename: llm_optimized_inference-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: llm_optimized_inference-0.1.4.dist-info/top_level.txt
+Filename: llm_optimized_inference-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_optimized_inference-0.1.4.dist-info/RECORD
+Filename: llm_optimized_inference-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llm/optimized/inference/_version.py

```diff
@@ -1,5 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
```

## llm/optimized/inference/constants.py

```diff
@@ -89,15 +89,16 @@
         "OrionForCausalLM",
         "QWenLMHeadModel",
         "Qwen2ForCausalLM",
         "RWForCausalLM",
         "StableLmForCausalLM",
         "DbrxForCausalLM",
         "Phi3MiniForCausalLM",
-        "PhiLongRoPEForCausalLM"
+        "PhiLongRoPEForCausalLM",
+        "YakForCausalLM"
     }
 
 
 class MIISupportedModels:
     """MII Supported Models."""
 
     # TODO: Add more models from different tasks
@@ -126,15 +127,16 @@
     Models = {
         "falcon": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWebModel": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWeb": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "dbrx": {"args": ["trust-remote-code"]},
         "deci_lm": {"args": ["trust-remote-code"]},
         "phi3mini": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
-        "phi_longrope": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]}
+        "phi_longrope": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
+        "yak": {"kwargs": {"quantization": "yq"}}
 
     }
 
     @classmethod
     def get_kwargs(cls, model_type: str):
         """Get the kwargs the vllm server needs for the model type."""
         params = cls.Models.get(model_type, {})
```

## Comparing `llm_optimized_inference-0.1.4.dist-info/METADATA` & `llm_optimized_inference-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-optimized-inference
-Version: 0.1.4
+Version: 0.1.5
 Home-page: 
 Author: Microsoft
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `llm_optimized_inference-0.1.4.dist-info/RECORD` & `llm_optimized_inference-0.1.5.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 llm/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/inference/__init__.py,sha256=rGZODP-qE2NOlUgdbmxhfuS3svmx9gM-kU97d9-jb50,703
-llm/optimized/inference/_version.py,sha256=xTMdyihKrF9Wwzf6EEZPWUMcTZtCY6fmsZCX3oPpH4o,204
+llm/optimized/inference/_version.py,sha256=aMIajadgoqRXx51Q5q1FRPYUqvpLEK0ugL8CtTU-DrA,204
 llm/optimized/inference/api_server.py,sha256=kyUIykJuk9jPajQyUqqMl4FEQKLZV57LykfGY0Z99Ak,28243
 llm/optimized/inference/configs.py,sha256=d5NKbQlfYVkUQ4SL03KVBQekdOG4VrcD0xGxVeHESeQ,3203
-llm/optimized/inference/constants.py,sha256=1MgHKQg67k-swDkfhsrRDRpMabW82ZKNfvdhSyP61vE,5469
+llm/optimized/inference/constants.py,sha256=FqDNm7XiTHbFbdUKxgFwYEeH7pOomJngU4PB3mOwgoI,5548
 llm/optimized/inference/conversation.py,sha256=cBrHv1sI1hrOQB57sSZKAarplKRgqQWqmYxT-wkZHLM,3255
 llm/optimized/inference/fm_score.py,sha256=7z7ZbLMXUXH6gp1-G_l3rOus9r9vSpIm5-wOj5X17aQ,5802
 llm/optimized/inference/logging_config.py,sha256=egtAiGCNVNoU8E_JPhp2aGJVIJ_QkTwLhkNjpVKjICI,664
 llm/optimized/inference/managed_inference.py,sha256=O_HlOPNl24Uoy68gFKrSM_gOG-rg4P_lishBQFAXyC8,9028
 llm/optimized/inference/model_config_factory.py,sha256=EpHH8QyUaE5DC6A5O5nKbie_kMEpfeqmufbOn0U6jFI,1369
 llm/optimized/inference/model_utils.py,sha256=W9nLxInrhuPnmhvZldBpS2POB7-u_SST7ostxatAYrA,6638
 llm/optimized/inference/prompt_formatter.py,sha256=xxM4MbvvPL6jQcLB37uKA9-wCHXTZUL9l5GiUu3r964,1575
@@ -25,12 +25,12 @@
 llm/optimized/inference/engine/__init__.py,sha256=8GqGW53dbRlGShwO11h5HQH4KjnUzoW0t0cChUUFDPY,259
 llm/optimized/inference/engine/_hf_predictors.py,sha256=AwQTIpmOHb7h31H2DF2Jx-9b03lcB5DOrgSbXGpamIk,38577
 llm/optimized/inference/engine/engine.py,sha256=xbpEVJBjovFyACw6WF8uqnmyodRWqb52oaR3s3pr8Sc,4583
 llm/optimized/inference/engine/hf_engine.py,sha256=4rRldNod-pMDJ_-3q0RDWEkigCTr6I62HyJspb01lAs,8617
 llm/optimized/inference/engine/mii_engine.py,sha256=TBfc_wt4-NKTzkjHCie5YpqRGS6pvBNigyYpTHt_jII,10797
 llm/optimized/inference/engine/mii_engine_v2.py,sha256=rI4tjRyj-dCZBDAiN0YNPKMBtkD3MXxcbucuSlHg6lI,7971
 llm/optimized/inference/engine/vllm_engine.py,sha256=IZDkMxOTMhsn7qCmsSAfIE8DFll4dfDRIWd5FU6_a3c,14278
-llm_optimized_inference-0.1.4.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-llm_optimized_inference-0.1.4.dist-info/METADATA,sha256=z3BdPc8OhIo4ByRfgRnJtPYq2shTK66a8dgLk162wr0,3113
-llm_optimized_inference-0.1.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-llm_optimized_inference-0.1.4.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
-llm_optimized_inference-0.1.4.dist-info/RECORD,,
+llm_optimized_inference-0.1.5.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+llm_optimized_inference-0.1.5.dist-info/METADATA,sha256=rry2yZ8rLf2ozc1k-3qP6kJ9fD6UkTYXpqsslblJgN0,3113
+llm_optimized_inference-0.1.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+llm_optimized_inference-0.1.5.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
+llm_optimized_inference-0.1.5.dist-info/RECORD,,
```


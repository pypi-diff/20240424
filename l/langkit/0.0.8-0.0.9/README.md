# Comparing `tmp/langkit-0.0.8.tar.gz` & `tmp/langkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.8.tar", max compression
+gzip compressed data, was "langkit-0.0.9.tar", max compression
```

## Comparing `langkit-0.0.8.tar` & `langkit-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.8/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.8/LICENSE
--rw-r--r--   0        0        0     1172 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/__init__.py
--rw-r--r--   0        0        0      596 2023-07-06 08:00:05.378422 langkit-0.0.8/langkit/all_metrics.py
--rw-r--r--   0        0        0     7915 2023-07-21 20:23:39.317422 langkit-0.0.8/langkit/callback_handler.py
--rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/config/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/config/environment.py
--rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/quality.md
--rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/relevance.md
--rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/security.md
--rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/sentiment.md
--rw-r--r--   0        0        0    13344 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/docs/modules.md
--rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/examples/Batch_to_Whylabs.ipynb
--rw-r--r--   0        0        0   247730 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/examples/ChatGPT_Behavioral_Monitoring.ipynb
--rw-r--r--   0        0        0     9709 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/examples/Intro_to_Langkit.ipynb
--rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
--rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/Sentiment_and_Toxicity.ipynb
--rw-r--r--   0        0        0    32760 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/examples/huggingface_langkit_whylabs.ipynb
--rw-r--r--   0        0        0    17916 2023-07-18 18:26:20.608508 langkit-0.0.8/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb
--rw-r--r--   0        0        0   109092 2023-07-07 22:52:41.698422 langkit-0.0.8/langkit/examples/tutorials/images/dashboard.png
--rw-r--r--   0        0        0   336393 2023-07-07 22:52:41.698422 langkit-0.0.8/langkit/examples/tutorials/images/safeguards_pipeline.png
--rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/injections.py
--rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/input_output.py
--rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/light_metrics.py
--rw-r--r--   0        0        0      730 2023-07-14 23:21:22.918508 langkit-0.0.8/langkit/llm_metrics.py
--rw-r--r--   0        0        0     1934 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/nlp_scores.py
--rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/openai/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/openai/openai.py
--rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/openai_wrapper.py
--rw-r--r--   0        0        0      807 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/pattern_groups.json
--rw-r--r--   0        0        0     3038 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/regexes.py
--rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/sentiment.py
--rw-r--r--   0        0        0     1172 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/tests/__init__.py
--rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/conftest.py
--rw-r--r--   0        0        0     4407 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/tests/test_callback_handler.py
--rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/test_injections.py
--rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0      653 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/tests/test_nlp_scores.py
--rw-r--r--   0        0        0     4700 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     3718 2023-07-18 23:33:02.638508 langkit-0.0.8/langkit/tests/test_themes.py
--rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/test_toxicity.py
--rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/textstat.py
--rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/themes.json.txt
--rw-r--r--   0        0        0     4220 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/themes.py
--rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/topics.py
--rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/transformer.py
--rw-r--r--   0        0        0     1159 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/whylogs/example_utils/guardrails_example_utils.py
--rw-r--r--   0        0        0     6609 2023-07-07 22:52:41.698422 langkit-0.0.8/langkit/whylogs/example_utils/guardrails_llm_schema.py
--rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.8/langkit/whylogs/reference_chats.json
--rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.8/langkit/whylogs/rolling_logger.py
--rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.8/langkit/whylogs/samples.py
--rw-r--r--   0        0        0     1118 2023-07-21 20:28:08.227422 langkit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 langkit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.9/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1172 2023-07-24 12:52:54.320304 langkit-0.0.9/langkit/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-06 08:00:05.378422 langkit-0.0.9/langkit/all_metrics.py
+-rw-r--r--   0        0        0     9351 2023-07-24 17:35:49.244675 langkit-0.0.9/langkit/callback_handler.py
+-rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.9/langkit/config/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.9/langkit/config/environment.py
+-rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.9/langkit/docs/features/quality.md
+-rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.9/langkit/docs/features/relevance.md
+-rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.9/langkit/docs/features/security.md
+-rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.9/langkit/docs/features/sentiment.md
+-rw-r--r--   0        0        0    13344 2023-07-24 12:52:54.320304 langkit-0.0.9/langkit/docs/modules.md
+-rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.9/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0   247730 2023-07-24 12:52:54.320304 langkit-0.0.9/langkit/examples/ChatGPT_Behavioral_Monitoring.ipynb
+-rw-r--r--   0        0        0     9709 2023-07-18 18:24:21.578508 langkit-0.0.9/langkit/examples/Intro_to_Langkit.ipynb
+-rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
+-rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0    32760 2023-07-21 03:21:01.012440 langkit-0.0.9/langkit/examples/huggingface_langkit_whylabs.ipynb
+-rw-r--r--   0        0        0    17916 2023-07-18 18:26:20.608508 langkit-0.0.9/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb
+-rw-r--r--   0        0        0   109092 2023-07-07 22:52:41.698422 langkit-0.0.9/langkit/examples/tutorials/images/dashboard.png
+-rw-r--r--   0        0        0   336393 2023-07-07 22:52:41.698422 langkit-0.0.9/langkit/examples/tutorials/images/safeguards_pipeline.png
+-rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/injections.py
+-rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/input_output.py
+-rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/light_metrics.py
+-rw-r--r--   0        0        0      730 2023-07-14 23:21:22.918508 langkit-0.0.9/langkit/llm_metrics.py
+-rw-r--r--   0        0        0     1934 2023-07-24 12:52:54.320304 langkit-0.0.9/langkit/nlp_scores.py
+-rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/openai/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/openai/openai.py
+-rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/openai_wrapper.py
+-rw-r--r--   0        0        0      807 2023-07-21 03:21:01.012440 langkit-0.0.9/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     3038 2023-07-21 03:21:01.012440 langkit-0.0.9/langkit/regexes.py
+-rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/sentiment.py
+-rw-r--r--   0        0        0     1172 2023-07-24 12:52:54.320304 langkit-0.0.9/langkit/tests/__init__.py
+-rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     4407 2023-07-18 18:24:21.578508 langkit-0.0.9/langkit/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/tests/test_injections.py
+-rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0      653 2023-07-24 12:52:54.320304 langkit-0.0.9/langkit/tests/test_nlp_scores.py
+-rw-r--r--   0        0        0     4700 2023-07-21 03:21:01.012440 langkit-0.0.9/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     3718 2023-07-18 23:33:02.638508 langkit-0.0.9/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/tests/test_toxicity.py
+-rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/textstat.py
+-rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/themes.json.txt
+-rw-r--r--   0        0        0     4220 2023-07-18 18:24:21.578508 langkit-0.0.9/langkit/themes.py
+-rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/topics.py
+-rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.9/langkit/transformer.py
+-rw-r--r--   0        0        0     1159 2023-07-18 18:24:21.578508 langkit-0.0.9/langkit/whylogs/example_utils/guardrails_example_utils.py
+-rw-r--r--   0        0        0     6609 2023-07-07 22:52:41.698422 langkit-0.0.9/langkit/whylogs/example_utils/guardrails_llm_schema.py
+-rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.9/langkit/whylogs/reference_chats.json
+-rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.9/langkit/whylogs/rolling_logger.py
+-rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.9/langkit/whylogs/samples.py
+-rw-r--r--   0        0        0     1118 2023-07-24 17:40:11.344675 langkit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 langkit-0.0.9/PKG-INFO
```

### Comparing `langkit-0.0.8/DESCRIPTION.md` & `langkit-0.0.9/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/LICENSE` & `langkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/__init__.py` & `langkit-0.0.9/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/all_metrics.py` & `langkit-0.0.9/langkit/all_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/callback_handler.py` & `langkit-0.0.9/langkit/callback_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 from functools import partial
 from logging import getLogger
+from time import time
 from typing import Any, Callable, Dict, List, Optional, Union
 from whylogs.api.logger.logger import Logger
 
 
 diagnostic_logger = getLogger(__name__)
 
 
@@ -56,32 +57,65 @@
 class LangKitCallback:
     def __init__(self, logger: Logger):
         """Bind the configured logger for this langKit callback handler."""
         self._logger = logger
         diagnostic_logger.info(
             f"Initialized LangKitCallback handler with configured whylogs Logger {logger}."
         )
+        self.records: Dict[str, Any] = dict()
 
-    def _profile_generations(self, generations: List[Any]) -> None:
+    def _extract_generation_responses(
+        self, generations: List[Any]
+    ) -> List[Dict[str, Any]]:
+        responses = list()
         for gen in generations:
             if hasattr(gen, "text"):
-                self._logger.log({"response": gen.text})
+                responses.append({"response": gen.text})
+        return responses
 
     # Start LLM events
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> None:
         """Pass the input prompts to the logger"""
-        for prompt in prompts:
-            self._logger.log({"prompt": prompt})
+        invocation_params = kwargs.get("invocation_params")
+        run_id = kwargs.get("run_id", 0)
+        self.records[run_id] = {"prompts": prompts, "t0": time()}
+        if hasattr(self._logger, "_current_profile"):
+            profile = self._logger._current_profile
+            if invocation_params is not None:
+                profile.track(
+                    {
+                        "invocation_params." + key: value
+                        for key, value in invocation_params.items()
+                    },
+                    execute_udfs=False,
+                )
 
     def on_llm_end(self, response: Any, **kwargs: Any) -> None:
         """Pass the generated response to the logger."""
-        for generations in response.generations:
-            self._profile_generations(generations)
+        run_id = kwargs.get("run_id", 0)
+        llm_record = self.records.get(run_id)
+        if llm_record is not None:
+            response_latency_s = time() - llm_record["t0"]
+            self._logger.log({"response_latency_s": response_latency_s})
+            index = 0
+            prompts = llm_record["prompts"]
+            for generations in response.generations:
+                responses = self._extract_generation_responses(generations)
+                for response_record in responses:
+                    response_record.update({"prompt": prompts[index]})
+                    self._logger.log(response_record)
+                index = index + 1
+
+        if hasattr(response, "llm_output"):
+            llm_output = response.llm_output
+            token_usage = llm_output.get("token_usage")
+            if token_usage:
+                self._logger.log(token_usage)
 
     def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         diagnostic_logger.debug(f"on_llm_new_token({token})")
 
     def on_llm_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> None:
```

### Comparing `langkit-0.0.8/langkit/config/environment.py` & `langkit-0.0.9/langkit/config/environment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/docs/features/quality.md` & `langkit-0.0.9/langkit/docs/features/quality.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/docs/features/relevance.md` & `langkit-0.0.9/langkit/docs/features/relevance.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/docs/features/security.md` & `langkit-0.0.9/langkit/docs/features/security.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/docs/features/sentiment.md` & `langkit-0.0.9/langkit/docs/features/sentiment.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/docs/modules.md` & `langkit-0.0.9/langkit/docs/modules.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/Batch_to_Whylabs.ipynb` & `langkit-0.0.9/langkit/examples/Batch_to_Whylabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/ChatGPT_Behavioral_Monitoring.ipynb` & `langkit-0.0.9/langkit/examples/ChatGPT_Behavioral_Monitoring.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/Intro_to_Langkit.ipynb` & `langkit-0.0.9/langkit/examples/Intro_to_Langkit.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.9/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb` & `langkit-0.0.9/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.9/langkit/examples/Logging_Text.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/Sentiment_and_Toxicity.ipynb` & `langkit-0.0.9/langkit/examples/Sentiment_and_Toxicity.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/huggingface_langkit_whylabs.ipynb` & `langkit-0.0.9/langkit/examples/huggingface_langkit_whylabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb` & `langkit-0.0.9/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/tutorials/images/dashboard.png` & `langkit-0.0.9/langkit/examples/tutorials/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/examples/tutorials/images/safeguards_pipeline.png` & `langkit-0.0.9/langkit/examples/tutorials/images/safeguards_pipeline.png`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/injections.py` & `langkit-0.0.9/langkit/injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/input_output.py` & `langkit-0.0.9/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/llm_metrics.py` & `langkit-0.0.9/langkit/llm_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/nlp_scores.py` & `langkit-0.0.9/langkit/nlp_scores.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/openai/openai.py` & `langkit-0.0.9/langkit/openai/openai.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/openai_wrapper.py` & `langkit-0.0.9/langkit/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/pattern_groups.json` & `langkit-0.0.9/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/regexes.py` & `langkit-0.0.9/langkit/regexes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/sentiment.py` & `langkit-0.0.9/langkit/sentiment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/__init__.py` & `langkit-0.0.9/langkit/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/conftest.py` & `langkit-0.0.9/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/test_callback_handler.py` & `langkit-0.0.9/langkit/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/test_injections.py` & `langkit-0.0.9/langkit/tests/test_injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/test_input_output.py` & `langkit-0.0.9/langkit/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/test_nlp_scores.py` & `langkit-0.0.9/langkit/tests/test_nlp_scores.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/test_patterns.py` & `langkit-0.0.9/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/test_themes.py` & `langkit-0.0.9/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/tests/test_toxicity.py` & `langkit-0.0.9/langkit/tests/test_toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/textstat.py` & `langkit-0.0.9/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/themes.json` & `langkit-0.0.9/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/themes.py` & `langkit-0.0.9/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/topics.py` & `langkit-0.0.9/langkit/topics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/toxicity.py` & `langkit-0.0.9/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/whylogs/example_utils/guardrails_example_utils.py` & `langkit-0.0.9/langkit/whylogs/example_utils/guardrails_example_utils.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/whylogs/example_utils/guardrails_llm_schema.py` & `langkit-0.0.9/langkit/whylogs/example_utils/guardrails_llm_schema.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/whylogs/reference_chats.json` & `langkit-0.0.9/langkit/whylogs/reference_chats.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/langkit/whylogs/samples.py` & `langkit-0.0.9/langkit/whylogs/samples.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.8/pyproject.toml` & `langkit-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.8"
+version = "0.0.9"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "DESCRIPTION.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `langkit-0.0.8/PKG-INFO` & `langkit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/bpm_ai_core-2.4.2.tar.gz` & `tmp/bpm_ai_core-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.4.2.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.5.0.tar", max compression
```

## Comparing `bpm_ai_core-2.4.2.tar` & `bpm_ai_core-2.5.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0       13 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/README.md
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/classification/__init__.py
--rw-r--r--   0        0        0     1420 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/classification/zero_shot_classifier.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      862 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     6645 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0     4872 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6141 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2445 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1455 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      430 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     7777 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     3340 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2698 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1220 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6259 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     1989 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3028 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1096 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0      827 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1428 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2894 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/token_classification/__init__.py
--rw-r--r--   0        0        0      909 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/token_classification/zero_shot_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4381 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2347 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1572 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      475 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     2290 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     6130 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     3135 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    22412 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     5280 2024-04-18 11:33:11.400128 bpm_ai_core-2.4.2/bpm_ai_core/util/remote_object.py
--rw-r--r--   0        0        0     2596 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      670 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/bpm_ai_core/util/text.py
--rw-r--r--   0        0        0      675 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1036 2024-04-18 11:33:11.404127 bpm_ai_core-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 bpm_ai_core-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/classification/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/classification/zero_shot_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     6753 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0     4929 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6142 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2674 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1459 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     8438 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     3397 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5669 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2789 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1631 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6420 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3086 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1463 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1188 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1486 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2894 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/token_classification/__init__.py
+-rw-r--r--   0        0        0      968 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4381 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2347 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1630 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      593 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     4125 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/caching.py
+-rw-r--r--   0        0        0     2290 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     6130 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     3135 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    22412 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     4278 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/rpc.py
+-rw-r--r--   0        0        0     2596 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      670 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/text.py
+-rw-r--r--   0        0        0      675 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1059 2024-04-24 14:39:08.476771 bpm_ai_core-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 bpm_ai_core-2.5.0/PKG-INFO
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/classification/zero_shot_classifier.py` & `bpm_ai_core-2.5.0/bpm_ai_core/classification/zero_shot_classifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 from pydantic import BaseModel
 
 from bpm_ai_core.tracing.decorators import span
+from bpm_ai_core.util.caching import cached
 
 
 class ClassificationResult(BaseModel):
     max_label: str
     max_score: float
     labels_scores: list[Tuple[str, float]]
 
@@ -23,14 +24,15 @@
             text: str,
             classes: list[str],
             hypothesis_template: str | None = None,
             multi_label: bool = False
     ) -> ClassificationResult:
         pass
 
+    @cached()
     @span(name="classifier")
     async def classify(
             self,
             text: str,
             classes: list[str],
             confidence_threshold: float | None = None,
             hypothesis_template: str | None = None,
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from anthropic import AsyncAnthropic
 
     _clients: ContextVar[dict[str, AsyncAnthropic]] = ContextVar('anthropic_clients', default={})
 except ImportError:
     pass
 
 
-def get_anthropic_client(endpoint: str = None, api_key: str = None) -> AsyncAnthropic:
+def get_anthropic_client(endpoint: str = None, api_key: str = None) -> "AsyncAnthropic":
     client_map = _clients.get()
     hash_key = hashlib.sha256(((endpoint or "default") + (api_key or "default")).encode()).hexdigest()
     if hash_key in client_map.keys():
         return client_map[hash_key]
     else:
         client = AsyncAnthropic(
             base_url=endpoint,
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 from bpm_ai_core.llm.anthropic_chat.util import messages_to_anthropic_dicts, json_schema_to_anthropic_tool, \
     tool_calls_to_tool_message
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.llm.common.message import ChatMessage, ToolCallMessage, AssistantMessage, SystemMessage
 from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.tracing.tracing import Tracing
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.json_schema import expand_simplified_json_schema
 
 logger = logging.getLogger(__name__)
 
 try:
     from anthropic import AsyncAnthropic, RateLimitError, InternalServerError, APIConnectionError
     from anthropic.types import Message, TextBlock
     from anthropic.types.beta.tools import ToolUseBlock, ToolsBetaMessage
 
     has_anthropic = True
 except ImportError:
     has_anthropic = False
 
 
+@cachable(
+    exclude_key_params=["max_retries", "client"]
+)
 class ChatAnthropic(LLM):
     """
     `Anthropic` Chat large language models API.
 
     To use, you should have the ``anthropic`` python package installed, and the
     environment variable ``ANTHROPIC_API_KEY`` set with your API key.
     """
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
                 filename = (" name='" + e.path + "'") if e.path else ''
                 text = f"<file{filename}>\n{text}\n</file>"
                 content.append(str_to_anthropic_text_dict(text))
             else:
                 raise ValueError(
                     "Elements in ChatMessage.content must be str or Blob (image/pdf/text)"
                 )
+    elif message.content is None:
+        content = None
     else:
         content = None
         logger.warning(
             "ChatMessage.content must be of type str or List[Union[str, PIL.Image]] if used for chat completions."
         )
     return {
         "role": message.role,
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/blob.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     """Location where the original content was found."""
 
     metadata: Dict[str, Any] = Field(default_factory=dict)
     """Metadata about the blob (e.g., source)"""
 
     class Config:
         arbitrary_types_allowed = True
-        frozen = True
 
     @property
     def source(self) -> Optional[str]:
         """The source location of the blob as string if known otherwise none.
 
         If a path is associated with the blob, it will default to the path location.
 
@@ -81,28 +80,29 @@
         ]
         return (self.mimetype.startswith("text/") or self.mimetype in app_text_mimetypes) if self.mimetype else False
 
     async def as_bytes(self) -> bytes:
         """Read data as bytes."""
         if self.data is None and (self.path.startswith('http://') or self.path.startswith('https://')):
             response = requests.get(self.path)
-            return response.content
+            self.data = response.content
         elif self.data is None and is_s3_url(self.path):
-            return await read_file_from_s3(self.path)
+            self.data = await read_file_from_s3(self.path)
         elif self.data is None and is_azure_blob_url(self.path):
-            return await read_file_from_azure_blob(self.path)
+            self.data = await read_file_from_azure_blob(self.path)
         elif isinstance(self.data, bytes):
-            return self.data
+            pass
         elif isinstance(self.data, str):
-            return self.data.encode("utf-8")
+            self.data = self.data.encode("utf-8")
         elif self.data is None and self.path:
             with open(str(self.path), "rb") as f:
-                return f.read()
+                self.data = f.read()
         else:
             raise ValueError(f"Unable to get bytes for blob {self}")
+        return self.data
 
     async def as_bytes_io(self) -> BytesIO:
         return BytesIO(await self.as_bytes())
 
     @classmethod
     def from_path_or_url(
             cls,
@@ -142,15 +142,14 @@
             metadata=metadata if metadata is not None else {},
         )
 
     @classmethod
     def from_data(
             cls,
             data: Union[str, bytes],
-            *,
             mime_type: str,
             path: Optional[str] = None,
             metadata: Optional[dict] = None,
     ) -> "Blob":
         """Initialize the blob from in-memory data.
 
         Args:
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import logging
 from abc import abstractmethod, ABC
 from typing import Any, Type
 
-from tenacity import stop_after_attempt, wait_exponential, retry_if_exception_type, Retrying
+from tenacity import stop_after_attempt, wait_exponential, retry_if_exception_type, Retrying, before_sleep_log
 
 from bpm_ai_core.llm.common.message import ChatMessage, AssistantMessage
 from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.tracing.tracing import Tracing
+from bpm_ai_core.util.caching import cached
+
+logger = logging.getLogger(__name__)
 
 
 class LLM(ABC):
     """
     Abstract class for large language models.
     """
 
@@ -22,14 +26,15 @@
         retryable_exceptions: list[Type[BaseException]] = None
     ):
         self.model = model
         self.temperature = temperature
         self.max_retries = max_retries
         self.retryable_exceptions = retryable_exceptions or [Exception]
 
+    @cached(disable_if="self.temperature > 0")
     async def generate_message(
         self,
         prompt: Prompt | list[ChatMessage],
         output_schema: dict[str, Any] = None,
         tools: list[Tool] = None,
         stop: list[str] = None
     ) -> AssistantMessage:
@@ -39,15 +44,16 @@
         messages = prompt if isinstance(prompt, list) else prompt.format(llm_name=self.name())
 
         Tracing.tracers().start_span(self.model, inputs={"messages": messages, "output_schema": output_schema, "tools": tools})
 
         for attempt in Retrying(
             wait=wait_exponential(multiplier=1.5, min=2, max=60),
             stop=stop_after_attempt(self.max_retries),
-            retry=retry_if_exception_type(tuple(self.retryable_exceptions))
+            retry=retry_if_exception_type(tuple(self.retryable_exceptions)),
+            before_sleep=before_sleep_log(logger, logging.ERROR),
         ):
             with attempt:
                 completion = await self._generate_message(messages, output_schema, tools, stop, attempt.retry_state.attempt_number)
 
         Tracing.tracers().end_span(outputs=completion.model_dump())
         return completion
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     from openai.lib.azure import AsyncAzureOpenAI
 
     _clients: ContextVar[dict[str, AsyncOpenAI]] = ContextVar('openai_clients', default={})
 except ImportError:
     pass
 
 
-def get_openai_client(endpoint: str = None, api_key: str = None) -> AsyncOpenAI:
+def get_openai_client(endpoint: str = None, api_key: str = None) -> "AsyncOpenAI":
     client_map = _clients.get()
     hash_key = hashlib.sha256(((endpoint or "default") + (api_key or "default")).encode()).hexdigest()
     if hash_key in client_map.keys():
         return client_map[hash_key]
     else:
         client = AsyncOpenAI(
             base_url=endpoint,
             api_key=api_key,
             **default_client_kwargs
         )
         client_map[hash_key] = client
         return client
 
 
-def get_azure_openai_client(azure_endpoint: str, api_version: str, api_key: str) -> AsyncOpenAI:
+def get_azure_openai_client(azure_endpoint: str, api_version: str, api_key: str) -> "AsyncOpenAI":
     client_map = _clients.get()
     hash_key = hashlib.sha256((azure_endpoint + api_key).encode()).hexdigest()
     if hash_key in client_map.keys():
         return client_map[hash_key]
     else:
         client = AsyncAzureOpenAI(
             azure_endpoint=azure_endpoint,
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 from bpm_ai_core.llm.common.message import ChatMessage, ToolCallMessage, AssistantMessage
 from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.llm.openai_chat import get_openai_client, get_azure_openai_client
 from bpm_ai_core.llm.openai_chat._constants import DEFAULT_MODEL, DEFAULT_TEMPERATURE, DEFAULT_SEED, \
     DEFAULT_MAX_RETRIES, AZURE_API_KEY_ENV_VAR, OPENAI_COMPATIBLE_API_KEY_ENV_VAR
 from bpm_ai_core.llm.openai_chat.util import messages_to_openai_dicts, json_schema_to_openai_function
 from bpm_ai_core.tracing.tracing import Tracing
+from bpm_ai_core.util.caching import cachable
 
 logger = logging.getLogger(__name__)
 
 try:
     from openai import AsyncOpenAI, APIConnectionError, InternalServerError, RateLimitError, OpenAIError
     from openai.types.chat import ChatCompletionMessage as OpenAIChatCompletionMessage, ChatCompletion
     from openai.lib.azure import AsyncAzureOpenAI
 
     has_openai = True
 except ImportError:
     has_openai = False
 
 
+@cachable(
+    exclude_key_params=["max_retries", "client"]
+)
 class ChatOpenAI(LLM):
     """
     `OpenAI` Chat large language models API.
     Also used for Azure OpenAI and other compatible servers.
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
@@ -121,14 +125,33 @@
             client=get_azure_openai_client(
                 azure_endpoint=azure_endpoint,
                 api_version=api_version,
                 api_key=api_key
             )
         )
 
+    @classmethod
+    def for_groq(
+        cls,
+        model: str = "llama3-70b-8192",
+        temperature: float = DEFAULT_TEMPERATURE,
+        seed: Optional[int] = DEFAULT_SEED,
+        max_retries: int = DEFAULT_MAX_RETRIES,
+    ):
+        return cls(
+            model=model,
+            temperature=temperature,
+            seed=seed,
+            max_retries=max_retries,
+            client=get_openai_client(
+                endpoint="https://api.groq.com/openai/v1",
+                api_key=os.environ["GROQ_API_KEY"]
+            )
+        )
+
     async def _generate_message(
         self,
         messages: List[ChatMessage],
         output_schema: Optional[Dict[str, Any]] = None,
         tools: Optional[List[Tool]] = None,
         stop: list[str] = None,
         current_try: int = None
@@ -180,15 +203,15 @@
             description=output_schema.pop("description", None) or "Stores your result",
             args_schema=output_schema
         )
 
     @staticmethod
     def _openai_tool_calls_to_tool_message(message: OpenAIChatCompletionMessage, tools: List[Tool]) -> AssistantMessage:
         return AssistantMessage(
-            name=", ".join([t.function.name for t in message.tool_calls]),
+            #name=", ".join([t.function.name for t in message.tool_calls]),
             content=message.content,
             tool_calls=[
                 ToolCallMessage(
                     id=t.id,
                     name=t.function.name,
                     payload=t.function.arguments,
                     tool=next((item for item in tools if item.name == t.function.name), None)
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/llm/openai_chat/util.py` & `bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,16 @@
                 filename = (" name='" + e.path + "'") if e.path else ''
                 text = f"<file{filename}>\n{text}\n</file>"
                 content.append(str_to_openai_text_dict(text))
             else:
                 raise ValueError(
                     "Elements in ChatMessage.content must be str or Blob (image/pdf/text)"
                 )
+    elif message.content is None:
+        content = None
     else:
         content = None
         logger.warning(
             "ChatMessage.content must be of type str or List[Union[str, PIL.Image]] if used for chat completions."
         )
     return {
         "role": message.role,
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.5.0/bpm_ai_core/ocr/amazon_textract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import asyncio
 
 from typing_extensions import override
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.ocr.ocr import OCR, OCRResult, OCRPage
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.image import blob_as_images
 from bpm_ai_core.util.storage import is_s3_url, parse_s3_url
 
 try:
     from aiobotocore.session import get_session
     from textractprettyprinter.t_pretty_print import get_text_from_layout_json
 
     has_textract = True
 except ImportError:
     has_textract = False
 
 IMAGE_FORMATS = ["png", "jpeg", "tiff"]
 
 
+@cachable()
 class AmazonTextractOCR(OCR):
     def __init__(self, region_name: str = None):
         if not has_textract:
             raise ImportError('aiobotocore and/or amazon-textract-prettyprinter are not installed')
         self.region_name = region_name
 
     @override
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.5.0/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from io import BytesIO
 
 from typing_extensions import override
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.ocr.ocr import OCR, OCRResult, OCRPage
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.image import blob_as_images
 
 try:
     from azure.ai.documentintelligence.aio import DocumentIntelligenceClient as AsyncDocumentIntelligenceClient
     from azure.core.credentials import AzureKeyCredential
 
     has_azure_doc = True
@@ -18,14 +19,15 @@
 
 azure_logger = logging.getLogger('azure')
 azure_logger.setLevel(logging.WARNING)
 
 IMAGE_FORMATS = ["png", "jpeg", "tiff"]
 
 
+@cachable()
 class AzureOCR(OCR):
     def __init__(self, endpoint: str = None):
         if not has_azure_doc:
             raise ImportError('azure-ai-documentintelligence is not installed')
         self.endpoint = endpoint or os.environ.get("AZURE_DOCUMENT_INTELLIGENCE_ENDPOINT")
 
     @override
@@ -55,25 +57,25 @@
             )
 
             # Wait for the extraction to complete asynchronously
             result = await document.result()
             markdown_content = result.content
 
             pages = []
-            for page in result.pages:
+            for i, page in enumerate(result.pages):
                 bboxes = []
                 words = []
                 for word in page.words:
                     polygon = word.polygon
                     x, y = polygon[0], polygon[1]
                     w, h = polygon[2] - x, polygon[5] - y
                     bboxes.append((x / page['width'], y / page['height'], (x + w) / page['width'], (y + h) / page['height']))
                     words.append(word.content)
 
                 page_data = OCRPage(
-                    text=" ".join(words),
+                    text=markdown_content if i == 0 else "",
                     words=words,
                     bboxes=bboxes
                 )
                 pages.append(page_data)
 
         return OCRResult(pages=pages)
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.5.0/bpm_ai_core/ocr/ocr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 from pydantic import BaseModel, Field
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.tracing.decorators import span
+from bpm_ai_core.util.caching import cached, calculate_cache_key
 
 
 class OCRPage(BaseModel):
     text: str
     words: list[str] = Field(..., exclude=True)
     bboxes: list[Tuple[float, float, float, float]] = Field(..., exclude=True)
     """Format: (x, y, x + w, y + h), normalized to 1"""
@@ -31,14 +32,22 @@
     async def _do_process(
             self,
             blob: Blob,
             language: str = None
     ) -> OCRResult:
         pass
 
+    async def _cache_key(self, blob_or_path: Blob | str, *args, **kwargs) -> str:
+        if isinstance(blob_or_path, str):
+            blob = Blob.from_path_or_url(blob_or_path)
+        else:  # Blob
+            blob = blob_or_path
+        return f"blob_bytes={await blob.as_bytes()}"
+
+    @cached(exclude=["blob_or_path"], key_func=_cache_key)
     @span(name="ocr")
     async def process(
             self,
             blob_or_path: Blob | str,
             language: str = None
     ) -> OCRResult:
         if isinstance(blob_or_path, str):
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.5.0/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.5.0/bpm_ai_core/prompt/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -135,7 +135,10 @@
         default_path = f"{path}.prompt"
         llm_specific_path = f"{path}.{llm_name}.prompt"
         filename = llm_specific_path if os.path.exists(llm_specific_path) else default_path
         if not os.path.exists(filename):
             raise FileNotFoundError(f"No prompt file found at {filename}")
         with open(filename, 'r') as f:
             return Template(f.read())
+
+    def __repr__(self):
+        return f"{self.__class__.__qualname__}(template_vars={self.template_vars}, path={self.path}, template_str={self.template_str})"
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.5.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import logging
 
 from typing_extensions import override
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering, QAResult
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.image import blob_as_images
 
 try:
     from aiobotocore.session import get_session
 
     has_textract = True
 except ImportError:
     has_textract = False
 
 logger = logging.getLogger(__name__)
 
 IMAGE_FORMATS = ["png", "jpeg", "tiff"]
 
 
+@cachable()
 class AmazonTextractDocVQA(QuestionAnswering):
     """
 
     """
     def __init__(self, region_name: str = None):
         if not has_textract:
             raise ImportError('aiobotocore is not installed')
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.5.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 from io import BytesIO
 
 from typing_extensions import override
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering, QAResult
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.image import blob_as_images
 from bpm_ai_core.util.linguistics import stopwords
 
 try:
     from azure.ai.documentintelligence.aio import DocumentIntelligenceClient as AsyncDocumentIntelligenceClient
     from azure.ai.documentintelligence.models import DocumentAnalysisFeature
     from azure.core.credentials import AzureKeyCredential
@@ -23,14 +24,15 @@
 azure_logger.setLevel(logging.WARNING)
 
 logger = logging.getLogger(__name__)
 
 IMAGE_FORMATS = ["png", "jpeg", "tiff"]
 
 
+@cachable()
 class AzureDocVQA(QuestionAnswering):
     def __init__(self, endpoint: str = None):
         if not has_azure_doc:
             raise ImportError('azure-ai-documentintelligence is not installed')
         self.endpoint = endpoint or os.environ.get("AZURE_DOCUMENT_INTELLIGENCE_ENDPOINT")
 
     @override
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.5.0/bpm_ai_core/question_answering/question_answering.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 
 from pydantic import BaseModel
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.tracing.decorators import span
+from bpm_ai_core.util.caching import cached, calculate_cache_key
 
 
 class QAResult(BaseModel):
     answer: str | None
     score: float
     start_index: int | None
     end_index: int | None
@@ -16,26 +17,33 @@
 class QuestionAnswering(ABC):
     """
     (Extractive) Question Answering Model
     """
 
     @abstractmethod
     async def _do_answer(
-            self,
-            context_str_or_blob: str | Blob,
-            question: str
+        self,
+        context_str_or_blob: str | Blob,
+        question: str
     ) -> QAResult:
         pass
 
+    async def _cache_key(self, context_str_or_blob: str | Blob, *args, **kwargs) -> str:
+        if isinstance(context_str_or_blob, str):
+            return f"context={context_str_or_blob}"
+        else:  # Blob
+            return f"blob_bytes={await context_str_or_blob.as_bytes()}"
+
+    @cached(exclude=["context_str_or_blob"])
     @span(name="qa")
     async def answer(
-            self,
-            context_str_or_blob: str | Blob,
-            question: str,
-            confidence_threshold: float | None = 0.1
+        self,
+        context_str_or_blob: str | Blob,
+        question: str,
+        confidence_threshold: float | None = 0.1
     ) -> QAResult | None:
         result = await self._do_answer(
             context_str_or_blob=context_str_or_blob,
             question=question
         )
         # Only return the answer if the score is above the threshold (if given)
         return result \
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/asr.py` & `bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/asr.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,28 +2,37 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Union
 
 from pydantic import BaseModel
 
 from bpm_ai_core.tracing.decorators import span
 from bpm_ai_core.util.audio import load_audio
+from bpm_ai_core.util.caching import cached
+
 
 class ASRResult(BaseModel):
     text: str
 
 
 class ASRModel(ABC):
     """
     Automatic Speech Recognition (ASR) model for transcribing audio.
     """
 
     @abstractmethod
     async def _do_transcribe(self, audio: io.BytesIO, language: Optional[str] = None) -> ASRResult:
         pass
 
+    async def _cache_key(self, audio_or_path: io.BytesIO | str, *args, **kwargs) -> str:
+        if isinstance(audio_or_path, str):
+            return f"path={audio_or_path}"
+        else:  # BytesIO
+            return f"audio_bytes={audio_or_path.getvalue()}"
+
+    @cached(exclude=["audio_or_path"], key_func=_cache_key)
     @span(name="asr")
-    async def transcribe(self, audio_or_path: Union[io.BytesIO, str], language: Optional[str] = None) -> ASRResult:
+    async def transcribe(self, audio_or_path: io.BytesIO | str, language: Optional[str] = None) -> ASRResult:
         if isinstance(audio_or_path, str):
             audio = load_audio(audio_or_path)
         else:
             audio = audio_or_path
         return await self._do_transcribe(audio, language)
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import io
 import logging
 from typing import Optional
 
 from typing_extensions import override
 
 from bpm_ai_core.speech_recognition.asr import ASRModel, ASRResult
+from bpm_ai_core.util.caching import cachable
 
 logger = logging.getLogger(__name__)
 
 try:
     from openai import AsyncOpenAI, OpenAIError
     import httpx
 
@@ -21,14 +22,15 @@
         )
     except OpenAIError as e:
         logger.error(e)
 except ImportError:
     has_openai = False
 
 
+@cachable()
 class OpenAIWhisperASR(ASRModel):
     """
     `OpenAI` Whisper Automatic Speech Recognition (ASR) API for transcribing audio.
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
     """
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.5.0/bpm_ai_core/testing/fake_llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/token_classification/zero_shot_token_classifier.py` & `bpm_ai_core-2.5.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import ABC, abstractmethod
 
 from pydantic import BaseModel
 
+from bpm_ai_core.util.caching import cached
+
 
 class TokenSpan(BaseModel):
     label: str
     score: float
     word: str
     start: int
     end: int
@@ -25,14 +27,15 @@
             self,
             text: str,
             classes: list[str],
             confidence_threshold: float | None = None
     ) -> TokenClassificationResult:
         pass
 
+    @cached()
     async def classify(
             self,
             text: str,
             classes: list[str],
             confidence_threshold: float | None = None
     ) -> TokenClassificationResult:
         return await self._do_classify(
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.5.0/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.5.0/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.5.0/bpm_ai_core/tracing/langfuse.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.5.0/bpm_ai_core/tracing/logging.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.5.0/bpm_ai_core/translation/amazon_translate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import asyncio
 from typing import List
 
 from typing_extensions import override
 
 from bpm_ai_core.translation.nmt import NMTModel
+from bpm_ai_core.util.caching import cachable
 
 try:
     from aiobotocore.session import get_session
 
     has_amazon_translate = True
 except ImportError:
     has_amazon_translate = False
 
 
+@cachable()
 class AmazonTranslate(NMTModel):
     """Amazon Translate NMT Model"""
     def __init__(self, region_name: str = None):
         if not has_amazon_translate:
             raise ImportError("aiobotocore is not installed")
         self.region_name = region_name
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.5.0/bpm_ai_core/translation/azure_translation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import logging
 import os
 
 from typing_extensions import override
 
 from bpm_ai_core.translation.nmt import NMTModel
+from bpm_ai_core.util.caching import cachable
 
 try:
     from azure.ai.translation.text import TranslatorCredential
     from azure.ai.translation.text.aio import TextTranslationClient
     from azure.ai.translation.text.models import InputTextItem
 
     has_azure_translation = True
 except ImportError:
     has_azure_translation = False
 
 azure_logger = logging.getLogger('azure')
 azure_logger.setLevel(logging.WARNING)
 
 
+@cachable()
 class AzureTranslation(NMTModel):
     """Azure Text Translation NMT Model"""
 
     def __init__(self, endpoint: str = None, region: str = "westeurope"):
         if not has_azure_translation:
             raise ImportError('azure-ai-translation-text  is not installed')
         self.key = os.getenv('AZURE_TRANSLATION_KEY')
```

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/file.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/file.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/image.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/image.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/json_schema.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/json_schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/linguistics.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/text.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/text.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.5.0/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.4.2/pyproject.toml` & `bpm_ai_core-2.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.4.2"
+version = "2.5.0"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
@@ -15,27 +15,28 @@
 pydantic = "^2.6.4"
 pillow = "^10.1.0"
 pdf2image = "^1.17.0"
 requests = "^2.31.0"
 xmltodict = "^0.13.0"
 aiohttp = "^3.9.3"
 pypdfium2 = "^4.29.0"
+diskcache = "^5.6.3"
+psutil = "^5.9.8"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.5"
 pytest-dotenv = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
 openai = "^1.11.0"
 anthropic = "^0.23.1"
 mistralai = "^0.1.3"
 langfuse = "^2.7.6"
-pyro5 = "^5.15"
 amazon-textract-prettyprinter = "^0.1.9"
 aiobotocore = "^2.12.1"
 azure-storage-blob = "^12.19.1"
 azure-ai-translation-text = "^1.0.0b1"
 azure-ai-documentintelligence = "^1.0.0b2"
```

### Comparing `bpm_ai_core-2.4.2/PKG-INFO` & `bpm_ai_core-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: bpm-ai-core
-Version: 2.4.2
+Version: 2.5.0
 Summary: Core AI abstractions and helpers.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pdf2image (>=1.17.0,<2.0.0)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pypdfium2 (>=4.29.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai
 Description-Content-Type: text/markdown
```


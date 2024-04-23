# Comparing `tmp/eidolon_ai_sdk-0.1.32.tar.gz` & `tmp/eidolon_ai_sdk-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.32.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.33.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.32.tar` & `eidolon_ai_sdk-0.1.33.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     2569 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/README.md
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2400 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3025 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2710 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0     1936 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/openai_whisper_agent.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1434 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2329 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2864 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3717 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    12914 2024-04-19 04:03:27.259571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1815 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     7743 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     9001 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      601 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      614 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      597 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      595 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      618 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4638 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2562 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     4062 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    13845 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     4680 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5762 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9430 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3591 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3962 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     2421 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      974 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    21705 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14172 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-04-19 04:03:27.263571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4902 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6521 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/logging.conf
--rw-r--r--   0        0        0     2030 2024-04-19 04:03:27.267571 eidolon_ai_sdk-0.1.32/pyproject.toml
--rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.32/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0     1311 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/audio_agent.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1434 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2329 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3717 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    12776 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     7743 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9079 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      618 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4638 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2562 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     7916 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     3718 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-04-23 22:56:56.156663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    13845 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4680 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5762 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9430 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3567 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     2421 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    21705 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14172 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4902 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6521 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-04-23 22:56:56.160663 eidolon_ai_sdk-0.1.33/logging.conf
+-rw-r--r--   0        0        0     2065 2024-04-23 22:57:19.392822 eidolon_ai_sdk-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.33/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.32/README.md` & `eidolon_ai_sdk-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/openai_whisper_agent.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/audio_agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 from typing import Annotated
 
 from fastapi import Body
 
 from eidolon_ai_client.events import FileHandle
 from eidolon_ai_sdk.agent.agent import AgentSpec, Agent, register_program
-from eidolon_ai_sdk.agent_os import AgentOS
-from eidolon_ai_sdk.cpu.llm.open_ai_speech import OpenAiSpeech
+from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.system.processes import ProcessDoc
 from eidolon_ai_sdk.system.reference_model import AnnotatedReference, Specable
 
 
 class AutonomousSpeechAgentSpec(AgentSpec):
-    speech_llm: AnnotatedReference[OpenAiSpeech]
+    speech_llm: AnnotatedReference[AudioUnit]
 
 
 class AutonomousSpeechAgent(Agent, Specable[AutonomousSpeechAgentSpec]):
-    speech_llm: OpenAiSpeech
+    speech_llm: AudioUnit
 
     def __init__(self, spec: AutonomousSpeechAgentSpec):
         super().__init__(spec=spec)
         self.speech_llm = self.spec.speech_llm.instantiate(processing_unit_locator=None)
         self.cpu = self.spec.cpu.instantiate()
 
     @register_program()
-    async def speech_to_text(self, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]):
-        process_id = audio.process_id
+    async def speech_to_text(self, process_id, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]):
         await ProcessDoc.set_delete_on_terminate(process_id, True)
-        file, metadata = await AgentOS.process_file_system.read_file(process_id, audio.file_id)
-        mimetype = "audio/wav"
-        if metadata and "mimetype" in metadata:
-            mimetype = metadata["mimetype"]
-        # audio = AudioSegment.from_file(file)
-        # # Convert to mp3
-        # audio_mp3 = audio.export("audio.mp3", format="mp3")
-
-        text = await self.speech_llm.speech_to_text(file, mimetype)
+        text = await self.speech_llm.speech_to_text(audio)
         return {"response": text}
 
     @register_program()
     async def text_to_speech(
-        self, process_id: str, text: Annotated[str, Body(description="The text to speak", embed=True)]
-    ) -> FileHandle:
-        audio_result = await self.speech_llm.text_to_speech(text)
-        file_id = await AgentOS.process_file_system.write_file(process_id, audio_result, {"mimetype": "audio/mpeg"})
-
-        return file_id
+        self, text: Annotated[str, Body(description="The text to speak", embed=True)]
+    ) -> str:
+        return await self.speech_llm.text_to_speech(text)
```

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 from eidolon_ai_sdk.util.schema_to_model import schema_to_model
 
 
 class ActionDefinition(BaseModel):
     name: str = "converse"
     description: Optional[str] = None
     user_prompt: str = "{{ body }}"
-    input_schema: dict = None
+    input_schema: Dict[str, dict] = {}
     output_schema: Union[Literal["str"], Dict[str, Any]] = "str"
     allow_file_upload: bool = False
     # allow all types for text, image, audio, word, pdf, json, etc
     supported_mime_types: List[str] = []  # an empty list means all types are supported
     allowed_states: List[str] = ["initialized", "idle", "http_error"]
     output_state: str = "idle"
 
     @field_validator("input_schema")
     def validate_prompt_properties(cls, input_dict):
         if not isinstance(input_dict, dict):
-            raise ValueError("prompt_properties must be a dict")
+            raise ValueError("input_schema must be a dict")
         for k, v in input_dict.items():
             if isinstance(v, dict):
                 if v.get("format") == "binary":
-                    raise ValueError("prompt_properties cannot contain format = 'binary' fields.")
+                    raise ValueError("input_schema cannot contain format = 'binary' fields.")
         return input_dict
 
     @field_validator("supported_mime_types")
     def validate_supported_mime_types(cls, supported_mime_types):
         if not isinstance(supported_mime_types, list):
             raise ValueError("supported_mime_types must be a List[str]")
         if not supported_mime_types:
@@ -76,22 +76,19 @@
     def make_input_schema(self, agent, handler):
         properties: Dict[str, Any] = {}
         required = []
         user_vars = meta.find_undeclared_variables(Environment().parse(self.user_prompt))
         # pop out any reserved keywords we will inject
         if "datetime_iso" in user_vars:
             user_vars.remove("datetime_iso")
-        if self.input_schema is not None:
-            properties["body"] = dict(type="object", properties=self.input_schema)
-            required.append("body")
-        elif len(user_vars) == 1 and "body" in user_vars and not agent.spec.apus and not self.allow_file_upload:
+        if len(user_vars) == 1 and "body" in user_vars and not agent.spec.apus and not self.allow_file_upload:
             properties["body"] = dict(type="string", default=Body(..., media_type="text/plain"))
             required.append("body")
         elif user_vars:
-            props = {v: dict(type="string") for v in user_vars}
+            props = {v: self.input_schema.get(v, dict(type="string")) for v in user_vars}
             properties["body"] = dict(type="object", properties=props)
             required.append("body")
 
         if self.allow_file_upload:
             properties["body"]["properties"]["attached_files"] = dict(type="array", items=FileHandle.model_json_schema())
 
         if agent.spec.apus:
```

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 from eidolon_ai_sdk.agent.doc_manager.loaders.filesystem_loader import FilesystemLoader
 from eidolon_ai_sdk.agent.doc_manager.loaders.github_loader import GitHubLoader
 from eidolon_ai_sdk.agent.doc_manager.parsers.auto_parser import AutoParser
 from eidolon_ai_sdk.agent.doc_manager.parsers.base_parser import DocumentParser
 from eidolon_ai_sdk.agent.doc_manager.transformer.auto_transformer import AutoTransformer
 from eidolon_ai_sdk.agent.doc_manager.transformer.document_transformer import DocumentTransformer
 from eidolon_ai_sdk.agent.generic_agent import GenericAgent
-from eidolon_ai_sdk.agent.openai_whisper_agent import AutonomousSpeechAgent
+from eidolon_ai_sdk.agent.audio_agent import AutonomousSpeechAgent
 from eidolon_ai_sdk.agent.retriever_agent.document_reranker import RAGFusionReranker, DocumentReranker
 from eidolon_ai_sdk.agent.retriever_agent.multi_question_transformer import MultiQuestionTransformer
 from eidolon_ai_sdk.agent.retriever_agent.question_transformer import QuestionTransformer
 from eidolon_ai_sdk.agent.retriever_agent.retriever import Retriever
 from eidolon_ai_sdk.agent.retriever_agent.retriever_agent import RetrieverAgent
 from eidolon_ai_sdk.agent.simple_agent import SimpleAgent
 from eidolon_ai_sdk.agent.tot_agent.checker import ToTChecker
 from eidolon_ai_sdk.agent.tot_agent.thought_generators import ThoughtGenerationStrategy, ProposePromptStrategy
 from eidolon_ai_sdk.agent.tot_agent.tot_agent import TreeOfThoughtsAgent
 from eidolon_ai_sdk.builtins.components.opentelemetry import OpenTelemetryManager, CustomSampler, NoopSpanExporter
 from eidolon_ai_sdk.builtins.components.usage import UsageMiddleware
 from eidolon_ai_sdk.builtins.logic_units.web_search import WebSearch, Browser, Search
 from eidolon_ai_sdk.cpu.agent_cpu import APU
 from eidolon_ai_sdk.cpu.agent_io import IOUnit
+from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.cpu.conversation_memory_unit import RawMemoryUnit
 from eidolon_ai_sdk.cpu.conversational_apu import ConversationalAPU
 from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.cpu.llm.anthropic_llm_unit import AnthropicLLMUnit
 from eidolon_ai_sdk.cpu.llm.mistral_llm_unit import MistralGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_connection_handler import OpenAIConnectionHandler, AzureOpenAIConnectionHandler
 from eidolon_ai_sdk.cpu.llm.open_ai_image_unit import OpenAIImageUnit
@@ -186,14 +187,15 @@
         RAGFusionReranker,
         (DocumentLoader, FilesystemLoader),
         DocumentProcessor,
         DocumentManager,
         FilesystemLoader,
         GitHubLoader,
         ToTChecker,
+        (AudioUnit, OpenAiSpeech),
         OpenAiSpeech,
         AsyncOpenAI,
         AsyncAzureOpenAI,
         UsageClient,
         OpenAIConnectionHandler,
         AzureOpenAIConnectionHandler,
         OpenAIImageUnit,
```

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,32 @@
 from typing import Optional, Literal
 
-from pydantic import BaseModel
-
 from eidolon_ai_client.events import FileHandle
 from eidolon_ai_client.util.request_context import RequestContext
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.cpu.logic_unit import LogicUnit, llm_function
-from eidolon_ai_sdk.system.reference_model import Specable
-
-
-class AudioUnitSpec(BaseModel):
-    pass
-
 
-class AudioUnit(LogicUnit, Specable[AudioUnitSpec]):
-    def __init__(self, spec: AudioUnitSpec = None, **kwargs):
-        super().__init__(**kwargs)
-        self.spec = spec
 
+class AudioUnit(LogicUnit):
     @llm_function()
     async def text_to_speech(self, text: str, response_format: Literal["mp3", "opus", "aac", "flac", "wav", "pcm"] = "mp3") -> str:
         """
         Converts text to speech. The result of the call is a file handle that should be returned to the user unchanged.
 
         Args:
             text (str): The text to convert to speech.
 
         Returns:
             FileHandle: A file handle that contains the audio data.
             :param text:
             :param response_format: Response audio format. Legal values are ["mp3", "opus", "aac", "flac", "wav", "pcm"].  Defaults to "mp3".
         """
         audio = await self._text_to_speech(text, response_format)
-        file_handle = await AgentOS.process_file_system.write_file(RequestContext.get("process_id"), audio, {"mimetype": f"audio/{response_format}"})
-        return f"{file_handle.machineURL}/processes/{file_handle.process_id}/files/{file_handle.file_id}"
+        handle = await AgentOS.process_file_system.write_file(RequestContext.get("process_id"), audio, {"mimetype": f"audio/{response_format}"})
+        return handle.get_url()
 
     async def _text_to_speech(self, text: str, response_format: Literal["mp3", "opus", "aac", "flac", "wav", "pcm"] = "mp3") -> bytes:
         """
         Converts text to speech.
 
         Args:
             text (str): The text to convert to speech.
@@ -63,15 +52,15 @@
         Returns:
             str: The result of the conversion
             :param audio: A file handle to the audio data.
             :param prompt: An optional text to guide the model's style or continue a previous audio segment. Defaults to the built-in prompt.
             :param language: The language of the input audio. Supplying the input language in ISO-639-1 format will improve accuracy and latency. This parameter is optional.
         """
         audio_data, metadata = await AgentOS.process_file_system.read_file(RequestContext.get("process_id"), audio.file_id)
-        return await self._speech_to_text(audio_data, metadata["mimetype"], prompt, language)
+        return await self._speech_to_text(audio_data, metadata.get("mimetype", "audio/wav"), prompt, language)
 
     async def _speech_to_text(
         self, audio: bytes, mime_type: str, prompt: Optional[str] = None, language: Optional[str] = None
     ) -> str:
         """
         Converts speech to text.
```

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional, Literal
 
 from openai import AsyncOpenAI
-from pydantic import Field
+from pydantic import Field, BaseModel
 
-from eidolon_ai_sdk.cpu.audio_unit import AudioUnit, AudioUnitSpec
+from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
-class OpenAiSpeechSpec(AudioUnitSpec):
+class OpenAiSpeechSpec(BaseModel):
     text_to_speech_model: Literal["tts-1", "tts-1-hd"] = Field(
         default="tts-1-hd", description="The model to use for text to speech."
     )
     text_to_speech_voice: Literal["alloy", "echo", "fable", "onyx", "nova", "shimmer"] = Field(
         default="alloy", description="The voice to use for text to speech."
     )
     speech_to_text_model: Literal["whisper-1"] = Field(
@@ -25,16 +25,16 @@
 
 class OpenAiSpeech(AudioUnit, Specable[OpenAiSpeechSpec]):
     model: str
     temperature: float
     llm: AsyncOpenAI = None
 
     def __init__(self, spec: OpenAiSpeechSpec, **kwargs):
-        super().__init__(spec, **kwargs)
-        Specable.__init__(self, spec, **kwargs)
+        super().__init__(**kwargs)
+        Specable.__init__(self, spec)
 
     async def _text_to_speech(self, text: str, response_format: str = "mp3") -> bytes:
         """
         Converts text to speech.
 
         Args:
             text (str): The text to convert to speech.
```

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.33/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/logging.conf` & `eidolon_ai_sdk-0.1.33/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.32/pyproject.toml` & `eidolon_ai_sdk-0.1.33/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.32"
+version = "0.1.33"
 description = "An Open Source Agent Services Framework"
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 include = ["logging.conf"]
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
@@ -72,7 +72,10 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = "project"
 
 [tool.ruff]
 line-length = 121
+
+[tool.eidolon]
+update-tag = "sdk"
```

### Comparing `eidolon_ai_sdk-0.1.32/PKG-INFO` & `eidolon_ai_sdk-0.1.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.32
+Version: 0.1.33
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
```


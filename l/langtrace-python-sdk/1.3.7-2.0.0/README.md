# Comparing `tmp/langtrace_python_sdk-1.3.7.tar.gz` & `tmp/langtrace_python_sdk-2.0.0.tar.gz`

## Comparing `langtrace_python_sdk-1.3.7.tar` & `langtrace_python_sdk-2.0.0.tar`

### file list

```diff
@@ -1,99 +1,107 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/__init__.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/cohere_example/embed_create.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/chat_completion.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/embeddings_create.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/function_calling.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/images_generate.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/openai/tool_calling_streaming.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    34590 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/__init__.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/LICENSE
--rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/README.md
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    36773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/conftest.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/LICENSE
+-rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/PKG-INFO
```

### Comparing `langtrace_python_sdk-1.3.7/src/run_example.py` & `langtrace_python_sdk-2.0.0/src/run_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,56 @@
-# from examples.langchain_example.basic import basic, load_and_split, rag
-
-
-# from examples.openai.chat_completion import chat_completion
 
-# from examples.openai import images_generate
-# from examples.openai.function_calling import function_calling
-# from examples.openai.tool_calling_nonstreaming import run_conversation
-# from examples.openai.async_tool_calling_nonstreaming import run_conversation
-
-# from examples.openai.tool_calling_streaming import run_conversation
-from examples.openai.async_tool_calling_streaming import run_conversation
+# Cohere
+# from examples.cohere_example.chat import chat_comp
+# from examples.cohere_example.chat_stream import chat_stream
+# from examples.cohere_example.tools import tool_calling
+# from examples.cohere_example.embed import embed
+from examples.cohere_example.rerank import rerank
+
+# OpenAI
+
+# from examples.openai_example.tool_calling import tool_calling
+# from examples.openai_example.chat_completion import chat_completion
+# from examples.openai_example.images_generate import images_generate
+# from examples.openai_example.embeddings_create import embeddings_create
+# from examples.openai_example.function_calling import function_calling
+# from examples.openai_example.tool_calling_nonstreaming import run_conversation
+# from examples.openai_example.async_tool_calling_nonstreaming import run_conversation
+# from examples.openai_example.tool_calling_streaming import run_conversation
+# from examples.openai.async_tool_calling_streaming import run_conversation
+# for async functions, use asyncio.run()
+# import asyncio
 
+# Anthropic
 # from examples.anthropic_example.completion import messages_create
 
+# Rest
+# from examples.langchain_example.basic import basic, load_and_split, rag
 # from examples.pinecone_example.basic import basic
 # from examples.chroma_example.basic import basic
 # from examples.llamaindex_example.basic import basic
 # from examples.langchain_example.basic import basic
-# from examples.cohere_example.chat import chat_comp
-# from examples.cohere_example.embed_create import embed_create
 # from examples.hiveagent_example.basic import basic
-
-# from examples.cohere_example.chat_stream import chat_stream
-
 # from examples.perplexity_example.basic import basic
 
-# load_and_split()
-# rag()
-# basic()
+# OpenAI
+# tool_calling()
 # chat_completion()
-# function_calling()
 # images_generate()
 # embeddings_create()
+# function_calling()
+# run_conversation()
+# asyncio.run(run_conversation())
+
+# Anthropic
 # messages_create()
+
+# Cohere
 # chat_comp()
-# embed_create()
 # chat_stream()
+# tool_calling()
+# embed()
+rerank()
 
-# for async functions, use asyncio.run()
-import asyncio
-asyncio.run(run_conversation())
-
-# run_conversation()
+# load_and_split()
+# rag()
+# basic()
```

### Comparing `langtrace_python_sdk-1.3.7/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.0.0/src/examples/anthropic_example/completion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Example of using the anthropic API to create a message."""
 
 import anthropic
 from dotenv import find_dotenv, load_dotenv
 
-from langtrace_python_sdk import langtrace
-from langtrace_python_sdk import with_langtrace_root_span
+from langtrace_python_sdk import langtrace, with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
 langtrace.init(write_to_langtrace_cloud=False)
 
+
 @with_langtrace_root_span("messages_create")
 def messages_create():
 
     client = anthropic.Anthropic()
 
     message = client.messages.create(
         model="claude-3-opus-20240229",
         max_tokens=1000,
         temperature=0.0,
         system="Respond only in Yoda-speak.",
         messages=[{"role": "user", "content": "How are you today?"}],
-        stream=False,
+        stream=True,
     )
 
-    print(message)
+    # print(message)
 
-    # for response in message:
-    #     pass
+    for response in message:
+        pass
```

### Comparing `langtrace_python_sdk-1.3.7/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.0.0/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.0.0/src/examples/cohere_example/chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from dotenv import find_dotenv, load_dotenv
 import cohere
+from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace
+
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
 langtrace.init(write_to_langtrace_cloud=False)
 
 co = cohere.Client()
@@ -14,13 +15,13 @@
 # @with_langtrace_root_span("chat_create")
 def chat_comp():
     response = co.chat(
         chat_history=[
             {"role": "USER", "message": "Who discovered gravity?"},
             {"role": "CHATBOT", "message": "The man who is widely credited with discovering gravity is Sir Isaac Newton"}
         ],
-        message="What is today's news?",
-        # preamble="answer like yoda",
+        message="Tell me a story in 3 sentences or less?",
+        preamble="answer like a pirate",
         # perform web search before answering the question. You can also use your own custom connector.
-        # connectors=[{"id": "web-search"}]
+        connectors=[{"id": "web-search"}]
     )
     print(response)
```

### Comparing `langtrace_python_sdk-1.3.7/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.0.0/src/examples/cohere_example/embed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from dotenv import find_dotenv, load_dotenv
 import cohere
+from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace
 
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
 langtrace.init(write_to_langtrace_cloud=False)
 
 co = cohere.Client()
 
 
-# @with_langtrace_root_span("chat_stream")
-def chat_stream():
-    result = []
-    for event in co.chat_stream(message="Tell me a short story in 2 lines"):
-        if event.event_type == "text-generation":
-            result.append(event.text)
-        elif event.event_type == "stream-end":
-            break
-    print("".join(result))
-    return result
+# @with_langtrace_root_span("embed_create")
+def embed():
+    response = co.embed(
+        texts=["hello", "goodbye"],
+        model="embed-english-v3.0",
+        input_type="classification",
+    )
+    print(response)
+    return response
```

### Comparing `langtrace_python_sdk-1.3.7/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.0.0/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.0.0/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.0.0/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/openai/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/openai/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/openai/embeddings_create.py` & `langtrace_python_sdk-2.0.0/src/examples/perplexity_example/basic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from dotenv import find_dotenv, load_dotenv
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
-from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
+from langtrace_python_sdk.utils.with_root_span import (
+    with_additional_attributes,
+    with_langtrace_root_span,
+)
 
-_ = load_dotenv(find_dotenv())
+# _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=True, log_spans_to_console=True, write_to_remote_url=False)
-client = OpenAI()
+langtrace.init(write_to_langtrace_cloud=False)
+client = OpenAI(base_url="https://api.perplexity.ai", api_key="PPLX_API_KEY")
 
 
-@with_langtrace_root_span()
-def embeddings_create():
-    result = client.embeddings.create(
-        model="text-embedding-ada-002",
-        input="Once upon a time, there was a frog.",
+@with_additional_attributes({"user.id": "1234", "user.feedback.rating": 1})
+def basic():
+    response = client.chat.completions.create(
+        model="pplx-70b-online",
+        messages=[{"role": "user", "content": "What is the capital of France?"}],
+        stream=False,
     )
+    print(response)
+    return response
```

### Comparing `langtrace_python_sdk-1.3.7/src/examples/openai/function_calling.py` & `langtrace_python_sdk-2.0.0/src/examples/openai_example/function_calling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import json
+# import json
 
 from dotenv import find_dotenv, load_dotenv
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
-from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
 langtrace.init(write_to_langtrace_cloud=False)
 
 client = OpenAI()
 
@@ -30,28 +29,27 @@
                 },
             },
         },
     }
 ]
 
 
-# @with_langtrace_root_span()
 def function_calling():
     response = client.chat.completions.create(
         model="gpt-3.5-turbo",
         messages=[
             {
                 "role": "user",
-                "content": "David Nguyen is a sophomore majoring in computer science at Stanford University. He is Asian American and has a 3.8 GPA. David is known for his programming skills and is an active member of the university's Robotics Club. He hopes to pursue a career in artificial intelligence after graduating.",
+                "content": "John is a grad student in computer science at Stanford University. He is an American and has a 3.8 GPA. John is known for his programming skills and is an active member of the university's Robotics Club. He hopes to pursue a career in artificial intelligence after graduating.",
             }
         ],
         functions=student_custom_functions,
-        function_call="auto",
         stream=True,
     )
+    # return response
 
     result = []
     for chunk in response:
         if chunk.choices[0].delta.function_call is not None:
             content = [
                 choice.delta.function_call.arguments if choice.delta.function_call and
                 choice.delta.function_call.arguments else ""
```

### Comparing `langtrace_python_sdk-1.3.7/src/examples/openai/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 _ = load_dotenv(find_dotenv())
 
 langtrace.init(write_to_langtrace_cloud=False)
 
 client = OpenAI()
 
+
 # Example dummy function hard coded to return the same weather
 # In production, this could be your backend API or an external API
 def get_current_weather(location, unit="fahrenheit"):
     """Get the current weather in a given location"""
     if "tokyo" in location.lower():
         return json.dumps({"location": "Tokyo", "temperature": "10", "unit": unit})
     elif "san francisco" in location.lower():
@@ -85,8 +86,8 @@
                 }
             )  # extend conversation with function response
         second_response = client.chat.completions.create(
             model="gpt-3.5-turbo-0125",
             messages=messages,
         )  # get a new response from the model where it can see the function response
         # print(second_response)
-        return second_response
+        return second_response
```

### Comparing `langtrace_python_sdk-1.3.7/src/examples/openai/tool_calling_streaming.py` & `langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.0.0/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 """
-This module contains the patching logic for the Anthropic library."""
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
 
 import json
 
 from langtrace.trace_attributes import Event, LLMSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
@@ -54,32 +67,36 @@
             attributes.llm_temperature = kwargs.get("temperature")
         if kwargs.get("top_p") is not None:
             attributes.llm_top_p = kwargs.get("top_p")
         if kwargs.get("top_k") is not None:
             attributes.llm_top_p = kwargs.get("top_k")
         if kwargs.get("user") is not None:
             attributes.llm_user = kwargs.get("user")
+        if kwargs.get("max_tokens") is not None:
+            attributes.llm_max_tokens = str(kwargs.get("max_tokens"))
 
         span = tracer.start_span(
             APIS["MESSAGES_CREATE"]["METHOD"], kind=SpanKind.CLIENT
         )
         for field, value in attributes.model_dump(by_alias=True).items():
             if value is not None:
                 span.set_attribute(field, value)
         try:
             # Attempt to call the original method
             result = wrapped(*args, **kwargs)
             if kwargs.get("stream") is False:
                 if hasattr(result, "content") and result.content is not None:
+                    span.set_attribute("llm.model", result.model if result.model else kwargs.get("model"))
                     span.set_attribute(
                         "llm.responses",
                         json.dumps(
                             [
                                 {
-                                    "text": result.content[0].text,
+                                    "role": result.role if result.role else "assistant",
+                                    "content": result.content[0].text,
                                     "type": result.content[0].type,
                                 }
                             ]
                         ),
                     )
                 else:
                     responses = []
@@ -102,31 +119,33 @@
                         }
                         span.set_attribute("llm.token.counts", json.dumps(usage_dict))
                 span.set_status(StatusCode.OK)
                 span.end()
                 return result
             else:
                 return handle_streaming_response(result, span)
-        except Exception as e:
+        except Exception as err:
             # Record the exception in the span
-            span.record_exception(e)
+            span.record_exception(err)
             # Set the span status to indicate an error
-            span.set_status(Status(StatusCode.ERROR, str(e)))
+            span.set_status(Status(StatusCode.ERROR, str(err)))
             # Reraise the exception to ensure it's not swallowed
             span.end()
             raise
 
     def handle_streaming_response(result, span):
         """Process and yield streaming response chunks."""
         result_content = []
         span.add_event(Event.STREAM_START.value)
         input_tokens = 0
         output_tokens = 0
         try:
             for chunk in result:
+                if hasattr(chunk, "message") and chunk.message is not None and hasattr(chunk.message, "model") and chunk.message.model is not None:
+                    span.set_attribute("llm.model", chunk.message.model)
                 content = ""
                 if hasattr(chunk, "delta") and chunk.delta is not None:
                     content = chunk.delta.text if hasattr(chunk.delta, "text") else ""
                 # Assuming content needs to be aggregated before processing
                 result_content.append(content if len(content) > 0 else "")
 
                 if hasattr(chunk, "message") and hasattr(chunk.message, "usage"):
@@ -161,14 +180,15 @@
                         "input_tokens": input_tokens,
                         "output_tokens": output_tokens,
                         "total_tokens": input_tokens + output_tokens,
                     }
                 ),
             )
             span.set_attribute(
-                "llm.responses", json.dumps([{"text": "".join(result_content)}])
+                "llm.responses",
+                json.dumps([{"role": "assistant", "content": "".join(result_content)}]),
             )
             span.set_status(StatusCode.OK)
             span.end()
 
     # return the wrapped method
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 """
-This module contains the patching logic for the Chroma client.
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 from langtrace.trace_attributes import DatabaseSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
@@ -43,18 +55,18 @@
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
                 result = wrapped(*args, **kwargs)
                 span.set_status(StatusCode.OK)
                 return result
-            except Exception as e:
+            except Exception as err:
                 # Record the exception in the span
-                span.record_exception(e)
+                span.record_exception(err)
 
                 # Set the span status to indicate an error
-                span.set_status(Status(StatusCode.ERROR, str(e)))
+                span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 """
-Instrumentation for Cohere
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 import importlib.metadata
+import logging
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.cohere.patch import (
-    chat_create,
-    chat_stream,
-    embed_create
-)
+from langtrace_python_sdk.constants.instrumentation.chroma import APIS
+from langtrace_python_sdk.instrumentation.chroma.patch import collection_patch
+
+logging.basicConfig(level=logging.FATAL)
+
 
-class CohereInstrumentation(BaseInstrumentor):
+class ChromaInstrumentation(BaseInstrumentor):
     """
-    The CohereInstrumentation class represents the Anthropic instrumentation
+    The ChromaInstrumentation class represents the ChromaDB instrumentation
     """
 
     def instrumentation_dependencies(self) -> Collection[str]:
-        return ["cohere >= 5.0.0"]
+        return ["chromadb >= 0.4.23"]
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
-        version = importlib.metadata.version("cohere")
+        version = importlib.metadata.version("chromadb")
 
-        wrap_function_wrapper(
-            "cohere.client",
-            "Client.chat",
-            chat_create("cohere.client.chat", version, tracer),
-        )
-
-        wrap_function_wrapper(
-            "cohere.client",
-            "Client.chat_stream",
-            chat_stream("cohere.client.chat_stream", version, tracer),
-        )
-
-        wrap_function_wrapper(
-            "cohere.client",
-            "Client.embed",
-            embed_create("cohere.client.embed", version, tracer),
-        )
+        for operation, _ in APIS.items():
+            wrap_function_wrapper(
+                "chromadb.api.models.Collection",
+                f"Collection.{operation.lower()}",
+                collection_patch(operation, version, tracer),
+            )
 
     def _instrument_module(self, module_name):
         pass
 
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 """
-Instrumentation for langchain.
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 import importlib.metadata
 import inspect
+import logging
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.langchain.patch import generic_patch
 
-import logging
-
 logging.basicConfig(level=logging.FATAL)
 
 
 def patch_module_classes(
     module_name, tracer, version, task, trace_output=True, trace_input=True
 ):
     """
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 """
-This module contains the patching logic for the langchain package.
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
+
 import json
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
-from opentelemetry.trace import SpanKind, StatusCode
-from opentelemetry.trace.status import Status
+from opentelemetry.trace import SpanKind
+from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
     LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
 
 
 def generic_patch(
     method_name, task, tracer, version, trace_output=True, trace_input=True
 ):
-    """
-    patch method for generic methods.
-    """
-
     def traced_method(wrapped, instance, args, kwargs):
-        service_provider = SERVICE_PROVIDERS["LANGCHAIN"]
+        service_provider = SERVICE_PROVIDERS["LANGCHAIN_COMMUNITY"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
             **(extra_attributes if extra_attributes is not None else {})
         }
 
-        if len(args) > 0 and trace_input:
+        if trace_input and len(args) > 0:
             span_attributes["langchain.inputs"] = to_json_string(args)
 
         attributes = FrameworkSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(method_name, kind=SpanKind.CLIENT) as span:
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
@@ -47,20 +56,20 @@
                 # Attempt to call the original method
                 result = wrapped(*args, **kwargs)
                 if trace_output:
                     span.set_attribute("langchain.outputs", to_json_string(result))
 
                 span.set_status(StatusCode.OK)
                 return result
-            except Exception as e:
+            except Exception as err:
                 # Record the exception in the span
-                span.record_exception(e)
+                span.record_exception(err)
 
                 # Set the span status to indicate an error
-                span.set_status(Status(StatusCode.ERROR, str(e)))
+                span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 """
-Instrumentation for langchain-community.
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 import importlib.metadata
 import inspect
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.langchain_community.patch import generic_patch
+from langtrace_python_sdk.instrumentation.langchain_community.patch import \
+    generic_patch
 
 
 def patch_module_classes(
     module_name, tracer, version, task, trace_output=True, trace_input=True
 ):
     """
     Generic function to patch all public methods of all classes in a given module.
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,56 @@
+"""
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import json
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
-from opentelemetry.trace import SpanKind
-from opentelemetry.trace.status import Status, StatusCode
+from opentelemetry.trace import SpanKind, StatusCode
+from opentelemetry.trace.status import Status
 
 from langtrace_python_sdk.constants.instrumentation.common import (
     LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
 
 
 def generic_patch(
     method_name, task, tracer, version, trace_output=True, trace_input=True
 ):
+    """
+    patch method for generic methods.
+    """
+
     def traced_method(wrapped, instance, args, kwargs):
-        service_provider = SERVICE_PROVIDERS["LANGCHAIN_COMMUNITY"]
+        service_provider = SERVICE_PROVIDERS["LANGCHAIN"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
             **(extra_attributes if extra_attributes is not None else {})
         }
 
-        if trace_input and len(args) > 0:
+        if len(args) > 0 and trace_input:
             span_attributes["langchain.inputs"] = to_json_string(args)
 
         attributes = FrameworkSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(method_name, kind=SpanKind.CLIENT) as span:
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
@@ -39,20 +59,20 @@
                 # Attempt to call the original method
                 result = wrapped(*args, **kwargs)
                 if trace_output:
                     span.set_attribute("langchain.outputs", to_json_string(result))
 
                 span.set_status(StatusCode.OK)
                 return result
-            except Exception as e:
+            except Exception as err:
                 # Record the exception in the span
-                span.record_exception(e)
+                span.record_exception(err)
 
                 # Set the span status to indicate an error
-                span.set_status(Status(StatusCode.ERROR, str(e)))
+                span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 """
-Instrumentation for langchain-core.
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 import importlib.metadata
 import inspect
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.langchain_core.patch import (
-    generic_patch,
-    runnable_patch,
-)
+    generic_patch, runnable_patch)
 
 
 # pylint: disable=dangerous-default-value
 def patch_module_classes(
     module_name,
     tracer,
     version,
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 """
-This module contains the patching functions for the langchain_core package.
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 import json
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind, StatusCode
@@ -64,20 +76,20 @@
                 # Attempt to call the original method
                 result = wrapped(*args, **kwargs)
                 if trace_output:
                     span.set_attribute("langchain.outputs", to_json_string(result))
 
                 span.set_status(StatusCode.OK)
                 return result
-            except Exception as e:
+            except Exception as err:
                 # Record the exception in the span
-                span.record_exception(e)
+                span.record_exception(err)
 
                 # Set the span status to indicate an error
-                span.set_status(Status(StatusCode.ERROR, str(e)))
+                span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
 
 
@@ -153,20 +165,20 @@
                                 outputs[field] = value
                     span.set_attribute("langchain.outputs", to_json_string(outputs))
                     if isinstance(result, str):
                         span.set_attribute("langchain.outputs", result)
 
                 span.set_status(StatusCode.OK)
                 return result
-            except Exception as e:
+            except Exception as err:
                 # Record the exception in the span
-                span.record_exception(e)
+                span.record_exception(err)
 
                 # Set the span status to indicate an error
-                span.set_status(Status(StatusCode.ERROR, str(e)))
+                span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 """
-This module contains the patching logic for the OpenAI library."""
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
 
 import json
 
 from langtrace.trace_attributes import Event, LLMSpanAttributes
-from opentelemetry import baggage, trace
+from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
-    SERVICE_PROVIDERS,
-)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
-from langtrace_python_sdk.utils.llm import calculate_prompt_tokens, estimate_tokens
+from langtrace_python_sdk.utils.llm import (calculate_prompt_tokens,
+                                            estimate_tokens)
 
 
 def images_generate(original_method, version, tracer):
     """
     Wrap the `generate` method of the `Images` class to trace it.
     """
 
@@ -36,15 +48,15 @@
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["IMAGES_GENERATION"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.stream": kwargs.get("stream"),
-            "llm.prompts": json.dumps([kwargs.get("prompt", [])]),
+            "llm.prompts": json.dumps([{"role": "user", "content": kwargs.get("prompt", [])}]),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(
             APIS["IMAGES_GENERATION"]["METHOD"], kind=SpanKind.CLIENT
@@ -59,20 +71,23 @@
                     data = (
                         result.data[0]
                         if hasattr(result, "data") and len(result.data) > 0
                         else {}
                     )
                     response = [
                         {
-                            "url": data.url if hasattr(data, "url") else "",
-                            "revised_prompt": (
-                                data.revised_prompt
-                                if hasattr(data, "revised_prompt")
-                                else ""
-                            ),
+                            "role": "assistant",
+                            "content": {
+                                "url": data.url if hasattr(data, "url") else "",
+                                "revised_prompt": (
+                                    data.revised_prompt
+                                    if hasattr(data, "revised_prompt")
+                                    else ""
+                                ),
+                            }
                         }
                     ]
                     span.set_attribute("llm.responses", json.dumps(response))
 
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
@@ -108,15 +123,15 @@
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["IMAGES_GENERATION"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.stream": kwargs.get("stream"),
-            "llm.prompts": json.dumps([kwargs.get("prompt", [])]),
+            "llm.prompts": json.dumps([{"role": "user", "content": kwargs.get("prompt", [])}]),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(
             APIS["IMAGES_GENERATION"]["METHOD"], kind=SpanKind.CLIENT
@@ -132,20 +147,23 @@
                     data = (
                         result.data[0]
                         if hasattr(result, "data") and len(result.data) > 0
                         else {}
                     )
                     response = [
                         {
-                            "url": data.url if hasattr(data, "url") else "",
-                            "revised_prompt": (
-                                data.revised_prompt
-                                if hasattr(data, "revised_prompt")
-                                else ""
-                            ),
+                            "role": "assistant",
+                            "content": {
+                                "url": data.url if hasattr(data, "url") else "",
+                                "revised_prompt": (
+                                    data.revised_prompt
+                                    if hasattr(data, "revised_prompt")
+                                    else ""
+                                ),
+                            }
                         }
                     ]
                     span.set_attribute("llm.responses", json.dumps(response))
 
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
@@ -226,15 +244,16 @@
         if kwargs.get("temperature") is not None:
             attributes.llm_temperature = kwargs.get("temperature")
         if kwargs.get("top_p") is not None:
             attributes.llm_top_p = kwargs.get("top_p")
         if kwargs.get("user") is not None:
             attributes.llm_user = kwargs.get("user")
         if kwargs.get("functions") is not None:
-            tools.append(json.dumps(kwargs.get("functions")))
+            for function in kwargs.get("functions"):
+                tools.append(json.dumps({"type": "function", "function": function}))
         if kwargs.get("tools") is not None:
             tools.append(json.dumps(kwargs.get("tools")))
         if len(tools) > 0:
             attributes.llm_tools = json.dumps(tools)
 
         # TODO(Karthik): Gotta figure out how to handle streaming with context
         # with tracer.start_as_current_span(APIS["CHAT_COMPLETION"]["METHOD"],
@@ -249,33 +268,30 @@
             # Attempt to call the original method
             result = wrapped(*args, **kwargs)
             if kwargs.get("stream") is False or kwargs.get("stream") is None:
                 span.set_attribute("llm.model", result.model)
                 if hasattr(result, "choices") and result.choices is not None:
                     responses = [
                         {
-                            "message": {
-                                "role": (
-                                    choice.message.role
-                                    if choice.message and choice.message.role
-                                    else "assistant"
-                                ),
-                                "content": extract_content(choice),
-                                **(
-                                    {
-                                        "content_filter_results": choice[
-                                            "content_filter_results"
-                                        ]
-                                    }
-                                    if "content_filter_results" in choice
-                                    else {}
-                                ),
-                            }
-                        }
-                        for choice in result.choices
+                            "role": (
+                                choice.message.role
+                                if choice.message and choice.message.role
+                                else "assistant"
+                            ),
+                            "content": extract_content(choice),
+                            **(
+                                {
+                                    "content_filter_results": choice[
+                                        "content_filter_results"
+                                    ]
+                                }
+                                if "content_filter_results" in choice
+                                else {}
+                            ),
+                        } for choice in result.choices
                     ]
                     span.set_attribute("llm.responses", json.dumps(responses))
                 else:
                     responses = []
                     span.set_attribute("llm.responses", json.dumps(responses))
                 if (
                     hasattr(result, "system_fingerprint")
@@ -344,27 +360,37 @@
                                 token_counts = estimate_tokens(choice.delta.content)
                                 completion_tokens += token_counts
                                 content = [choice.delta.content]
                     elif function_call:
                         for choice in chunk.choices:
                             if (
                                 choice.delta
-                                and choice.delta.function_call
+                                and choice.delta.function_call is not None
                                 and choice.delta.function_call.arguments is not None
                             ):
                                 token_counts = estimate_tokens(
                                     choice.delta.function_call.arguments
                                 )
                                 completion_tokens += token_counts
                                 content = [choice.delta.function_call.arguments]
                     elif tool_calls:
-                        # TODO(Karthik): Tool calls streaming is tricky. The chunks after the
-                        # first one are missing the function name and id though the arguments
-                        # are spread across the chunks.
-                        content = []
+                        for choice in chunk.choices:
+                            tool_call = ""
+                            if (choice.delta and choice.delta.tool_calls is not None):
+                                toolcalls = choice.delta.tool_calls
+                                content = []
+                                for tool_call in toolcalls:
+                                    if tool_call and tool_call.function is not None and tool_call.function.arguments is not None:
+                                        token_counts = estimate_tokens(
+                                            tool_call.function.arguments
+                                        )
+                                        completion_tokens += token_counts
+                                        content = content + [tool_call.function.arguments]
+                                    else:
+                                        content = content + []
                 else:
                     content = []
                 span.add_event(
                     Event.STREAM_OUTPUT.value,
                     {
                         "response": (
                             "".join(content)
@@ -389,18 +415,16 @@
                 ),
             )
             span.set_attribute(
                 "llm.responses",
                 json.dumps(
                     [
                         {
-                            "message": {
-                                "role": "assistant",
-                                "content": "".join(result_content),
-                            }
+                            "role": "assistant",
+                            "content": "".join(result_content),
                         }
                     ]
                 ),
             )
             span.set_status(StatusCode.OK)
             span.end()
 
@@ -473,15 +497,16 @@
         if kwargs.get("temperature") is not None:
             attributes.llm_temperature = kwargs.get("temperature")
         if kwargs.get("top_p") is not None:
             attributes.llm_top_p = kwargs.get("top_p")
         if kwargs.get("user") is not None:
             attributes.llm_user = kwargs.get("user")
         if kwargs.get("functions") is not None:
-            tools.append(json.dumps(kwargs.get("functions")))
+            for function in kwargs.get("functions"):
+                tools.append(json.dumps({"type": "function", "function": function}))
         if kwargs.get("tools") is not None:
             tools.append(json.dumps(kwargs.get("tools")))
         if len(tools) > 0:
             attributes.llm_tools = json.dumps(tools)
 
         # TODO(Karthik): Gotta figure out how to handle streaming with context
         # with tracer.start_as_current_span(APIS["CHAT_COMPLETION"]["METHOD"],
@@ -496,33 +521,30 @@
             # Attempt to call the original method
             result = await wrapped(*args, **kwargs)
             if kwargs.get("stream") is False or kwargs.get("stream") is None:
                 span.set_attribute("llm.model", result.model)
                 if hasattr(result, "choices") and result.choices is not None:
                     responses = [
                         {
-                            "message": {
-                                "role": (
-                                    choice.message.role
-                                    if choice.message and choice.message.role
-                                    else "assistant"
-                                ),
-                                "content": extract_content(choice),
-                                **(
-                                    {
-                                        "content_filter_results": choice[
-                                            "content_filter_results"
-                                        ]
-                                    }
-                                    if "content_filter_results" in choice
-                                    else {}
-                                ),
-                            }
-                        }
-                        for choice in result.choices
+                            "role": (
+                                choice.message.role
+                                if choice.message and choice.message.role
+                                else "assistant"
+                            ),
+                            "content": extract_content(choice),
+                            **(
+                                {
+                                    "content_filter_results": choice[
+                                        "content_filter_results"
+                                    ]
+                                }
+                                if "content_filter_results" in choice
+                                else {}
+                            ),
+                        } for choice in result.choices
                     ]
                     span.set_attribute("llm.responses", json.dumps(responses))
                 else:
                     responses = []
                     span.set_attribute("llm.responses", json.dumps(responses))
                 if (
                     hasattr(result, "system_fingerprint")
@@ -600,18 +622,28 @@
                             ):
                                 token_counts = estimate_tokens(
                                     choice.delta.function_call.arguments
                                 )
                                 completion_tokens += token_counts
                                 content = [choice.delta.function_call.arguments]
                     elif tool_calls:
-                        # TODO(Karthik): Tool calls streaming is tricky. The chunks after the
-                        # first one are missing the function name and id though the arguments
-                        # are spread across the chunks.
-                        content = []
+                        for choice in chunk.choices:
+                            tool_call = ""
+                            if (choice.delta and choice.delta.tool_calls is not None):
+                                toolcalls = choice.delta.tool_calls
+                                content = []
+                                for tool_call in toolcalls:
+                                    if tool_call and tool_call.function is not None and tool_call.function.arguments is not None:
+                                        token_counts = estimate_tokens(
+                                            tool_call.function.arguments
+                                        )
+                                        completion_tokens += token_counts
+                                        content = content + [tool_call.function.arguments]
+                                    else:
+                                        content = content + []
                 else:
                     content = []
                 span.add_event(
                     Event.STREAM_OUTPUT.value,
                     {
                         "response": (
                             "".join(content)
@@ -636,18 +668,16 @@
                 ),
             )
             span.set_attribute(
                 "llm.responses",
                 json.dumps(
                     [
                         {
-                            "message": {
-                                "role": "assistant",
-                                "content": "".join(result_content),
-                            }
+                            "role": "assistant",
+                            "content": "".join(result_content),
                         }
                     ]
                 ),
             )
             span.set_status(StatusCode.OK)
             span.end()
 
@@ -676,17 +706,21 @@
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["EMBEDDINGS_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.prompts": "",
+            "llm.embedding_inputs": json.dumps([kwargs.get("input", "")]),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
+        if kwargs.get("encoding_format") is not None:
+            span_attributes["llm.encoding_format"] = json.dumps([kwargs.get("encoding_format")])
+
         attributes = LLMSpanAttributes(**span_attributes)
         kwargs.get("encoding_format")
 
         if kwargs.get("encoding_format") is not None:
             attributes.llm_encoding_format = kwargs.get("encoding_format")
         if kwargs.get("dimensions") is not None:
             attributes["llm.dimensions"] = kwargs.get("dimensions")
@@ -738,15 +772,15 @@
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["EMBEDDINGS_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
-            "llm.prompts": "",
+            "llm.prompts": json.dumps([{"role": "user", "content": kwargs.get("input", "")}]),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
         kwargs.get("encoding_format")
 
         if kwargs.get("encoding_format") is not None:
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 """
-Pinecone instrumentation
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 import importlib.metadata
+import logging
 from typing import Collection
 
 import pinecone
 from langtrace.trace_attributes import PineconeMethods
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
 from langtrace_python_sdk.instrumentation.pinecone.patch import generic_patch
 
-import logging
-
 logging.basicConfig(level=logging.FATAL)
 
 
 class PineconeInstrumentation(BaseInstrumentor):
     """
     The PineconeInstrumentation class represents the Pinecone instrumentation"""
```

### Comparing `langtrace_python_sdk-1.3.7/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 """
-This module contains the patching logic for the Pinecone client."""
+Copyright (c) 2024 Scale3 Labs
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
 
 from langtrace.trace_attributes import DatabaseSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
@@ -38,18 +51,18 @@
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
                 result = original_method(instance, *args, **kwargs)
                 span.set_status(StatusCode.OK)
                 return result
-            except Exception as e:
+            except Exception as err:
                 # Record the exception in the span
-                span.record_exception(e)
+                span.record_exception(err)
 
                 # Set the span status to indicate an error
-                span.set_status(Status(StatusCode.ERROR, str(e)))
+                span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.7/src/tests/utils.py` & `langtrace_python_sdk-2.0.0/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,69 @@
+
 import unittest
 from unittest.mock import MagicMock, call
-from langtrace_python_sdk.instrumentation.anthropic.patch import messages_create
+from langtrace_python_sdk.instrumentation.langchain.patch import generic_patch
 from opentelemetry.trace import SpanKind
+from opentelemetry.trace import get_tracer
 import importlib.metadata
-from langtrace_python_sdk.constants.instrumentation.anthropic import APIS
+from langtrace_python_sdk.constants.instrumentation.openai import APIS
 from opentelemetry.trace.status import Status, StatusCode
-import json
-from langtrace.trace_attributes import Event, LLMSpanAttributes
-
 from tests.utils import common_setup
+import json
 
-class TestAnthropic(unittest.TestCase):
-
-    data = {
-        "content" : [MagicMock(text="Some text", type="text")],
-        "system_fingerprint" : "None",
-        "usage" : MagicMock(input_tokens=23, output_tokens=44),
-        "chunks" : [MagicMock(delta="Some text", message="text")]}
-
-
+class TestGenericPatch(unittest.TestCase):
+    data = {"key": "value"}
     def setUp(self):
-        
-        # Mock the original method
-        self.anthropic_mock, self.tracer, self.span = common_setup(self.data, None)
+        self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
 
     def tearDown(self):
+        # Clean up after each test case
         pass
-
-    def test_anthropic(self):
+      
+    def test_generic_patch(self):
         # Arrange
-        version = importlib.metadata.version('anthropic')        
-        kwargs = {
-            "model": "claude-3-opus-20240229",
-            "messages" : [{"role": "user", "content": "How are you today?"}],
-            "stream": False
-        }   
+        method_name = "example_method"
+        trace_output = False
+        trace_input = False  # Change as per your requirement
+        args = (1, 2, 3)
+        task = "split_text"
+        kwargs = {'key': 'value'}
+        version = importlib.metadata.version('langchain')
 
         # Act
-        wrapped_function = messages_create("anthropic.messages.create", version, self.tracer)
-        result = wrapped_function(self.anthropic_mock, MagicMock(), (), kwargs)
-        
+        wrapped_function = generic_patch("langchain.text_splitter", task, self.tracer, version, trace_output, trace_input)
+        result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with("anthropic.messages.create", kind=SpanKind.CLIENT))
-        self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
+        self.assertTrue(self.tracer.start_as_current_span.called_once_with(method_name, kind=SpanKind.CLIENT))
         
+        service_provider = "Langchain"
         expected_attributes = {
-            "langtrace.sdk.name": "langtrace-python-sdk",
-            "langtrace.service.name": "Anthropic",
-            "langtrace.service.type": "llm",
+            'langtrace.sdk.name': 'langtrace-python-sdk',
+            "langtrace.service.name": service_provider,
+            "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "url.full": "/v1/messages",
-            "llm.api": APIS["MESSAGES_CREATE"]["ENDPOINT"],
-            "llm.model": kwargs.get("model"),
-            "llm.prompts": json.dumps(kwargs.get("messages", [])),
-            "llm.stream": kwargs.get("stream"),
+            "langchain.task.name": task,
         }
-
+        
+        
         self.assertTrue(
             self.span.set_attribute.has_calls(
                 [call(key, value) for key, value in expected_attributes.items()], any_order=True
             )
         )
-       
-        expected_result_data = {"system_fingerprint": "None"  }   
+                
+        actual_calls = self.span.set_attribute.call_args_list
+
+        for key, value in expected_attributes.items():
+            self.assertIn(call(key, value), actual_calls)
+        
+        self.assertEqual(self.span.set_status.call_count, 1)
+        self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
-        self.assertEqual(result.system_fingerprint, expected_result_data["system_fingerprint"])
+        expected_result_data = {"key": "value"  }   
 
+        self.assertEqual(result.key, expected_result_data["key"])
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `langtrace_python_sdk-1.3.7/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.0.0/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_community.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 
 import unittest
-from unittest.mock import MagicMock, call
-from langtrace_python_sdk.instrumentation.langchain.patch import generic_patch
+from unittest.mock import MagicMock, Mock, patch, call
+from langtrace_python_sdk.instrumentation.langchain_community.patch import generic_patch
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace import get_tracer
 import importlib.metadata
+import openai
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
 from opentelemetry.trace.status import Status, StatusCode
-from tests.utils import common_setup
 import json
-
+from tests.utils import common_setup
 class TestGenericPatch(unittest.TestCase):
     data = {"key": "value"}
     def setUp(self):
         self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
 
     def tearDown(self):
         # Clean up after each test case
         pass
-      
+
     def test_generic_patch(self):
         # Arrange
         method_name = "example_method"
         trace_output = False
-        trace_input = False  # Change as per your requirement
+        trace_input = False 
         args = (1, 2, 3)
-        task = "split_text"
+        task = "vector_store"
         kwargs = {'key': 'value'}
-        version = importlib.metadata.version('langchain')
+        version = importlib.metadata.version("langchain-community")
 
         # Act
-        wrapped_function = generic_patch("langchain.text_splitter", task, self.tracer, version, trace_output, trace_input)
+        wrapped_function = generic_patch("langchain_community.vectorstores.faiss", task, self.tracer, version, trace_output, trace_input)
         result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
 
         # Assert
         self.assertTrue(self.tracer.start_as_current_span.called_once_with(method_name, kind=SpanKind.CLIENT))
         
-        service_provider = "Langchain"
+        service_provider = "Langchain Community"
         expected_attributes = {
             'langtrace.sdk.name': 'langtrace-python-sdk',
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
@@ -58,12 +58,12 @@
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
         
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
         expected_result_data = {"key": "value"  }   
-
         self.assertEqual(result.key, expected_result_data["key"])
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `langtrace_python_sdk-1.3.7/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.0.0/src/tests/pinecone/test_pinecone.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,72 @@
-
-import unittest
-from unittest.mock import MagicMock, Mock, patch, call
-from langtrace_python_sdk.instrumentation.langchain_community.patch import generic_patch
+from unittest.mock import MagicMock, patch, call
+from langtrace_python_sdk.instrumentation.pinecone.patch import generic_patch
 from opentelemetry.trace import SpanKind
-from opentelemetry.trace import get_tracer
 import importlib.metadata
-import openai
-from langtrace_python_sdk.constants.instrumentation.openai import APIS
+import pinecone
+from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
+from langtrace_python_sdk.constants.instrumentation.common import SERVICE_PROVIDERS
+from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
+import unittest
 import json
 from tests.utils import common_setup
-class TestGenericPatch(unittest.TestCase):
-    data = {"key": "value"}
+
+
+class TestPinecone(unittest.TestCase):
+    data = {
+    "status": "success",
+    "message": "Data upserted successfully",
+    "upserted_ids": [1, 2, 3]
+    }
+    
     def setUp(self):
-        self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
+        self.pinecone_mock, self.tracer, self.span = common_setup(self.data, 'pinecone.Index.upsert')
+
 
     def tearDown(self):
-        # Clean up after each test case
-        pass
+        self.pinecone_mock.stop()
 
-    def test_generic_patch(self):
-        # Arrange
-        method_name = "example_method"
-        trace_output = False
-        trace_input = False 
-        args = (1, 2, 3)
-        task = "vector_store"
-        kwargs = {'key': 'value'}
-        version = importlib.metadata.version("langchain-community")
+    def test_pinecone(self):
+    
+       # Arrange
+        version = importlib.metadata.version('pinecone-client')
+        method = "UPSERT"
+        vectors = [[1, 2, 3], [4, 5, 6]]
 
         # Act
-        wrapped_function = generic_patch("langchain_community.vectorstores.faiss", task, self.tracer, version, trace_output, trace_input)
-        result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
+        wrapped_function = generic_patch(pinecone.Index.upsert, method, version, self.tracer)
+        result = wrapped_function(MagicMock(), MagicMock(), (vectors,), {})
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with(method_name, kind=SpanKind.CLIENT))
-        
-        service_provider = "Langchain Community"
+        self.assertTrue(self.tracer.start_as_current_span.called_once_with("pinecone.data.index", kind=SpanKind.CLIENT))
+        api = APIS[method]
+        service_provider = SERVICE_PROVIDERS["PINECONE"]
         expected_attributes = {
             'langtrace.sdk.name': 'langtrace-python-sdk',
             "langtrace.service.name": service_provider,
-            "langtrace.service.type": "framework",
+            "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "langchain.task.name": task,
+            "db.system": "pinecone",
+            "db.operation": api["OPERATION"],
         }
-        
-        
         self.assertTrue(
             self.span.set_attribute.has_calls(
                 [call(key, value) for key, value in expected_attributes.items()], any_order=True
             )
-        )
-                
+        )      
+
         actual_calls = self.span.set_attribute.call_args_list
 
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
-        
+            
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
-        expected_result_data = {"key": "value"  }   
-        self.assertEqual(result.key, expected_result_data["key"])
-
+        expected_result = ['status', 'message', 'upserted_ids']
+        result_keys = json.loads(result).keys()
+        self.assertSetEqual(set(expected_result), set(result_keys), "Keys mismatch")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `langtrace_python_sdk-1.3.7/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.0.0/src/tests/anthropic/test_anthropic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,142 +1,109 @@
 import pytest
-import importlib
 import json
-from langtrace_python_sdk.constants.instrumentation.openai import APIS
+import importlib
+from langtrace_python_sdk.constants.instrumentation.anthropic import APIS
 
 
 @pytest.mark.vcr()
-def test_chat_completion(exporter, openai_client):
-    llm_model_value = "gpt-4"
-    messages_value = [{"role": "user", "content": "Say this is a test three times"}]
+def test_anthropic(anthropic_client, exporter):
+    llm_model_value = "claude-3-opus-20240229"
+    messages_value = [{"role": "user", "content": "How are you today?"}]
 
     kwargs = {
         "model": llm_model_value,
         "messages": messages_value,
+        # "system": "Respond only in Yoda-speak.",
         "stream": False,
+        "max_tokens": 1024,
     }
-
-    openai_client.chat.completions.create(**kwargs)
+    response = anthropic_client.messages.create(**kwargs)
     spans = exporter.get_finished_spans()
     completion_span = spans[-1]
-    assert completion_span.name == "openai.chat.completions.create"
 
+    assert completion_span.name == "anthropic.messages.create"
     attributes = completion_span.attributes
+
     assert attributes.get("langtrace.sdk.name") == "langtrace-python-sdk"
-    assert attributes.get("langtrace.service.name") == "OpenAI"
+    assert attributes.get("langtrace.service.name") == "Anthropic"
     assert attributes.get("langtrace.service.type") == "llm"
     assert attributes.get("langtrace.service.version") == importlib.metadata.version(
-        "openai"
+        "anthropic"
     )
     assert attributes.get("langtrace.version") == "1.0.0"
-    assert attributes.get("url.full") == "https://api.openai.com/v1/"
-    assert attributes.get("llm.api") == APIS["CHAT_COMPLETION"]["ENDPOINT"]
-    assert attributes.get("llm.model") == "gpt-4-0613"
+    assert attributes.get("url.full") == "https://api.anthropic.com"
+    assert attributes.get("llm.api") == APIS["MESSAGES_CREATE"]["ENDPOINT"]
+    assert attributes.get("llm.model") == llm_model_value
     assert attributes.get("llm.prompts") == json.dumps(messages_value)
     assert attributes.get("llm.stream") is False
 
     tokens = json.loads(attributes.get("llm.token.counts"))
     output_tokens = tokens.get("output_tokens")
     prompt_tokens = tokens.get("input_tokens")
     total_tokens = tokens.get("total_tokens")
 
     assert output_tokens and prompt_tokens and total_tokens
     assert output_tokens + prompt_tokens == total_tokens
 
-
-@pytest.mark.vcr()
-def test_chat_completion_streaming(exporter, openai_client):
-    llm_model_value = "gpt-4"
-    messages_value = [{"role": "user", "content": "Say this is a test three times"}]
-
-    kwargs = {
-        "model": llm_model_value,
-        "messages": messages_value,
-        "stream": True,
-    }
-
-    response = openai_client.chat.completions.create(**kwargs)
-    chunk_count = 0
-    for _ in response:
-        chunk_count += 1
-
-    spans = exporter.get_finished_spans()
-    streaming_span = spans[-1]
-
-    assert streaming_span.name == "openai.chat.completions.create"
-    attributes = streaming_span.attributes
-
-    assert attributes.get("langtrace.sdk.name") == "langtrace-python-sdk"
-    assert attributes.get("langtrace.service.name") == "OpenAI"
-    assert attributes.get("langtrace.service.type") == "llm"
-    assert attributes.get("langtrace.service.version") == importlib.metadata.version(
-        "openai"
-    )
-    assert attributes.get("langtrace.version") == "1.0.0"
-    assert attributes.get("url.full") == "https://api.openai.com/v1/"
-    assert attributes.get("llm.api") == APIS["CHAT_COMPLETION"]["ENDPOINT"]
-    assert attributes.get("llm.model") == "gpt-4-0613"
-    assert attributes.get("llm.prompts") == json.dumps(messages_value)
-    assert attributes.get("llm.stream") is True
-
-    events = streaming_span.events
-    assert len(events) - 2 == chunk_count  # -2 for start and end events
-
-    # check token usage attributes for stream
-    tokens = json.loads(attributes.get("llm.token.counts"))
-
-    output_tokens = tokens.get("output_tokens")
-    prompt_tokens = tokens.get("input_tokens")
-    total_tokens = tokens.get("total_tokens")
-
-    assert output_tokens and prompt_tokens and total_tokens
-    assert output_tokens + prompt_tokens == total_tokens
+    langtrace_responses = json.loads(attributes.get("llm.responses"))
+    assert isinstance(langtrace_responses, list)
+    for langtrace_response in langtrace_responses:
+        assert isinstance(langtrace_response, dict)
+        assert "role" in langtrace_response
+        assert "content" in langtrace_response
 
 
 @pytest.mark.vcr()
-@pytest.mark.asyncio()
-async def test_async_chat_completion_streaming(exporter, async_openai_client):
-    llm_model_value = "gpt-4"
-    messages_value = [{"role": "user", "content": "Say this is a test three times"}]
+def test_anthropic_streaming(anthropic_client, exporter):
+    llm_model_value = "claude-3-opus-20240229"
+    messages_value = [{"role": "user", "content": "How are you today?"}]
 
     kwargs = {
         "model": llm_model_value,
         "messages": messages_value,
+        # "system": "Respond only in Yoda-speak.",
         "stream": True,
+        "max_tokens": 1024,
     }
-
-    response = await async_openai_client.chat.completions.create(**kwargs)
+    response = anthropic_client.messages.create(**kwargs)
     chunk_count = 0
-    async for _ in response:
-        chunk_count += 1
+
+    for chunk in response:
+        if chunk:
+            chunk_count += 1
 
     spans = exporter.get_finished_spans()
     streaming_span = spans[-1]
 
-    assert streaming_span.name == "openai.chat.completions.create"
+    assert streaming_span.name == "anthropic.messages.create"
     attributes = streaming_span.attributes
 
     assert attributes.get("langtrace.sdk.name") == "langtrace-python-sdk"
-    assert attributes.get("langtrace.service.name") == "OpenAI"
+    assert attributes.get("langtrace.service.name") == "Anthropic"
     assert attributes.get("langtrace.service.type") == "llm"
     assert attributes.get("langtrace.service.version") == importlib.metadata.version(
-        "openai"
+        "anthropic"
     )
     assert attributes.get("langtrace.version") == "1.0.0"
-    assert attributes.get("url.full") == "https://api.openai.com/v1/"
-    assert attributes.get("llm.api") == APIS["CHAT_COMPLETION"]["ENDPOINT"]
-    assert attributes.get("llm.model") == "gpt-4-0613"
+    assert attributes.get("url.full") == "https://api.anthropic.com"
+    assert attributes.get("llm.api") == APIS["MESSAGES_CREATE"]["ENDPOINT"]
+    assert attributes.get("llm.model") == llm_model_value
     assert attributes.get("llm.prompts") == json.dumps(messages_value)
     assert attributes.get("llm.stream") is True
-
     events = streaming_span.events
+
     assert len(events) - 2 == chunk_count  # -2 for start and end events
 
-    # check token usage attributes for stream
     tokens = json.loads(attributes.get("llm.token.counts"))
-
     output_tokens = tokens.get("output_tokens")
     prompt_tokens = tokens.get("input_tokens")
     total_tokens = tokens.get("total_tokens")
 
     assert output_tokens and prompt_tokens and total_tokens
     assert output_tokens + prompt_tokens == total_tokens
+
+    langtrace_responses = json.loads(attributes.get("llm.responses"))
+    assert isinstance(langtrace_responses, list)
+    for langtrace_response in langtrace_responses:
+        assert isinstance(langtrace_response, dict)
+        assert "role" in langtrace_response
+        assert "content" in langtrace_response
```

### Comparing `langtrace_python_sdk-1.3.7/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.0.0/src/tests/openai/test_image_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,21 +26,27 @@
     assert attributes.get("langtrace.service.version") == importlib.metadata.version(
         "openai"
     )
     assert attributes.get("langtrace.version") == "1.0.0"
     assert attributes.get("url.full") == "https://api.openai.com/v1/"
     assert attributes.get("llm.api") == APIS["IMAGES_GENERATION"]["ENDPOINT"]
     assert attributes.get("llm.model") == llm_model_value
-    assert attributes.get("llm.prompts") == json.dumps([prompt])
+    prompts = json.loads(attributes.get("llm.prompts"))
+    assert prompts[0]["content"] == prompt
 
     langtrace_responses = json.loads(attributes.get("llm.responses"))
+    assert isinstance(langtrace_responses, list)
     for langtrace_response in langtrace_responses:
-        assert response.data[0].url == langtrace_response.get("url")
-        assert response.data[0].revised_prompt == langtrace_response.get(
-            "revised_prompt"
+        assert isinstance(langtrace_response, dict)
+        assert "role" in langtrace_response
+        assert "content" in langtrace_response
+        assert response.data[0].url == langtrace_response["content"]["url"]
+        assert (
+            response.data[0].revised_prompt
+            == langtrace_response["content"]["revised_prompt"]
         )
 
 
 @pytest.mark.vcr()
 @pytest.mark.asyncio()
 async def test_async_image_generation(async_openai_client, exporter):
     llm_model_value = "dall-e-3"
@@ -63,15 +69,21 @@
     assert attributes.get("langtrace.service.version") == importlib.metadata.version(
         "openai"
     )
     assert attributes.get("langtrace.version") == "1.0.0"
     assert attributes.get("url.full") == "https://api.openai.com/v1/"
     assert attributes.get("llm.api") == APIS["IMAGES_GENERATION"]["ENDPOINT"]
     assert attributes.get("llm.model") == llm_model_value
-    assert attributes.get("llm.prompts") == json.dumps([prompt])
+    prompts = json.loads(attributes.get("llm.prompts"))
+    assert prompts[0]["content"] == prompt
 
     langtrace_responses = json.loads(attributes.get("llm.responses"))
+    assert isinstance(langtrace_responses, list)
     for langtrace_response in langtrace_responses:
-        assert response.data[0].url == langtrace_response.get("url")
-        assert response.data[0].revised_prompt == langtrace_response.get(
-            "revised_prompt"
+        assert isinstance(langtrace_response, dict)
+        assert "role" in langtrace_response
+        assert "content" in langtrace_response
+        assert response.data[0].url == langtrace_response["content"]["url"]
+        assert (
+            response.data[0].revised_prompt
+            == langtrace_response["content"]["revised_prompt"]
         )
```

### Comparing `langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/.gitignore` & `langtrace_python_sdk-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/LICENSE` & `langtrace_python_sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/README.md` & `langtrace_python_sdk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.7/pyproject.toml` & `langtrace_python_sdk-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 license = "Apache-2.0"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'trace-attributes==1.0.32',
+  'trace-attributes==3.0.2',
   'opentelemetry-api',
   'opentelemetry-sdk',
   'opentelemetry-instrumentation',
   'pinecone-client',
   'tiktoken'
 ]
```

### Comparing `langtrace_python_sdk-1.3.7/PKG-INFO` & `langtrace_python_sdk-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 1.3.7
+Version: 2.0.0
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: pinecone-client
 Requires-Dist: tiktoken
-Requires-Dist: trace-attributes==1.0.32
+Requires-Dist: trace-attributes==3.0.2
 Provides-Extra: dev
 Requires-Dist: anthropic; extra == 'dev'
 Requires-Dist: chromadb; extra == 'dev'
 Requires-Dist: cohere; extra == 'dev'
 Requires-Dist: langchain; extra == 'dev'
 Requires-Dist: langchain-openai; extra == 'dev'
 Requires-Dist: llama-index; extra == 'dev'
```


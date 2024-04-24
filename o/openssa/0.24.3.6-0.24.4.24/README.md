# Comparing `tmp/openssa-0.24.3.6.tar.gz` & `tmp/openssa-0.24.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openssa-0.24.3.6.tar", max compression
+gzip compressed data, was "openssa-0.24.4.24.tar", max compression
```

## Comparing `openssa-0.24.3.6.tar` & `openssa-0.24.4.24.tar`

### file list

```diff
@@ -1,105 +1,106 @@
--rw-r--r--   0        0        0    11347 2024-03-07 07:35:52.393311 openssa-0.24.3.6/LICENSE.md
--rw-r--r--   0        0        0     7619 2024-03-07 07:35:52.393311 openssa-0.24.3.6/README.md
--rw-r--r--   0        0        0       79 2024-03-07 07:35:52.441311 openssa-0.24.3.6/openssa/Makefile
--rw-r--r--   0        0        0     2553 2024-03-07 07:35:52.441311 openssa-0.24.3.6/openssa/README.md
--rw-r--r--   0        0        0     2118 2024-03-07 07:35:52.441311 openssa-0.24.3.6/openssa/__init__.py
--rw-r--r--   0        0        0      330 2024-03-07 07:35:52.441311 openssa-0.24.3.6/openssa/contrib/__init__.py
--rw-r--r--   0        0        0       24 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/.gitignore
--rw-r--r--   0        0        0       80 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/.streamlit/secrets.toml.template
--rw-r--r--   0        0        0       81 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/Makefile
--rw-r--r--   0        0        0    15622 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/__init__.py
--rw-r--r--   0        0        0      956 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/main.py
--rw-r--r--   0        0        0     1116 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/pages/Semiconductor_ALD_SSA.py
--rw-r--r--   0        0        0      398 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/pages/Your_SSA_#1.py
--rw-r--r--   0        0        0      398 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/pages/Your_SSA_#2.py
--rw-r--r--   0        0        0      398 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/pages/Your_SSA_#3.py
--rw-r--r--   0        0        0       73 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/requirements.txt
--rw-r--r--   0        0        0     2122 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/adapter/abstract_adapter.py
--rw-r--r--   0        0        0     4725 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/adapter/base_adapter.py
--rw-r--r--   0        0        0     1982 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/backend/abstract_backend.py
--rw-r--r--   0        0        0     2185 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/backend/base_backend.py
--rw-r--r--   0        0        0     6205 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/backend/rag_backend.py
--rw-r--r--   0        0        0      968 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/backend/text_backend.py
--rw-r--r--   0        0        0      809 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/inferencer/abstract_inferencer.py
--rw-r--r--   0        0        0      458 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/inferencer/base_inferencer.py
--rw-r--r--   0        0        0     3150 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda/deprecated/solver.py
--rw-r--r--   0        0        0      177 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda/heuristic.py
--rw-r--r--   0        0        0     2702 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda/ooda_loop.py
--rw-r--r--   0        0        0     2673 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda/task.py
--rw-r--r--   0        0        0     8179 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/builtin_agents.py
--rw-r--r--   0        0        0     5860 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/custom.py
--rw-r--r--   0        0        0     2954 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/heuristic.py
--rw-r--r--   0        0        0      668 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/notifier.py
--rw-r--r--   0        0        0     9700 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/ooda_rag.py
--rw-r--r--   0        0        0    13949 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/prompts.py
--rw-r--r--   0        0        0     2252 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/query_rewritting_engine.py
--rw-r--r--   0        0        0     3073 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/solver.py
--rw-r--r--   0        0        0     4299 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ooda_rag/tools.py
--rw-r--r--   0        0        0     4695 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/prompts.py
--rw-r--r--   0        0        0     4567 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/rag_ooda/rag_ooda.py
--rw-r--r--   0        0        0     8461 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/rag_ooda/resources/dense_x/base.py
--rw-r--r--   0        0        0     2112 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/rag_ooda/resources/dense_x/dense_x.py
--rw-r--r--   0        0        0      298 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/rag_ooda/resources/rag_resource.py
--rw-r--r--   0        0        0      822 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/rag_ooda/resources/standard_vi/standard_vi.py
--rw-r--r--   0        0        0     1079 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/slm/abstract_slm.py
--rw-r--r--   0        0        0     3726 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/slm/base_slm.py
--rw-r--r--   0        0        0      452 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/slm/memory/conversation_db.py
--rw-r--r--   0        0        0     1644 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/slm/memory/sqlite_conversation_db.py
--rw-r--r--   0        0        0     2203 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssa/agent.py
--rw-r--r--   0        0        0     7338 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssa/rag_ssa.py
--rw-r--r--   0        0        0     2094 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssa/ssa.py
--rw-r--r--   0        0        0     3349 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssa/ssa_service.py
--rw-r--r--   0        0        0     3041 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssm/abstract_ssm.py
--rw-r--r--   0        0        0     1488 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssm/abstract_ssm_builder.py
--rw-r--r--   0        0        0     8445 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssm/base_ssm.py
--rw-r--r--   0        0        0     1942 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssm/base_ssm_builder.py
--rw-r--r--   0        0        0     7587 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/core/ssm/rag_ssm.py
--rw-r--r--   0        0        0       62 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/README.md
--rw-r--r--   0        0        0      647 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/api_context.py
--rw-r--r--   0        0        0     4148 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/azure/ssm.py
--rw-r--r--   0        0        0     4445 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/huggingface/slm.py
--rw-r--r--   0        0        0      459 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/huggingface/ssm.py
--rw-r--r--   0        0        0     2125 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/lepton_ai/ssm.py
--rw-r--r--   0        0        0     6832 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/llama_index/README.md
--rw-r--r--   0        0        0     5008 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/llama_index/backend.py
--rw-r--r--   0        0        0     1883 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/llama_index/ssm.py
--rw-r--r--   0        0        0     5470 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/integrations/openai/ssm.py
--rw-r--r--   0        0        0     1908 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/agent/abstract.py
--rw-r--r--   0        0        0      691 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/agent/agent.py
--rw-r--r--   0        0        0      109 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/knowledge/fact/abstract.py
--rw-r--r--   0        0        0      124 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/knowledge/heuristic/abstract.py
--rw-r--r--   0        0        0      138 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/knowledge/inference_rule/abstract.py
--rw-r--r--   0        0        0     1791 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/planning/abstract.py
--rw-r--r--   0        0        0     5987 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/planning/hierarchical/__init__.py
--rw-r--r--   0        0        0     3183 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/planning/hierarchical/_prompts.py
--rw-r--r--   0        0        0      274 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/planning/map_reduce/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 07:35:52.445311 openssa-0.24.3.6/openssa/l2/planning/map_reduce/_prompts.py
--rw-r--r--   0        0        0      706 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/reasoning/abstract.py
--rw-r--r--   0        0        0      732 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/reasoning/base.py
--rw-r--r--   0        0        0      490 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/reasoning/ooda/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/reasoning/ooda/_prompts.py
--rw-r--r--   0        0        0      774 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/_global.py
--rw-r--r--   0        0        0      394 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/_prompts.py
--rw-r--r--   0        0        0      834 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/abstract.py
--rw-r--r--   0        0        0      215 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/db.py
--rw-r--r--   0        0        0     1430 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/file.py
--rw-r--r--   0        0        0      206 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/rss.py
--rw-r--r--   0        0        0      215 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/sensor.py
--rw-r--r--   0        0        0      206 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/resource/web.py
--rw-r--r--   0        0        0     1729 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/task/abstract.py
--rw-r--r--   0        0        0      230 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/task/status.py
--rw-r--r--   0        0        0     1153 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/task/task.py
--rw-r--r--   0        0        0       68 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/l2/tool/abstract.py
--rw-r--r--   0        0        0     1341 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/cli/__init__.py
--rw-r--r--   0        0        0      859 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/cli/contrib/ssa_prob_solver.py
--rw-r--r--   0        0        0     2344 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/config.py
--rw-r--r--   0        0        0     1271 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/deprecated/aitomatic_llm_config.py
--rw-r--r--   0        0        0    13318 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/deprecated/llama_index_api.py
--rw-r--r--   0        0        0     3887 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/fs.py
--rw-r--r--   0        0        0     6004 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/llms.py
--rw-r--r--   0        0        0     4627 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/logs.py
--rw-r--r--   0        0        0     3605 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/rag_service_contexts.py
--rw-r--r--   0        0        0     1248 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/usage_logger.py
--rw-r--r--   0        0        0    11686 2024-03-07 07:35:52.449311 openssa-0.24.3.6/openssa/utils/utils.py
--rw-r--r--   0        0        0     3336 2024-03-07 07:35:52.449311 openssa-0.24.3.6/pyproject.toml
--rw-r--r--   0        0        0     9259 1970-01-01 00:00:00.000000 openssa-0.24.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-04-24 08:04:48.276068 openssa-0.24.4.24/LICENSE.md
+-rw-r--r--   0        0        0     4145 2024-04-24 08:04:48.276068 openssa-0.24.4.24/README.md
+-rw-r--r--   0        0        0       79 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/Makefile
+-rw-r--r--   0        0        0     2553 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/README.md
+-rw-r--r--   0        0        0     2166 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/.gitignore
+-rw-r--r--   0        0        0       56 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/.streamlit/secrets.toml.template
+-rw-r--r--   0        0        0       81 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/Makefile
+-rw-r--r--   0        0        0    15690 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/main.py
+-rw-r--r--   0        0        0     1116 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/pages/Semiconductor_ALD_SSA.py
+-rw-r--r--   0        0        0      398 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/pages/Your_SSA_#1.py
+-rw-r--r--   0        0        0      398 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/pages/Your_SSA_#2.py
+-rw-r--r--   0        0        0      398 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/pages/Your_SSA_#3.py
+-rw-r--r--   0        0        0       73 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/requirements.txt
+-rw-r--r--   0        0        0     2122 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/adapter/abstract_adapter.py
+-rw-r--r--   0        0        0     4725 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/adapter/base_adapter.py
+-rw-r--r--   0        0        0     1982 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/backend/abstract_backend.py
+-rw-r--r--   0        0        0     2185 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/backend/base_backend.py
+-rw-r--r--   0        0        0     6150 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/backend/rag_backend.py
+-rw-r--r--   0        0        0      968 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/backend/text_backend.py
+-rw-r--r--   0        0        0      809 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/inferencer/abstract_inferencer.py
+-rw-r--r--   0        0        0      458 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/inferencer/base_inferencer.py
+-rw-r--r--   0        0        0     3150 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/ooda/deprecated/solver.py
+-rw-r--r--   0        0        0      177 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/ooda/heuristic.py
+-rw-r--r--   0        0        0     2702 2024-04-24 08:04:48.288068 openssa-0.24.4.24/openssa/core/ooda/ooda_loop.py
+-rw-r--r--   0        0        0     2673 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda/task.py
+-rw-r--r--   0        0        0    10308 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/builtin_agents.py
+-rw-r--r--   0        0        0     5879 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/custom.py
+-rw-r--r--   0        0        0     2954 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/heuristic.py
+-rw-r--r--   0        0        0      668 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/notifier.py
+-rw-r--r--   0        0        0     9700 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/ooda.py
+-rw-r--r--   0        0        0     3069 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/ooda_ssa.py
+-rw-r--r--   0        0        0    14852 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/prompts.py
+-rw-r--r--   0        0        0     2253 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/query_rewritting_engine.py
+-rw-r--r--   0        0        0     4563 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/rag_ooda.py
+-rw-r--r--   0        0        0     8462 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/resources/dense_x/base.py
+-rw-r--r--   0        0        0     2112 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/resources/dense_x/dense_x.py
+-rw-r--r--   0        0        0      298 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/resources/rag_resource.py
+-rw-r--r--   0        0        0      822 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/resources/standard_vi/standard_vi.py
+-rw-r--r--   0        0        0     4299 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ooda_rag/tools.py
+-rw-r--r--   0        0        0     4695 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/prompts.py
+-rw-r--r--   0        0        0     1079 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/slm/abstract_slm.py
+-rw-r--r--   0        0        0     3726 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/slm/base_slm.py
+-rw-r--r--   0        0        0      452 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/slm/memory/conversation_db.py
+-rw-r--r--   0        0        0     1644 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/slm/memory/sqlite_conversation_db.py
+-rw-r--r--   0        0        0     2203 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssa/agent.py
+-rw-r--r--   0        0        0     7338 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssa/rag_ssa.py
+-rw-r--r--   0        0        0     2094 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssa/ssa.py
+-rw-r--r--   0        0        0     3379 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssa/ssa_service.py
+-rw-r--r--   0        0        0     3041 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssm/abstract_ssm.py
+-rw-r--r--   0        0        0     1488 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssm/abstract_ssm_builder.py
+-rw-r--r--   0        0        0     8445 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssm/base_ssm.py
+-rw-r--r--   0        0        0     1942 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssm/base_ssm_builder.py
+-rw-r--r--   0        0        0     7587 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/core/ssm/rag_ssm.py
+-rw-r--r--   0        0        0       62 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/README.md
+-rw-r--r--   0        0        0      647 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/api_context.py
+-rw-r--r--   0        0        0     4148 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/azure/ssm.py
+-rw-r--r--   0        0        0     4445 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/huggingface/slm.py
+-rw-r--r--   0        0        0      459 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/huggingface/ssm.py
+-rw-r--r--   0        0        0     2125 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/lepton_ai/ssm.py
+-rw-r--r--   0        0        0     6832 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/llama_index/README.md
+-rw-r--r--   0        0        0     5205 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/llama_index/backend.py
+-rw-r--r--   0        0        0     1883 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/llama_index/ssm.py
+-rw-r--r--   0        0        0     5470 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/integrations/openai/ssm.py
+-rw-r--r--   0        0        0     5235 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/agent/abstract.py
+-rw-r--r--   0        0        0      598 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/agent/agent.py
+-rw-r--r--   0        0        0      109 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/knowledge/fact/abstract.py
+-rw-r--r--   0        0        0      124 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/knowledge/heuristic/abstract.py
+-rw-r--r--   0        0        0      138 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/knowledge/inference_rule/abstract.py
+-rw-r--r--   0        0        0     1153 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/planning/abstract/plan.py
+-rw-r--r--   0        0        0     1225 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/planning/abstract/planner.py
+-rw-r--r--   0        0        0     6477 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/planning/hierarchical/__init__.py
+-rw-r--r--   0        0        0     3390 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/planning/hierarchical/_prompts.py
+-rw-r--r--   0        0        0      327 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/planning/map_reduce/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/planning/map_reduce/_prompts.py
+-rw-r--r--   0        0        0      614 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/reasoning/abstract.py
+-rw-r--r--   0        0        0     1627 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/reasoning/base/__init__.py
+-rw-r--r--   0        0        0      390 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/reasoning/base/_prompts.py
+-rw-r--r--   0        0        0     3006 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/reasoning/ooda/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/reasoning/ooda/_prompts.py
+-rw-r--r--   0        0        0      670 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/_global.py
+-rw-r--r--   0        0        0      629 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/_prompts.py
+-rw-r--r--   0        0        0     1047 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/abstract.py
+-rw-r--r--   0        0        0      215 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/db.py
+-rw-r--r--   0        0        0    11633 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/file.py
+-rw-r--r--   0        0        0      206 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/rss.py
+-rw-r--r--   0        0        0      215 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/sensor.py
+-rw-r--r--   0        0        0      206 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/resource/web.py
+-rw-r--r--   0        0        0     2905 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/task/abstract.py
+-rw-r--r--   0        0        0      215 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/task/status.py
+-rw-r--r--   0        0        0       93 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/task/task.py
+-rw-r--r--   0        0        0       68 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/l2/tool/abstract.py
+-rw-r--r--   0        0        0     1341 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/utils/cli/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/utils/cli/contrib/ssa_prob_solver.py
+-rw-r--r--   0        0        0     2344 2024-04-24 08:04:48.292068 openssa-0.24.4.24/openssa/utils/config.py
+-rw-r--r--   0        0        0     1271 2024-04-24 08:04:48.296068 openssa-0.24.4.24/openssa/utils/deprecated/aitomatic_llm_config.py
+-rw-r--r--   0        0        0    13318 2024-04-24 08:04:48.296068 openssa-0.24.4.24/openssa/utils/deprecated/llama_index_api.py
+-rw-r--r--   0        0        0     7040 2024-04-24 08:04:48.296068 openssa-0.24.4.24/openssa/utils/llms.py
+-rw-r--r--   0        0        0     4627 2024-04-24 08:04:48.296068 openssa-0.24.4.24/openssa/utils/logs.py
+-rw-r--r--   0        0        0     3605 2024-04-24 08:04:48.296068 openssa-0.24.4.24/openssa/utils/rag_service_contexts.py
+-rw-r--r--   0        0        0     1248 2024-04-24 08:04:48.296068 openssa-0.24.4.24/openssa/utils/usage_logger.py
+-rw-r--r--   0        0        0    11700 2024-04-24 08:04:48.296068 openssa-0.24.4.24/openssa/utils/utils.py
+-rw-r--r--   0        0        0     4082 2024-04-24 08:04:48.296068 openssa-0.24.4.24/pyproject.toml
+-rw-r--r--   0        0        0     6419 1970-01-01 00:00:00.000000 openssa-0.24.4.24/PKG-INFO
```

### Comparing `openssa-0.24.3.6/LICENSE.md` & `openssa-0.24.4.24/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/README.md` & `openssa-0.24.4.24/openssa/README.md`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/__init__.py` & `openssa-0.24.4.24/openssa/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import version, PackageNotFoundError
 from pathlib import Path
 import tomllib
 
 from openssa.core.ooda_rag.heuristic import TaskDecompositionHeuristic
-from openssa.core.ooda_rag.solver import OodaSSA
+from openssa.core.ooda_rag.ooda_ssa import OodaSSA
 from openssa.core.prompts import Prompts
 from openssa.core.slm.base_slm import BaseSLM
 from openssa.core.ssa.ssa import BaseSSA
 from openssa.core.ssm.base_ssm import BaseSSM
 from openssa.integrations.azure.ssm import GPT3ChatCompletionSSM as AzureGPT3ChatCompletionSSM
 from openssa.integrations.azure.ssm import GPT3CompletionSSM as AzureGPT3CompletionSSM
 from openssa.integrations.azure.ssm import GPT4ChatCompletionSSM as AzureGPT4ChatCompletionSSM
@@ -21,15 +21,16 @@
 from openssa.integrations.openai.ssm import GPT3CompletionSSM as OpenAIGPT3CompletionSSM
 from openssa.utils.config import Config
 from openssa.utils.logs import Logs, logger, mlogger
 from openssa.utils.utils import Utils
 
 from .l2.agent.agent import Agent
 
-from .l2.planning.abstract import AbstractPlan, AbstractPlanner
+from .l2.planning.abstract.plan import AbstractPlan
+from .l2.planning.abstract.planner import AbstractPlanner
 from .l2.planning.hierarchical import HTP, AutoHTPlanner
 
 from .l2.reasoning.abstract import AbstractReasoner
 from .l2.reasoning.base import BaseReasoner
 from .l2.reasoning.ooda import OodaReasoner
 
 from .l2.resource.abstract import AbstractResource
```

### Comparing `openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/__init__.py` & `openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from uuid import UUID
 
 import streamlit as st
 from streamlit_mic_recorder import speech_to_text
 
 from openssa.core.ooda_rag.heuristic import TaskDecompositionHeuristic
 from openssa.core.ooda_rag.custom import CustomSSM
-from openssa.core.ooda_rag.solver import OodaSSA
-from openssa.utils.fs import DirOrFilePath, FilePathSet, FileSource
+from openssa.core.ooda_rag.ooda_ssa import OodaSSA
+from openssa.l2.resource.file import DirOrFileStrPath, FileStrPathSet, FileResource
 
 if TYPE_CHECKING:
     from collections.abc import Iterable, MutableMapping
     from openssa.core.ssa.ssa import RagSSA
 
 
 # Streamlit Session State alias "SSS" for brevity
@@ -41,16 +41,16 @@
 
 
 class SSAProbSolver:
     """SSA Problem-Solver Streamlit Component."""
 
     # some typing for clarity to developers/maintainers
     # =================================================
-    Uid: type = int | str | UUID  # accepted type(s) for unique IDs of SSAProbSolver instances & SSA conversations
-    DocSrcHash: type = DirOrFilePath | FilePathSet  # type for documentary knowledge source hashes
+    type Uid = int | str | UUID  # accepted type(s) for unique IDs of SSAProbSolver instances & SSA conversations
+    type DocSrcHash = DirOrFileStrPath | FileStrPathSet  # type for documentary knowledge source hashes
 
     # relevant Streamlit Session State (SSS) elements
     # ===============================================
     DOC_SRC_PATHS_SSS_KEY: str = '_doc_src_paths'
     DOC_SRC_FILE_RELPATH_SETS_SSS_KEY: str = '_doc_src_file_relpath_sets'
 
     PROBLEMS_SSS_KEY: str = '_problems'
@@ -58,15 +58,15 @@
     FINE_TUNED_MODELS_SSS_KEY: str = '_fine_tuned_models'
 
     SSAS_SSS_KEY: str = '_ssas'
 
     def __init__(self, unique_name: Uid, domain: str = '',
                  problem: str = '', expert_instructions: str = '',
                  fine_tuned_model_url: str = '',
-                 doc_src_path: DirOrFilePath = '', doc_src_file_relpaths: FilePathSet = frozenset()):
+                 doc_src_path: DirOrFileStrPath = '', doc_src_file_relpaths: FileStrPathSet = frozenset()):
         # pylint: disable=too-many-arguments
         """Initialize and start running SSAProbSolver instance."""
         # initialize Streamlit Session State (SSS) elements if necessary
         # (this has to be done upon each instantiation to avoid missing-state errors on multiple Streamlit sessions)
         self._init_sss()
 
         # set Unique Name
@@ -86,28 +86,28 @@
 
         # set Fine-Tuned Model URL
         if not self.fine_tuned_model_url:
             self.fine_tuned_model_url: str = fine_tuned_model_url
 
         # set Documentary Knowledge Source Path & any specific File Relative Paths if given
         if doc_src_path:
-            self.doc_src_path: DirOrFilePath = doc_src_path
+            self.doc_src_path: DirOrFileStrPath = doc_src_path
             if doc_src_file_relpaths:
-                self.doc_src_file_relpaths: FilePathSet = doc_src_file_relpaths
+                self.doc_src_file_relpaths: FileStrPathSet = doc_src_file_relpaths
 
         # start running in Streamlit app page
         self.run()
 
     @classmethod
     def _init_sss(cls):
         if cls.DOC_SRC_PATHS_SSS_KEY not in sss:
-            sss[cls.DOC_SRC_PATHS_SSS_KEY]: defaultdict[cls.Uid, DirOrFilePath] = defaultdict(str)
+            sss[cls.DOC_SRC_PATHS_SSS_KEY]: defaultdict[cls.Uid, DirOrFileStrPath] = defaultdict(str)
 
         if cls.DOC_SRC_FILE_RELPATH_SETS_SSS_KEY not in sss:
-            sss[cls.DOC_SRC_FILE_RELPATH_SETS_SSS_KEY]: defaultdict[cls.Uid, defaultdict[DirOrFilePath, FilePathSet]] = \
+            sss[cls.DOC_SRC_FILE_RELPATH_SETS_SSS_KEY]: defaultdict[cls.Uid, defaultdict[DirOrFileStrPath, FileStrPathSet]] = \
                 defaultdict(lambda: defaultdict(frozenset))
 
         if cls.PROBLEMS_SSS_KEY not in sss:
             sss[cls.PROBLEMS_SSS_KEY]: defaultdict[cls.Uid, str] = defaultdict(str)
 
         if cls.EXPERT_INSTRUCTIONS_SSS_KEY not in sss:
             sss[cls.EXPERT_INSTRUCTIONS_SSS_KEY]: defaultdict[cls.Uid, str] = defaultdict(str)
@@ -145,42 +145,42 @@
 
     @fine_tuned_model_url.setter
     def fine_tuned_model_url(self, fine_tuned_model_url: str, /):
         if fine_tuned_model_url != sss[self.FINE_TUNED_MODELS_SSS_KEY][self.unique_name]:
             sss[self.FINE_TUNED_MODELS_SSS_KEY][self.unique_name]: str = fine_tuned_model_url
 
     @property
-    def doc_src_path(self) -> DirOrFilePath:
+    def doc_src_path(self) -> DirOrFileStrPath:
         return sss[self.DOC_SRC_PATHS_SSS_KEY][self.unique_name]
 
     @doc_src_path.setter
-    def doc_src_path(self, path: DirOrFilePath, /):
+    def doc_src_path(self, path: DirOrFileStrPath, /):
         assert (clean_path := path.strip().rstrip('/')), ValueError(f'{path} not non-empty path')
 
         if clean_path != sss[self.DOC_SRC_PATHS_SSS_KEY][self.unique_name]:
-            sss[self.DOC_SRC_PATHS_SSS_KEY][self.unique_name]: DirOrFilePath = clean_path
+            sss[self.DOC_SRC_PATHS_SSS_KEY][self.unique_name]: DirOrFileStrPath = clean_path
 
     @property
-    def _doc_file_src(self) -> FileSource:
+    def _doc_file_src(self) -> FileResource:
         assert (_ := self.doc_src_path), ValueError('Documentary Knowledge Source Path not yet specified')
-        return FileSource(_)
+        return FileResource(_)
 
     @property
-    def doc_src_file_relpaths(self) -> FilePathSet:
+    def doc_src_file_relpaths(self) -> FileStrPathSet:
         assert self._doc_file_src.is_dir, ValueError('Documentary Knowledge Source Path not directory')
 
         return sss[self.DOC_SRC_FILE_RELPATH_SETS_SSS_KEY][self.unique_name][self.doc_src_path]
 
     @doc_src_file_relpaths.setter
     def doc_src_file_relpaths(self, file_relpaths: Iterable[str], /):
         assert self._doc_file_src.is_dir, ValueError('Documentary Knowledge Source Path not directory')
 
         if (file_relpath_set := frozenset(file_relpaths)) != \
                 sss[self.DOC_SRC_FILE_RELPATH_SETS_SSS_KEY][self.unique_name][self.doc_src_path]:
-            sss[self.DOC_SRC_FILE_RELPATH_SETS_SSS_KEY][self.unique_name][self.doc_src_path]: FilePathSet = file_relpath_set
+            sss[self.DOC_SRC_FILE_RELPATH_SETS_SSS_KEY][self.unique_name][self.doc_src_path]: FileStrPathSet = file_relpath_set
 
     @property
     def _hashable_doc_src_repr(self) -> DocSrcHash:
         """Return a hashable representation of Documentary Knowledge Source."""
         if self._doc_file_src.is_dir and (doc_src_file_relpaths := self.doc_src_file_relpaths):
             return frozenset(f'{self.doc_src_path}/{_}' for _ in doc_src_file_relpaths)
 
@@ -313,18 +313,18 @@
                                          type='default',
                                          help='Resources Directory/File Path _(Local/S3)_',
                                          autocomplete=None,
                                          on_change=None, args=None, kwargs=None,
                                          placeholder='Resources Directory/File Path (Local|S3)',
                                          disabled=False,
                                          label_visibility='visible'):
-            self.doc_src_path: DirOrFilePath = doc_src_path
+            self.doc_src_path: DirOrFileStrPath = doc_src_path
 
             if self._doc_file_src.is_dir:
-                self.doc_src_file_relpaths: FilePathSet = frozenset(
+                self.doc_src_file_relpaths: FileStrPathSet = frozenset(
                     st.multiselect(label='Specific File Relpaths _(if cherry-picking)_',
                                    options=self._doc_file_src.file_paths(relative=True),
                                    default=sorted(self.doc_src_file_relpaths),
                                    # format_func=None,
                                    key=None,
                                    help='Specific File Relpaths _(if cherry-picking)_',
                                    on_change=None, args=None, kwargs=None,
```

### Comparing `openssa-0.24.3.6/openssa/contrib/streamlit_ssa_prob_solver/pages/Semiconductor_ALD_SSA.py` & `openssa-0.24.4.24/openssa/contrib/streamlit_ssa_prob_solver/pages/Semiconductor_ALD_SSA.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/adapter/abstract_adapter.py` & `openssa-0.24.4.24/openssa/core/adapter/abstract_adapter.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/adapter/base_adapter.py` & `openssa-0.24.4.24/openssa/core/adapter/base_adapter.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/backend/abstract_backend.py` & `openssa-0.24.4.24/openssa/core/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/backend/base_backend.py` & `openssa-0.24.4.24/openssa/core/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/backend/rag_backend.py` & `openssa-0.24.4.24/openssa/core/backend/rag_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from openssa.core.backend.base_backend import BaseBackend
 from openssa.utils.logs import Logs
 from openssa.utils.utils import Utils
 
 
 class AbstractRAGBackend(BaseBackend, ABC):
     def _get_source_dir(self, storage_dir: str):
-        # return os.path.join(storage_dir, ".sources")
         if storage_dir is None:
             storage_dir = './'
         return os.path.abspath(storage_dir)
 
     def _get_index_dir(self, storage_dir: str):
         if storage_dir is None:
             storage_dir = './'
```

### Comparing `openssa-0.24.3.6/openssa/core/backend/text_backend.py` & `openssa-0.24.4.24/openssa/core/backend/text_backend.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/inferencer/abstract_inferencer.py` & `openssa-0.24.4.24/openssa/core/inferencer/abstract_inferencer.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ooda/deprecated/solver.py` & `openssa-0.24.4.24/openssa/core/ooda/deprecated/solver.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ooda/ooda_loop.py` & `openssa-0.24.4.24/openssa/core/ooda/ooda_loop.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ooda/task.py` & `openssa-0.24.4.24/openssa/core/ooda/task.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/builtin_agents.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/builtin_agents.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,31 @@
 
 
 class TaskAgent(ABC):
     """
     Abstract base class for all task agents.
     """
 
+    def __init__(self, llm: AnLLM, messages: List) -> None:
+        self.llm = llm
+        self.messages = messages
+
+    def _execute(self, is_json: bool = True) -> str:
+        """
+        Execute the task agent with the given task.
+        """
+        if is_json:
+            response = self.llm.call(
+                messages=self.messages,
+                response_format={"type": "json_object"},
+            )
+        else:
+            response = self.llm.call(messages=self.messages)
+        return response.choices[0].message.content
+
     @abstractmethod
     def execute(self, task: str) -> str:
         """
         Execute the task agent with the given task.
         """
         pass
 
@@ -63,39 +80,82 @@
         try:
             return json.loads(json_str)
         except json.JSONDecodeError:
             logger.error("Failed to decode the response as JSON for ask user agent.")
             return {}
 
 
-class CommAgent(TaskAgent):
+class AskUserAgentV2(TaskAgent):
     """
-    CommAgent helps update tone, voice, format and language of the assistant final response
+    AskUserAgent helps to determine if user wants to provide additional information
     """
 
     def __init__(
-        self, llm: AnLLM = OpenAILLM(), instruction: str = ""
+        self,
+        llm: AnLLM = OpenAILLM.get_gpt_4_1106_preview(),
+        ask_user_heuristic: str = "",
+        conversation: Optional[List] = None,
     ) -> None:
         self.llm = llm
+        self.ask_user_heuristic = ask_user_heuristic.strip()
+        self.conversation = conversation[-10:] if conversation else []
+
+    @Utils.timeit
+    def execute(self, task: str = "") -> str:
+        if not self.ask_user_heuristic:
+            return ""
+        system_message = {
+            "role": Persona.SYSTEM,
+            "content": BuiltInAgentPrompt.ASK_USER.format(
+                heuristic=self.ask_user_heuristic
+            ),
+        }
+        messages = self.conversation + [system_message]
+        response = self.llm.call(
+            messages=messages,
+            response_format={"type": "json_object"},
+        )
+        json_str = response.choices[0].message.content
+        logger.debug(f"ask user response is: {json_str}")
+        try:
+            return json.loads(json_str).get("question", "")
+        except json.JSONDecodeError:
+            logger.error("Failed to decode the response as JSON for ask user agent.")
+            return ""
+
+
+class CommAgent(TaskAgent):
+    """
+    CommAgent helps update tone, voice, format and language of the assistant final response
+    """
+
+    def __init__(self, llm: AnLLM = OpenAILLM(), instruction: str = "") -> None:
+        self.llm = llm
         self.instruction = instruction
 
     @Utils.timeit
     def execute(self, task: str = "") -> str:
         system_message = {
             "role": Persona.SYSTEM,
             "content": BuiltInAgentPrompt.COMMUNICATION.format(
                 instruction=self.instruction, message=task
             ),
         }
         conversation = [system_message]
         response = self.llm.call(
             messages=conversation,
-            response_format={"type": "text"},
+            response_format={"type": "json_object"},
         )
-        return response.choices[0].message.content
+        json_str = response.choices[0].message.content
+        logger.debug(f"comm response is: {json_str}")
+        try:
+            return json.loads(json_str).get("message", "")
+        except json.JSONDecodeError:
+            logger.error("Failed to decode the response as JSON for ask comm agent.")
+            return task
 
 
 class GoalAgent(TaskAgent):
     """
     GoalAgent helps to determine problem statement from the conversation between user and SSA
     """
```

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/custom.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
             recursive=True,  # non-default
             encoding="utf-8",
             filename_as_id=True,
             required_exts=None,
             file_extractor=None,
             num_files_limit=None,
             file_metadata=filename_fn,
-        ).load_data()
+        ).load_data(show_progress=True)
+
         self.documents = documents
         self._create_index(documents, storage_dir)
 
     def get_citation_type(self, filename: str) -> str:
         extension = filename.split(".")[-1]
         return extension.strip().lower() if extension else "unknown"
```

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/heuristic.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/heuristic.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/notifier.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/notifier.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/ooda_rag.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/ooda.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/prompts.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,78 +67,84 @@
 
 class BuiltInAgentPrompt:
     COMMUNICATION = (
         "You are an expert in communication. Your will help to format following message with this instruction:\n"
         "###{instruction}###\n\n"
         "Here is the message:\n"
         "###{message}###\n\n"
+        "Output the response in JSON format with the keyword 'message'."
     )
 
     PROBLEM_STATEMENT = (
-        "You are tasked with constructing the problem statement from a conversation "
-        "between a user and an AI chatbot. Your focus should be on the entire context "
-        "of the conversation, especially the most recent messages from the user, "
-        "to understand the issue comprehensively. Extract specific details "
-        "that define the current concerns or questions posed by the user, "
-        "which the assistant is expected to address. The problem statement should be "
-        "clear, and constructed carefully with complete context and in the user's voice. "
-        'Output the response in JSON format with the keyword "problem statement". Think step by step.\n'
-        "Example 1:\n"
-        "Assistant: Hello, what can I help you with today?\n"
-        "User: My boiler is not functioning, please help to troubleshoot.\n"
-        "Assistant: Can you check and provide the temperature, pressure, and on-off status?\n"
-        "User: The temperature is 120°C.\n\n"
-        "Response:\n"
-        "{\n"
-        '    "problem statement": "Can you help to troubleshoot a non-functioning '
-        'boiler, given the temperature is 120°C?"\n'
-        "}\n\n"
-        "Example 2:\n"
-        "Assistant: Hi, what can I help you with?\n"
-        "User: I don't know how to go to the airport\n"
-        "Assistant: Where are you and which airport do you want to go to?\n"
-        "User: I'm in New York\n"
-        "Response:\n"
-        "{\n"
-        '    "problem statement": "How do I get to the airport from my current '
-        'location in New York?"\n'
-        "}\n\n"
-        "Example 3 (Ambiguity):\n"
-        "Assistant: How can I assist you today?\n"
-        "User: I'm not sure what's wrong, but my computer is acting weird.\n"
-        "Assistant: Can you describe the issues you are experiencing?\n"
-        "User: Hey I am good, the sky is blue.\n\n"
+        "Formulate a concise problem statement from the most recent question asked by a user in a conversation "
+        "with an AI expert. Focus on the question that remains unanswered (Question B), "
+        "ignoring any questions that have already been addressed (Question A). The problem statement should be "
+        "direct and to the point, avoiding any additional explanatory text or context not explicitly mentioned "
+        "by the user. Ensure to correct any spelling or grammatical errors, and replace pronouns or ambiguous terms "
+        "with precise names or technical terms. The outcome should be "
+        "a succinct problem statement, accurately reflecting the user's query for use in a retrieval system. "
+        "Format the response in JSON, clearly labeled as 'problem statement'.\n\n"
+        "Example:\n"
+        "User: What is the flow rate for Argon in machine XYZ? (Question A)\n"
+        "Assistant: The flow rate for Argon is 500 cm^3 per minute.\n"
+        "User: Can you also give me its velocity? (Question B)\n\n"
         "Response:\n"
         "{\n"
-        '    "problem statement": ""\n'
+        '    "problem statement": "What is the velocity of Argon in machine XYZ."\n'
         "}\n\n"
-        "Example 4 (Multiple Issues):\n"
-        "Assistant: What do you need help with?\n"
-        "User: My internet is down, and I can't access my email either.\n"
-        "Assistant: Are both issues related, or did they start separately?\n"
-        "User: They started at the same time, I think.\n\n"
-        "Response:\n"
-        "{\n"
-        '    "problem statement": "Can you help with my internet being down and also '
-        'accessing my email?"\n'
-        "}"
     )
 
+    # ASK_USER = (
+    #     "Your task is to assist an AI assistant in formulating a question for the user. "
+    #     "This should be based on the ongoing conversation, the presented problem statement, "
+    #     "and a specific heuristic guideline. "
+    #     "The assistant should formulate the question strictly based on the heuristic. "
+    #     "If the heuristic does not apply or is irrelevant to the problem statement, "
+    #     "return empty string for the question. "
+    #     "Below is the heuristic guideline:\n"
+    #     "###{heuristic}###\n\n"
+    #     "Here is the problem statement or the user's current question:\n"
+    #     "###{problem_statement}###\n\n"
+    #     'Output the response in JSON format with the keyword "question".'
+    # )
+
     ASK_USER = (
-        "Your task is to assist an AI assistant in formulating a question for the user. "
-        "This should be based on the ongoing conversation, the presented problem statement, "
-        "and a specific heuristic guideline. "
-        "The assistant should formulate the question strictly based on the heuristic. "
-        "If the heuristic does not apply or is irrelevant to the problem statement, "
-        "return empty string for the question. "
-        "Below is the heuristic guideline:\n"
+        "Your task is to generate a question for the user to gather necessary "
+        "information for troubleshooting or solving their problem, based on the "
+        "ongoing conversation. Follow the heuristic guidelines closely to "
+        "determine the relevance and necessity of asking a question. If the "
+        "discussion does not align with these guidelines or the required "
+        "information has already been addressed and the user has indicated "
+        "ignorance on the matter, you should refrain from asking a question. "
+        "In such cases, produce an output with an empty 'question' field in JSON "
+        "format. Ask questions judiciously, only when the conditions explicitly "
+        "meet the heuristic criteria.\n"
+        "Guidelines for Question Generation:\n"
+        "1. Relevance: Ensure the question is directly related to the user's "
+        "stated issue.\n"
+        "2. Condition Clarity: Only ask if the scenario clearly matches the "
+        "heuristics.\n"
+        "3. Non-redundancy: Avoid repeating questions already answered or where "
+        "the user expressed ignorance.\n"
+        "4. Output Format: Provide the question in a JSON object with the keyword "
+        "'question'. If no question is warranted, return an empty 'question' value.\n\n"
+        "Example 1:\n"
+        '- User says: "My printer is not working, can you help me fix it?"\n'
+        "- Heuristic guideline: Ask for the printer model if the user seeks help "
+        "with a printer issue but does not specify the model.\n"
+        "- Output:\n"
+        '{{ "question": "Could you provide the printer model?" }}\n\n'
+        "Example 2:\n"
+        '- User says: "I couldn\'t open the cabin of my car, can you help?"\n'
+        "- Heuristic guideline: Ask about boiler's status and external "
+        "conditions if the user is seeking help with mechanical troubleshooting.\n"
+        "- Output:\n"
+        '{{ "question": "" }}\n\n'
+        "Below is the heuristic guideline:\n\n"
         "###{heuristic}###\n\n"
-        "Here is the problem statement or the user's current question:\n"
-        "###{problem_statement}###\n\n"
-        'Output the response in JSON format with the keyword "question".'
     )
 
     ASK_USER_OODA = (
         "Your task is to assist an AI assistant in formulating a question for the user. "
         "This is done through using OODA reasoning. "
         "This should be based on the ongoing conversation, the presented problem statement, "
         "and a specific heuristic guideline. "
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/query_rewritting_engine.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/query_rewritting_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     """
 
     def __init__(
         self,
         index: VectorStoreIndex = None,  # type: ignore
         chunk_size: int = 1024,
-        vector_similarity_top_k: int = 5,
+        vector_similarity_top_k: int = 10,
         fusion_similarity_top_k: int = 10,
         service_context: ServiceContext = None,
         **kwargs: Any,
     ) -> None:
         """Init params."""
         if not service_context:
             service_context = ServiceContextManager.get_openai_sc(chunk_size=chunk_size)
```

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/solver.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/ooda_ssa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 from openssa.core.ooda_rag.custom import CustomSSM
-from openssa.core.ooda_rag.ooda_rag import Solver, History
+from openssa.core.ooda_rag.ooda import Solver, History
 from openssa.core.ooda_rag.heuristic import (
     Heuristic,
     TaskDecompositionHeuristic,
     HeuristicSet,
 )
 from openssa.core.ooda_rag.tools import ReasearchAgentTool, Tool
 from openssa.core.ooda_rag.builtin_agents import GoalAgent, Persona, AskUserAgent
```

### Comparing `openssa-0.24.3.6/openssa/core/ooda_rag/tools.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/tools.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/prompts.py` & `openssa-0.24.4.24/openssa/core/prompts.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/rag_ooda/rag_ooda.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/rag_ooda.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     AnswerValidator,
     GoalAgent,
 )
 from openssa.core.ooda_rag.tools import (
     ResearchQueryEngineTool,
     Tool,
 )
-from openssa.core.rag_ooda.resources.rag_resource import RagResource
-from openssa.core.ooda_rag.ooda_rag import Solver, Notifier, SimpleNotifier, EventTypes
+from openssa.core.ooda_rag.resources.rag_resource import RagResource
+from openssa.core.ooda_rag.ooda import Solver, Notifier, SimpleNotifier, EventTypes
 from openssa.utils.utils import Utils
 
 
 class RagOODA:
     _conversations: ClassVar[dict] = {}
 
     @classmethod
```

### Comparing `openssa-0.24.3.6/openssa/core/rag_ooda/resources/dense_x/base.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/resources/dense_x/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def __init__(
         self,
         documents: List[Document],
         proposition_llm: Optional[LLM] = None,
         query_llm: Optional[LLM] = None,
         embed_model: Optional[BaseEmbedding] = None,
         text_splitter: TextSplitter = SentenceSplitter(),
-        similarity_top_k: int = 4,
+        similarity_top_k: int = 10,
     ) -> None:
         """Init params."""
         self._proposition_llm = proposition_llm or OpenAI(
             model="gpt-3.5-turbo",
             temperature=0.1,
             max_tokens=750,
         )
```

### Comparing `openssa-0.24.3.6/openssa/core/rag_ooda/resources/dense_x/dense_x.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/resources/dense_x/dense_x.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from llama_index.core import SimpleDirectoryReader
 from llama_index.llms.openai import OpenAI
 from openssa.utils.utils import Utils
 from llama_index.core import StorageContext, load_index_from_storage, ServiceContext
 from llama_index.core.retrievers import RecursiveRetriever
 from llama_index.core.query_engine import RetrieverQueryEngine
 from llama_index.core.node_parser import SentenceSplitter
-from openssa.core.rag_ooda.resources.dense_x.base import (
+from openssa.core.ooda_rag.resources.dense_x.base import (
     DenseXRetrievalPack,
     load_nodes_dict,
     store_nodes_dict,
 )
-from openssa.core.rag_ooda.resources.rag_resource import RagResource
+from openssa.core.ooda_rag.resources.rag_resource import RagResource
 
 
 @Utils.timeit
 def load_dense_x(data_dir: str, cache_dir: str, nodes_cache_path: str) -> RagResource:
     if (
         cache_dir is not None
         and os.path.exists(cache_dir)
```

### Comparing `openssa-0.24.3.6/openssa/core/rag_ooda/resources/standard_vi/standard_vi.py` & `openssa-0.24.4.24/openssa/core/ooda_rag/resources/standard_vi/standard_vi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os.path
 from llama_index.core import VectorStoreIndex, SimpleDirectoryReader, StorageContext, load_index_from_storage
-from openssa.core.rag_ooda.resources.rag_resource import RagResource
+from openssa.core.ooda_rag.resources.rag_resource import RagResource
 from openssa.utils.utils import Utils
 
 
 @Utils.timeit
 def load_standard_vi(data_dir: str, cache_dir: str) -> RagResource:
     if not os.path.exists(cache_dir):
         documents = SimpleDirectoryReader(data_dir).load_data()
```

### Comparing `openssa-0.24.3.6/openssa/core/slm/abstract_slm.py` & `openssa-0.24.4.24/openssa/core/slm/abstract_slm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/slm/base_slm.py` & `openssa-0.24.4.24/openssa/core/slm/base_slm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/slm/memory/sqlite_conversation_db.py` & `openssa-0.24.4.24/openssa/core/slm/memory/sqlite_conversation_db.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssa/agent.py` & `openssa-0.24.4.24/openssa/core/ssa/agent.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssa/rag_ssa.py` & `openssa-0.24.4.24/openssa/core/ssa/rag_ssa.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssa/ssa.py` & `openssa-0.24.4.24/openssa/core/ssa/ssa.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssa/ssa_service.py` & `openssa-0.24.4.24/openssa/core/ssa/ssa_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def chat(cls, message, config=None) -> str:
         """Chat with a Small Specialist Agent."""
         # NOTE: before using chat, the model must be deploy after train
 
         config = config or {}
         payload = {
             "user_input": message,
-            "endpoint_name": config.get("endpoint_name"),
+            "endpoint_name": config.get("endpoint_name")
         }
 
         aiso_url = config.get("aiso_url") or SSAService.AIMO_API_URL
 
         with httpx.Client() as client:
             response = client.post(aiso_url + "/api/chat", json=payload)
 
@@ -69,21 +69,22 @@
         with httpx.Client(timeout=5000) as client:
             response = client.post(
                 SSAService.AIMO_API_URL + "/api/agents/create", json=payload
             )
             return response.json()
 
     @classmethod
-    def chat(cls, agent_id: str, message: str) -> str:
+    def chat(cls, agent_id: str, message: str, **kwargs) -> str:
         """Chat with a Small Specialist Agent."""
         # NOTE: before using chat, the model must be deploy after train
 
         payload = {
             "message": message,
             "agent_id": agent_id,
+            **kwargs
         }
 
         aiso_url = SSAService.AIMO_API_URL
         with httpx.Client(timeout=5000) as client:
             response = client.post(aiso_url + "/api/agents/chat", json=payload)
             return response.json()
```

### Comparing `openssa-0.24.3.6/openssa/core/ssm/abstract_ssm.py` & `openssa-0.24.4.24/openssa/core/ssm/abstract_ssm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssm/abstract_ssm_builder.py` & `openssa-0.24.4.24/openssa/core/ssm/abstract_ssm_builder.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssm/base_ssm.py` & `openssa-0.24.4.24/openssa/core/ssm/base_ssm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssm/base_ssm_builder.py` & `openssa-0.24.4.24/openssa/core/ssm/base_ssm_builder.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/core/ssm/rag_ssm.py` & `openssa-0.24.4.24/openssa/core/ssm/rag_ssm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/integrations/api_context.py` & `openssa-0.24.4.24/openssa/integrations/api_context.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/integrations/azure/ssm.py` & `openssa-0.24.4.24/openssa/integrations/azure/ssm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/integrations/huggingface/slm.py` & `openssa-0.24.4.24/openssa/integrations/huggingface/slm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/integrations/lepton_ai/ssm.py` & `openssa-0.24.4.24/openssa/integrations/lepton_ai/ssm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/integrations/llama_index/README.md` & `openssa-0.24.4.24/openssa/integrations/llama_index/README.md`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/integrations/llama_index/backend.py` & `openssa-0.24.4.24/openssa/integrations/llama_index/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from dataclasses import dataclass
+from multiprocessing import cpu_count
+
 from llama_index.core import (
     load_index_from_storage,
     SimpleDirectoryReader,
     VectorStoreIndex,
     Response,
     ServiceContext,
 )
@@ -15,15 +17,15 @@
 
 
 @dataclass
 class Backend(AbstractRAGBackend):
     def __init__(
         self,
         relevance_threshold: float = 0.5,
-        similarity_top_k: int = 4,
+        similarity_top_k: int = 10,
         service_context: ServiceContext = None,
     ):
         """
         Initialize the backend.
 
         @param relevance_threshold: The relevance threshold for the MMR query engine.
         0-1 (default: 0.5) The higher the threshold, the stricter the document relevance requirement.
@@ -98,25 +100,29 @@
             documents, service_context=self._service_context, show_progress=True
         )
 
     def _do_read_directory(self, storage_dir: str):
         documents = SimpleDirectoryReader(
             input_dir=self._get_source_dir(storage_dir),
             input_files=None,
-            exclude=None,
+            exclude=[
+                '.DS_Store',  # MacOS
+                '*.json',  # potential nested index files
+            ],
             exclude_hidden=False,  # non-default
             errors="strict",  # non-default
             recursive=True,  # non-default
             encoding="utf-8",
             filename_as_id=False,
             required_exts=None,
             file_extractor=None,
             num_files_limit=None,
             file_metadata=None,
-        ).load_data(num_workers=5)
+        ).load_data(show_progress=True,
+                    num_workers=cpu_count())
 
         self._create_index(documents, storage_dir)
 
     def _do_read_website(self, urls: list[str], storage_dir: str):
         documents = SimpleWebPageReader(html_to_text=True).load_data(urls)
         self._create_index(documents, storage_dir)
```

### Comparing `openssa-0.24.3.6/openssa/integrations/llama_index/ssm.py` & `openssa-0.24.4.24/openssa/integrations/llama_index/ssm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/integrations/openai/ssm.py` & `openssa-0.24.4.24/openssa/integrations/openai/ssm.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/l2/planning/hierarchical/__init__.py` & `openssa-0.24.4.24/openssa/l2/planning/hierarchical/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,149 @@
 """Hierarchical task-planning classes."""
 
 
 from __future__ import annotations
 
-from dataclasses import dataclass, asdict, field
+from dataclasses import dataclass, field
 import json
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, TypedDict, Required, NotRequired
 
 from loguru import logger
 from tqdm import tqdm
 
-from openssa.l2.planning.abstract import AbstractPlan, AbstractPlanner
+from openssa.l2.planning.abstract.plan import AbstractPlan, AskAnsPair
+from openssa.l2.planning.abstract.planner import AbstractPlanner
 from openssa.l2.reasoning.base import BaseReasoner
-from openssa.l2.task.abstract import TaskDict
 from openssa.l2.task.status import TaskStatus
 from openssa.l2.task.task import Task
 
 from ._prompts import (HTP_PROMPT_TEMPLATE, HTP_WITH_RESOURCES_PROMPT_TEMPLATE, HTP_UPDATE_RESOURCES_PROMPT_TEMPLATE,
                        HTP_RESULTS_SYNTH_PROMPT_TEMPLATE)
 
 if TYPE_CHECKING:
-    from openssa.l2.reasoning.abstract import AbstractReasoner
-    from openssa.l2.resource.abstract import AbstractResource
+    from openssa.l2.reasoning.abstract import AReasoner
+    from openssa.l2.resource.abstract import AResource
+    from openssa.l2.task.abstract import TaskDict
 
 
-HTPDict: type = dict[str, TaskDict | str | list[dict]]
+class HTPDict(TypedDict, total=False):
+    task: Required[TaskDict | str]
+    sub_plans: NotRequired[list[HTPDict]]
 
 
-@dataclass(init=True,
-           repr=True,
-           eq=True,
-           order=False,
-           unsafe_hash=False,
-           frozen=False,  # mutable
-           match_args=True,
-           kw_only=False,
-           slots=False,
-           weakref_slot=False)
+@dataclass
 class HTP(AbstractPlan):
     """Hierarchical task plan (HTP)."""
 
-    sub_plans: list[HTP] = field(default_factory=list,
-                                 init=True,
-                                 repr=True,
-                                 hash=False,  # mutable
-                                 compare=True,
-                                 metadata=None,
-                                 kw_only=True)
-
     @classmethod
     def from_dict(cls, htp_dict: HTPDict, /) -> HTP:
-        """Create hierarchical task plan from dictionary representation."""
+        """Create HTP from dictionary representation."""
         return HTP(task=Task.from_dict_or_str(htp_dict['task']),  # pylint: disable=unexpected-keyword-arg
                    sub_plans=[HTP.from_dict(d) for d in htp_dict.get('sub-plans', [])])
 
     def to_dict(self) -> HTPDict:
-        """Return dictionary representation."""
-        return {'task': asdict(self.task),
+        """Return dictionary representation of HTP."""
+        return {'task': self.task.to_json_dict(),
                 'sub-plans': [p.to_dict() for p in self.sub_plans]}
 
     def fix_missing_resources(self):
         """Fix missing resources in HTP."""
         for p in self.sub_plans:
-            if not p.task.resource:
-                p.task.resource: AbstractResource | None = self.task.resource
+            if not p.task.resources:
+                p.task.resources: set[AResource] = self.task.resources
             p.fix_missing_resources()
 
-    def execute(self, reasoner: AbstractReasoner = BaseReasoner()) -> str:
+    def execute(self, reasoner: AReasoner = BaseReasoner(), other_results: list[AskAnsPair] | None = None) -> str:
         """Execute and return result, using specified reasoner to reason through involved tasks."""
+        reasoning_wo_sub_results: str = reasoner.reason(self.task)
+
         if self.sub_plans:
-            sub_results: tuple[str, str] = ((p.task.ask, p.execute(reasoner)) for p in tqdm(self.sub_plans))
+            sub_results: list[AskAnsPair] = []
+            for p in tqdm(self.sub_plans):
+                sub_results.append((p.task.ask, (p.task.result
+                                                 if p.task.status == TaskStatus.DONE
+                                                 else p.execute(reasoner, other_results=sub_results))))
 
             prompt: str = HTP_RESULTS_SYNTH_PROMPT_TEMPLATE.format(
                 ask=self.task.ask,
-                supporting_info='\n\n'.join((f'SUPPORTING QUESTION/TASK #{i + 1}:\n{ask}\n'
-                                             '\n'
-                                             f'SUPPORTING RESULT #{i + 1}:\n{result}\n')
-                                            for i, (ask, result) in enumerate(sub_results)))
+                info=(f'REASONING WITHOUT FURTHER SUPPORTING RESULTS:\n{reasoning_wo_sub_results}\n'
+                      '\n\n' +
+                      '\n\n'.join((f'SUPPORTING QUESTION/TASK #{i + 1}:\n{ask}\n'
+                                   '\n'
+                                   f'SUPPORTING RESULT #{i + 1}:\n{result}\n')
+                                  for i, (ask, result) in enumerate(sub_results)) +
+                      (('\n\n' +
+                        '\n\n'.join((f'OTHER QUESTION/TASK #{i + 1}:\n{ask}\n'
+                                     '\n'
+                                     f'OTHER RESULT #{i + 1}:\n{result}\n')
+                                    for i, (ask, result) in enumerate(other_results)))
+                       if other_results
+                       else '')))
             logger.debug(prompt)
 
             self.task.result: str = reasoner.lm.get_response(prompt)
 
         else:
-            self.task.result: str = reasoner.reason(self.task)
+            self.task.result: str = reasoning_wo_sub_results
 
         self.task.status: TaskStatus = TaskStatus.DONE
         return self.task.result
 
 
-@dataclass(init=True,
-           repr=True,
-           eq=True,
-           order=False,
-           unsafe_hash=False,
-           frozen=False,  # mutable
-           match_args=True,
-           kw_only=False,
-           slots=False,
-           weakref_slot=False)
+@dataclass
 class AutoHTPlanner(AbstractPlanner):
     """Automated (generative) hierarchical task planner."""
 
-    max_depth: int = 3
-    max_subtasks_per_decomp: int = 9
+    def one_level_deep(self) -> AutoHTPlanner:
+        """Make 1-level-deep planner."""
+        return AutoHTPlanner(lm=self.lm,
+                             max_depth=1,
+                             max_subtasks_per_decomp=self.max_subtasks_per_decomp)
+
+    def one_fewer_level_deep(self) -> AutoHTPlanner:
+        """Make 1-fewer-level-deep planner."""
+        return AutoHTPlanner(lm=self.lm,
+                             max_depth=self.max_depth - 1,
+                             max_subtasks_per_decomp=self.max_subtasks_per_decomp)
 
-    def plan(self, problem: str, resources: set[AbstractResource] | None = None) -> HTP:
-        """Make hierarchical task plan (HTP) for solving problem."""
+    def plan(self, problem: str, resources: set[AResource] | None = None) -> HTP:
+        """Make HTP for solving problem."""
         prompt: str = (
             HTP_WITH_RESOURCES_PROMPT_TEMPLATE.format(problem=problem,
                                                       resource_overviews={r.unique_name: r.overview for r in resources},
                                                       max_depth=self.max_depth,
                                                       max_subtasks_per_decomp=self.max_subtasks_per_decomp)
             if resources
             else HTP_PROMPT_TEMPLATE.format(problem=problem,
                                             max_depth=self.max_depth,
                                             max_subtasks_per_decomp=self.max_subtasks_per_decomp)
         )
 
-        # TODO: more rigorous JSON schema validation
         htp_dict: HTPDict = {}
-        while not htp_dict:
+        while not (isinstance(htp_dict, dict) and htp_dict):
             htp_dict: HTPDict = self.lm.parse_output(self.lm.get_response(prompt))
 
         htp: HTP = HTP.from_dict(htp_dict)
 
         if resources:
             htp.fix_missing_resources()
 
         return htp
 
-    def update_plan_resources(self, plan: HTP, /, resources: set[AbstractResource]) -> HTP:
-        """Make updated hierarchical task plan (HTP) copy with relevant informational resources."""
+    def update_plan_resources(self, plan: HTP, /, resources: set[AResource]) -> HTP:
+        """Make updated HTP copy with relevant informational resources."""
         assert isinstance(plan, HTP), TypeError(f'*** {plan} NOT OF TYPE {HTP.__name__} ***')
         assert resources, ValueError(f'*** {resources} NOT A NON-EMPTY SET OF INFORMATIONAL RESOURCES ***')
 
         prompt: str = HTP_UPDATE_RESOURCES_PROMPT_TEMPLATE.format(resource_overviews={r.unique_name: r.overview
                                                                                       for r in resources},
                                                                   htp_json=json.dumps(obj=plan.to_dict()))
 
-        # TODO: more rigorous JSON schema validation
         updated_htp_dict: HTPDict = {}
-        while not updated_htp_dict:
+        while not (isinstance(updated_htp_dict, dict) and updated_htp_dict):
             updated_htp_dict: HTPDict = self.lm.parse_output(self.lm.get_response(prompt))
 
         updated_htp: HTP = HTP.from_dict(updated_htp_dict)
 
         updated_htp.fix_missing_resources()
 
         return updated_htp
```

### Comparing `openssa-0.24.3.6/openssa/l2/planning/hierarchical/_prompts.py` & `openssa-0.24.4.24/openssa/l2/planning/hierarchical/_prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 HTP_JSON_TEMPLATE: str = """
 {{
-    "task": "(textual description of problem/task to solve)",
+    "task": "(textual description of question/problem/task to answer/solve)",
     "sub-plans": [
         {{
-            "task": "(textual description of 1st sub-problem/sub-task to solve)",
+            "task": "(textual description of 1st sub-question/problem/task to answer/solve)",
             "sub-plans": [
                 (... nested sub-plans ...)
             ]
         }},
         {{
-            "task": "(textual description of 2nd sub-problem/sub-task to solve)",
+            "task": "(textual description of 2nd sub-question/problem/task to answer/solve)",
             "sub-plans": [
                 (... nested sub-plans ...)
             ]
         }},
         ...
     ]
 }}
 """
 
 HTP_WITH_RESOURCES_JSON_TEMPLATE: str = """
 {{
     "task": {{
-        "ask": "(textual description of problem/task to solve)"
+        "ask": "(textual description of question/problem/task to answer/solve)"
     }},
     "sub-plans": [
         {{
             "task": {{
-                "ask": "(textual description of 1st sub-problem/sub-task to solve)",
-                "resource": "(unique name of most relevant informational resource, IF ANY)" OR null
+                "ask": "(textual description of 1st sub-question/problem/task to answer/solve)",
+                "resources": [
+                    (... unique names of most relevant informational resources, if any ...)
+                ]
             }},
             "sub-plans": [
                 (... nested sub-plans ...)
             ]
         }},
         {{
             "task": {{
-                "ask": "(textual description of 2nd sub-problem/sub-task to solve)",
-                "resource": "(unique name of most relevant informational resource, IF ANY)" OR null
+                "ask": "(textual description of 2nd sub-question/problem/task to answer/solve)",
+                "resources": [
+                    (... unique names of most relevant informational resources, if any ...)
+                ]
             }},
             "sub-plans": [
                 (... nested sub-plans ...)
             ]
         }},
         ...
     ]
@@ -83,16 +87,17 @@
 
 HTP_WITH_RESOURCES_PROMPT_TEMPLATE: str = RESOURCE_OVERVIEW_PROMPT_SECTION + htp_prompt_template(with_resources=True)
 
 
 HTP_UPDATE_RESOURCES_PROMPT_TEMPLATE: str = (
 RESOURCE_OVERVIEW_PROMPT_SECTION +  # noqa: E122
 """please return an updated version of the following JSON hierarchical task plan
-by appropriately replacing `"resource": null` with `"resource": "(unique name of most relevant informational resource)"`
-for any case in which such a relevant informational resource can be identified for the corresponding problem/task:
+by appropriately replacing `"resources": null` or `"resources": []`
+with `"resources": [(... unique names of most relevant informational resources ...)]`
+for any case in which such relevant informational resource(s) can be identified for the corresponding question/problem/task:
 
 ```json
 {htp_json}
 ```
 
 Please return ONLY the UPDATED JSON DICTIONARY and no other text, not even the "```json" wrapping!
 """  # noqa: E122
@@ -102,14 +107,14 @@
 HTP_RESULTS_SYNTH_PROMPT_TEMPLATE: str = (
 """Synthesize an answer/solution for the following question/problem/task:
 
 ```
 {ask}
 ```
 
-given the following supporting information:
+given the following collection of reasoning and results:
 
 ```
-{supporting_info}
+{info}
 ```
 """  # noqa: E122
 )
```

### Comparing `openssa-0.24.3.6/openssa/l2/reasoning/abstract.py` & `openssa-0.24.4.24/openssa/l2/reasoning/abstract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Abstract reasoner."""
 
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
+from typing import TypeVar
 
-from openssa.l2.task.task import Task
+from openssa.l2.task.abstract import ATask
 from openssa.utils.llms import AnLLM, OpenAILLM
 
 
-@dataclass(init=True,
-           repr=True,
-           eq=True,
-           order=False,
-           unsafe_hash=False,
-           frozen=False,  # mutable
-           match_args=True,
-           kw_only=False,
-           slots=False,
-           weakref_slot=False)
+@dataclass
 class AbstractReasoner(ABC):
     """Abstract reasoner."""
 
     lm: AnLLM = field(default_factory=OpenAILLM.get_gpt_4_1106_preview)
 
     @abstractmethod
-    def reason(self, task: Task) -> str:
+    def reason(self, task: ATask, n_words: int = 1000) -> str:
         """Reason through task and return conclusion."""
+
+
+AReasoner: TypeVar = TypeVar('AReasoner', bound=AbstractReasoner, covariant=False, contravariant=False)
```

### Comparing `openssa-0.24.3.6/openssa/l2/resource/_global.py` & `openssa-0.24.4.24/openssa/l2/resource/_global.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Global informational resources register."""
 
 
 from typing import TYPE_CHECKING
 
-from .abstract import AbstractResource
+from .abstract import AResource
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
 
-GLOBAL_RESOURCES: dict[str, AbstractResource] = {}
+GLOBAL_RESOURCES: dict[str, AResource] = {}
 
 
 def global_register(resource_class):
     orig_init: Callable[..., None] = resource_class.__init__
 
     def wrapped_init(self, *args, **kwargs) -> None:
         orig_init(self, *args, **kwargs)  # pylint: disable=unnecessary-dunder-call
 
-        assert self.unique_name not in GLOBAL_RESOURCES, \
-            KeyError(f'*** RESOURCE UNIQUE NAME CONFLICT: "{self.unique_name}"')
-        GLOBAL_RESOURCES[self.unique_name]: AbstractResource = self
+        if self.unique_name not in GLOBAL_RESOURCES:
+            GLOBAL_RESOURCES[self.unique_name]: AResource = self
 
     resource_class.__init__: Callable[..., None] = wrapped_init
 
     return resource_class
```

### Comparing `openssa-0.24.3.6/openssa/l2/resource/abstract.py` & `openssa-0.24.4.24/openssa/l2/resource/abstract.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Abstract informational resource."""
 
 
 from abc import ABC, abstractmethod
 from functools import cached_property
+from typing import TypeVar
 
 from ._prompts import RESOURCE_OVERVIEW_PROMPT_TEMPLATE
 
 
 class AbstractResource(ABC):
     """Abstract informational resource."""
 
     @cached_property
     @abstractmethod
     def unique_name(self) -> str:
-        """Return globally-unique name."""
+        """Return globally-unique name of informational resource."""
 
     @cached_property
     @abstractmethod
     def name(self) -> str:
-        """Return potentially non-unique, but informationally helpful name."""
+        """Return potentially non-unique, but informationally helpful name of informational resource."""
 
     @abstractmethod
-    def answer(self, question: str) -> str:
+    def answer(self, question: str, n_words: int = 1000) -> str:
         """Answer question from informational resource."""
 
     @cached_property
-    def overview(self):
+    def overview(self) -> str:
         """Return overview of informational resource."""
         return self.answer(question=RESOURCE_OVERVIEW_PROMPT_TEMPLATE.format(name=self.name))
+
+
+AResource: TypeVar = TypeVar('AResource', bound=AbstractResource, covariant=False, contravariant=False)
```

### Comparing `openssa-0.24.3.6/openssa/l2/task/abstract.py` & `openssa-0.24.4.24/openssa/l2/task/abstract.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,87 @@
 """Abstract task."""
 
 
+from __future__ import annotations
+
 from abc import ABC
-from dataclasses import dataclass
-from typing import Self
+from dataclasses import dataclass, asdict, field
+from typing import TYPE_CHECKING, Self, TypedDict, Required, NotRequired, TypeVar
 
-from openssa.l2.resource.abstract import AbstractResource
+from openssa.l2.planning.abstract.planner import AbstractPlanner
 from openssa.l2.resource._global import GLOBAL_RESOURCES
 
 from .status import TaskStatus
 
+if TYPE_CHECKING:
+    from openssa.l2.planning.abstract.plan import APlan
+    from openssa.l2.planning.abstract.planner import APlanner
+    from openssa.l2.resource.abstract import AResource
+
 
-TaskDict: type = dict[str, str | AbstractResource | TaskStatus | None]
+class TaskDict(TypedDict, total=False):
+    ask: Required[str]
+    resources: NotRequired[set[AResource]]
+    status: NotRequired[TaskStatus]
+    result: NotRequired[str]
+    dynamic_decomposer: NotRequired[APlanner]
 
 
-@dataclass(init=True,
-           repr=True,
-           eq=True,
-           order=False,
-           unsafe_hash=False,
-           frozen=False,  # mutable
-           match_args=True,
-           kw_only=False,
-           slots=False,
-           weakref_slot=False)
+@dataclass
 class AbstractTask(ABC):
     """Abstract task."""
 
     ask: str
-    resource: AbstractResource | None = None
+    resources: set[AResource] = field(default_factory=set,
+                                      init=True,
+                                      repr=True,
+                                      hash=False,  # mutable
+                                      compare=True,
+                                      metadata=None,
+                                      kw_only=True)
     status: TaskStatus = TaskStatus.PENDING
     result: str | None = None
+    dynamic_decomposer: APlanner | None = None
 
     @classmethod
     def from_dict(cls, d: TaskDict, /) -> Self:
-        """Create resource instance from dictionary representation."""
+        """Create task from dictionary representation."""
         task: Self = cls(**d)
 
-        if isinstance(task.resource, str):
-            task.resource: AbstractResource = GLOBAL_RESOURCES[task.resource]
+        if task.resources:
+            task.resources: set[AResource] = {(GLOBAL_RESOURCES[r] if isinstance(r, str) else r)
+                                              for r in task.resources}
 
         task.status: TaskStatus = TaskStatus(task.status)
 
         return task
 
+    def to_json_dict(self) -> dict:
+        d: TaskDict = asdict(self)
+        d['resources']: list[AResource] = list(d['resources'])
+        return d
+
     @classmethod
     def from_str(cls, s: str, /) -> Self:
-        """Create resource instance from dictionary representation."""
+        """Create task from string representation."""
         return cls(ask=s)
 
     @classmethod
     def from_dict_or_str(cls, dict_or_str: TaskDict | str, /) -> Self:
-        """Create resource instance from dictionary or string representation."""
+        """Create task from dictionary or string representation."""
         if isinstance(dict_or_str, dict):
             return cls.from_dict(dict_or_str)
 
         if isinstance(dict_or_str, str):
             return cls.from_str(dict_or_str)
 
         raise TypeError(f'*** {dict_or_str} IS NEITHER A DICTIONARY NOR A STRING ***')
+
+    def decompose(self) -> APlan:
+        """Decompose task into modular plan."""
+        assert isinstance(self.dynamic_decomposer, AbstractPlanner), \
+            TypeError('*** Dynamic Decomposer must be Planner instance ***')
+
+        return self.dynamic_decomposer.plan(problem=self.ask, resources=self.resources)
+
+
+ATask: TypeVar = TypeVar('ATask', bound=AbstractTask, covariant=False, contravariant=False)
```

### Comparing `openssa-0.24.3.6/openssa/utils/cli/__init__.py` & `openssa-0.24.4.24/openssa/utils/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/cli/contrib/ssa_prob_solver.py` & `openssa-0.24.4.24/openssa/utils/cli/contrib/ssa_prob_solver.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/config.py` & `openssa-0.24.4.24/openssa/utils/config.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/deprecated/aitomatic_llm_config.py` & `openssa-0.24.4.24/openssa/utils/deprecated/aitomatic_llm_config.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/deprecated/llama_index_api.py` & `openssa-0.24.4.24/openssa/utils/deprecated/llama_index_api.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/llms.py` & `openssa-0.24.4.24/openssa/utils/llms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Language Model (LM) interfaces."""
 
-
 from __future__ import annotations
-
 import json
 from loguru import logger
-
-from openai import OpenAI, AzureOpenAI
+from openai import OpenAI, AzureOpenAI, AsyncOpenAI, AsyncAzureOpenAI
 from openssa.utils.config import Config
 from openssa.utils.usage_logger import BasicUsageLogger, AbstractUsageLogger
 
 
 class AnLLM:
     """
     This class provides a consistent API for the different LLM services.
@@ -41,48 +38,64 @@
     ):
         self.model = model
         self.api_base = api_base
         self.api_key = api_key
         self.user_id = user_id
         self.usage_logger = usage_logger
         self._client = None
+        self._aclient = None
         self._additional_kwargs = additional_kwargs
 
     @property
     def client(self):
         pass
 
+    @property
+    def aclient(self):
+        pass
+
     def call(self, is_chat: bool = True, **kwargs):
         if is_chat:
             result = self.client.chat.completions.create(
                 model=self.model, **kwargs, **self._additional_kwargs
             )
         else:
             result = self.client.completions.create(
                 model=self.model, **kwargs, **self._additional_kwargs
             )
         self.usage_logger.log_usage(user=self.user_id, result=result)
         return result
 
+    async def acall(self, is_chat: bool = True, **kwargs):
+        if is_chat:
+            result = await self.aclient.chat.completions.create(
+                model=self.model, **kwargs, **self._additional_kwargs
+            )
+        else:
+            result = await self.aclient.completions.create(
+                model=self.model, **kwargs, **self._additional_kwargs
+            )
+        self.usage_logger.log_usage(user=self.user_id, result=result)
+        return result
+
     def create_embeddings(self):
         return self.client.embeddings.create(model=self.model)
 
     def get_response(
         self, prompt: str, messages: list = None, role: str = "user", **kwargs
     ) -> str:
         messages = messages if messages else []
         messages.append({"role": role, "content": prompt})
         return self.call(messages=messages, **kwargs).choices[0].message.content
 
     def parse_output(self, output: str) -> dict:
         try:
             return json.loads(output)
-
         except json.JSONDecodeError:
-            logger.debug(f'*** Could Not JSONify:\n{output} ***')
+            logger.debug(f"*** Could Not JSONify:\n{output} ***")
             return {}
 
 
 class OpenAILLM(AnLLM):
     """
     This class represents the OpenAI-hosted LLMs
     """
@@ -100,14 +113,20 @@
 
     @property
     def client(self) -> OpenAI:
         if self._client is None:
             self._client = OpenAI(api_key=self.api_key, base_url=self.api_base)
         return self._client
 
+    @property
+    def aclient(self) -> AsyncOpenAI:
+        if self._aclient is None:
+            self._aclient = AsyncOpenAI(api_key=self.api_key, base_url=self.api_base)
+        return self._aclient
+
     @classmethod
     def get_default(cls) -> OpenAILLM:
         return cls()
 
     @classmethod
     def get_gpt_35_turbo_1106(cls) -> OpenAILLM:
         return cls(model="gpt-3.5-turbo-1106")
@@ -194,14 +213,22 @@
     def client(self) -> AzureOpenAI:
         if self._client is None:
             self._client = AzureOpenAI(
                 api_key=self.api_key, azure_endpoint=self.api_base
             )
         return self._client
 
+    @property
+    def aclient(self) -> AsyncAzureOpenAI:
+        if self._aclient is None:
+            self._aclient = AsyncAzureOpenAI(
+                api_key=self.api_key, azure_endpoint=self.api_base
+            )
+        return self._aclient
+
     @classmethod
     def get_default(cls) -> AzureLLM:
         return cls.get_gpt_35()
 
     @classmethod
     def get_gpt_35(cls) -> AzureLLM:
         return cls(model="gpt-35-turbo")
```

### Comparing `openssa-0.24.3.6/openssa/utils/logs.py` & `openssa-0.24.4.24/openssa/utils/logs.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/rag_service_contexts.py` & `openssa-0.24.4.24/openssa/utils/rag_service_contexts.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/usage_logger.py` & `openssa-0.24.4.24/openssa/utils/usage_logger.py`

 * *Files identical despite different names*

### Comparing `openssa-0.24.3.6/openssa/utils/utils.py` & `openssa-0.24.4.24/openssa/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from uuid import uuid4
 from loguru import logger
 import googleapiclient.errors
 from google.oauth2.service_account import Credentials
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaIoBaseDownload
 from s3fs import S3FileSystem
-from openssa.utils.fs import FileSource
+from openssa.l2.resource.file import FileResource
 from openssa.utils.logs import mlogger
 
 
 class Utils:
     """Class containing various utility methods."""
 
     @staticmethod
@@ -311,21 +311,21 @@
         os.makedirs(local_dir)
 
         if isinstance(s3_paths, str):
             s3_paths: set[str] = {s3_paths}
 
         for s3_file_path in set(
             chain.from_iterable(
-                FileSource(path=s3_path).file_paths(relative=False)
+                FileResource(path=s3_path).file_paths(relative=False)
                 for s3_path in s3_paths
             )
         ):
             # temp file path each document is copied to must retain same extension/suffix
             local_file_path: str = os.path.join(
-                local_dir, f"{uuid4()}-{Path(s3_file_path).name}"
+                local_dir, f"{uuid4()} ~ {Path(s3_file_path).name}"
             )
 
             Utils._S3FS.download(
                 rpath=s3_file_path, lpath=local_file_path, recursive=False
             )
 
     @staticmethod
```


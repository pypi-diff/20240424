# Comparing `tmp/prompt2model-0.0.9.tar.gz` & `tmp/prompt2model-0.1.0.tar.gz`

## Comparing `prompt2model-0.0.9.tar` & `prompt2model-0.1.0.tar`

### file list

```diff
@@ -1,71 +1,77 @@
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/__init__.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/run_locally.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/version.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_generator/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_generator/base.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_generator/mock.py
--rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_generator/prompt_based.py
--rw-r--r--   0        0        0    17763 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_generator/prompt_template.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_processor/__init__.py
--rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_processor/base.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_processor/mock.py
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_processor/textualize.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_retriever/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_retriever/base.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_retriever/column_selection_prompt.py
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_retriever/description_dataset_retriever.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_retriever/mock.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_retriever/retrieve_dataset_info.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/dataset_retriever/run_dataset_retriever.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/demo_creator/__init__.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/demo_creator/create.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/demo_creator/mock.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_evaluator/__init__.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_evaluator/base.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_evaluator/mock.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_evaluator/seq2seq.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_executor/__init__.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_executor/base.py
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_executor/generate.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_executor/mock.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_retriever/__init__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_retriever/base.py
--rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_retriever/description_based_retriever.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_retriever/generate_hypothetical_document.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_retriever/mock.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_retriever/run_model_retriever.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_trainer/__init__.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_trainer/base.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_trainer/callback.py
--rw-r--r--   0        0        0    18377 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_trainer/generate.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/model_trainer/mock.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/param_selector/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/param_selector/base.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/param_selector/mock.py
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/param_selector/search_with_optuna.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/prompt_parser/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/prompt_parser/base.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/prompt_parser/instr_parser.py
--rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/prompt_parser/instr_parser_prompt.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/prompt_parser/mock.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/__init__.py
--rw-r--r--   0        0        0     9911 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/api_tools.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/config.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/dataset_utils.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/logging_utils.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/parse_json_responses.py
--rwxr-xr-x   0        0        0     2723 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/retrieve_model_info.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/rng.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/tevatron_utils/__init__.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/tevatron_utils/encode.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 prompt2model-0.0.9/prompt2model/utils/tevatron_utils/retrieve.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 prompt2model-0.0.9/test_helpers/__init__.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 prompt2model-0.0.9/test_helpers/mock_api.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 prompt2model-0.0.9/test_helpers/mock_retrieval.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 prompt2model-0.0.9/test_helpers/model_and_tokenizer.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 prompt2model-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 prompt2model-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 prompt2model-0.0.9/LICENSE
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 prompt2model-0.0.9/README.md
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 prompt2model-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 prompt2model-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/__init__.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/run_locally.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/version.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_generator/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_generator/base.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_generator/mock.py
+-rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_generator/prompt_based.py
+-rw-r--r--   0        0        0    17763 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_generator/prompt_template.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_processor/__init__.py
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_processor/base.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_processor/mock.py
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_processor/textualize.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/base.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/column_selection_prompt.py
+-rw-r--r--   0        0        0    30980 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/description_dataset_retriever.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/mock.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/reranking_prompt.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/run_dataset_retriever.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_retriever/task_expansion_prompt.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_transformer/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_transformer/base.py
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_transformer/prompt_based.py
+-rw-r--r--   0        0        0    32998 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/dataset_transformer/prompt_template.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/demo_creator/__init__.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/demo_creator/create.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/demo_creator/mock.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_evaluator/__init__.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_evaluator/base.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_evaluator/mock.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_evaluator/seq2seq.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_executor/__init__.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_executor/base.py
+-rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_executor/generate.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_executor/mock.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_retriever/__init__.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_retriever/base.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_retriever/description_based_retriever.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_retriever/generate_hypothetical_document.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_retriever/mock.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_retriever/run_model_retriever.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_trainer/__init__.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_trainer/base.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_trainer/callback.py
+-rw-r--r--   0        0        0    18377 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_trainer/generate.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_trainer/mock.py
+-rw-r--r--   0        0        0     9073 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/model_trainer/qlora_trainer.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/param_selector/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/param_selector/base.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/param_selector/mock.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/param_selector/search_with_optuna.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/prompt_parser/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/prompt_parser/base.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/prompt_parser/instr_parser.py
+-rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/prompt_parser/instr_parser_prompt.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/prompt_parser/mock.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/__init__.py
+-rw-r--r--   0        0        0    10624 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/api_tools.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/config.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/dataset_utils.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/logging_utils.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/parse_responses.py
+-rwxr-xr-x   0        0        0     2723 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/retrieve_model_info.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/rng.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/tevatron_utils/__init__.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/tevatron_utils/encode.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 prompt2model-0.1.0/prompt2model/utils/tevatron_utils/retrieve.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 prompt2model-0.1.0/test_helpers/__init__.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 prompt2model-0.1.0/test_helpers/mock_api.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 prompt2model-0.1.0/test_helpers/mock_retrieval.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 prompt2model-0.1.0/test_helpers/model_and_tokenizer.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 prompt2model-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 prompt2model-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 prompt2model-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 prompt2model-0.1.0/README.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 prompt2model-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    18541 2020-02-02 00:00:00.000000 prompt2model-0.1.0/PKG-INFO
```

### Comparing `prompt2model-0.0.9/prompt2model/run_locally.py` & `prompt2model-0.1.0/prompt2model/run_locally.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_generator/base.py` & `prompt2model-0.1.0/prompt2model/dataset_generator/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_generator/mock.py` & `prompt2model-0.1.0/prompt2model/dataset_generator/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_generator/prompt_based.py` & `prompt2model-0.1.0/prompt2model/dataset_generator/prompt_based.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_generator/prompt_template.py` & `prompt2model-0.1.0/prompt2model/dataset_generator/prompt_template.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_processor/base.py` & `prompt2model-0.1.0/prompt2model/dataset_processor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,16 @@
             maximum_example_num: Maximum number of examples
                 to include in each set.
 
         Returns:
             datasets.DatasetDict: A dictionary containing the `train`,
                 `val`, and `test` datasets.
         """
+        if "train" in dataset:
+            dataset = dataset["train"]
         num_of_examples = len(dataset)
         train_num = int(train_proportion * num_of_examples)
         val_num = int(val_proportion * num_of_examples)
         test_num = num_of_examples - train_num - val_num
 
         if maximum_example_num is not None:
             train_num = min(train_num, maximum_example_num.get("train", sys.maxsize))
```

### Comparing `prompt2model-0.0.9/prompt2model/dataset_processor/mock.py` & `prompt2model-0.1.0/prompt2model/dataset_processor/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_processor/textualize.py` & `prompt2model-0.1.0/prompt2model/dataset_processor/textualize.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_retriever/base.py` & `prompt2model-0.1.0/prompt2model/dataset_retriever/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_retriever/column_selection_prompt.py` & `prompt2model-0.1.0/prompt2model/dataset_retriever/column_selection_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Utilities to construct an LLM "metaprompt" for our column selection."""
 
 from __future__ import annotations  # noqa FI58
 
-import json
-
 METAPROMPT_BASE = """Your objective is to carefully analyze the task and the dataset mentioned, and decide whether the columns are relevant input, relevant output, irrelevant for the given task, or if it is ambiguous. There should be at most one output column. It is possible to have no relevant columns, in which case return the input and output column as empty lists.  Answer in a json format, with the following keys: input, output, irrelevant, ambiguous"""  # noqa: E501
 METAPROMPT_EXAMPLES = [
     (
         """You are tasked with the following process. In this task, you will generate summaries for given texts. For this task, you will use the Scientific Papers dataset from HuggingFace. Dataset_description: Scientific papers datasets contains two sets of long and structured documents. The datasets are obtained from ArXiv and PubMed OpenAccess repositories.
         A sample data instance from this dataset is as follows.
         {
             "abstract": "\" we have studied the leptonic decay @xmath0 , via the decay channel @xmath1 , using a sample of tagged @xmath2 decays collected...",
@@ -86,41 +84,28 @@
 INPUT_PROMPT_TEMPLATE = """You are tasked with the following process. {instruction} For this task, you will use the {dataset_name} dataset from HuggingFace. Dataset Description: {dataset_description} \nA sample data instance from this is as follows. {sample_row}.\nThis dataset has the following columns: [{dataset_columns} ]."""  # noqa: E501
 SINGLE_DEMONSTRATION_TEMPLATE = (
     'Task: """\n{prompt}\n"""\n\nRequired Columns :\n{columns}'
 )
 ENDING_LINE = "After seeing these examples with the required columns, please provide the relevant columns for this context:"  # noqa: E501
 
 
-def truncate_row(example_row: dict, max_length=50) -> str:
-    """Truncate the row before displaying if it is too long."""
-    truncated_row = {}
-    for key in example_row.keys():
-        curr_row = json.dumps(example_row[key])
-        truncated_row[key] = (
-            curr_row
-            if len(curr_row) <= max_length - 3
-            else curr_row[:max_length] + "..."
-        )
-    return json.dumps(truncated_row)
-
-
 def build_input(
     instruction: str,
     dataset_name: str,
     dataset_description: str,
     dataset_columns: str,
     sample_row: dict,
 ) -> str:
     """Template function to build input based on arguments."""
     input_prompt = INPUT_PROMPT_TEMPLATE.format(
         instruction=instruction,
         dataset_name=dataset_name,
         dataset_description=dataset_description,
         dataset_columns=dataset_columns,
-        sample_row=truncate_row(sample_row),
+        sample_row=sample_row,
     )
     input_prompt = SINGLE_DEMONSTRATION_TEMPLATE.format(
         prompt=input_prompt, columns=""
     )  # columns="" because that is what we are trying to predict
     return input_prompt
```

### Comparing `prompt2model-0.0.9/prompt2model/dataset_retriever/mock.py` & `prompt2model-0.1.0/prompt2model/dataset_retriever/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/dataset_retriever/run_dataset_retriever.py` & `prompt2model-0.1.0/prompt2model/dataset_retriever/run_dataset_retriever.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/demo_creator/create.py` & `prompt2model-0.1.0/prompt2model/demo_creator/create.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/demo_creator/mock.py` & `prompt2model-0.1.0/prompt2model/demo_creator/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_evaluator/base.py` & `prompt2model-0.1.0/prompt2model/model_evaluator/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_evaluator/mock.py` & `prompt2model-0.1.0/prompt2model/model_evaluator/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_evaluator/seq2seq.py` & `prompt2model-0.1.0/prompt2model/model_evaluator/seq2seq.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_executor/base.py` & `prompt2model-0.1.0/prompt2model/model_executor/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_executor/generate.py` & `prompt2model-0.1.0/prompt2model/model_executor/generate.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_executor/mock.py` & `prompt2model-0.1.0/prompt2model/model_executor/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_retriever/base.py` & `prompt2model-0.1.0/prompt2model/model_retriever/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_retriever/description_based_retriever.py` & `prompt2model-0.1.0/prompt2model/model_retriever/description_based_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,19 +127,18 @@
 
         We load metadata from json files in the model_descriptions_index_path
         directory, filter out models from certain organizations, and initialize a list
         of ModelInfo objects corresponding to the models we want to search against.
         """
         if not os.path.isdir(self.model_descriptions_index_path):
             # If the model descriptions directory is not populated, then populate it.
-            urllib.request.urlretrieve(
-                "http://phontron.com/data/prompt2model/model_info.tgz",
-                "/tmp/model_info.tgz",
+            temporary_file, _ = urllib.request.urlretrieve(
+                "http://phontron.com/data/prompt2model/model_info.tgz"
             )
-            tar = tarfile.open("/tmp/model_info.tgz")
+            tar = tarfile.open(temporary_file)
             os.makedirs(self.model_descriptions_index_path)
             tar.extractall(path=self.model_descriptions_index_path)
 
         description_files = os.listdir(self.model_descriptions_index_path)
         # We store model names and descriptions in a list of ModelInfo objects.
         self.model_infos: list[ModelInfo] = []
         for f in tqdm(description_files):
```

### Comparing `prompt2model-0.0.9/prompt2model/model_retriever/generate_hypothetical_document.py` & `prompt2model-0.1.0/prompt2model/model_retriever/generate_hypothetical_document.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_retriever/mock.py` & `prompt2model-0.1.0/prompt2model/model_retriever/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_retriever/run_model_retriever.py` & `prompt2model-0.1.0/prompt2model/model_retriever/run_model_retriever.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_trainer/base.py` & `prompt2model-0.1.0/prompt2model/model_trainer/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_trainer/callback.py` & `prompt2model-0.1.0/prompt2model/model_trainer/callback.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_trainer/generate.py` & `prompt2model-0.1.0/prompt2model/model_trainer/generate.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/model_trainer/mock.py` & `prompt2model-0.1.0/prompt2model/model_trainer/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/param_selector/base.py` & `prompt2model-0.1.0/prompt2model/param_selector/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/param_selector/mock.py` & `prompt2model-0.1.0/prompt2model/param_selector/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/param_selector/search_with_optuna.py` & `prompt2model-0.1.0/prompt2model/param_selector/search_with_optuna.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/prompt_parser/base.py` & `prompt2model-0.1.0/prompt2model/prompt_parser/base.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/prompt_parser/instr_parser.py` & `prompt2model-0.1.0/prompt2model/prompt_parser/instr_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from prompt2model.prompt_parser.base import PromptSpec, TaskType
 
 from prompt2model.prompt_parser.instr_parser_prompt import (  # isort: split
     construct_prompt_for_instruction_parsing,
 )
 
-from prompt2model.utils.parse_json_responses import parse_prompt_to_fields
+from prompt2model.utils.parse_responses import parse_prompt_to_fields
 
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 
 class PromptBasedInstructionParser(PromptSpec):
     """Parse the prompt to separate instructions from task demonstrations."""
 
@@ -42,12 +42,22 @@
 
         Args:
             prompt: User prompt to parse into two specific fields:
                     "instruction" and "demonstrations".
         """
         parsing_prompt_for_chatgpt = construct_prompt_for_instruction_parsing(prompt)
         required_keys = ["Instruction", "Demonstrations"]
+
         extraction = parse_prompt_to_fields(
-            parsing_prompt_for_chatgpt, required_keys, max_api_calls=self.max_api_calls
+            parsing_prompt_for_chatgpt,
+            required_keys,
+            max_api_calls=self.max_api_calls,
         )
         self._instruction = extraction["Instruction"]
         self._examples = extraction["Demonstrations"]
+
+    def set_instruction_and_examples(
+        self, instruction: str = "", examples: str = ""
+    ) -> None:
+        """Set the instruction and examples directly."""
+        self._instruction = instruction
+        self._examples = examples
```

### Comparing `prompt2model-0.0.9/prompt2model/prompt_parser/instr_parser_prompt.py` & `prompt2model-0.1.0/prompt2model/prompt_parser/instr_parser_prompt.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/prompt_parser/mock.py` & `prompt2model-0.1.0/prompt2model/prompt_parser/mock.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/utils/__init__.py` & `prompt2model-0.1.0/prompt2model/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/utils/api_tools.py` & `prompt2model-0.1.0/prompt2model/utils/api_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 """Tools for accessing API-based models."""
 
 from __future__ import annotations  # noqa FI58
 
 import asyncio
 import json
 import logging
+import re
 import time
 
 import aiolimiter
 import litellm.utils
 import openai
-import openai.error
 import tiktoken
 from aiohttp import ClientSession
 from litellm import acompletion, completion
 from tqdm.asyncio import tqdm_asyncio
 
 # Note that litellm converts all API errors into openai errors,
 # so openai errors are valid even when using other services.
 API_ERRORS = (
-    openai.error.APIError,
-    openai.error.Timeout,
-    openai.error.RateLimitError,
-    openai.error.ServiceUnavailableError,
-    openai.error.InvalidRequestError,
+    openai.APIError,
+    openai.APITimeoutError,
+    openai.RateLimitError,
+    openai.BadRequestError,
+    openai.APIStatusError,
     json.decoder.JSONDecodeError,
     AssertionError,
 )
 
 ERROR_ERRORS_TO_MESSAGES = {
-    openai.error.InvalidRequestError: "API Invalid Request: Prompt was filtered",
-    openai.error.RateLimitError: "API rate limit exceeded. Sleeping for 10 seconds.",
-    openai.error.APIConnectionError: "Error Communicating with API",
-    openai.error.Timeout: "API Timeout Error: API Timeout",
-    openai.error.ServiceUnavailableError: "API service unavailable error: {e}",
-    openai.error.APIError: "API error: {e}",
+    openai.BadRequestError: "API Invalid Request: Prompt was filtered",
+    openai.RateLimitError: "API rate limit exceeded. Sleeping for 10 seconds.",
+    openai.APIConnectionError: "Error Communicating with API",
+    openai.APITimeoutError: "API Timeout Error: API Timeout",
+    openai.APIStatusError: "API service unavailable error: {e}",
+    openai.APIError: "API error: {e}",
 }
+BUFFER_DURATION = 2
 
 
 class APIAgent:
     """A class for accessing API-based models."""
 
     def __init__(
         self,
-        model_name: str = "gpt-3.5-turbo",
-        max_tokens: int | None = None,
+        model_name: str = "gpt-4",
+        max_tokens: int | None = 4000,
         api_base: str | None = None,
     ):
         """Initialize APIAgent with model_name and max_tokens.
 
         Args:
-            model_name: Name fo the model to use (by default, gpt-3.5-turbo).
+            model_name: Name of the model to use (by default, gpt-4).
             max_tokens: The maximum number of tokens to generate. Defaults to the max
                 value for the model if available through litellm.
             api_base: Custom endpoint for Hugging Face's inference API.
         """
         self.model_name = model_name
         self.max_tokens = max_tokens
         self.api_base = api_base
@@ -98,15 +99,14 @@
             In case of API-specific error, Exception object is captured and returned.
         """
         num_prompt_tokens = count_tokens_from_string(prompt)
         if self.max_tokens:
             max_tokens = self.max_tokens - num_prompt_tokens - token_buffer
         else:
             max_tokens = 3 * num_prompt_tokens
-
         response = completion(  # completion gets the key from os.getenv
             model=self.model_name,
             messages=[
                 {"role": "user", "content": f"{prompt}"},
             ],
             api_base=self.api_base,
             temperature=temperature,
@@ -138,107 +138,126 @@
                 number of tokens, this prevents service errors. On the other hand, this
                 may lead to generating fewer tokens in the completion than is actually
                 possible.
 
         Returns:
             List of generated responses.
         """
-        openai.aiosession.set(ClientSession())
-        limiter = aiolimiter.AsyncLimiter(requests_per_minute)
+        async with ClientSession() as _:
+            limiter = aiolimiter.AsyncLimiter(requests_per_minute)
 
-        async def _throttled_completion_acreate(
-            model: str,
-            messages: list[dict[str, str]],
-            temperature: float,
-            max_tokens: int,
-            n: int,
-            top_p: float,
-            limiter: aiolimiter.AsyncLimiter,
-        ):
-            async with limiter:
-                for _ in range(3):
-                    try:
-                        return await acompletion(
-                            model=model,
-                            messages=messages,
-                            api_base=self.api_base,
-                            temperature=temperature,
-                            max_tokens=max_tokens,
-                            n=n,
-                            top_p=top_p,
-                        )
-                    except tuple(ERROR_ERRORS_TO_MESSAGES.keys()) as e:
-                        if isinstance(
-                            e,
-                            (
-                                openai.error.ServiceUnavailableError,
-                                openai.error.APIError,
-                            ),
-                        ):
-                            logging.warning(
-                                ERROR_ERRORS_TO_MESSAGES[type(e)].format(e=e)
+            async def _throttled_completion_acreate(
+                model: str,
+                messages: list[dict[str, str]],
+                temperature: float,
+                max_tokens: int,
+                n: int,
+                top_p: float,
+                limiter: aiolimiter.AsyncLimiter,
+            ):
+                async with limiter:
+                    for _ in range(3):
+                        try:
+                            return await acompletion(
+                                model=model,
+                                messages=messages,
+                                api_base=self.api_base,
+                                temperature=temperature,
+                                max_tokens=max_tokens,
+                                n=n,
+                                top_p=top_p,
                             )
-                        elif isinstance(e, openai.error.InvalidRequestError):
-                            logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
-                            return {
-                                "choices": [
-                                    {
-                                        "message": {
-                                            "content": "Invalid Request: Prompt was filtered"  # noqa E501
+                        except tuple(ERROR_ERRORS_TO_MESSAGES.keys()) as e:
+                            if isinstance(
+                                e,
+                                (
+                                    openai.APIStatusError,
+                                    openai.APIError,
+                                ),
+                            ):
+                                logging.warning(
+                                    ERROR_ERRORS_TO_MESSAGES[type(e)].format(e=e)
+                                )
+                            elif isinstance(e, openai.BadRequestError):
+                                logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
+                                return {
+                                    "choices": [
+                                        {
+                                            "message": {
+                                                "content": "Invalid Request: Prompt was filtered"  # noqa E501
+                                            }
                                         }
-                                    }
-                                ]
-                            }
-                        else:
-                            logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
-                        await asyncio.sleep(10)
-                return {"choices": [{"message": {"content": ""}}]}
+                                    ]
+                                }
+                            else:
+                                logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
+                            await asyncio.sleep(10)
+                    return {"choices": [{"message": {"content": ""}}]}
 
-        num_prompt_tokens = max(count_tokens_from_string(prompt) for prompt in prompts)
-        if self.max_tokens:
-            max_tokens = self.max_tokens - num_prompt_tokens - token_buffer
-        else:
-            max_tokens = 3 * num_prompt_tokens
-
-        async_responses = [
-            _throttled_completion_acreate(
-                model=self.model_name,
-                messages=[
-                    {"role": "user", "content": f"{prompt}"},
-                ],
-                temperature=temperature,
-                max_tokens=max_tokens,
-                n=responses_per_request,
-                top_p=1,
-                limiter=limiter,
+            num_prompt_tokens = max(
+                count_tokens_from_string(prompt) for prompt in prompts
             )
-            for prompt in prompts
-        ]
-        responses = await tqdm_asyncio.gather(*async_responses)
+            if self.max_tokens:
+                max_tokens = self.max_tokens - num_prompt_tokens - token_buffer
+            else:
+                max_tokens = 3 * num_prompt_tokens
+
+            async_responses = [
+                _throttled_completion_acreate(
+                    model=self.model_name,
+                    messages=[
+                        {"role": "user", "content": f"{prompt}"},
+                    ],
+                    temperature=temperature,
+                    max_tokens=max_tokens,
+                    n=responses_per_request,
+                    top_p=1,
+                    limiter=limiter,
+                )
+                for prompt in prompts
+            ]
+            responses = await tqdm_asyncio.gather(*async_responses)
         # Note: will never be none because it's set, but mypy doesn't know that.
-        await openai.aiosession.get().close()
         return responses
 
 
-def handle_api_error(e) -> None:
+def handle_api_error(e, backoff_duration=1) -> None:
     """Handle OpenAI errors or related errors that the API may raise.
 
+    Sleeps incase error is some type of timeout, else throws error.
+
     Args:
         e: The error to handle. This could be an OpenAI error or a related
            non-fatal error, such as JSONDecodeError or AssertionError.
+        backoff_duration: The duration (in s) to wait before retrying.
+
+    Raises:
+        e: If the error is not an instance of APIError, Timeout, or RateLimitError.
+
+    Returns:
+        None
     """
     logging.error(e)
+
     if not isinstance(e, API_ERRORS):
         raise e
+
     if isinstance(
         e,
-        (openai.error.APIError, openai.error.Timeout, openai.error.RateLimitError),
+        (openai.APIError, openai.APITimeoutError, openai.RateLimitError),
     ):
-        # For these errors, OpenAI recommends waiting before retrying.
-        time.sleep(1)
+
+        match = re.search(r"Please retry after (\d+) seconds", str(e))
+        # If OpenAI mentions how long to sleep, use that. Otherwise, do
+        # exponential backoff.
+        if match is not None:
+            backoff_duration = int(match.group(1)) + BUFFER_DURATION
+
+        logging.info(f"Retrying in {backoff_duration} seconds...")
+        time.sleep(backoff_duration)
 
 
 def count_tokens_from_string(string: str, encoding_name: str = "cl100k_base") -> int:
     """Handle count the tokens in a string with OpenAI's tokenizer.
 
     Args:
         string: The string to count.
@@ -250,8 +269,8 @@
     encoding = tiktoken.get_encoding(encoding_name)
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
 
 # This is the default API agent that is used everywhere if a different agent is not
 # specified
-default_api_agent = APIAgent()
+default_api_agent = APIAgent(max_tokens=4000)
```

### Comparing `prompt2model-0.0.9/prompt2model/utils/logging_utils.py` & `prompt2model-0.1.0/prompt2model/utils/logging_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,18 @@
         logger_name: The name of the logger, usually the name
             of the component that uses the logger.
 
     Returns:
         A logger object.
     """
     logger = logging.getLogger(logger_name)
-    ch = logging.StreamHandler()
-    formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    )
-    ch.setFormatter(formatter)
-    logger.addHandler(ch)
+    # Check if the logger already has a StreamHandler to prevent adding another one.
+    if not any(
+        isinstance(handler, logging.StreamHandler) for handler in logger.handlers
+    ):
+        ch = logging.StreamHandler()
+        formatter = logging.Formatter(
+            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+        )
+        ch.setFormatter(formatter)
+        logger.addHandler(ch)
     return logger
```

### Comparing `prompt2model-0.0.9/prompt2model/utils/retrieve_model_info.py` & `prompt2model-0.1.0/prompt2model/utils/retrieve_model_info.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/utils/rng.py` & `prompt2model-0.1.0/prompt2model/utils/rng.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/utils/tevatron_utils/encode.py` & `prompt2model-0.1.0/prompt2model/utils/tevatron_utils/encode.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/prompt2model/utils/tevatron_utils/retrieve.py` & `prompt2model-0.1.0/prompt2model/utils/tevatron_utils/retrieve.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/test_helpers/__init__.py` & `prompt2model-0.1.0/test_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/test_helpers/mock_api.py` & `prompt2model-0.1.0/test_helpers/mock_api.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/test_helpers/mock_retrieval.py` & `prompt2model-0.1.0/test_helpers/mock_retrieval.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/test_helpers/model_and_tokenizer.py` & `prompt2model-0.1.0/test_helpers/model_and_tokenizer.py`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/LICENSE` & `prompt2model-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt2model-0.0.9/README.md` & `prompt2model-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -91,19 +91,34 @@
 - or reach out to [@vijaytarian](https://twitter.com/vijaytarian)
   and [@Chenan3_Zhao](https://twitter.com/Chenan3_Zhao) on Twitter
 
 ## Cite
 
 We have [written a paper describing Prompt2Model in detail](https://arxiv.org/abs/2308.12261).
 
-If you use Prompt2Model in your research, please cite our paper:
+If you use Prompt2Model in your research, please cite us!
+
+If you discuss or use the overall prompt2model framework, please reference
 
 ```bibtex
 @misc{prompt2model,
       title={Prompt2Model: Generating Deployable Models from Natural Language Instructions},
       author={Vijay Viswanathan and Chenyang Zhao and Amanda Bertsch and Tongshuang Wu and Graham Neubig},
       year={2023},
       eprint={2308.12261},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
+
+If you discuss or use our dataset retrieval and transformation tools, please reference
+
+```bibtex
+@misc{prompt2modeldatatune,
+      title={Better Synthetic Data by Retrieving and Transforming Existing Datasets}, 
+      author={Saumya Gandhi and Ritu Gala and Vijay Viswanathan and Tongshuang Wu and Graham Neubig},
+      year={2024},
+      eprint={2404.14361},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
```

### Comparing `prompt2model-0.0.9/pyproject.toml` & `prompt2model-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "transformers",
     "datasets",
     "pandas",
     "fastapi",
     "gradio==3.38.0",
     "torch",
     "pytest",
-    "openai==0.27.10",
+    "openai",
     "sentencepiece",
     "bert_score",
     "sacrebleu",
     "evaluate",
     "tevatron",
     "faiss-cpu",
     "mdtex2html",
@@ -41,15 +41,16 @@
     "tiktoken",
     "aiolimiter",
     "pyfiglet",
     "termcolor",
     "psutil",
     "protobuf",
     "nest-asyncio",
-    "litellm==0.1.583"
+    "litellm",
+    "peft"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest>=6.0.0",
```

### Comparing `prompt2model-0.0.9/PKG-INFO` & `prompt2model-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: prompt2model
-Version: 0.0.9
+Version: 0.1.0
 Summary: A library for distilling models from prompts.
 Author-email: Vijay Viswanathan <vijayv@andrew.cmu.edu>, Chenyang Zhao <zhaochen20@mails.tsinghua.edu.cn>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,19 +212,20 @@
 Requires-Dist: aiolimiter
 Requires-Dist: bert-score
 Requires-Dist: datasets
 Requires-Dist: evaluate
 Requires-Dist: faiss-cpu
 Requires-Dist: fastapi
 Requires-Dist: gradio==3.38.0
-Requires-Dist: litellm==0.1.583
+Requires-Dist: litellm
 Requires-Dist: mdtex2html
 Requires-Dist: nest-asyncio
-Requires-Dist: openai==0.27.10
+Requires-Dist: openai
 Requires-Dist: pandas
+Requires-Dist: peft
 Requires-Dist: protobuf
 Requires-Dist: psutil
 Requires-Dist: pyfiglet
 Requires-Dist: pytest
 Requires-Dist: retriv
 Requires-Dist: sacrebleu
 Requires-Dist: scikit-learn
@@ -334,19 +335,34 @@
 - or reach out to [@vijaytarian](https://twitter.com/vijaytarian)
   and [@Chenan3_Zhao](https://twitter.com/Chenan3_Zhao) on Twitter
 
 ## Cite
 
 We have [written a paper describing Prompt2Model in detail](https://arxiv.org/abs/2308.12261).
 
-If you use Prompt2Model in your research, please cite our paper:
+If you use Prompt2Model in your research, please cite us!
+
+If you discuss or use the overall prompt2model framework, please reference
 
 ```bibtex
 @misc{prompt2model,
       title={Prompt2Model: Generating Deployable Models from Natural Language Instructions},
       author={Vijay Viswanathan and Chenyang Zhao and Amanda Bertsch and Tongshuang Wu and Graham Neubig},
       year={2023},
       eprint={2308.12261},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
+
+If you discuss or use our dataset retrieval and transformation tools, please reference
+
+```bibtex
+@misc{prompt2modeldatatune,
+      title={Better Synthetic Data by Retrieving and Transforming Existing Datasets}, 
+      author={Saumya Gandhi and Ritu Gala and Vijay Viswanathan and Tongshuang Wu and Graham Neubig},
+      year={2024},
+      eprint={2404.14361},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
```


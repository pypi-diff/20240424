# Comparing `tmp/distilabel-1.0.1.tar.gz` & `tmp/distilabel-1.0.2.tar.gz`

## Comparing `distilabel-1.0.1.tar` & `distilabel-1.0.2.tar`

### file list

```diff
@@ -1,256 +1,256 @@
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.1/Makefile
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 distilabel-1.0.1/mkdocs.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/blank-issue-template.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/🆕-feature-request.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/🐛-bug-report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/📚-documentation-update.md
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/CNAME
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/index.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/overview.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/cli.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/anthropic.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/anyscale.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/azure.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/huggingface.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/index.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/litellm.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/llamacpp.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/mistral.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/ollama.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/openai.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/together.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/vertexai.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/vllm.md
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/pipeline/pipeline.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/argilla.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/decorator.md
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/extra.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/index.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/generator_steps/generator_steps.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/global_steps/global_steps.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/tasks/embeddings.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/tasks/preference_tasks.md
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/tasks/text_generation.md
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-badge-dark.png
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-badge-light.png
--rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-black.png
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-icon.svg
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-white.png
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/logo.svg
--rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/distilabel-diagram-dark.svg
--rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/distilabel-diagram.svg
--rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_1.png
--rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_2.png
--rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_3.png
--rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_4.png
--rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/cli/cli_pipe.png
--rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/preference.png
--rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/text_generation.png
--rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
--rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
--rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/datasets.png
--rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/diversity.png
--rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/overview.png
--rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/results.png
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/scripts/gen_ref_pages.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/caching.md
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/cli.md
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/distiset.md
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/index.md
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/llms/index.md
--rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/pipelines/index.md
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/argilla.md
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/general_steps.md
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/generator_steps.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/global_steps.md
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/index.md
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/feedback_tasks.md
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/index.md
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/special_tasks.md
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/text_generation.md
--rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/deita.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/index.md
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/instruction_backtranslation.md
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/ultrafeedback.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/__main__.py
--rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/distiset.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/app.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/pipeline/app.py
--rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/pipeline/utils.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/anthropic.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/anyscale.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/azure.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/base.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/chat_templates.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/cohere.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/litellm.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/llamacpp.py
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/mistral.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/mixins.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/ollama.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/openai.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/together.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/typing.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/vertexai.py
--rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/vllm.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/huggingface/inference_endpoints.py
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/huggingface/transformers.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/mixins/__init__.py
--rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/mixins/runtime_parameters.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/__init__.py
--rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/_dag.py
--rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/base.py
--rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/local.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/utils.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/__init__.py
--rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/base.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/combine.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/conversation.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/decorator.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/deita.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/expand.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/keep.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/typing.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/base.py
--rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/preference.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/text_generation.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/generators/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/generators/data.py
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/generators/huggingface.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/globals/__init__.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/globals/huggingface.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/__init__.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/base.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/complexity_scorer.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/generate_embeddings.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/instruction_backtranslation.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/pair_rm.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/quality_scorer.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/self_instruct.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/text_generation.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/typing.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/ultrafeedback.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/base.py
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/generator.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/base.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/utils.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/self-instruct.jinja2
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/chat.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/dicts.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/docstring.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/files.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/itertools.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/lists.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/logging.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/notebook.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/serialization.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/typing_.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/card/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/card/dataset_card.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/card/distilabel_template.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/integration/test_pipe_llms.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/integration/test_pipe_simple.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/test_distiset.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/test_imports.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/test_pipeline.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/pipeline/test_app.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_anthropic.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_anyscale.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_azure.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_cohere.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_litellm.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_llamacpp.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_mistral.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_mixins.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_ollama.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_openai.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_together.py
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_vertexai.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/huggingface/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/huggingface/test_inference_endpoints.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/huggingface/test_transformers.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/mixins/__init__.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/mixins/test_runtime_parameters.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/__init__.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/conftest.py
--rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/test_base.py
--rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/test_dag.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/test_local.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/__init__.py
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_base.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_combine.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_conversation.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_decorator.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_deita.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_expand.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_keep.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/test_base.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/test_preference.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/test_text_generation.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/generators/test_data.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/conftest.py
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_base.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_complexity_scorer.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_generate_embeddings.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_instruction_backtranslation.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_pair_rm.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_quality_scorer.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_self_instruct.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_text_generation.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_ultrafeedback.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_base.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_generator.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_quality/test_base.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_chat.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_docstring.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_lists.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_typing.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.1/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.1/LICENSE
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.1/LICENSE_HEADER
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 distilabel-1.0.1/README.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 distilabel-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.2/Makefile
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 distilabel-1.0.2/mkdocs.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/blank-issue-template.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/🆕-feature-request.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/🐛-bug-report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/📚-documentation-update.md
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/CNAME
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/index.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/overview.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/cli.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/anthropic.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/anyscale.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/azure.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/huggingface.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/index.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/litellm.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/llamacpp.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/mistral.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/ollama.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/openai.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/together.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/vertexai.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/vllm.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/pipeline/pipeline.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/argilla.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/decorator.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/extra.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/index.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/generator_steps/generator_steps.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/global_steps/global_steps.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/tasks/embeddings.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/tasks/preference_tasks.md
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/tasks/text_generation.md
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-badge-dark.png
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-badge-light.png
+-rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-black.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-icon.svg
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-white.png
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/logo.svg
+-rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/distilabel-diagram-dark.svg
+-rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/distilabel-diagram.svg
+-rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_1.png
+-rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_2.png
+-rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_3.png
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_4.png
+-rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/cli/cli_pipe.png
+-rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/preference.png
+-rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/text_generation.png
+-rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
+-rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/datasets.png
+-rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/diversity.png
+-rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/overview.png
+-rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/results.png
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/caching.md
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/cli.md
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/distiset.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/index.md
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/llms/index.md
+-rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/pipelines/index.md
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/argilla.md
+-rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/general_steps.md
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/generator_steps.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/global_steps.md
+-rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/index.md
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/feedback_tasks.md
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/index.md
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/special_tasks.md
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/text_generation.md
+-rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/deita.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/index.md
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/instruction_backtranslation.md
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/ultrafeedback.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/__main__.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/distiset.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/app.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/pipeline/app.py
+-rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/pipeline/utils.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/anthropic.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/anyscale.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/azure.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/base.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/chat_templates.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/cohere.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/litellm.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/llamacpp.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/mistral.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/mixins.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/ollama.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/openai.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/together.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/typing.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/vertexai.py
+-rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/vllm.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    15916 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/huggingface/inference_endpoints.py
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/huggingface/transformers.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/mixins/__init__.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/mixins/runtime_parameters.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/__init__.py
+-rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/_dag.py
+-rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/base.py
+-rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/local.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/utils.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/__init__.py
+-rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/base.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/combine.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/conversation.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/decorator.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/deita.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/expand.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/keep.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/typing.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/base.py
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/preference.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/text_generation.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/generators/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/generators/data.py
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/generators/huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/globals/__init__.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/globals/huggingface.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/base.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/complexity_scorer.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/generate_embeddings.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/instruction_backtranslation.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/pair_rm.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/quality_scorer.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/self_instruct.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/text_generation.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/typing.py
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/ultrafeedback.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/base.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/generator.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/base.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/utils.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/self-instruct.jinja2
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/chat.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/dicts.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/docstring.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/files.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/itertools.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/lists.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/logging.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/notebook.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/serialization.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/typing_.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/card/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/card/dataset_card.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/card/distilabel_template.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/integration/test_pipe_llms.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/integration/test_pipe_simple.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/test_distiset.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/test_imports.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/test_pipeline.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/pipeline/test_app.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_anthropic.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_anyscale.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_azure.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_cohere.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_litellm.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_llamacpp.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_mistral.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_mixins.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_ollama.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_openai.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_together.py
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_vertexai.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/huggingface/test_inference_endpoints.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/huggingface/test_transformers.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/mixins/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/mixins/test_runtime_parameters.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/conftest.py
+-rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/test_base.py
+-rw-r--r--   0        0        0    18140 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/test_dag.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/test_local.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/__init__.py
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_base.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_combine.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_conversation.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_decorator.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_deita.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_expand.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_keep.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/test_base.py
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/test_preference.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/test_text_generation.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/generators/test_data.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/conftest.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_base.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_complexity_scorer.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_generate_embeddings.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_instruction_backtranslation.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_pair_rm.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_quality_scorer.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_self_instruct.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_text_generation.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_ultrafeedback.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_base.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_generator.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/test_base.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_chat.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_docstring.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_lists.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_typing.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.2/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.2/LICENSE
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.2/LICENSE_HEADER
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 distilabel-1.0.2/README.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 distilabel-1.0.2/PKG-INFO
```

### Comparing `distilabel-1.0.1/.pre-commit-config.yaml` & `distilabel-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/mkdocs.yml` & `distilabel-1.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/.github/ISSUE_TEMPLATE/🆕-feature-request.md` & `distilabel-1.0.2/.github/ISSUE_TEMPLATE/🆕-feature-request.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/.github/ISSUE_TEMPLATE/🐛-bug-report.md` & `distilabel-1.0.2/.github/ISSUE_TEMPLATE/🐛-bug-report.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/.github/ISSUE_TEMPLATE/📚-documentation-update.md` & `distilabel-1.0.2/.github/ISSUE_TEMPLATE/📚-documentation-update.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/.github/workflows/docs.yml` & `distilabel-1.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/.github/workflows/release.yml` & `distilabel-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/.github/workflows/test.yml` & `distilabel-1.0.2/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
           python_version=$(python -c "import sys; print(sys.version_info[:2])")
 
           if [ "${python_version}" != "(3, 8)" ]; then
             pip install -e .[dev,tests,cohere,hf-transformers,hf-inference-endpoints,vertexai,ollama,openai,together,argilla,mistralai,llama-cpp,anthropic,litellm]
           else
             pip install -e .[dev,tests,cohere,hf-transformers,hf-inference-endpoints,vertexai,ollama,openai,together,argilla,llama-cpp,anthropic,litellm]
           fi
-          pip install git+https://github.com/yuchenlin/LLM-Blender.git@3c2d71f
+          pip install git+https://github.com/argilla-io/LLM-Blender.git
 
       - name: Lint
         run: make lint
 
       - name: Unit Tests
         run: make unit-tests
```

### Comparing `distilabel-1.0.1/docs/index.md` & `distilabel-1.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/api/steps/tasks/text_generation.md` & `distilabel-1.0.2/docs/api/steps/tasks/text_generation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/distilabel-badge-dark.png` & `distilabel-1.0.2/docs/assets/distilabel-badge-dark.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/distilabel-badge-light.png` & `distilabel-1.0.2/docs/assets/distilabel-badge-light.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/distilabel-black.png` & `distilabel-1.0.2/docs/assets/distilabel-black.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/distilabel-icon.svg` & `distilabel-1.0.2/docs/assets/distilabel-icon.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/distilabel-white.png` & `distilabel-1.0.2/docs/assets/distilabel-white.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/logo.svg` & `distilabel-1.0.2/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/distilabel-diagram-dark.svg` & `distilabel-1.0.2/docs/assets/images/distilabel-diagram-dark.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/distilabel-diagram.svg` & `distilabel-1.0.2/docs/assets/images/distilabel-diagram.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_1.png` & `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_1.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_2.png` & `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_2.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_3.png` & `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_3.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_4.png` & `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_4.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/sections/cli/cli_pipe.png` & `distilabel-1.0.2/docs/assets/images/sections/cli/cli_pipe.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/preference.png` & `distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/preference.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/text_generation.png` & `distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/text_generation.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png` & `distilabel-1.0.2/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/tutorials-assets/preference_dataset_notus_ui.png` & `distilabel-1.0.2/docs/assets/tutorials-assets/preference_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/tutorials-assets/deita/datasets.png` & `distilabel-1.0.2/docs/assets/tutorials-assets/deita/datasets.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/tutorials-assets/deita/diversity.png` & `distilabel-1.0.2/docs/assets/tutorials-assets/deita/diversity.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/tutorials-assets/deita/overview.png` & `distilabel-1.0.2/docs/assets/tutorials-assets/deita/overview.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/assets/tutorials-assets/deita/results.png` & `distilabel-1.0.2/docs/assets/tutorials-assets/deita/results.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/scripts/gen_ref_pages.py` & `distilabel-1.0.2/docs/scripts/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/caching.md` & `distilabel-1.0.2/docs/sections/learn/caching.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/cli.md` & `distilabel-1.0.2/docs/sections/learn/cli.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/distiset.md` & `distilabel-1.0.2/docs/sections/learn/distiset.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/llms/index.md` & `distilabel-1.0.2/docs/sections/learn/llms/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/pipelines/index.md` & `distilabel-1.0.2/docs/sections/learn/pipelines/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/steps/argilla.md` & `distilabel-1.0.2/docs/sections/learn/steps/argilla.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/steps/general_steps.md` & `distilabel-1.0.2/docs/sections/learn/steps/general_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/steps/generator_steps.md` & `distilabel-1.0.2/docs/sections/learn/steps/generator_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/steps/global_steps.md` & `distilabel-1.0.2/docs/sections/learn/steps/global_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/steps/index.md` & `distilabel-1.0.2/docs/sections/learn/steps/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/tasks/feedback_tasks.md` & `distilabel-1.0.2/docs/sections/learn/tasks/feedback_tasks.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/tasks/index.md` & `distilabel-1.0.2/docs/sections/learn/tasks/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/tasks/special_tasks.md` & `distilabel-1.0.2/docs/sections/learn/tasks/special_tasks.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/learn/tasks/text_generation.md` & `distilabel-1.0.2/docs/sections/learn/tasks/text_generation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/papers/deita.md` & `distilabel-1.0.2/docs/sections/papers/deita.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/papers/instruction_backtranslation.md` & `distilabel-1.0.2/docs/sections/papers/instruction_backtranslation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/docs/sections/papers/ultrafeedback.md` & `distilabel-1.0.2/docs/sections/papers/ultrafeedback.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/__init__.py` & `distilabel-1.0.2/src/distilabel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rich import traceback as rich_traceback
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 rich_traceback.install(show_locals=True)
```

### Comparing `distilabel-1.0.1/src/distilabel/__main__.py` & `distilabel-1.0.2/src/distilabel/__main__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/distiset.py` & `distilabel-1.0.2/src/distilabel/distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/cli/__init__.py` & `distilabel-1.0.2/src/distilabel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/cli/app.py` & `distilabel-1.0.2/src/distilabel/cli/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/cli/pipeline/__init__.py` & `distilabel-1.0.2/src/distilabel/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/cli/pipeline/app.py` & `distilabel-1.0.2/src/distilabel/cli/pipeline/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/cli/pipeline/utils.py` & `distilabel-1.0.2/src/distilabel/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/__init__.py` & `distilabel-1.0.2/src/distilabel/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/anthropic.py` & `distilabel-1.0.2/src/distilabel/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/anyscale.py` & `distilabel-1.0.2/src/distilabel/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/azure.py` & `distilabel-1.0.2/src/distilabel/llms/azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/base.py` & `distilabel-1.0.2/src/distilabel/llms/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/chat_templates.py` & `distilabel-1.0.2/src/distilabel/llms/chat_templates.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/cohere.py` & `distilabel-1.0.2/src/distilabel/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/litellm.py` & `distilabel-1.0.2/src/distilabel/llms/litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/llamacpp.py` & `distilabel-1.0.2/src/distilabel/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/mistral.py` & `distilabel-1.0.2/src/distilabel/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/mixins.py` & `distilabel-1.0.2/src/distilabel/llms/mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/ollama.py` & `distilabel-1.0.2/src/distilabel/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/openai.py` & `distilabel-1.0.2/src/distilabel/llms/openai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/together.py` & `distilabel-1.0.2/src/distilabel/llms/together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/typing.py` & `distilabel-1.0.2/src/distilabel/llms/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/vertexai.py` & `distilabel-1.0.2/src/distilabel/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/vllm.py` & `distilabel-1.0.2/src/distilabel/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/huggingface/__init__.py` & `distilabel-1.0.2/src/distilabel/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/llms/huggingface/inference_endpoints.py` & `distilabel-1.0.2/src/distilabel/llms/huggingface/inference_endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
 import os
+import random
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from pydantic import (
     Field,
     PrivateAttr,
     SecretStr,
     ValidationError,
@@ -345,14 +346,17 @@
                 max_new_tokens=max_new_tokens,
                 do_sample=do_sample,
                 typical_p=typical_p,
                 repetition_penalty=repetition_penalty,
                 temperature=temperature,
                 top_p=top_p,
                 top_k=top_k,
+                # NOTE: here to ensure that the cache is not used and a different response is
+                # generated every time
+                seed=random.randint(0, 2147483647),
             )
             return [completion]
         except Exception as e:
             self._logger.warning(
                 f"⚠️ Received no response using Inference Client (model: '{self.model_name}')."
                 f" Finish reason was: {e}"
             )
```

### Comparing `distilabel-1.0.1/src/distilabel/llms/huggingface/transformers.py` & `distilabel-1.0.2/src/distilabel/llms/huggingface/transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/mixins/__init__.py` & `distilabel-1.0.2/src/distilabel/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/mixins/runtime_parameters.py` & `distilabel-1.0.2/src/distilabel/mixins/runtime_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         for name, value in runtime_parameters.items():
             if name not in self.runtime_parameters_names:
                 continue
 
             attr = getattr(self, name)
             if isinstance(attr, RuntimeParametersMixin):
                 attr.set_runtime_parameters(value)
+                self._runtime_parameters[name] = value
                 continue
 
             # Handle settings values for `_SecretField`
             field_info = self.model_fields[name]
             inner_type = _extract_runtime_parameter_inner_type(field_info.annotation)
             if inspect.isclass(inner_type) and issubclass(inner_type, _SecretField):
                 value = inner_type(value)
```

### Comparing `distilabel-1.0.1/src/distilabel/pipeline/__init__.py` & `distilabel-1.0.2/src/distilabel/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/pipeline/_dag.py` & `distilabel-1.0.2/src/distilabel/pipeline/_dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -341,15 +341,17 @@
             and step_input_parameter.kind != inspect.Parameter.VAR_POSITIONAL
         ):
             raise ValueError(
                 f"Step '{step_name}' should have a `*args` parameter with type hint `StepInput`"
                 f" to receive outputs from previous steps."
             )
 
-    def _validate_step_process_runtime_parameters(self, step: "_Step") -> None:
+    def _validate_step_process_runtime_parameters(  # noqa: C901
+        self, step: "_Step"
+    ) -> None:
         """Validates that the required runtime parameters of the step are provided. A
         runtime parameter is considered required if it doesn't have a default value. The
         name of the runtime parameters are separated by dots to represent nested parameters.
 
         Args:
             step: The step to validate.
 
@@ -363,34 +365,56 @@
             result = f'pipeline.run(parameters={{"{step_name}":'
             nested_dict = "..."
             for part in reversed(parts):
                 nested_dict = f' {{"{part}": {nested_dict}}}'
             result += nested_dict + "})"
             return result
 
+        def _get_attribute_default(
+            step: "_Step", composed_param_name: str
+        ) -> Union[Any, None]:
+            parts = composed_param_name.split(".")
+            attr = step
+            for part in parts:
+                if isinstance(attr, dict):
+                    attr = attr.get(part, None)
+                elif isinstance(attr, object):
+                    attr = getattr(attr, part)
+            return attr
+
         def _check_required_parameter(
             param_name: str,
             composed_param_name: str,
             is_optional_or_nested: Union[bool, "RuntimeParametersNames"],
             runtime_parameters: Dict[str, Any],
             runtime_parameters_names: "RuntimeParametersNames",
         ) -> None:
             if isinstance(is_optional_or_nested, dict):
                 runtime_parameters_names = runtime_parameters_names[param_name]  # type: ignore
                 for subparam, value in runtime_parameters_names.items():
                     _check_required_parameter(
                         param_name=subparam,
                         composed_param_name=f"{composed_param_name}.{subparam}",
                         is_optional_or_nested=value,
-                        runtime_parameters=runtime_parameters.get(subparam, {}),
+                        # NOTE: `runtime_parameters` get is for the specific case of `LLM` in `Task`
+                        runtime_parameters=runtime_parameters.get(
+                            param_name, runtime_parameters
+                        ),
                         runtime_parameters_names=runtime_parameters_names,
                     )
                 return
 
-            if not is_optional_or_nested and param_name not in runtime_parameters:
+            if (
+                not is_optional_or_nested
+                and param_name not in runtime_parameters
+                and _get_attribute_default(
+                    step=step, composed_param_name=composed_param_name
+                )
+                is None
+            ):
                 aux_code = _get_pipeline_aux_code(step.name, composed_param_name)
                 raise ValueError(
                     f"Step '{step.name}' is missing required runtime parameter '{param_name}'."
                     " Please, provide a value for it when calling `Pipeline.run` method:\n\n"
                     f"    {aux_code}"
                 )
```

### Comparing `distilabel-1.0.1/src/distilabel/pipeline/base.py` & `distilabel-1.0.2/src/distilabel/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/pipeline/local.py` & `distilabel-1.0.2/src/distilabel/pipeline/local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/pipeline/utils.py` & `distilabel-1.0.2/src/distilabel/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/base.py` & `distilabel-1.0.2/src/distilabel/steps/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/combine.py` & `distilabel-1.0.2/src/distilabel/steps/combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/conversation.py` & `distilabel-1.0.2/src/distilabel/steps/conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/decorator.py` & `distilabel-1.0.2/src/distilabel/steps/decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/deita.py` & `distilabel-1.0.2/src/distilabel/steps/deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/expand.py` & `distilabel-1.0.2/src/distilabel/steps/expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/keep.py` & `distilabel-1.0.2/src/distilabel/steps/keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/typing.py` & `distilabel-1.0.2/src/distilabel/steps/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/argilla/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/argilla/base.py` & `distilabel-1.0.2/src/distilabel/steps/argilla/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/argilla/preference.py` & `distilabel-1.0.2/src/distilabel/steps/argilla/preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/argilla/text_generation.py` & `distilabel-1.0.2/src/distilabel/steps/argilla/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/generators/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/generators/data.py` & `distilabel-1.0.2/src/distilabel/steps/generators/data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/generators/huggingface.py` & `distilabel-1.0.2/src/distilabel/steps/generators/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/globals/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/globals/huggingface.py` & `distilabel-1.0.2/src/distilabel/steps/globals/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/base.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/complexity_scorer.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/generate_embeddings.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/instruction_backtranslation.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/pair_rm.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/quality_scorer.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/self_instruct.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/text_generation.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/typing.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/ultrafeedback.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/base.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/generator.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/utils.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/__init__.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/base.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/utils.py` & `distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2` & `distilabel-1.0.2/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2` & `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2` & `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2` & `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2` & `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2` & `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/__init__.py` & `distilabel-1.0.2/src/distilabel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/chat.py` & `distilabel-1.0.2/src/distilabel/utils/chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/dicts.py` & `distilabel-1.0.2/src/distilabel/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/docstring.py` & `distilabel-1.0.2/src/distilabel/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/files.py` & `distilabel-1.0.2/src/distilabel/utils/files.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/itertools.py` & `distilabel-1.0.2/src/distilabel/utils/itertools.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/lists.py` & `distilabel-1.0.2/src/distilabel/utils/lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/logging.py` & `distilabel-1.0.2/src/distilabel/utils/logging.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/notebook.py` & `distilabel-1.0.2/src/distilabel/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/serialization.py` & `distilabel-1.0.2/src/distilabel/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/typing_.py` & `distilabel-1.0.2/src/distilabel/utils/typing_.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/card/__init__.py` & `distilabel-1.0.2/src/distilabel/utils/card/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/card/dataset_card.py` & `distilabel-1.0.2/src/distilabel/utils/card/dataset_card.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/src/distilabel/utils/card/distilabel_template.md` & `distilabel-1.0.2/src/distilabel/utils/card/distilabel_template.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/__init__.py` & `distilabel-1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/integration/test_pipe_llms.py` & `distilabel-1.0.2/tests/integration/test_pipe_llms.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/integration/test_pipe_simple.py` & `distilabel-1.0.2/tests/integration/test_pipe_simple.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/__init__.py` & `distilabel-1.0.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/test_distiset.py` & `distilabel-1.0.2/tests/unit/test_distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/test_imports.py` & `distilabel-1.0.2/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/cli/__init__.py` & `distilabel-1.0.2/tests/unit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/cli/test_pipeline.yaml` & `distilabel-1.0.2/tests/unit/cli/test_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/cli/utils.py` & `distilabel-1.0.2/tests/unit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/cli/pipeline/__init__.py` & `distilabel-1.0.2/tests/unit/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/cli/pipeline/test_app.py` & `distilabel-1.0.2/tests/unit/cli/pipeline/test_app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/cli/pipeline/utils.py` & `distilabel-1.0.2/tests/unit/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/__init__.py` & `distilabel-1.0.2/tests/unit/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_anthropic.py` & `distilabel-1.0.2/tests/unit/llms/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_anyscale.py` & `distilabel-1.0.2/tests/unit/llms/test_anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_azure.py` & `distilabel-1.0.2/tests/unit/llms/test_azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_cohere.py` & `distilabel-1.0.2/tests/unit/llms/test_cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_litellm.py` & `distilabel-1.0.2/tests/unit/llms/test_litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_llamacpp.py` & `distilabel-1.0.2/tests/unit/llms/test_llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_mistral.py` & `distilabel-1.0.2/tests/unit/llms/test_mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_mixins.py` & `distilabel-1.0.2/tests/unit/llms/test_mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_ollama.py` & `distilabel-1.0.2/tests/unit/llms/test_ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_openai.py` & `distilabel-1.0.2/tests/unit/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_together.py` & `distilabel-1.0.2/tests/unit/llms/test_together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/test_vertexai.py` & `distilabel-1.0.2/tests/unit/llms/test_vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/huggingface/__init__.py` & `distilabel-1.0.2/tests/unit/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/huggingface/test_inference_endpoints.py` & `distilabel-1.0.2/tests/unit/llms/huggingface/test_inference_endpoints.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/llms/huggingface/test_transformers.py` & `distilabel-1.0.2/tests/unit/llms/huggingface/test_transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/mixins/__init__.py` & `distilabel-1.0.2/tests/unit/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/mixins/test_runtime_parameters.py` & `distilabel-1.0.2/tests/unit/mixins/test_runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/pipeline/__init__.py` & `distilabel-1.0.2/tests/unit/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/pipeline/conftest.py` & `distilabel-1.0.2/tests/unit/pipeline/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/pipeline/test_base.py` & `distilabel-1.0.2/tests/unit/pipeline/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/pipeline/test_dag.py` & `distilabel-1.0.2/tests/unit/pipeline/test_dag.py`

 * *Files 5% similar despite different names*

```diff
@@ -315,29 +315,57 @@
             def inputs(self) -> List[str]:
                 return ["instruction"]
 
             @property
             def outputs(self) -> List[str]:
                 return ["response"]
 
-            def process(self) -> "GeneratorStepOutput":
+            def process(self, offset: int = 0) -> "GeneratorStepOutput":
                 yield [{"response": "response1"}], False
 
         step = DummyGeneratorStep(name="dummy_generator_step", pipeline=pipeline)  # type: ignore
         step.set_runtime_parameters({})
 
         dag = DAG()
         dag.add_step(step)
 
         with pytest.raises(
             ValueError,
             match="Step 'dummy_generator_step' is missing required runtime parameter 'runtime_param1'",
         ):
             dag.validate()
 
+    def test_validate_step_process_runtime_parameters(
+        self, pipeline: "Pipeline"
+    ) -> None:
+        class DummyGeneratorStep(GeneratorStep):
+            runtime_param1: RuntimeParameter[int]
+            runtime_param2: RuntimeParameter[int] = 5
+
+            @property
+            def inputs(self) -> List[str]:
+                return ["instruction"]
+
+            @property
+            def outputs(self) -> List[str]:
+                return ["response"]
+
+            def process(self, offset: int = 0) -> "GeneratorStepOutput":  # type: ignore
+                yield [{"response": "response1"}], False
+
+        step = DummyGeneratorStep(
+            name="dummy_generator_step", runtime_param1=2, pipeline=pipeline
+        )
+        step.set_runtime_parameters({})
+
+        dag = DAG()
+        dag.add_step(step)
+
+        dag.validate()
+
     def test_step_invalid_input_mappings(self, pipeline: "Pipeline") -> None:
         class DummyStep(Step):
             @property
             def inputs(self) -> List[str]:
                 return ["instruction"]
 
             @property
@@ -398,15 +426,17 @@
             def inputs(self) -> List[str]:
                 return ["instruction"]
 
             @property
             def outputs(self) -> List[str]:
                 return ["response"]
 
-            def process(self, *inputs: StepInput) -> "GeneratorStepOutput":  # type: ignore
+            def process(
+                self, *inputs: StepInput, offset: int = 0
+            ) -> "GeneratorStepOutput":  # type: ignore
                 yield [{"response": "response1"}], False
 
         step = DummyGeneratorStep(name="dummy_generator_step", pipeline=pipeline)
 
         dag = DAG()
         dag.add_step(step)
```

### Comparing `distilabel-1.0.1/tests/unit/pipeline/test_local.py` & `distilabel-1.0.2/tests/unit/pipeline/test_local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/pipeline/utils.py` & `distilabel-1.0.2/tests/unit/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/__init__.py` & `distilabel-1.0.2/tests/unit/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/test_base.py` & `distilabel-1.0.2/tests/unit/steps/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/test_combine.py` & `distilabel-1.0.2/tests/unit/steps/test_combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/test_conversation.py` & `distilabel-1.0.2/tests/unit/steps/test_conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/test_decorator.py` & `distilabel-1.0.2/tests/unit/steps/test_decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/test_deita.py` & `distilabel-1.0.2/tests/unit/steps/test_deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/test_expand.py` & `distilabel-1.0.2/tests/unit/steps/test_expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/test_keep.py` & `distilabel-1.0.2/tests/unit/steps/test_keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/argilla/__init__.py` & `distilabel-1.0.2/tests/unit/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/argilla/test_base.py` & `distilabel-1.0.2/tests/unit/steps/argilla/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/argilla/test_preference.py` & `distilabel-1.0.2/tests/unit/steps/argilla/test_preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/argilla/test_text_generation.py` & `distilabel-1.0.2/tests/unit/steps/argilla/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/generators/test_data.py` & `distilabel-1.0.2/tests/unit/steps/generators/test_data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/__init__.py` & `distilabel-1.0.2/tests/unit/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/conftest.py` & `distilabel-1.0.2/tests/unit/steps/tasks/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_base.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,162 +8,126 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, Any, Dict, List, Union
-
 import pytest
+from distilabel.llms.base import LLM
 from distilabel.pipeline.local import Pipeline
-from distilabel.steps.tasks.base import Task
+from distilabel.steps.tasks.evol_quality.base import (
+    EvolQuality,
+)
+from distilabel.steps.tasks.evol_quality.utils import MUTATION_TEMPLATES
 from pydantic import ValidationError
 
-from tests.unit.steps.tasks.utils import DummyLLM
-
-if TYPE_CHECKING:
-    from distilabel.steps.tasks.typing import ChatType
-
-
-class DummyTask(Task):
-    @property
-    def inputs(self) -> List[str]:
-        return ["instruction"]
-
-    def format_input(self, input: Dict[str, Any]) -> "ChatType":
-        return [
-            {"role": "system", "content": ""},
-            {"role": "user", "content": input["instruction"]},
-        ]
-
-    def format_output(self, output: Union[str, None], input: Dict[str, Any]) -> dict:
-        return {"output": output}
-
-
-class TestTask:
-    def test_passing_pipeline(self) -> None:
-        pipeline = Pipeline(name="unit-test-pipeline")
-        llm = DummyLLM()
-        task = DummyTask(name="task", llm=llm, pipeline=pipeline)
-        assert task.name == "task"
-        assert task.llm is llm
-        assert task.num_generations == 1
-        assert task.group_generations is False
-        assert task.pipeline is pipeline
-
-    def test_within_pipeline_context(self) -> None:
-        with Pipeline(name="unit-test-pipeline") as pipeline:
-            llm = DummyLLM()
-            task = DummyTask(name="task", llm=llm, pipeline=pipeline)
-            assert task.name == "task"
-            assert task.llm is llm
-        assert task.pipeline == pipeline
-
-    def test_with_errors(self) -> None:
-        with pytest.raises(ValueError, match="Step 'task' hasn't received a pipeline"):
-            DummyTask(name="task", llm=DummyLLM())
 
+class TestEvolQuality:
+    def test_with_errors(self, dummy_llm: LLM) -> None:
         with pytest.raises(
-            ValidationError, match="llm\n  Field required \\[type=missing"
+            ValidationError, match="num_evolutions\n  Field required \\[type=missing"
         ):
-            DummyTask(name="task", pipeline=Pipeline(name="unit-test-pipeline"))  # type: ignore
+            EvolQuality(name="task", pipeline=Pipeline(name="unit-test-pipeline"))  # type: ignore
 
-        with pytest.raises(
-            TypeError,
-            match="Can't instantiate abstract class Task with abstract methods format_input, format_output",
-        ):
-            Task(name="task", llm=DummyLLM())  # type: ignore
+        with pytest.raises(ValueError, match="Step 'task' hasn't received a pipeline"):
+            EvolQuality(name="task", llm=dummy_llm, num_evolutions=2)
+
+    def test_process(self, dummy_llm: LLM) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        task = EvolQuality(
+            name="task", llm=dummy_llm, num_evolutions=2, pipeline=pipeline
+        )
+        task.load()
+        assert list(task.process([{"instruction": "test", "response": "mock"}])) == [
+            [
+                {
+                    "instruction": "test",
+                    "response": "mock",
+                    "evolved_response": "output",
+                    "model_name": "test",
+                }
+            ]
+        ]
 
-    @pytest.mark.parametrize(
-        "group_generations, expected",
-        [
-            (
-                False,
-                [
-                    {"instruction": "test", "output": "output", "model_name": "test"},
-                    {"instruction": "test", "output": "output", "model_name": "test"},
-                    {"instruction": "test", "output": "output", "model_name": "test"},
-                ],
-            ),
-            (
-                True,
-                [
-                    {
-                        "instruction": "test",
-                        "output": ["output", "output", "output"],
-                        "model_name": "test",
-                    },
-                ],
-            ),
-        ],
-    )
-    def test_process(
-        self, group_generations: bool, expected: List[Dict[str, Any]]
-    ) -> None:
+    def test_process_store_evolutions(self, dummy_llm: LLM) -> None:
         pipeline = Pipeline(name="unit-test-pipeline")
-        llm = DummyLLM()
-        task = DummyTask(
+        task = EvolQuality(
             name="task",
-            llm=llm,
+            llm=dummy_llm,
+            num_evolutions=2,
+            store_evolutions=True,
             pipeline=pipeline,
-            group_generations=group_generations,
-            num_generations=3,
         )
-        result = next(task.process([{"instruction": "test"}]))
-        assert result == expected
+        task.load()
+        assert list(task.process([{"instruction": "test", "response": "mock"}])) == [
+            [
+                {
+                    "instruction": "test",
+                    "response": "mock",
+                    "evolved_responses": ["output", "output"],
+                    "model_name": "test",
+                }
+            ]
+        ]
 
-    def test_serialization(self) -> None:
+    def test_serialization(self, dummy_llm: LLM) -> None:
         pipeline = Pipeline(name="unit-test-pipeline")
-        llm = DummyLLM()
-        task = DummyTask(name="task", llm=llm, pipeline=pipeline)
+        task = EvolQuality(
+            name="task", llm=dummy_llm, num_evolutions=2, pipeline=pipeline
+        )
+        task.load()
         assert task.dump() == {
             "name": "task",
-            "input_mappings": {},
-            "output_mappings": {},
-            "input_batch_size": 50,
+            "input_mappings": task.input_mappings,
+            "output_mappings": task.output_mappings,
+            "input_batch_size": task.input_batch_size,
             "llm": {
                 "generation_kwargs": {},
                 "type_info": {
-                    "module": "tests.unit.steps.tasks.utils",
-                    "name": "DummyLLM",
+                    "module": task.llm.__module__,
+                    "name": task.llm.__class__.__name__,
                 },
             },
-            "group_generations": False,
-            "num_generations": 1,
+            "num_evolutions": task.num_evolutions,
+            "store_evolutions": task.store_evolutions,
+            "mutation_templates": MUTATION_TEMPLATES,
+            "num_generations": task.num_generations,
+            "group_generations": task.group_generations,
+            "include_original_response": task.include_original_response,
+            "seed": task.seed,
             "runtime_parameters_info": [
                 {
                     "description": "The number of rows that will contain the batches processed by the step.",
                     "name": "input_batch_size",
                     "optional": True,
                 },
                 {
                     "name": "llm",
                     "runtime_parameters_info": [
                         {
-                            "description": "The kwargs to be propagated to either `generate` or "
-                            "`agenerate` methods within each `LLM`.",
-                            "keys": [
-                                {
-                                    "name": "kwargs",
-                                    "optional": False,
-                                },
-                            ],
                             "name": "generation_kwargs",
-                        },
+                            "description": "The kwargs to be propagated to either `generate` or `agenerate` methods within each `LLM`.",
+                            "keys": [],
+                        }
                     ],
                 },
                 {
                     "name": "num_generations",
+                    "optional": True,
                     "description": "The number of generations to be produced per input.",
+                },
+                {
+                    "name": "seed",
                     "optional": True,
+                    "description": "As `numpy` is being used in order to randomly pick a mutation method, then is nice to set a random seed.",
                 },
             ],
             "type_info": {
-                "module": "tests.unit.steps.tasks.test_base",
-                "name": "DummyTask",
+                "module": task.__module__,
+                "name": task.__class__.__name__,
             },
         }
 
         with Pipeline(name="unit-test-pipeline") as pipeline:
-            new_task = DummyTask.from_dict(task.dump())
-            assert isinstance(new_task, DummyTask)
+            new_task = EvolQuality.from_dict(task.dump())
+            assert isinstance(new_task, EvolQuality)
```

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_complexity_scorer.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_generate_embeddings.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_instruction_backtranslation.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_pair_rm.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_quality_scorer.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_self_instruct.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_text_generation.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/test_ultrafeedback.py` & `distilabel-1.0.2/tests/unit/steps/tasks/test_ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/utils.py` & `distilabel-1.0.2/tests/unit/steps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_base.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_generator.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/steps/tasks/evol_quality/__init__.py` & `distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/utils/__init__.py` & `distilabel-1.0.2/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/utils/test_chat.py` & `distilabel-1.0.2/tests/unit/utils/test_chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/utils/test_docstring.py` & `distilabel-1.0.2/tests/unit/utils/test_docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/utils/test_lists.py` & `distilabel-1.0.2/tests/unit/utils/test_lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/tests/unit/utils/test_typing.py` & `distilabel-1.0.2/tests/unit/utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/.gitignore` & `distilabel-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/LICENSE` & `distilabel-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/LICENSE_HEADER` & `distilabel-1.0.2/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/README.md` & `distilabel-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/pyproject.toml` & `distilabel-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.1/PKG-INFO` & `distilabel-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: distilabel
-Version: 1.0.1
+Version: 1.0.2
 Summary: AI Feedback (AIF) framework
 Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues
 Project-URL: Source, https://github.com/argilla/distilabel
 Author-email: Argilla <admin@argilla.io>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cdvnpxu2_/tmpdjfm52sb_TarContainer/0/255", line 85, column 75: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: distilabel Version: 1.0.1 Summary: AI Feedback
+Metadata-Version: 2.3 Name: distilabel Version: 1.0.2 Summary: AI Feedback
 (AIF) framework Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues Project-URL:
 Source, https://github.com/argilla/distilabel Author-email: Argilla
 argilla.io> License-Expression: MIT License-File: LICENSE License-File:
 LICENSE_HEADER Keywords: alignment,annotation,data,llm,rlaif,synthetic
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
```


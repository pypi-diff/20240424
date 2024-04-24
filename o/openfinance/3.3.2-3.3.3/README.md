# Comparing `tmp/openfinance-3.3.2.tar.gz` & `tmp/openfinance-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfinance-3.3.2.tar", last modified: Wed Apr 17 09:39:51 2024, max compression
+gzip compressed data, was "openfinance-3.3.3.tar", last modified: Tue Apr 23 07:15:59 2024, max compression
```

## Comparing `openfinance-3.3.2.tar` & `openfinance-3.3.3.tar`

### file list

```diff
@@ -1,404 +1,405 @@
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.850245 openfinance-3.3.2/
--rw-r-----   0 root         (0) root         (0)     1062 2023-06-14 01:17:13.000000 openfinance-3.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2274 2024-04-17 09:39:51.850245 openfinance-3.3.2/PKG-INFO
--rw-r-----   0 root         (0) root         (0)     1840 2023-12-21 07:23:25.000000 openfinance-3.3.2/README.md
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.806244 openfinance-3.3.2/openfinance/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.807244 openfinance-3.3.2/openfinance/agentflow/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agentflow/__init__.py
--rw-r-----   0 root         (0) root         (0)      213 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agentflow/base_parser.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.807244 openfinance-3.3.2/openfinance/agentflow/flow/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agentflow/flow/__init__.py
--rw-r-----   0 root         (0) root         (0)     2006 2024-04-07 08:43:31.000000 openfinance-3.3.2/openfinance/agentflow/flow/agent_base.py
--rw-r-----   0 root         (0) root         (0)      879 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agentflow/flow/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.808244 openfinance-3.3.2/openfinance/agentflow/llm/
--rw-r-----   0 root         (0) root         (0)        1 2024-03-22 06:30:29.000000 openfinance-3.3.2/openfinance/agentflow/llm/__init__.py
--rw-r-----   0 root         (0) root         (0)     1672 2024-02-02 09:21:46.000000 openfinance-3.3.2/openfinance/agentflow/llm/aliyungpt.py
--rw-r-----   0 root         (0) root         (0)     1420 2023-12-26 02:09:05.000000 openfinance-3.3.2/openfinance/agentflow/llm/base.py
--rw-r-----   0 root         (0) root         (0)     1690 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agentflow/llm/chatgpt.py
--rw-r-----   0 root         (0) root         (0)     2121 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agentflow/llm/ernie.py
--rw-r-----   0 root         (0) root         (0)     1455 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/agentflow/llm/manager.py
--rw-r-----   0 root         (0) root         (0)     1387 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agentflow/llm/webgpt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.808244 openfinance-3.3.2/openfinance/agentflow/memory/
--rw-r-----   0 root         (0) root         (0)        0 2024-01-12 03:13:37.000000 openfinance-3.3.2/openfinance/agentflow/memory/__init__.py
--rw-r-----   0 root         (0) root         (0)     1264 2024-01-19 08:54:48.000000 openfinance-3.3.2/openfinance/agentflow/memory/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.808244 openfinance-3.3.2/openfinance/agentflow/prompt/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agentflow/prompt/__init__.py
--rw-r-----   0 root         (0) root         (0)      582 2024-01-17 09:39:08.000000 openfinance-3.3.2/openfinance/agentflow/prompt/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.809244 openfinance-3.3.2/openfinance/agentflow/tool/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agentflow/tool/__init__.py
--rw-r-----   0 root         (0) root         (0)      947 2024-03-26 02:20:47.000000 openfinance-3.3.2/openfinance/agentflow/tool/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.809244 openfinance-3.3.2/openfinance/agents/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-29 03:13:30.000000 openfinance-3.3.2/openfinance/agents/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.810244 openfinance-3.3.2/openfinance/agents/agent/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-25 05:50:49.000000 openfinance-3.3.2/openfinance/agents/agent/__init__.py
--rw-r-----   0 root         (0) root         (0)     1149 2024-04-08 09:39:41.000000 openfinance-3.3.2/openfinance/agents/agent/agent_prompt.py
--rw-r-----   0 root         (0) root         (0)     2693 2024-04-07 09:58:21.000000 openfinance-3.3.2/openfinance/agents/agent/base.py
--rw-r-----   0 root         (0) root         (0)     1102 2024-01-19 03:21:37.000000 openfinance-3.3.2/openfinance/agents/agent/output_parser.py
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agents/callback.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.810244 openfinance-3.3.2/openfinance/agents/promptflow/
--rw-r-----   0 root         (0) root         (0)        0 2024-01-05 06:44:58.000000 openfinance-3.3.2/openfinance/agents/promptflow/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.810244 openfinance-3.3.2/openfinance/agents/promptflow/crawl/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-26 07:00:28.000000 openfinance-3.3.2/openfinance/agents/promptflow/crawl/__init__.py
--rw-r-----   0 root         (0) root         (0)     3466 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/crawl/base.py
--rw-r-----   0 root         (0) root         (0)      398 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/crawl/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.811244 openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/
--rw-r-----   0 root         (0) root         (0)        0 2024-01-26 03:18:11.000000 openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/__init__.py
--rw-r-----   0 root         (0) root         (0)     1808 2024-01-31 06:54:31.000000 openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/base.py
--rw-r-----   0 root         (0) root         (0)      514 2024-02-02 09:39:38.000000 openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/output_parser.py
--rw-r-----   0 root         (0) root         (0)     1140 2024-02-02 09:47:29.000000 openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.811244 openfinance-3.3.2/openfinance/agents/promptflow/entity/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-13 08:33:15.000000 openfinance-3.3.2/openfinance/agents/promptflow/entity/__init__.py
--rw-r-----   0 root         (0) root         (0)     3452 2024-01-25 08:48:24.000000 openfinance-3.3.2/openfinance/agents/promptflow/entity/base.py
--rw-r-----   0 root         (0) root         (0)      693 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/entity/output_parser.py
--rw-r-----   0 root         (0) root         (0)      491 2024-01-25 08:50:41.000000 openfinance-3.3.2/openfinance/agents/promptflow/entity/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.811244 openfinance-3.3.2/openfinance/agents/promptflow/factor/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-08 14:06:54.000000 openfinance-3.3.2/openfinance/agents/promptflow/factor/__init__.py
--rw-r-----   0 root         (0) root         (0)     2471 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/agents/promptflow/factor/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.812244 openfinance-3.3.2/openfinance/agents/promptflow/function/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/__init__.py
--rw-r-----   0 root         (0) root         (0)     5006 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.812244 openfinance-3.3.2/openfinance/agents/promptflow/function/multi_function/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-25 02:41:44.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/multi_function/__init__.py
--rw-r-----   0 root         (0) root         (0)     3224 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/multi_function/base.py
--rw-r-----   0 root         (0) root         (0)      923 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/multi_function/output_parser.py
--rw-r-----   0 root         (0) root         (0)      445 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/multi_function/prompt.py
--rw-r-----   0 root         (0) root         (0)      923 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/output_parser.py
--rw-r-----   0 root         (0) root         (0)      702 2024-01-26 02:54:07.000000 openfinance-3.3.2/openfinance/agents/promptflow/function/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.813244 openfinance-3.3.2/openfinance/agents/promptflow/percept/
--rw-r-----   0 root         (0) root         (0)       72 2024-01-05 08:38:23.000000 openfinance-3.3.2/openfinance/agents/promptflow/percept/__init__.py
--rw-r-----   0 root         (0) root         (0)     2311 2024-02-02 04:43:18.000000 openfinance-3.3.2/openfinance/agents/promptflow/percept/match.py
--rw-r-----   0 root         (0) root         (0)     1514 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/percept/opinion.py
--rw-r-----   0 root         (0) root         (0)      696 2024-01-25 09:30:05.000000 openfinance-3.3.2/openfinance/agents/promptflow/percept/output_parser.py
--rw-r-----   0 root         (0) root         (0)     2155 2024-03-11 06:34:31.000000 openfinance-3.3.2/openfinance/agents/promptflow/percept/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.814244 openfinance-3.3.2/openfinance/agents/promptflow/plan/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agents/promptflow/plan/__init__.py
--rw-r-----   0 root         (0) root         (0)     1666 2024-01-18 06:08:03.000000 openfinance-3.3.2/openfinance/agents/promptflow/plan/base.py
--rw-r-----   0 root         (0) root         (0)     1070 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/plan/output_parser.py
--rw-r-----   0 root         (0) root         (0)     1062 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/plan/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.814244 openfinance-3.3.2/openfinance/agents/promptflow/recall/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-23 07:10:45.000000 openfinance-3.3.2/openfinance/agents/promptflow/recall/__init__.py
--rw-r-----   0 root         (0) root         (0)     1853 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/agents/promptflow/recall/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.814244 openfinance-3.3.2/openfinance/agents/promptflow/summary/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/agents/promptflow/summary/__init__.py
--rw-r-----   0 root         (0) root         (0)     1676 2024-01-18 06:09:00.000000 openfinance-3.3.2/openfinance/agents/promptflow/summary/base.py
--rw-r-----   0 root         (0) root         (0)      576 2024-02-01 08:33:31.000000 openfinance-3.3.2/openfinance/agents/promptflow/summary/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.815244 openfinance-3.3.2/openfinance/agents/role/
--rw-r-----   0 root         (0) root         (0)        0 2024-01-11 09:40:34.000000 openfinance-3.3.2/openfinance/agents/role/__init__.py
--rw-r-----   0 root         (0) root         (0)      143 2024-04-09 02:31:25.000000 openfinance-3.3.2/openfinance/agents/role/base.py
--rw-r-----   0 root         (0) root         (0)     1415 2024-04-09 02:29:48.000000 openfinance-3.3.2/openfinance/agents/role/manager.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.816244 openfinance-3.3.2/openfinance/agents/role/prompts/
--rw-r-----   0 root         (0) root         (0)      827 2024-01-17 08:00:36.000000 openfinance-3.3.2/openfinance/agents/role/prompts/__init__.py
--rw-r-----   0 root         (0) root         (0)      547 2024-04-07 08:41:47.000000 openfinance-3.3.2/openfinance/agents/role/prompts/base.py
--rw-r-----   0 root         (0) root         (0)      268 2024-04-07 08:40:42.000000 openfinance-3.3.2/openfinance/agents/role/prompts/catherine_wood.py
--rw-r-----   0 root         (0) root         (0)      258 2024-04-07 08:40:42.000000 openfinance-3.3.2/openfinance/agents/role/prompts/elon_musk.py
--rw-r-----   0 root         (0) root         (0)      261 2024-04-07 08:40:42.000000 openfinance-3.3.2/openfinance/agents/role/prompts/growth_investor.py
--rw-r-----   0 root         (0) root         (0)      259 2024-04-07 08:40:42.000000 openfinance-3.3.2/openfinance/agents/role/prompts/quant_investor.py
--rw-r-----   0 root         (0) root         (0)      258 2024-04-07 08:40:48.000000 openfinance-3.3.2/openfinance/agents/role/prompts/ray_dalio.py
--rw-r-----   0 root         (0) root         (0)      263 2024-04-07 08:40:42.000000 openfinance-3.3.2/openfinance/agents/role/prompts/valuation_investor.py
--rw-r-----   0 root         (0) root         (0)      268 2024-04-07 08:40:42.000000 openfinance-3.3.2/openfinance/agents/role/prompts/warren_buffett.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.816244 openfinance-3.3.2/openfinance/agents/third_party/
--rw-r-----   0 root         (0) root         (0)        0 2024-01-08 02:44:19.000000 openfinance-3.3.2/openfinance/agents/third_party/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.817244 openfinance-3.3.2/openfinance/agents/tool/
--rw-r-----   0 root         (0) root         (0)        0 2024-01-05 06:48:36.000000 openfinance-3.3.2/openfinance/agents/tool/__init__.py
--rw-r-----   0 root         (0) root         (0)     2546 2024-04-17 09:24:46.000000 openfinance-3.3.2/openfinance/agents/tool/factor_search.py
--rw-r-----   0 root         (0) root         (0)     2486 2024-04-17 09:24:46.000000 openfinance-3.3.2/openfinance/agents/tool/search.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.817244 openfinance-3.3.2/openfinance/config/
--rw-r-----   0 root         (0) root         (0)       39 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/config/__init__.py
--rw-r-----   0 root         (0) root         (0)      575 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/config/config.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.817244 openfinance-3.3.2/openfinance/datacenter/
--rw-r-----   0 root         (0) root         (0)        0 2023-08-05 14:03:51.000000 openfinance-3.3.2/openfinance/datacenter/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.817244 openfinance-3.3.2/openfinance/datacenter/database/
--rw-r-----   0 root         (0) root         (0)       43 2023-12-08 14:06:54.000000 openfinance-3.3.2/openfinance/datacenter/database/__init__.py
--rw-r-----   0 root         (0) root         (0)    18948 2024-03-27 02:50:21.000000 openfinance-3.3.2/openfinance/datacenter/database/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.819244 openfinance-3.3.2/openfinance/datacenter/database/fundamental/
--rw-r-----   0 root         (0) root         (0)      813 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/__init__.py
--rw-r-----   0 root         (0) root         (0)      810 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/business_model.py
--rw-r-----   0 root         (0) root         (0)     2427 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/competitiveness.py
--rw-r-----   0 root         (0) root         (0)    14000 2024-04-08 09:58:55.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/financial.py
--rw-r-----   0 root         (0) root         (0)      906 2024-03-15 08:37:17.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/fundamental.py
--rw-r-----   0 root         (0) root         (0)     1984 2024-03-15 08:54:13.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/industry.py
--rw-r-----   0 root         (0) root         (0)    10779 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/macro.py
--rw-r-----   0 root         (0) root         (0)     2522 2024-03-15 08:37:17.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/market.py
--rw-r-----   0 root         (0) root         (0)     3198 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/money_flow.py
--rw-r-----   0 root         (0) root         (0)     2757 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/news.py
--rw-r-----   0 root         (0) root         (0)     2653 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/sentiment.py
--rw-r-----   0 root         (0) root         (0)     2215 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/valuation.py
--rw-r-----   0 root         (0) root         (0)     2883 2024-03-04 09:07:54.000000 openfinance-3.3.2/openfinance/datacenter/database/fundamental/volume.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.822245 openfinance-3.3.2/openfinance/datacenter/database/quant/
--rw-r-----   0 root         (0) root         (0)     1339 2024-03-04 07:35:50.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/ADX.py
--rw-r-----   0 root         (0) root         (0)     1091 2024-03-04 07:38:24.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/AROON.py
--rw-r-----   0 root         (0) root         (0)     1242 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/BBIC.py
--rw-r-----   0 root         (0) root         (0)     1361 2023-12-19 06:39:24.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/BR.py
--rw-r-----   0 root         (0) root         (0)     1347 2023-12-19 05:46:41.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/BearBullPower.py
--rw-r-----   0 root         (0) root         (0)     1443 2023-12-19 05:46:42.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/CCI.py
--rw-r-----   0 root         (0) root         (0)     1549 2023-12-19 05:46:42.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/CR.py
--rw-r-----   0 root         (0) root         (0)     1081 2024-03-20 08:24:55.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/MACD.py
--rw-r-----   0 root         (0) root         (0)     1132 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/MASS.py
--rw-r-----   0 root         (0) root         (0)     1360 2024-03-04 07:41:13.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/OBV.py
--rw-r-----   0 root         (0) root         (0)     1103 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/RSI.py
--rw-r-----   0 root         (0) root         (0)     1334 2023-12-19 05:46:42.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/TRIX.py
--rw-r-----   0 root         (0) root         (0)     1603 2023-12-19 05:46:42.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/VPT.py
--rw-r-----   0 root         (0) root         (0)     1419 2023-12-19 05:46:42.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/VR.py
--rw-r-----   0 root         (0) root         (0)     1033 2023-12-19 05:52:40.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/__init__.py
--rw-r-----   0 root         (0) root         (0)      613 2024-03-05 09:18:46.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/call.py
--rw-r-----   0 root         (0) root         (0)     1082 2023-12-26 02:39:35.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/technical.py
--rw-r-----   0 root         (0) root         (0)     1819 2023-12-19 05:47:37.000000 openfinance-3.3.2/openfinance/datacenter/database/quant/utils.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.822245 openfinance-3.3.2/openfinance/datacenter/database/source/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.822245 openfinance-3.3.2/openfinance/datacenter/database/source/cninfo/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/cninfo/__init__.py
--rw-r-----   0 root         (0) root         (0)     1269 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/cninfo/report.py
--rw-r-----   0 root         (0) root         (0)     2282 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/cninfo/util.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.824244 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/
--rw-r-----   0 root         (0) root         (0)      139 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/__init__.py
--rw-r-----   0 root         (0) root         (0)     3459 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/bond.py
--rw-r-----   0 root         (0) root         (0)    10569 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/fund.py
--rw-r-----   0 root         (0) root         (0)     3741 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/fundamental.py
--rw-r-----   0 root         (0) root         (0)     4489 2024-03-01 07:31:12.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/future.py
--rw-r-----   0 root         (0) root         (0)     9195 2023-12-26 07:30:59.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/industry.py
--rw-r-----   0 root         (0) root         (0)     2827 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/market.py
--rw-r-----   0 root         (0) root         (0)     3103 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/money.py
--rw-r-----   0 root         (0) root         (0)     3894 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/news.py
--rw-r-----   0 root         (0) root         (0)    32264 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/report.py
--rw-r-----   0 root         (0) root         (0)     5460 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/technical.py
--rw-r-----   0 root         (0) root         (0)    30214 2024-03-20 03:32:53.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/trade.py
--rw-r-----   0 root         (0) root         (0)     8795 2024-02-08 07:26:20.000000 openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/util.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.825245 openfinance-3.3.2/openfinance/datacenter/database/source/event/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/event/__init__.py
--rw-r-----   0 root         (0) root         (0)     1007 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/event/base.py
--rw-r-----   0 root         (0) root         (0)     2436 2024-01-30 02:45:38.000000 openfinance-3.3.2/openfinance/datacenter/database/source/event/cailianshe.py
--rw-r-----   0 root         (0) root         (0)     2644 2023-12-22 09:38:08.000000 openfinance-3.3.2/openfinance/datacenter/database/source/event/caixing.py
--rw-r-----   0 root         (0) root         (0)     2462 2024-01-30 09:08:46.000000 openfinance-3.3.2/openfinance/datacenter/database/source/event/investing.py
--rw-r-----   0 root         (0) root         (0)     5305 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/database/source/event/jin10.py
--rw-r-----   0 root         (0) root         (0)     6609 2023-12-13 08:33:15.000000 openfinance-3.3.2/openfinance/datacenter/database/source/event/news.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.825245 openfinance-3.3.2/openfinance/datacenter/database/source/sina/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/source/sina/__init__.py
--rw-r-----   0 root         (0) root         (0)      236 2024-02-27 06:53:18.000000 openfinance-3.3.2/openfinance/datacenter/database/source/sina/moneyflow.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.826244 openfinance-3.3.2/openfinance/datacenter/database/storage/
--rw-r-----   0 root         (0) root         (0)     1543 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/__init__.py
--rw-r-----   0 root         (0) root         (0)     1034 2023-12-01 06:19:13.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.827245 openfinance-3.3.2/openfinance/datacenter/database/storage/china/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/china/__init__.py
--rw-r-----   0 root         (0) root         (0)     4870 2023-12-26 08:47:24.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/china/industry.py
--rw-r-----   0 root         (0) root         (0)    20814 2023-12-14 08:18:55.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/china/macro.py
--rw-r-----   0 root         (0) root         (0)     1866 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/china/market.py
--rw-r-----   0 root         (0) root         (0)     1568 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/china/quant.py
--rw-r-----   0 root         (0) root         (0)    28030 2024-03-15 06:33:38.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/china/stock.py
--rw-r-----   0 root         (0) root         (0)    10418 2024-03-18 02:34:13.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/financial.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.828245 openfinance-3.3.2/openfinance/datacenter/database/storage/fred/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/fred/__init__.py
--rw-r-----   0 root         (0) root         (0)     2084 2023-12-01 06:17:14.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/fred/base.py
--rw-r-----   0 root         (0) root         (0)     1065 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/fred/store.py
--rw-r-----   0 root         (0) root         (0)     1066 2024-03-18 02:34:08.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/gov_stat.py
--rw-r-----   0 root         (0) root         (0)     1815 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/industry.py
--rw-r-----   0 root         (0) root         (0)     1693 2024-03-18 02:34:01.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/macro.py
--rw-r-----   0 root         (0) root         (0)      926 2024-03-18 02:34:18.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/market.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.828245 openfinance-3.3.2/openfinance/datacenter/database/storage/national_data/
--rw-r-----   0 root         (0) root         (0)      912 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/national_data/__init__.py
--rw-r-----   0 root         (0) root         (0)     2343 2023-11-27 13:51:06.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/national_data/base.py
--rw-r-----   0 root         (0) root         (0)     1090 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/national_data/store.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.829244 openfinance-3.3.2/openfinance/datacenter/database/storage/us/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/us/__init__.py
--rw-r-----   0 root         (0) root         (0)     8558 2023-12-19 09:14:17.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/us/base.py
--rw-r-----   0 root         (0) root         (0)     1194 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/us/financial.py
--rw-r-----   0 root         (0) root         (0)     4001 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/storage/us/util.py
--rw-r-----   0 root         (0) root         (0)     1495 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/datacenter/database/wrapper.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.830245 openfinance-3.3.2/openfinance/datacenter/echarts/
--rw-r-----   0 root         (0) root         (0)      578 2023-11-24 01:27:33.000000 openfinance-3.3.2/openfinance/datacenter/echarts/__init__.py
--rw-r-----   0 root         (0) root         (0)     1222 2023-10-12 07:53:22.000000 openfinance-3.3.2/openfinance/datacenter/echarts/bar.py
--rw-r-----   0 root         (0) root         (0)      523 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/datacenter/echarts/base.py
--rw-r-----   0 root         (0) root         (0)     1045 2023-10-13 06:59:29.000000 openfinance-3.3.2/openfinance/datacenter/echarts/multibar.py
--rw-r-----   0 root         (0) root         (0)     1337 2023-10-12 09:56:12.000000 openfinance-3.3.2/openfinance/datacenter/echarts/pie.py
--rw-r-----   0 root         (0) root         (0)     1981 2023-11-24 01:27:33.000000 openfinance-3.3.2/openfinance/datacenter/echarts/stacked_line.py
--rw-r-----   0 root         (0) root         (0)     1665 2023-11-24 01:27:33.000000 openfinance-3.3.2/openfinance/datacenter/echarts/tree.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.831245 openfinance-3.3.2/openfinance/datacenter/knowledge/
--rw-r-----   0 root         (0) root         (0)        0 2023-08-05 14:03:51.000000 openfinance-3.3.2/openfinance/datacenter/knowledge/__init__.py
--rw-r-----   0 root         (0) root         (0)     1047 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/knowledge/decorator.py
--rw-r-----   0 root         (0) root         (0)     4636 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/knowledge/entity_graph.py
--rw-r-----   0 root         (0) root         (0)     2861 2024-03-26 02:15:35.000000 openfinance-3.3.2/openfinance/datacenter/knowledge/executor.py
--rw-r-----   0 root         (0) root         (0)     4012 2024-03-29 09:58:11.000000 openfinance-3.3.2/openfinance/datacenter/knowledge/factor.py
--rw-r-----   0 root         (0) root         (0)     5825 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/datacenter/knowledge/graph.py
--rw-r-----   0 root         (0) root         (0)     1583 2023-12-08 14:06:54.000000 openfinance-3.3.2/openfinance/datacenter/knowledge/wrapper.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.831245 openfinance-3.3.2/openfinance/robot/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-15 01:39:28.000000 openfinance-3.3.2/openfinance/robot/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.831245 openfinance-3.3.2/openfinance/searchhub/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.832244 openfinance-3.3.2/openfinance/searchhub/page_manage/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/page_manage/__init__.py
--rw-r-----   0 root         (0) root         (0)      518 2023-09-16 02:17:44.000000 openfinance-3.3.2/openfinance/searchhub/page_manage/base.py
--rw-r-----   0 root         (0) root         (0)     1838 2024-03-15 08:53:08.000000 openfinance-3.3.2/openfinance/searchhub/page_manage/company.py
--rw-r-----   0 root         (0) root         (0)     1356 2023-08-05 14:03:51.000000 openfinance-3.3.2/openfinance/searchhub/page_manage/factor.py
--rw-r-----   0 root         (0) root         (0)     2096 2023-09-18 06:50:34.000000 openfinance-3.3.2/openfinance/searchhub/page_manage/model.py
--rw-r-----   0 root         (0) root         (0)     1040 2024-01-31 02:53:57.000000 openfinance-3.3.2/openfinance/searchhub/page_manage/role.py
--rw-r-----   0 root         (0) root         (0)     2620 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/searchhub/page_manage/user.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.832244 openfinance-3.3.2/openfinance/searchhub/page_rank/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/page_rank/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.833245 openfinance-3.3.2/openfinance/searchhub/query_understand/
--rw-r-----   0 root         (0) root         (0)        0 2023-12-13 09:36:00.000000 openfinance-3.3.2/openfinance/searchhub/query_understand/__init__.py
--rw-r-----   0 root         (0) root         (0)     1239 2023-12-14 07:14:38.000000 openfinance-3.3.2/openfinance/searchhub/query_understand/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.833245 openfinance-3.3.2/openfinance/searchhub/recall/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:31:57.000000 openfinance-3.3.2/openfinance/searchhub/recall/__init__.py
--rw-r-----   0 root         (0) root         (0)      928 2023-11-30 08:38:33.000000 openfinance-3.3.2/openfinance/searchhub/recall/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.833245 openfinance-3.3.2/openfinance/searchhub/recall/channel/
--rw-r-----   0 root         (0) root         (0)        0 2023-08-05 14:03:51.000000 openfinance-3.3.2/openfinance/searchhub/recall/channel/__init__.py
--rw-r-----   0 root         (0) root         (0)      110 2023-11-29 03:41:36.000000 openfinance-3.3.2/openfinance/searchhub/recall/channel/analysis.py
--rw-r-----   0 root         (0) root         (0)      138 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/searchhub/recall/channel/search.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.834245 openfinance-3.3.2/openfinance/searchhub/task/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-25 05:51:52.000000 openfinance-3.3.2/openfinance/searchhub/task/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.834245 openfinance-3.3.2/openfinance/searchhub/task/analysis/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-23 09:14:10.000000 openfinance-3.3.2/openfinance/searchhub/task/analysis/__init__.py
--rw-r-----   0 root         (0) root         (0)     4422 2024-04-07 09:13:07.000000 openfinance-3.3.2/openfinance/searchhub/task/analysis/analysis_task.py
--rw-r-----   0 root         (0) root         (0)      744 2024-01-19 08:33:50.000000 openfinance-3.3.2/openfinance/searchhub/task/analysis/auto_analysis.py
--rw-r-----   0 root         (0) root         (0)     5720 2024-04-07 09:14:02.000000 openfinance-3.3.2/openfinance/searchhub/task/analysis/fixed_analysis_task.py
--rw-r-----   0 root         (0) root         (0)      440 2023-11-28 05:35:02.000000 openfinance-3.3.2/openfinance/searchhub/task/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.834245 openfinance-3.3.2/openfinance/searchhub/task/compare/
--rw-r-----   0 root         (0) root         (0)        0 2023-07-12 08:28:39.000000 openfinance-3.3.2/openfinance/searchhub/task/compare/__init__.py
--rw-r-----   0 root         (0) root         (0)      360 2023-11-24 12:55:22.000000 openfinance-3.3.2/openfinance/searchhub/task/compare/compare_task.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.835245 openfinance-3.3.2/openfinance/searchhub/task/percept/
--rw-r-----   0 root         (0) root         (0)        0 2023-08-17 04:23:05.000000 openfinance-3.3.2/openfinance/searchhub/task/percept/__init__.py
--rw-r-----   0 root         (0) root         (0)     5727 2024-03-15 08:52:32.000000 openfinance-3.3.2/openfinance/searchhub/task/percept/online_percept_task.py
--rw-r-----   0 root         (0) root         (0)     5542 2024-04-17 09:24:46.000000 openfinance-3.3.2/openfinance/searchhub/task/percept/percept_task.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.835245 openfinance-3.3.2/openfinance/searchhub/task/portfolio/
--rw-r-----   0 root         (0) root         (0)        0 2023-07-13 01:58:04.000000 openfinance-3.3.2/openfinance/searchhub/task/portfolio/__init__.py
--rw-r-----   0 root         (0) root         (0)        0 2023-07-20 09:18:04.000000 openfinance-3.3.2/openfinance/searchhub/task/portfolio/test_portfolio.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.835245 openfinance-3.3.2/openfinance/searchhub/task/qa_search/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/__init__.py
--rw-r-----   0 root         (0) root         (0)      650 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.836245 openfinance-3.3.2/openfinance/searchhub/task/qa_search/industry/
--rw-r-----   0 root         (0) root         (0)       94 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/industry/__init__.py
--rw-r-----   0 root         (0) root         (0)     7566 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/industry/base.py
--rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/industry/output_parser.py
--rw-r-----   0 root         (0) root         (0)      482 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/industry/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.837245 openfinance-3.3.2/openfinance/searchhub/task/qa_search/macro/
--rw-r-----   0 root         (0) root         (0)      117 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/macro/__init__.py
--rw-r-----   0 root         (0) root         (0)     7547 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/macro/base.py
--rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/macro/output_parser.py
--rw-r-----   0 root         (0) root         (0)      480 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/macro/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.837245 openfinance-3.3.2/openfinance/searchhub/task/qa_search/stock/
--rw-r-----   0 root         (0) root         (0)       99 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/stock/__init__.py
--rw-r-----   0 root         (0) root         (0)     7566 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/stock/base.py
--rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/stock/output_parser.py
--rw-r-----   0 root         (0) root         (0)      484 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/stock/prompt.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.838245 openfinance-3.3.2/openfinance/searchhub/task/qa_search/strategy/
--rw-r-----   0 root         (0) root         (0)      109 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/strategy/__init__.py
--rw-r-----   0 root         (0) root         (0)     7607 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/strategy/base.py
--rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/strategy/output_parser.py
--rw-r-----   0 root         (0) root         (0)      429 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/strategy/prompt.py
--rw-r-----   0 root         (0) root         (0)     1349 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/searchhub/task/qa_search/test_intent_search.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.838245 openfinance-3.3.2/openfinance/searchhub/task/role/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-20 09:45:18.000000 openfinance-3.3.2/openfinance/searchhub/task/role/__init__.py
--rw-r-----   0 root         (0) root         (0)      952 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/searchhub/task/role/role_task.py
--rw-r-----   0 root         (0) root         (0)      992 2024-01-17 08:00:36.000000 openfinance-3.3.2/openfinance/searchhub/task/role/test_charcter.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.838245 openfinance-3.3.2/openfinance/searchhub/task/search/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-23 08:14:35.000000 openfinance-3.3.2/openfinance/searchhub/task/search/__init__.py
--rw-r-----   0 root         (0) root         (0)     2345 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/searchhub/task/search/search_task.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.839245 openfinance-3.3.2/openfinance/searchhub/task/search_sql/
--rw-r-----   0 root         (0) root         (0)        0 2023-09-11 01:12:58.000000 openfinance-3.3.2/openfinance/searchhub/task/search_sql/__init__.py
--rw-r-----   0 root         (0) root         (0)     1855 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/searchhub/task/search_sql/search_sql_task.py
--rw-r-----   0 root         (0) root         (0)     1884 2024-03-25 08:45:46.000000 openfinance-3.3.2/openfinance/searchhub/task/task_manager.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.840245 openfinance-3.3.2/openfinance/service/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-19 06:20:41.000000 openfinance-3.3.2/openfinance/service/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.840245 openfinance-3.3.2/openfinance/service/auth/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:33:19.000000 openfinance-3.3.2/openfinance/service/auth/__init__.py
--rw-r-----   0 root         (0) root         (0)     2366 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/service/auth/login.py
--rw-r-----   0 root         (0) root         (0)      602 2023-10-16 09:59:41.000000 openfinance-3.3.2/openfinance/service/base.py
--rw-r-----   0 root         (0) root         (0)     5560 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/service/chat_http_server.py
--rw-r-----   0 root         (0) root         (0)     6044 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/service/chat_socket_server.py
--rw-r-----   0 root         (0) root         (0)     1707 2023-11-24 01:27:33.000000 openfinance-3.3.2/openfinance/service/easy_embedding_service.py
--rw-r-----   0 root         (0) root         (0)     3736 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/service/easy_quant.py
--rw-r-----   0 root         (0) root         (0)     3258 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/service/embedding_service.py
--rw-r-----   0 root         (0) root         (0)      832 2023-06-19 06:20:41.000000 openfinance-3.3.2/openfinance/service/error.py
--rw-r-----   0 root         (0) root         (0)     3922 2024-01-17 08:01:06.000000 openfinance-3.3.2/openfinance/service/finance_service.py
--rw-r-----   0 root         (0) root         (0)     6460 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/service/homepage_server.py
--rw-r-----   0 root         (0) root         (0)     6895 2024-03-29 09:55:35.000000 openfinance-3.3.2/openfinance/service/push_data_service.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.841245 openfinance-3.3.2/openfinance/strategy/
--rw-r-----   0 root         (0) root         (0)      237 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/__init__.py
--rw-r-----   0 root         (0) root         (0)     2039 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.841245 openfinance-3.3.2/openfinance/strategy/data_storage/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-19 08:18:33.000000 openfinance-3.3.2/openfinance/strategy/data_storage/__init__.py
--rw-r-----   0 root         (0) root         (0)     2089 2024-03-26 09:44:42.000000 openfinance-3.3.2/openfinance/strategy/data_storage/company_storage.py
--rw-r-----   0 root         (0) root         (0)     2204 2024-03-26 09:45:39.000000 openfinance-3.3.2/openfinance/strategy/data_storage/market_storage.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.842245 openfinance-3.3.2/openfinance/strategy/feature/
--rw-r-----   0 root         (0) root         (0)       84 2024-03-20 02:39:13.000000 openfinance-3.3.2/openfinance/strategy/feature/__init__.py
--rw-r-----   0 root         (0) root         (0)     6036 2024-03-27 03:21:32.000000 openfinance-3.3.2/openfinance/strategy/feature/base.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.842245 openfinance-3.3.2/openfinance/strategy/feature/company/
--rw-r-----   0 root         (0) root         (0)      774 2024-03-24 12:45:18.000000 openfinance-3.3.2/openfinance/strategy/feature/company/__init__.py
--rw-r-----   0 root         (0) root         (0)     1070 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/company/divident_mean.py
--rw-r-----   0 root         (0) root         (0)     1100 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/company/divident_stability.py
--rw-r-----   0 root         (0) root         (0)      490 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/company/moneyflow_direction.py
--rw-r-----   0 root         (0) root         (0)      822 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/company/news_sentiment.py
--rw-r-----   0 root         (0) root         (0)     1988 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/company/win_cost_distribution.py
--rw-r-----   0 root         (0) root         (0)     5464 2024-03-27 02:40:37.000000 openfinance-3.3.2/openfinance/strategy/feature/data_adaptor.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.843245 openfinance-3.3.2/openfinance/strategy/feature/macro/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-19 08:18:47.000000 openfinance-3.3.2/openfinance/strategy/feature/macro/__init__.py
--rw-r-----   0 root         (0) root         (0)     4539 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/macro/vix.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.843245 openfinance-3.3.2/openfinance/strategy/feature/market/
--rw-r-----   0 root         (0) root         (0)      666 2024-03-24 12:45:13.000000 openfinance-3.3.2/openfinance/strategy/feature/market/__init__.py
--rw-r-----   0 root         (0) root         (0)      699 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/market/market_volume.py
--rw-r-----   0 root         (0) root         (0)      597 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/market/north_moneyflow.py
--rw-r-----   0 root         (0) root         (0)      620 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/market/north_moneyflow_position.py
--rw-r-----   0 root         (0) root         (0)     4660 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/feature/market/vix.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.844245 openfinance-3.3.2/openfinance/strategy/model/
--rw-r-----   0 root         (0) root         (0)       84 2024-02-06 02:44:38.000000 openfinance-3.3.2/openfinance/strategy/model/__init__.py
--rw-r-----   0 root         (0) root         (0)     1069 2024-03-04 03:14:30.000000 openfinance-3.3.2/openfinance/strategy/model/base.py
--rw-r-----   0 root         (0) root         (0)     3149 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/model/index_sort.py
--rw-r-----   0 root         (0) root         (0)     1346 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/model/linear_regression.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.846245 openfinance-3.3.2/openfinance/strategy/operator/
--rw-r-----   0 root         (0) root         (0)     1037 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/__init__.py
--rw-r-----   0 root         (0) root         (0)      542 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/acc.py
--rw-r-----   0 root         (0) root         (0)     1288 2024-02-18 09:47:31.000000 openfinance-3.3.2/openfinance/strategy/operator/base.py
--rw-r-----   0 root         (0) root         (0)     1029 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/coefficient_variance.py
--rw-r-----   0 root         (0) root         (0)      505 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/divide_latest.py
--rw-r-----   0 root         (0) root         (0)      528 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/hist.py
--rw-r-----   0 root         (0) root         (0)      445 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/latest.py
--rw-r-----   0 root         (0) root         (0)      924 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/latest_position_index.py
--rw-r-----   0 root         (0) root         (0)     1748 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/macd.py
--rw-r-----   0 root         (0) root         (0)      552 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/mean.py
--rw-r-----   0 root         (0) root         (0)      708 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/moving_average.py
--rw-r-----   0 root         (0) root         (0)     1299 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/obv.py
--rw-r-----   0 root         (0) root         (0)     1093 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/rsi.py
--rw-r-----   0 root         (0) root         (0)      398 2024-03-24 12:40:05.000000 openfinance-3.3.2/openfinance/strategy/operator/yoy.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.847245 openfinance-3.3.2/openfinance/strategy/policy/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-19 08:19:00.000000 openfinance-3.3.2/openfinance/strategy/policy/__init__.py
--rw-r-----   0 root         (0) root         (0)     2314 2024-04-09 03:17:49.000000 openfinance-3.3.2/openfinance/strategy/policy/base.py
--rw-r-----   0 root         (0) root         (0)     2703 2024-03-27 08:39:19.000000 openfinance-3.3.2/openfinance/strategy/policy/company_ranker.py
--rw-r-----   0 root         (0) root         (0)     1201 2024-03-27 02:31:54.000000 openfinance-3.3.2/openfinance/strategy/policy/lr_ranker.py
--rw-r-----   0 root         (0) root         (0)     1452 2024-03-27 07:01:17.000000 openfinance-3.3.2/openfinance/strategy/policy/market_danger.py
--rw-r-----   0 root         (0) root         (0)     1467 2024-03-27 07:01:30.000000 openfinance-3.3.2/openfinance/strategy/policy/market_sentiment.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.847245 openfinance-3.3.2/openfinance/strategy/third_party/
--rw-r-----   0 root         (0) root         (0)       84 2024-02-06 02:04:09.000000 openfinance-3.3.2/openfinance/strategy/third_party/__init__.py
--rw-r-----   0 root         (0) root         (0)    11423 2024-02-06 01:59:24.000000 openfinance-3.3.2/openfinance/strategy/third_party/eastmoney_pool.py
--rw-r-----   0 root         (0) root         (0)    14601 2024-02-06 01:59:24.000000 openfinance-3.3.2/openfinance/strategy/third_party/ths_em_pool.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.847245 openfinance-3.3.2/openfinance/utils/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/utils/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.848245 openfinance-3.3.2/openfinance/utils/embeddings/
--rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.2/openfinance/utils/embeddings/__init__.py
--rw-r-----   0 root         (0) root         (0)      407 2023-12-04 15:14:03.000000 openfinance-3.3.2/openfinance/utils/embeddings/base.py
--rw-r-----   0 root         (0) root         (0)      931 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/utils/embeddings/embedding_manager.py
--rw-r-----   0 root         (0) root         (0)     2139 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/utils/embeddings/huggingface_embedding.py
--rw-r-----   0 root         (0) root         (0)      189 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/utils/embeddings/openai_embedding.py
--rw-r-----   0 root         (0) root         (0)     2227 2024-01-05 02:04:31.000000 openfinance-3.3.2/openfinance/utils/embeddings/sentence_transformers.py
--rw-r-----   0 root         (0) root         (0)     2298 2024-01-18 06:03:38.000000 openfinance-3.3.2/openfinance/utils/embeddings/sentence_transformers_cn.py
--rw-r-----   0 root         (0) root         (0)     1525 2024-04-17 09:36:32.000000 openfinance-3.3.2/openfinance/utils/log.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.849245 openfinance-3.3.2/openfinance/utils/recall/
--rw-r-----   0 root         (0) root         (0)        0 2023-11-29 03:25:50.000000 openfinance-3.3.2/openfinance/utils/recall/__init__.py
--rw-r-----   0 root         (0) root         (0)      621 2023-11-29 03:25:50.000000 openfinance-3.3.2/openfinance/utils/recall/base.py
--rw-r-----   0 root         (0) root         (0)     4054 2024-04-17 09:24:54.000000 openfinance-3.3.2/openfinance/utils/recall/es.py
--rw-r-----   0 root         (0) root         (0)     3074 2024-01-29 02:20:37.000000 openfinance-3.3.2/openfinance/utils/recall/faiss.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.849245 openfinance-3.3.2/openfinance/utils/redis/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:32:16.000000 openfinance-3.3.2/openfinance/utils/redis/__init__.py
--rw-r-----   0 root         (0) root         (0)      636 2023-07-21 10:35:44.000000 openfinance-3.3.2/openfinance/utils/redis/redis_tools.py
--rw-r-----   0 root         (0) root         (0)      423 2023-09-14 10:10:05.000000 openfinance-3.3.2/openfinance/utils/singleton.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.850245 openfinance-3.3.2/openfinance/utils/string_tools/
--rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:32:14.000000 openfinance-3.3.2/openfinance/utils/string_tools/__init__.py
--rw-r-----   0 root         (0) root         (0)     1350 2023-08-05 14:03:51.000000 openfinance-3.3.2/openfinance/utils/string_tools/parser.py
--rw-r-----   0 root         (0) root         (0)      285 2023-11-27 14:02:49.000000 openfinance-3.3.2/openfinance/utils/string_tools/util.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-17 09:39:51.850245 openfinance-3.3.2/openfinance.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2274 2024-04-17 09:39:50.000000 openfinance-3.3.2/openfinance.egg-info/PKG-INFO
--rw-r-----   0 root         (0) root         (0)    15022 2024-04-17 09:39:51.000000 openfinance-3.3.2/openfinance.egg-info/SOURCES.txt
--rw-r-----   0 root         (0) root         (0)        1 2024-04-17 09:39:50.000000 openfinance-3.3.2/openfinance.egg-info/dependency_links.txt
--rw-r-----   0 root         (0) root         (0)       17 2024-04-17 09:39:50.000000 openfinance-3.3.2/openfinance.egg-info/requires.txt
--rw-r-----   0 root         (0) root         (0)       12 2024-04-17 09:39:50.000000 openfinance-3.3.2/openfinance.egg-info/top_level.txt
--rw-r-----   0 root         (0) root         (0)       78 2024-04-17 09:39:51.851245 openfinance-3.3.2/setup.cfg
--rw-r-----   0 root         (0) root         (0)      643 2024-04-17 09:39:36.000000 openfinance-3.3.2/setup.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.326808 openfinance-3.3.3/
+-rw-r-----   0 root         (0) root         (0)     1062 2023-06-14 01:17:13.000000 openfinance-3.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-23 07:15:59.326808 openfinance-3.3.3/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)     1840 2023-12-21 07:23:25.000000 openfinance-3.3.3/README.md
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.277808 openfinance-3.3.3/openfinance/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.278808 openfinance-3.3.3/openfinance/agentflow/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agentflow/__init__.py
+-rw-r-----   0 root         (0) root         (0)      213 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agentflow/base_parser.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.279808 openfinance-3.3.3/openfinance/agentflow/flow/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agentflow/flow/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2006 2024-04-07 08:43:31.000000 openfinance-3.3.3/openfinance/agentflow/flow/agent_base.py
+-rw-r-----   0 root         (0) root         (0)      879 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agentflow/flow/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.280808 openfinance-3.3.3/openfinance/agentflow/llm/
+-rw-r-----   0 root         (0) root         (0)        1 2024-03-22 06:30:29.000000 openfinance-3.3.3/openfinance/agentflow/llm/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1672 2024-02-02 09:21:46.000000 openfinance-3.3.3/openfinance/agentflow/llm/aliyungpt.py
+-rw-r-----   0 root         (0) root         (0)     1420 2023-12-26 02:09:05.000000 openfinance-3.3.3/openfinance/agentflow/llm/base.py
+-rw-r-----   0 root         (0) root         (0)     1690 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agentflow/llm/chatgpt.py
+-rw-r-----   0 root         (0) root         (0)     2121 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agentflow/llm/ernie.py
+-rw-r-----   0 root         (0) root         (0)     1455 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/agentflow/llm/manager.py
+-rw-r-----   0 root         (0) root         (0)     1387 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agentflow/llm/webgpt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.280808 openfinance-3.3.3/openfinance/agentflow/memory/
+-rw-r-----   0 root         (0) root         (0)        0 2024-01-12 03:13:37.000000 openfinance-3.3.3/openfinance/agentflow/memory/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1264 2024-01-19 08:54:48.000000 openfinance-3.3.3/openfinance/agentflow/memory/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.280808 openfinance-3.3.3/openfinance/agentflow/prompt/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agentflow/prompt/__init__.py
+-rw-r-----   0 root         (0) root         (0)      582 2024-01-17 09:39:08.000000 openfinance-3.3.3/openfinance/agentflow/prompt/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.280808 openfinance-3.3.3/openfinance/agentflow/tool/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agentflow/tool/__init__.py
+-rw-r-----   0 root         (0) root         (0)      920 2024-04-18 09:36:40.000000 openfinance-3.3.3/openfinance/agentflow/tool/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.281808 openfinance-3.3.3/openfinance/agents/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-29 03:13:30.000000 openfinance-3.3.3/openfinance/agents/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.281808 openfinance-3.3.3/openfinance/agents/agent/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-25 05:50:49.000000 openfinance-3.3.3/openfinance/agents/agent/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1149 2024-04-08 09:39:41.000000 openfinance-3.3.3/openfinance/agents/agent/agent_prompt.py
+-rw-r-----   0 root         (0) root         (0)     2693 2024-04-07 09:58:21.000000 openfinance-3.3.3/openfinance/agents/agent/base.py
+-rw-r-----   0 root         (0) root         (0)     1102 2024-01-19 03:21:37.000000 openfinance-3.3.3/openfinance/agents/agent/output_parser.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agents/callback.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.281808 openfinance-3.3.3/openfinance/agents/promptflow/
+-rw-r-----   0 root         (0) root         (0)        0 2024-01-05 06:44:58.000000 openfinance-3.3.3/openfinance/agents/promptflow/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.282808 openfinance-3.3.3/openfinance/agents/promptflow/crawl/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-26 07:00:28.000000 openfinance-3.3.3/openfinance/agents/promptflow/crawl/__init__.py
+-rw-r-----   0 root         (0) root         (0)     3466 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/crawl/base.py
+-rw-r-----   0 root         (0) root         (0)      398 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/crawl/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.282808 openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/
+-rw-r-----   0 root         (0) root         (0)        0 2024-01-26 03:18:11.000000 openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1808 2024-01-31 06:54:31.000000 openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/base.py
+-rw-r-----   0 root         (0) root         (0)      514 2024-02-02 09:39:38.000000 openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/output_parser.py
+-rw-r-----   0 root         (0) root         (0)     1140 2024-02-02 09:47:29.000000 openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.283808 openfinance-3.3.3/openfinance/agents/promptflow/entity/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-13 08:33:15.000000 openfinance-3.3.3/openfinance/agents/promptflow/entity/__init__.py
+-rw-r-----   0 root         (0) root         (0)     3452 2024-01-25 08:48:24.000000 openfinance-3.3.3/openfinance/agents/promptflow/entity/base.py
+-rw-r-----   0 root         (0) root         (0)      693 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/entity/output_parser.py
+-rw-r-----   0 root         (0) root         (0)      491 2024-01-25 08:50:41.000000 openfinance-3.3.3/openfinance/agents/promptflow/entity/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.283808 openfinance-3.3.3/openfinance/agents/promptflow/factor/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-08 14:06:54.000000 openfinance-3.3.3/openfinance/agents/promptflow/factor/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2471 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/agents/promptflow/factor/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.283808 openfinance-3.3.3/openfinance/agents/promptflow/function/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/__init__.py
+-rw-r-----   0 root         (0) root         (0)     5006 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.284808 openfinance-3.3.3/openfinance/agents/promptflow/function/multi_function/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-25 02:41:44.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/multi_function/__init__.py
+-rw-r-----   0 root         (0) root         (0)     3224 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/multi_function/base.py
+-rw-r-----   0 root         (0) root         (0)      923 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/multi_function/output_parser.py
+-rw-r-----   0 root         (0) root         (0)      445 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/multi_function/prompt.py
+-rw-r-----   0 root         (0) root         (0)      923 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/output_parser.py
+-rw-r-----   0 root         (0) root         (0)      702 2024-01-26 02:54:07.000000 openfinance-3.3.3/openfinance/agents/promptflow/function/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.285808 openfinance-3.3.3/openfinance/agents/promptflow/percept/
+-rw-r-----   0 root         (0) root         (0)       72 2024-01-05 08:38:23.000000 openfinance-3.3.3/openfinance/agents/promptflow/percept/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2311 2024-02-02 04:43:18.000000 openfinance-3.3.3/openfinance/agents/promptflow/percept/match.py
+-rw-r-----   0 root         (0) root         (0)     1514 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/percept/opinion.py
+-rw-r-----   0 root         (0) root         (0)      696 2024-01-25 09:30:05.000000 openfinance-3.3.3/openfinance/agents/promptflow/percept/output_parser.py
+-rw-r-----   0 root         (0) root         (0)     2155 2024-03-11 06:34:31.000000 openfinance-3.3.3/openfinance/agents/promptflow/percept/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.285808 openfinance-3.3.3/openfinance/agents/promptflow/plan/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agents/promptflow/plan/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1666 2024-01-18 06:08:03.000000 openfinance-3.3.3/openfinance/agents/promptflow/plan/base.py
+-rw-r-----   0 root         (0) root         (0)     1070 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/plan/output_parser.py
+-rw-r-----   0 root         (0) root         (0)     1062 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/plan/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.286808 openfinance-3.3.3/openfinance/agents/promptflow/recall/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-23 07:10:45.000000 openfinance-3.3.3/openfinance/agents/promptflow/recall/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1853 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/agents/promptflow/recall/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.286808 openfinance-3.3.3/openfinance/agents/promptflow/summary/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/agents/promptflow/summary/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1676 2024-01-18 06:09:00.000000 openfinance-3.3.3/openfinance/agents/promptflow/summary/base.py
+-rw-r-----   0 root         (0) root         (0)      576 2024-02-01 08:33:31.000000 openfinance-3.3.3/openfinance/agents/promptflow/summary/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.286808 openfinance-3.3.3/openfinance/agents/role/
+-rw-r-----   0 root         (0) root         (0)        0 2024-01-11 09:40:34.000000 openfinance-3.3.3/openfinance/agents/role/__init__.py
+-rw-r-----   0 root         (0) root         (0)      143 2024-04-09 02:31:25.000000 openfinance-3.3.3/openfinance/agents/role/base.py
+-rw-r-----   0 root         (0) root         (0)     1415 2024-04-09 02:29:48.000000 openfinance-3.3.3/openfinance/agents/role/manager.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.288808 openfinance-3.3.3/openfinance/agents/role/prompts/
+-rw-r-----   0 root         (0) root         (0)      827 2024-01-17 08:00:36.000000 openfinance-3.3.3/openfinance/agents/role/prompts/__init__.py
+-rw-r-----   0 root         (0) root         (0)      547 2024-04-07 08:41:47.000000 openfinance-3.3.3/openfinance/agents/role/prompts/base.py
+-rw-r-----   0 root         (0) root         (0)      268 2024-04-07 08:40:42.000000 openfinance-3.3.3/openfinance/agents/role/prompts/catherine_wood.py
+-rw-r-----   0 root         (0) root         (0)      258 2024-04-07 08:40:42.000000 openfinance-3.3.3/openfinance/agents/role/prompts/elon_musk.py
+-rw-r-----   0 root         (0) root         (0)      261 2024-04-07 08:40:42.000000 openfinance-3.3.3/openfinance/agents/role/prompts/growth_investor.py
+-rw-r-----   0 root         (0) root         (0)      259 2024-04-07 08:40:42.000000 openfinance-3.3.3/openfinance/agents/role/prompts/quant_investor.py
+-rw-r-----   0 root         (0) root         (0)      258 2024-04-07 08:40:48.000000 openfinance-3.3.3/openfinance/agents/role/prompts/ray_dalio.py
+-rw-r-----   0 root         (0) root         (0)      263 2024-04-07 08:40:42.000000 openfinance-3.3.3/openfinance/agents/role/prompts/valuation_investor.py
+-rw-r-----   0 root         (0) root         (0)      268 2024-04-07 08:40:42.000000 openfinance-3.3.3/openfinance/agents/role/prompts/warren_buffett.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.288808 openfinance-3.3.3/openfinance/agents/skill/
+-rw-r-----   0 root         (0) root         (0)        0 2024-04-18 09:23:53.000000 openfinance-3.3.3/openfinance/agents/skill/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2463 2024-04-18 09:30:57.000000 openfinance-3.3.3/openfinance/agents/skill/analysis.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.288808 openfinance-3.3.3/openfinance/agents/third_party/
+-rw-r-----   0 root         (0) root         (0)        0 2024-01-08 02:44:19.000000 openfinance-3.3.3/openfinance/agents/third_party/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.289808 openfinance-3.3.3/openfinance/agents/tool/
+-rw-r-----   0 root         (0) root         (0)        0 2024-01-05 06:48:36.000000 openfinance-3.3.3/openfinance/agents/tool/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2520 2024-04-18 09:42:02.000000 openfinance-3.3.3/openfinance/agents/tool/factor_search.py
+-rw-r-----   0 root         (0) root         (0)     2460 2024-04-18 09:29:23.000000 openfinance-3.3.3/openfinance/agents/tool/search.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.289808 openfinance-3.3.3/openfinance/config/
+-rw-r-----   0 root         (0) root         (0)       39 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/config/__init__.py
+-rw-r-----   0 root         (0) root         (0)      575 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/config/config.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.289808 openfinance-3.3.3/openfinance/datacenter/
+-rw-r-----   0 root         (0) root         (0)        0 2023-08-05 14:03:51.000000 openfinance-3.3.3/openfinance/datacenter/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.289808 openfinance-3.3.3/openfinance/datacenter/database/
+-rw-r-----   0 root         (0) root         (0)       43 2023-12-08 14:06:54.000000 openfinance-3.3.3/openfinance/datacenter/database/__init__.py
+-rw-r-----   0 root         (0) root         (0)    19357 2024-04-23 07:15:12.000000 openfinance-3.3.3/openfinance/datacenter/database/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.292808 openfinance-3.3.3/openfinance/datacenter/database/fundamental/
+-rw-r-----   0 root         (0) root         (0)      813 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/__init__.py
+-rw-r-----   0 root         (0) root         (0)      810 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/business_model.py
+-rw-r-----   0 root         (0) root         (0)     2427 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/competitiveness.py
+-rw-r-----   0 root         (0) root         (0)    14000 2024-04-08 09:58:55.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/financial.py
+-rw-r-----   0 root         (0) root         (0)      906 2024-03-15 08:37:17.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/fundamental.py
+-rw-r-----   0 root         (0) root         (0)     1984 2024-03-15 08:54:13.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/industry.py
+-rw-r-----   0 root         (0) root         (0)    10779 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/macro.py
+-rw-r-----   0 root         (0) root         (0)     2522 2024-03-15 08:37:17.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/market.py
+-rw-r-----   0 root         (0) root         (0)     3198 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/money_flow.py
+-rw-r-----   0 root         (0) root         (0)     2757 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/news.py
+-rw-r-----   0 root         (0) root         (0)     2653 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/sentiment.py
+-rw-r-----   0 root         (0) root         (0)     2215 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/valuation.py
+-rw-r-----   0 root         (0) root         (0)     2883 2024-03-04 09:07:54.000000 openfinance-3.3.3/openfinance/datacenter/database/fundamental/volume.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.294808 openfinance-3.3.3/openfinance/datacenter/database/quant/
+-rw-r-----   0 root         (0) root         (0)     1339 2024-03-04 07:35:50.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/ADX.py
+-rw-r-----   0 root         (0) root         (0)     1091 2024-03-04 07:38:24.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/AROON.py
+-rw-r-----   0 root         (0) root         (0)     1242 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/BBIC.py
+-rw-r-----   0 root         (0) root         (0)     1361 2023-12-19 06:39:24.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/BR.py
+-rw-r-----   0 root         (0) root         (0)     1347 2023-12-19 05:46:41.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/BearBullPower.py
+-rw-r-----   0 root         (0) root         (0)     1443 2023-12-19 05:46:42.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/CCI.py
+-rw-r-----   0 root         (0) root         (0)     1549 2023-12-19 05:46:42.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/CR.py
+-rw-r-----   0 root         (0) root         (0)     1081 2024-03-20 08:24:55.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/MACD.py
+-rw-r-----   0 root         (0) root         (0)     1132 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/MASS.py
+-rw-r-----   0 root         (0) root         (0)     1360 2024-03-04 07:41:13.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/OBV.py
+-rw-r-----   0 root         (0) root         (0)     1103 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/RSI.py
+-rw-r-----   0 root         (0) root         (0)     1334 2023-12-19 05:46:42.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/TRIX.py
+-rw-r-----   0 root         (0) root         (0)     1603 2023-12-19 05:46:42.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/VPT.py
+-rw-r-----   0 root         (0) root         (0)     1419 2023-12-19 05:46:42.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/VR.py
+-rw-r-----   0 root         (0) root         (0)     1033 2023-12-19 05:52:40.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/__init__.py
+-rw-r-----   0 root         (0) root         (0)      613 2024-03-05 09:18:46.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/call.py
+-rw-r-----   0 root         (0) root         (0)     1082 2023-12-26 02:39:35.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/technical.py
+-rw-r-----   0 root         (0) root         (0)     1819 2023-12-19 05:47:37.000000 openfinance-3.3.3/openfinance/datacenter/database/quant/utils.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.295808 openfinance-3.3.3/openfinance/datacenter/database/source/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.295808 openfinance-3.3.3/openfinance/datacenter/database/source/cninfo/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/cninfo/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1269 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/cninfo/report.py
+-rw-r-----   0 root         (0) root         (0)     2282 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/cninfo/util.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.297808 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/
+-rw-r-----   0 root         (0) root         (0)      139 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/__init__.py
+-rw-r-----   0 root         (0) root         (0)     3459 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/bond.py
+-rw-r-----   0 root         (0) root         (0)    10569 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/fund.py
+-rw-r-----   0 root         (0) root         (0)     3741 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/fundamental.py
+-rw-r-----   0 root         (0) root         (0)     4489 2024-03-01 07:31:12.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/future.py
+-rw-r-----   0 root         (0) root         (0)     9195 2023-12-26 07:30:59.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/industry.py
+-rw-r-----   0 root         (0) root         (0)     2827 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/market.py
+-rw-r-----   0 root         (0) root         (0)     3103 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/money.py
+-rw-r-----   0 root         (0) root         (0)     3894 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/news.py
+-rw-r-----   0 root         (0) root         (0)    32264 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/report.py
+-rw-r-----   0 root         (0) root         (0)     5460 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/technical.py
+-rw-r-----   0 root         (0) root         (0)    30214 2024-03-20 03:32:53.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/trade.py
+-rw-r-----   0 root         (0) root         (0)     8795 2024-02-08 07:26:20.000000 openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/util.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.298808 openfinance-3.3.3/openfinance/datacenter/database/source/event/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/event/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1007 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/event/base.py
+-rw-r-----   0 root         (0) root         (0)     2436 2024-01-30 02:45:38.000000 openfinance-3.3.3/openfinance/datacenter/database/source/event/cailianshe.py
+-rw-r-----   0 root         (0) root         (0)     2644 2023-12-22 09:38:08.000000 openfinance-3.3.3/openfinance/datacenter/database/source/event/caixing.py
+-rw-r-----   0 root         (0) root         (0)     2462 2024-01-30 09:08:46.000000 openfinance-3.3.3/openfinance/datacenter/database/source/event/investing.py
+-rw-r-----   0 root         (0) root         (0)     5305 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/database/source/event/jin10.py
+-rw-r-----   0 root         (0) root         (0)     6609 2023-12-13 08:33:15.000000 openfinance-3.3.3/openfinance/datacenter/database/source/event/news.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.298808 openfinance-3.3.3/openfinance/datacenter/database/source/sina/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/source/sina/__init__.py
+-rw-r-----   0 root         (0) root         (0)      236 2024-02-27 06:53:18.000000 openfinance-3.3.3/openfinance/datacenter/database/source/sina/moneyflow.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.299808 openfinance-3.3.3/openfinance/datacenter/database/storage/
+-rw-r-----   0 root         (0) root         (0)     1543 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1034 2023-12-01 06:19:13.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.300808 openfinance-3.3.3/openfinance/datacenter/database/storage/china/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/china/__init__.py
+-rw-r-----   0 root         (0) root         (0)     4870 2023-12-26 08:47:24.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/china/industry.py
+-rw-r-----   0 root         (0) root         (0)    20814 2023-12-14 08:18:55.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/china/macro.py
+-rw-r-----   0 root         (0) root         (0)     1866 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/china/market.py
+-rw-r-----   0 root         (0) root         (0)     1568 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/china/quant.py
+-rw-r-----   0 root         (0) root         (0)    28030 2024-03-15 06:33:38.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/china/stock.py
+-rw-r-----   0 root         (0) root         (0)    10418 2024-03-18 02:34:13.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/financial.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.301808 openfinance-3.3.3/openfinance/datacenter/database/storage/fred/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/fred/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2084 2023-12-01 06:17:14.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/fred/base.py
+-rw-r-----   0 root         (0) root         (0)     1065 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/fred/store.py
+-rw-r-----   0 root         (0) root         (0)     1066 2024-03-18 02:34:08.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/gov_stat.py
+-rw-r-----   0 root         (0) root         (0)     1815 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/industry.py
+-rw-r-----   0 root         (0) root         (0)     1693 2024-03-18 02:34:01.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/macro.py
+-rw-r-----   0 root         (0) root         (0)      926 2024-03-18 02:34:18.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/market.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.301808 openfinance-3.3.3/openfinance/datacenter/database/storage/national_data/
+-rw-r-----   0 root         (0) root         (0)      912 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/national_data/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2343 2023-11-27 13:51:06.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/national_data/base.py
+-rw-r-----   0 root         (0) root         (0)     1090 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/national_data/store.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.302808 openfinance-3.3.3/openfinance/datacenter/database/storage/us/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/us/__init__.py
+-rw-r-----   0 root         (0) root         (0)     8558 2023-12-19 09:14:17.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/us/base.py
+-rw-r-----   0 root         (0) root         (0)     1194 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/us/financial.py
+-rw-r-----   0 root         (0) root         (0)     4001 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/storage/us/util.py
+-rw-r-----   0 root         (0) root         (0)     1495 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/datacenter/database/wrapper.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.303808 openfinance-3.3.3/openfinance/datacenter/echarts/
+-rw-r-----   0 root         (0) root         (0)      578 2023-11-24 01:27:33.000000 openfinance-3.3.3/openfinance/datacenter/echarts/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1222 2023-10-12 07:53:22.000000 openfinance-3.3.3/openfinance/datacenter/echarts/bar.py
+-rw-r-----   0 root         (0) root         (0)      523 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/datacenter/echarts/base.py
+-rw-r-----   0 root         (0) root         (0)     1045 2023-10-13 06:59:29.000000 openfinance-3.3.3/openfinance/datacenter/echarts/multibar.py
+-rw-r-----   0 root         (0) root         (0)     1337 2023-10-12 09:56:12.000000 openfinance-3.3.3/openfinance/datacenter/echarts/pie.py
+-rw-r-----   0 root         (0) root         (0)     1981 2023-11-24 01:27:33.000000 openfinance-3.3.3/openfinance/datacenter/echarts/stacked_line.py
+-rw-r-----   0 root         (0) root         (0)     1665 2023-11-24 01:27:33.000000 openfinance-3.3.3/openfinance/datacenter/echarts/tree.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.304808 openfinance-3.3.3/openfinance/datacenter/knowledge/
+-rw-r-----   0 root         (0) root         (0)        0 2023-08-05 14:03:51.000000 openfinance-3.3.3/openfinance/datacenter/knowledge/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1047 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/knowledge/decorator.py
+-rw-r-----   0 root         (0) root         (0)     4636 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/knowledge/entity_graph.py
+-rw-r-----   0 root         (0) root         (0)     2861 2024-03-26 02:15:35.000000 openfinance-3.3.3/openfinance/datacenter/knowledge/executor.py
+-rw-r-----   0 root         (0) root         (0)     4012 2024-03-29 09:58:11.000000 openfinance-3.3.3/openfinance/datacenter/knowledge/factor.py
+-rw-r-----   0 root         (0) root         (0)     5825 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/datacenter/knowledge/graph.py
+-rw-r-----   0 root         (0) root         (0)     1583 2023-12-08 14:06:54.000000 openfinance-3.3.3/openfinance/datacenter/knowledge/wrapper.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.304808 openfinance-3.3.3/openfinance/robot/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-15 01:39:28.000000 openfinance-3.3.3/openfinance/robot/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.304808 openfinance-3.3.3/openfinance/searchhub/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.305808 openfinance-3.3.3/openfinance/searchhub/page_manage/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/page_manage/__init__.py
+-rw-r-----   0 root         (0) root         (0)      518 2023-09-16 02:17:44.000000 openfinance-3.3.3/openfinance/searchhub/page_manage/base.py
+-rw-r-----   0 root         (0) root         (0)     1838 2024-03-15 08:53:08.000000 openfinance-3.3.3/openfinance/searchhub/page_manage/company.py
+-rw-r-----   0 root         (0) root         (0)     1356 2023-08-05 14:03:51.000000 openfinance-3.3.3/openfinance/searchhub/page_manage/factor.py
+-rw-r-----   0 root         (0) root         (0)     2096 2023-09-18 06:50:34.000000 openfinance-3.3.3/openfinance/searchhub/page_manage/model.py
+-rw-r-----   0 root         (0) root         (0)     1040 2024-01-31 02:53:57.000000 openfinance-3.3.3/openfinance/searchhub/page_manage/role.py
+-rw-r-----   0 root         (0) root         (0)     2620 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/searchhub/page_manage/user.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.305808 openfinance-3.3.3/openfinance/searchhub/query_understand/
+-rw-r-----   0 root         (0) root         (0)        0 2023-12-13 09:36:00.000000 openfinance-3.3.3/openfinance/searchhub/query_understand/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1239 2023-12-14 07:14:38.000000 openfinance-3.3.3/openfinance/searchhub/query_understand/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.306808 openfinance-3.3.3/openfinance/searchhub/recall/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:31:57.000000 openfinance-3.3.3/openfinance/searchhub/recall/__init__.py
+-rw-r-----   0 root         (0) root         (0)      928 2023-11-30 08:38:33.000000 openfinance-3.3.3/openfinance/searchhub/recall/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.306808 openfinance-3.3.3/openfinance/searchhub/recall/channel/
+-rw-r-----   0 root         (0) root         (0)        0 2023-08-05 14:03:51.000000 openfinance-3.3.3/openfinance/searchhub/recall/channel/__init__.py
+-rw-r-----   0 root         (0) root         (0)      110 2023-11-29 03:41:36.000000 openfinance-3.3.3/openfinance/searchhub/recall/channel/analysis.py
+-rw-r-----   0 root         (0) root         (0)      138 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/searchhub/recall/channel/search.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.307808 openfinance-3.3.3/openfinance/searchhub/task/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-25 05:51:52.000000 openfinance-3.3.3/openfinance/searchhub/task/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.307808 openfinance-3.3.3/openfinance/searchhub/task/analysis/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-23 09:14:10.000000 openfinance-3.3.3/openfinance/searchhub/task/analysis/__init__.py
+-rw-r-----   0 root         (0) root         (0)     4422 2024-04-07 09:13:07.000000 openfinance-3.3.3/openfinance/searchhub/task/analysis/analysis_task.py
+-rw-r-----   0 root         (0) root         (0)      744 2024-01-19 08:33:50.000000 openfinance-3.3.3/openfinance/searchhub/task/analysis/auto_analysis.py
+-rw-r-----   0 root         (0) root         (0)     5720 2024-04-07 09:14:02.000000 openfinance-3.3.3/openfinance/searchhub/task/analysis/fixed_analysis_task.py
+-rw-r-----   0 root         (0) root         (0)      440 2023-11-28 05:35:02.000000 openfinance-3.3.3/openfinance/searchhub/task/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.307808 openfinance-3.3.3/openfinance/searchhub/task/compare/
+-rw-r-----   0 root         (0) root         (0)        0 2023-07-12 08:28:39.000000 openfinance-3.3.3/openfinance/searchhub/task/compare/__init__.py
+-rw-r-----   0 root         (0) root         (0)      360 2023-11-24 12:55:22.000000 openfinance-3.3.3/openfinance/searchhub/task/compare/compare_task.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.308808 openfinance-3.3.3/openfinance/searchhub/task/percept/
+-rw-r-----   0 root         (0) root         (0)        0 2023-08-17 04:23:05.000000 openfinance-3.3.3/openfinance/searchhub/task/percept/__init__.py
+-rw-r-----   0 root         (0) root         (0)     5727 2024-03-15 08:52:32.000000 openfinance-3.3.3/openfinance/searchhub/task/percept/online_percept_task.py
+-rw-r-----   0 root         (0) root         (0)     5541 2024-04-18 09:12:55.000000 openfinance-3.3.3/openfinance/searchhub/task/percept/percept_task.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.308808 openfinance-3.3.3/openfinance/searchhub/task/portfolio/
+-rw-r-----   0 root         (0) root         (0)        0 2023-07-13 01:58:04.000000 openfinance-3.3.3/openfinance/searchhub/task/portfolio/__init__.py
+-rw-r-----   0 root         (0) root         (0)        0 2023-07-20 09:18:04.000000 openfinance-3.3.3/openfinance/searchhub/task/portfolio/test_portfolio.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.309808 openfinance-3.3.3/openfinance/searchhub/task/qa_search/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/__init__.py
+-rw-r-----   0 root         (0) root         (0)      650 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.309808 openfinance-3.3.3/openfinance/searchhub/task/qa_search/industry/
+-rw-r-----   0 root         (0) root         (0)       94 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/industry/__init__.py
+-rw-r-----   0 root         (0) root         (0)     7566 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/industry/base.py
+-rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/industry/output_parser.py
+-rw-r-----   0 root         (0) root         (0)      482 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/industry/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.310808 openfinance-3.3.3/openfinance/searchhub/task/qa_search/macro/
+-rw-r-----   0 root         (0) root         (0)      117 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/macro/__init__.py
+-rw-r-----   0 root         (0) root         (0)     7547 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/macro/base.py
+-rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/macro/output_parser.py
+-rw-r-----   0 root         (0) root         (0)      480 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/macro/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.310808 openfinance-3.3.3/openfinance/searchhub/task/qa_search/stock/
+-rw-r-----   0 root         (0) root         (0)       99 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/stock/__init__.py
+-rw-r-----   0 root         (0) root         (0)     7566 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/stock/base.py
+-rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/stock/output_parser.py
+-rw-r-----   0 root         (0) root         (0)      484 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/stock/prompt.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.311808 openfinance-3.3.3/openfinance/searchhub/task/qa_search/strategy/
+-rw-r-----   0 root         (0) root         (0)      109 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/strategy/__init__.py
+-rw-r-----   0 root         (0) root         (0)     7607 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/strategy/base.py
+-rw-r-----   0 root         (0) root         (0)      969 2023-09-15 07:18:57.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/strategy/output_parser.py
+-rw-r-----   0 root         (0) root         (0)      429 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/strategy/prompt.py
+-rw-r-----   0 root         (0) root         (0)     1349 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/searchhub/task/qa_search/test_intent_search.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.311808 openfinance-3.3.3/openfinance/searchhub/task/role/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-20 09:45:18.000000 openfinance-3.3.3/openfinance/searchhub/task/role/__init__.py
+-rw-r-----   0 root         (0) root         (0)      952 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/searchhub/task/role/role_task.py
+-rw-r-----   0 root         (0) root         (0)      992 2024-01-17 08:00:36.000000 openfinance-3.3.3/openfinance/searchhub/task/role/test_charcter.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.312808 openfinance-3.3.3/openfinance/searchhub/task/search/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-23 08:14:35.000000 openfinance-3.3.3/openfinance/searchhub/task/search/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2345 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/searchhub/task/search/search_task.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.312808 openfinance-3.3.3/openfinance/searchhub/task/search_sql/
+-rw-r-----   0 root         (0) root         (0)        0 2023-09-11 01:12:58.000000 openfinance-3.3.3/openfinance/searchhub/task/search_sql/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1855 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/searchhub/task/search_sql/search_sql_task.py
+-rw-r-----   0 root         (0) root         (0)     1884 2024-03-25 08:45:46.000000 openfinance-3.3.3/openfinance/searchhub/task/task_manager.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.313808 openfinance-3.3.3/openfinance/service/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-19 06:20:41.000000 openfinance-3.3.3/openfinance/service/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.314808 openfinance-3.3.3/openfinance/service/auth/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:33:19.000000 openfinance-3.3.3/openfinance/service/auth/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2366 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/service/auth/login.py
+-rw-r-----   0 root         (0) root         (0)      602 2023-10-16 09:59:41.000000 openfinance-3.3.3/openfinance/service/base.py
+-rw-r-----   0 root         (0) root         (0)     5560 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/service/chat_http_server.py
+-rw-r-----   0 root         (0) root         (0)     6044 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/service/chat_socket_server.py
+-rw-r-----   0 root         (0) root         (0)     1707 2023-11-24 01:27:33.000000 openfinance-3.3.3/openfinance/service/easy_embedding_service.py
+-rw-r-----   0 root         (0) root         (0)     3736 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/service/easy_quant.py
+-rw-r-----   0 root         (0) root         (0)     3258 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/service/embedding_service.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-06-19 06:20:41.000000 openfinance-3.3.3/openfinance/service/error.py
+-rw-r-----   0 root         (0) root         (0)     3922 2024-01-17 08:01:06.000000 openfinance-3.3.3/openfinance/service/finance_service.py
+-rw-r-----   0 root         (0) root         (0)     6460 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/service/homepage_server.py
+-rw-r-----   0 root         (0) root         (0)     6895 2024-03-29 09:55:35.000000 openfinance-3.3.3/openfinance/service/push_data_service.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.314808 openfinance-3.3.3/openfinance/strategy/
+-rw-r-----   0 root         (0) root         (0)      237 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2039 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.314808 openfinance-3.3.3/openfinance/strategy/data_storage/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-19 08:18:33.000000 openfinance-3.3.3/openfinance/strategy/data_storage/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2089 2024-03-26 09:44:42.000000 openfinance-3.3.3/openfinance/strategy/data_storage/company_storage.py
+-rw-r-----   0 root         (0) root         (0)     2204 2024-03-26 09:45:39.000000 openfinance-3.3.3/openfinance/strategy/data_storage/market_storage.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.315808 openfinance-3.3.3/openfinance/strategy/feature/
+-rw-r-----   0 root         (0) root         (0)       84 2024-03-20 02:39:13.000000 openfinance-3.3.3/openfinance/strategy/feature/__init__.py
+-rw-r-----   0 root         (0) root         (0)     6036 2024-03-27 03:21:32.000000 openfinance-3.3.3/openfinance/strategy/feature/base.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.316808 openfinance-3.3.3/openfinance/strategy/feature/company/
+-rw-r-----   0 root         (0) root         (0)      774 2024-03-24 12:45:18.000000 openfinance-3.3.3/openfinance/strategy/feature/company/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1070 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/company/divident_mean.py
+-rw-r-----   0 root         (0) root         (0)     1100 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/company/divident_stability.py
+-rw-r-----   0 root         (0) root         (0)      490 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/company/moneyflow_direction.py
+-rw-r-----   0 root         (0) root         (0)      822 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/company/news_sentiment.py
+-rw-r-----   0 root         (0) root         (0)     1988 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/company/win_cost_distribution.py
+-rw-r-----   0 root         (0) root         (0)     5464 2024-03-27 02:40:37.000000 openfinance-3.3.3/openfinance/strategy/feature/data_adaptor.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.316808 openfinance-3.3.3/openfinance/strategy/feature/macro/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-19 08:18:47.000000 openfinance-3.3.3/openfinance/strategy/feature/macro/__init__.py
+-rw-r-----   0 root         (0) root         (0)     4539 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/macro/vix.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.318808 openfinance-3.3.3/openfinance/strategy/feature/market/
+-rw-r-----   0 root         (0) root         (0)      666 2024-03-24 12:45:13.000000 openfinance-3.3.3/openfinance/strategy/feature/market/__init__.py
+-rw-r-----   0 root         (0) root         (0)      699 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/market/market_volume.py
+-rw-r-----   0 root         (0) root         (0)      597 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/market/north_moneyflow.py
+-rw-r-----   0 root         (0) root         (0)      620 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/market/north_moneyflow_position.py
+-rw-r-----   0 root         (0) root         (0)     4660 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/feature/market/vix.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.319808 openfinance-3.3.3/openfinance/strategy/model/
+-rw-r-----   0 root         (0) root         (0)       84 2024-02-06 02:44:38.000000 openfinance-3.3.3/openfinance/strategy/model/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1069 2024-03-04 03:14:30.000000 openfinance-3.3.3/openfinance/strategy/model/base.py
+-rw-r-----   0 root         (0) root         (0)     3149 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/model/index_sort.py
+-rw-r-----   0 root         (0) root         (0)     1346 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/model/linear_regression.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.321808 openfinance-3.3.3/openfinance/strategy/operator/
+-rw-r-----   0 root         (0) root         (0)     1037 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/__init__.py
+-rw-r-----   0 root         (0) root         (0)      542 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/acc.py
+-rw-r-----   0 root         (0) root         (0)     1288 2024-02-18 09:47:31.000000 openfinance-3.3.3/openfinance/strategy/operator/base.py
+-rw-r-----   0 root         (0) root         (0)     1029 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/coefficient_variance.py
+-rw-r-----   0 root         (0) root         (0)      505 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/divide_latest.py
+-rw-r-----   0 root         (0) root         (0)      528 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/hist.py
+-rw-r-----   0 root         (0) root         (0)      445 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/latest.py
+-rw-r-----   0 root         (0) root         (0)      924 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/latest_position_index.py
+-rw-r-----   0 root         (0) root         (0)     1748 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/macd.py
+-rw-r-----   0 root         (0) root         (0)      552 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/mean.py
+-rw-r-----   0 root         (0) root         (0)      708 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/moving_average.py
+-rw-r-----   0 root         (0) root         (0)     1299 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/obv.py
+-rw-r-----   0 root         (0) root         (0)     1093 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/rsi.py
+-rw-r-----   0 root         (0) root         (0)      398 2024-03-24 12:40:05.000000 openfinance-3.3.3/openfinance/strategy/operator/yoy.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.322808 openfinance-3.3.3/openfinance/strategy/policy/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-19 08:19:00.000000 openfinance-3.3.3/openfinance/strategy/policy/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2314 2024-04-09 03:17:49.000000 openfinance-3.3.3/openfinance/strategy/policy/base.py
+-rw-r-----   0 root         (0) root         (0)     2703 2024-03-27 08:39:19.000000 openfinance-3.3.3/openfinance/strategy/policy/company_ranker.py
+-rw-r-----   0 root         (0) root         (0)     1201 2024-03-27 02:31:54.000000 openfinance-3.3.3/openfinance/strategy/policy/lr_ranker.py
+-rw-r-----   0 root         (0) root         (0)     1452 2024-03-27 07:01:17.000000 openfinance-3.3.3/openfinance/strategy/policy/market_danger.py
+-rw-r-----   0 root         (0) root         (0)     1467 2024-03-27 07:01:30.000000 openfinance-3.3.3/openfinance/strategy/policy/market_sentiment.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.322808 openfinance-3.3.3/openfinance/strategy/third_party/
+-rw-r-----   0 root         (0) root         (0)       84 2024-02-06 02:04:09.000000 openfinance-3.3.3/openfinance/strategy/third_party/__init__.py
+-rw-r-----   0 root         (0) root         (0)    11423 2024-02-06 01:59:24.000000 openfinance-3.3.3/openfinance/strategy/third_party/eastmoney_pool.py
+-rw-r-----   0 root         (0) root         (0)    14601 2024-02-06 01:59:24.000000 openfinance-3.3.3/openfinance/strategy/third_party/ths_em_pool.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.323808 openfinance-3.3.3/openfinance/utils/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/utils/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.324808 openfinance-3.3.3/openfinance/utils/embeddings/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-14 01:17:13.000000 openfinance-3.3.3/openfinance/utils/embeddings/__init__.py
+-rw-r-----   0 root         (0) root         (0)      407 2023-12-04 15:14:03.000000 openfinance-3.3.3/openfinance/utils/embeddings/base.py
+-rw-r-----   0 root         (0) root         (0)      931 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/utils/embeddings/embedding_manager.py
+-rw-r-----   0 root         (0) root         (0)     2139 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/utils/embeddings/huggingface_embedding.py
+-rw-r-----   0 root         (0) root         (0)      189 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/utils/embeddings/openai_embedding.py
+-rw-r-----   0 root         (0) root         (0)     2227 2024-01-05 02:04:31.000000 openfinance-3.3.3/openfinance/utils/embeddings/sentence_transformers.py
+-rw-r-----   0 root         (0) root         (0)     2298 2024-01-18 06:03:38.000000 openfinance-3.3.3/openfinance/utils/embeddings/sentence_transformers_cn.py
+-rw-r-----   0 root         (0) root         (0)     1525 2024-04-17 09:36:32.000000 openfinance-3.3.3/openfinance/utils/log.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.324808 openfinance-3.3.3/openfinance/utils/recall/
+-rw-r-----   0 root         (0) root         (0)        0 2023-11-29 03:25:50.000000 openfinance-3.3.3/openfinance/utils/recall/__init__.py
+-rw-r-----   0 root         (0) root         (0)      621 2023-11-29 03:25:50.000000 openfinance-3.3.3/openfinance/utils/recall/base.py
+-rw-r-----   0 root         (0) root         (0)     4052 2024-04-18 08:49:35.000000 openfinance-3.3.3/openfinance/utils/recall/es.py
+-rw-r-----   0 root         (0) root         (0)     3074 2024-01-29 02:20:37.000000 openfinance-3.3.3/openfinance/utils/recall/faiss.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.325808 openfinance-3.3.3/openfinance/utils/redis/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:32:16.000000 openfinance-3.3.3/openfinance/utils/redis/__init__.py
+-rw-r-----   0 root         (0) root         (0)      636 2023-07-21 10:35:44.000000 openfinance-3.3.3/openfinance/utils/redis/redis_tools.py
+-rw-r-----   0 root         (0) root         (0)      423 2023-09-14 10:10:05.000000 openfinance-3.3.3/openfinance/utils/singleton.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.325808 openfinance-3.3.3/openfinance/utils/string_tools/
+-rw-r-----   0 root         (0) root         (0)        0 2024-03-18 06:32:14.000000 openfinance-3.3.3/openfinance/utils/string_tools/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1350 2023-08-05 14:03:51.000000 openfinance-3.3.3/openfinance/utils/string_tools/parser.py
+-rw-r-----   0 root         (0) root         (0)      285 2023-11-27 14:02:49.000000 openfinance-3.3.3/openfinance/utils/string_tools/util.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-23 07:15:59.325808 openfinance-3.3.3/openfinance.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-23 07:15:58.000000 openfinance-3.3.3/openfinance.egg-info/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)    15052 2024-04-23 07:15:59.000000 openfinance-3.3.3/openfinance.egg-info/SOURCES.txt
+-rw-r-----   0 root         (0) root         (0)        1 2024-04-23 07:15:58.000000 openfinance-3.3.3/openfinance.egg-info/dependency_links.txt
+-rw-r-----   0 root         (0) root         (0)       17 2024-04-23 07:15:58.000000 openfinance-3.3.3/openfinance.egg-info/requires.txt
+-rw-r-----   0 root         (0) root         (0)       12 2024-04-23 07:15:58.000000 openfinance-3.3.3/openfinance.egg-info/top_level.txt
+-rw-r-----   0 root         (0) root         (0)       78 2024-04-23 07:15:59.326808 openfinance-3.3.3/setup.cfg
+-rw-r-----   0 root         (0) root         (0)      643 2024-04-23 07:15:50.000000 openfinance-3.3.3/setup.py
```

### Comparing `openfinance-3.3.2/LICENSE` & `openfinance-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/PKG-INFO` & `openfinance-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfinance
-Version: 3.3.2
+Version: 3.3.3
 Summary: an open financial agent framework powered by llm
 Home-page: 
 Author: Bin ZHU
 Author-email: zhubin_n@outlook.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openfinance-3.3.2/README.md` & `openfinance-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/flow/agent_base.py` & `openfinance-3.3.3/openfinance/agentflow/flow/agent_base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/flow/base.py` & `openfinance-3.3.3/openfinance/agentflow/flow/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/llm/aliyungpt.py` & `openfinance-3.3.3/openfinance/agentflow/llm/aliyungpt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/llm/base.py` & `openfinance-3.3.3/openfinance/agentflow/llm/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/llm/chatgpt.py` & `openfinance-3.3.3/openfinance/agentflow/llm/chatgpt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/llm/ernie.py` & `openfinance-3.3.3/openfinance/agentflow/llm/ernie.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/llm/manager.py` & `openfinance-3.3.3/openfinance/agentflow/llm/manager.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/llm/webgpt.py` & `openfinance-3.3.3/openfinance/agentflow/llm/webgpt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/memory/base.py` & `openfinance-3.3.3/openfinance/agentflow/memory/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/prompt/base.py` & `openfinance-3.3.3/openfinance/agentflow/prompt/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agentflow/tool/base.py` & `openfinance-3.3.3/openfinance/agentflow/tool/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,43 +7,45 @@
     List
 )
 from pydantic import BaseModel
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 class Tool(ABC, BaseModel):
+    """
+        Tool is not built-in ability
+    """    
     name: str
-    func: Callable
     description: str
 
     def __call__(
         self,
         *args: Any,        
         **kwargs: Any        
     ) -> Any:
         return self.call(*args, **kwargs)
 
     def call(
         self,
         *args: Any,
         **kwargs: Any        
     ) -> Any:
-        return self.func(*args, **kwargs)
+        pass
     
     async def _acall(
         self,
         *args: Any,        
         **kwargs: Any        
     ) -> Any:
         return await self.acall(*args, **kwargs)
 
     async def acall(
         self,
         *args: Any,        
         **kwargs: Any        
     ) -> Any:
-        return await self.func(*args, **kwargs) 
+        pass
 
 @dataclass
 class Action:
     name: str = ""
     action_input: str = ""
```

### Comparing `openfinance-3.3.2/openfinance/agents/agent/agent_prompt.py` & `openfinance-3.3.3/openfinance/agents/agent/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/agent/base.py` & `openfinance-3.3.3/openfinance/agents/agent/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/agent/output_parser.py` & `openfinance-3.3.3/openfinance/agents/agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/crawl/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/crawl/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/output_parser.py` & `openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/data_analysis/prompt.py` & `openfinance-3.3.3/openfinance/agents/promptflow/data_analysis/prompt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/entity/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/entity/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/entity/output_parser.py` & `openfinance-3.3.3/openfinance/agents/promptflow/entity/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/factor/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/factor/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/function/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/function/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/function/multi_function/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/function/multi_function/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/function/multi_function/output_parser.py` & `openfinance-3.3.3/openfinance/agents/promptflow/function/multi_function/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/function/output_parser.py` & `openfinance-3.3.3/openfinance/agents/promptflow/function/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/function/prompt.py` & `openfinance-3.3.3/openfinance/agents/promptflow/function/prompt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/percept/match.py` & `openfinance-3.3.3/openfinance/agents/promptflow/percept/match.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/percept/opinion.py` & `openfinance-3.3.3/openfinance/agents/promptflow/percept/opinion.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/percept/output_parser.py` & `openfinance-3.3.3/openfinance/agents/promptflow/percept/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/percept/prompt.py` & `openfinance-3.3.3/openfinance/agents/promptflow/percept/prompt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/plan/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/plan/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/plan/output_parser.py` & `openfinance-3.3.3/openfinance/agents/promptflow/plan/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/plan/prompt.py` & `openfinance-3.3.3/openfinance/agents/promptflow/plan/prompt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/recall/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/recall/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/summary/base.py` & `openfinance-3.3.3/openfinance/agents/promptflow/summary/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/promptflow/summary/prompt.py` & `openfinance-3.3.3/openfinance/agents/promptflow/summary/prompt.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/role/manager.py` & `openfinance-3.3.3/openfinance/agents/role/manager.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/role/prompts/__init__.py` & `openfinance-3.3.3/openfinance/agents/role/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/role/prompts/base.py` & `openfinance-3.3.3/openfinance/agents/role/prompts/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/agents/tool/factor_search.py` & `openfinance-3.3.3/openfinance/agents/tool/factor_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from openfinance.agents.promptflow.factor.base import RecallFlow
 from openfinance.agents.promptflow.function.base import FuncFlow
 from openfinance.agentflow.tool.base import Tool
 
 class FactorSearchTool(Tool):
     description = "Get result for indicator or query"
-    func: Callable = None
     recall: RecallFlow
     func: FuncFlow
 
     class Config:
         """Configuration for this pydantic object."""
         arbitrary_types_allowed = True
```

### Comparing `openfinance-3.3.2/openfinance/agents/tool/search.py` & `openfinance-3.3.3/openfinance/agents/tool/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from openfinance.agents.promptflow.factor.base import RecallFlow
 from openfinance.agents.promptflow.function.base import FuncFlow
 from openfinance.agentflow.tool.base import Tool
 
 
 class SearchTool(Tool):
     description = "Get result for explicit indicator or easy query"
-    func: Callable = None
     recall: RecallFlow
     func: FuncFlow
 
     class Config:
         """Configuration for this pydantic object."""
         arbitrary_types_allowed = True
```

### Comparing `openfinance-3.3.2/openfinance/config/config.py` & `openfinance-3.3.3/openfinance/config/config.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/base.py` & `openfinance-3.3.3/openfinance/datacenter/database/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,63 +446,70 @@
             idx += 1
         if len(hit_columns) == 0:
             return EMPTY_DATA
         result = " \n".join(v[:-2] for k, v in hit_columns.items())
         return result
 
 class AsyncDB:
-    conn = None
+    pool = None
     connected = False
-    conf = None
 
     def __init__(
         self,
         conf
     ):
         self.conf = conf
 
-    async def connect(
+    async def init_pool(
         self
     ):
-        if not self.connected:
-            self.conn = await aiomysql.connect(
-                host = self.conf.get("host", "localhost"), 
-                port = self.conf.get("port", "3306"), 
-                user = self.conf.get("user", "root"), 
-                password = self.conf.get("pw", ""),
-                db = self.conf.get("db", "")
-            )
-            self.connected = True
+        self.pool = await aiomysql.create_pool(
+            host = self.conf.get("host", "localhost"), 
+            port = self.conf.get("port", "3306"), 
+            user = self.conf.get("user", "root"), 
+            password = self.conf.get("pw", ""),
+            db = self.conf.get("db", "")
+        )
+        self.connected = True
      
     async def exec(
         self,
         sql
     ):
         try:
-            async with self.conn.cursor() as cursor:
-                await cursor.execute(sql)
-                return await cursor.fetchall()
+            # print("conected: ", self.connected)
+            if not self.connected:
+                 await self.init_pool()
+            async with self.pool.acquire() as conn:
+                async with conn.cursor() as cursor:
+                    await cursor.execute(sql)
+                    result = await cursor.fetchall()
+                    field_names = [desc[0] for desc in cursor.description]
+                    return [dict(zip(field_names, row)) for row in result]
         except pymysql.Error as e:
             print(e)
             return False
 
     async def select_more(
         self,
         table, 
         range_str="", 
         field='*'        
     ):
         try:
+            if not self.connected:
+                 await self.init_pool()            
             if range_str:
                 sql = 'SELECT ' + field + ' FROM ' + table + ' WHERE ' + range_str
             else:
                 sql = 'SELECT ' + field + ' FROM ' + table
-            async with self.conn.cursor() as cursor:
-                await cursor.execute(sql)
-                return await cursor.fetchall()
+            async with self.pool.acquire() as conn:
+                async with conn.cursor() as cursor:
+                    await cursor.execute(sql)
+                    return await cursor.fetchall()
         except pymysql.Error as e:
             print(e)
             return False
 
 class DataBaseManager(metaclass=Singleton):
     name_to_databases: Dict[str, Database] = {}
```

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/__init__.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/business_model.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/business_model.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/competitiveness.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/competitiveness.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/financial.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/financial.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/fundamental.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/fundamental.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/industry.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/industry.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/macro.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/macro.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/market.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/market.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/money_flow.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/money_flow.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/news.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/news.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/sentiment.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/sentiment.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/valuation.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/valuation.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/fundamental/volume.py` & `openfinance-3.3.3/openfinance/datacenter/database/fundamental/volume.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/ADX.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/ADX.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/AROON.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/AROON.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/BBIC.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/BBIC.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/BR.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/BR.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/BearBullPower.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/BearBullPower.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/CCI.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/CCI.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/CR.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/CR.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/MACD.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/MACD.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/MASS.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/MASS.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/OBV.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/OBV.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/RSI.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/RSI.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/TRIX.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/TRIX.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/VPT.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/VPT.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/VR.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/VR.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/__init__.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/call.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/call.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/technical.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/technical.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/quant/utils.py` & `openfinance-3.3.3/openfinance/datacenter/database/quant/utils.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/cninfo/report.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/cninfo/report.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/cninfo/util.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/cninfo/util.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/bond.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/bond.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/fund.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/fund.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/fundamental.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/fundamental.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/future.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/future.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/industry.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/industry.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/market.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/market.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/money.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/money.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/news.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/news.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/report.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/report.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/technical.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/technical.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/trade.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/trade.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/eastmoney/util.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/eastmoney/util.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/event/base.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/event/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/event/cailianshe.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/event/cailianshe.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/event/caixing.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/event/caixing.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/event/investing.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/event/investing.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/event/jin10.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/event/jin10.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/source/event/news.py` & `openfinance-3.3.3/openfinance/datacenter/database/source/event/news.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/__init__.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/base.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/china/industry.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/china/industry.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/china/macro.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/china/macro.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/china/market.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/china/market.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/china/quant.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/china/quant.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/china/stock.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/china/stock.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/financial.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/financial.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/fred/base.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/fred/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/fred/store.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/fred/store.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/gov_stat.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/gov_stat.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/industry.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/industry.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/macro.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/macro.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/market.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/market.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/national_data/__init__.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/national_data/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/national_data/base.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/national_data/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/national_data/store.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/national_data/store.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/us/base.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/us/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/us/financial.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/us/financial.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/storage/us/util.py` & `openfinance-3.3.3/openfinance/datacenter/database/storage/us/util.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/database/wrapper.py` & `openfinance-3.3.3/openfinance/datacenter/database/wrapper.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/echarts/__init__.py` & `openfinance-3.3.3/openfinance/datacenter/echarts/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/echarts/bar.py` & `openfinance-3.3.3/openfinance/datacenter/echarts/bar.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/echarts/base.py` & `openfinance-3.3.3/openfinance/datacenter/echarts/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/echarts/multibar.py` & `openfinance-3.3.3/openfinance/datacenter/echarts/multibar.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/echarts/pie.py` & `openfinance-3.3.3/openfinance/datacenter/echarts/pie.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/echarts/stacked_line.py` & `openfinance-3.3.3/openfinance/datacenter/echarts/stacked_line.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/echarts/tree.py` & `openfinance-3.3.3/openfinance/datacenter/echarts/tree.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/knowledge/decorator.py` & `openfinance-3.3.3/openfinance/datacenter/knowledge/decorator.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/knowledge/entity_graph.py` & `openfinance-3.3.3/openfinance/datacenter/knowledge/entity_graph.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/knowledge/executor.py` & `openfinance-3.3.3/openfinance/datacenter/knowledge/executor.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/knowledge/factor.py` & `openfinance-3.3.3/openfinance/datacenter/knowledge/factor.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/knowledge/graph.py` & `openfinance-3.3.3/openfinance/datacenter/knowledge/graph.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/datacenter/knowledge/wrapper.py` & `openfinance-3.3.3/openfinance/datacenter/knowledge/wrapper.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/page_manage/base.py` & `openfinance-3.3.3/openfinance/searchhub/page_manage/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/page_manage/company.py` & `openfinance-3.3.3/openfinance/searchhub/page_manage/company.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/page_manage/factor.py` & `openfinance-3.3.3/openfinance/searchhub/page_manage/factor.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/page_manage/model.py` & `openfinance-3.3.3/openfinance/searchhub/page_manage/model.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/page_manage/role.py` & `openfinance-3.3.3/openfinance/searchhub/page_manage/role.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/page_manage/user.py` & `openfinance-3.3.3/openfinance/searchhub/page_manage/user.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/query_understand/base.py` & `openfinance-3.3.3/openfinance/searchhub/query_understand/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/recall/base.py` & `openfinance-3.3.3/openfinance/searchhub/recall/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/analysis/analysis_task.py` & `openfinance-3.3.3/openfinance/searchhub/task/analysis/analysis_task.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/analysis/auto_analysis.py` & `openfinance-3.3.3/openfinance/searchhub/task/analysis/auto_analysis.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/analysis/fixed_analysis_task.py` & `openfinance-3.3.3/openfinance/searchhub/task/analysis/fixed_analysis_task.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/percept/online_percept_task.py` & `openfinance-3.3.3/openfinance/searchhub/task/percept/online_percept_task.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/percept/percept_task.py` & `openfinance-3.3.3/openfinance/searchhub/task/percept/percept_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             self.llm, 
         )
         self.match = MatchFlow.from_llm(
             self.llm,
             index_manager
         )
 
-    def  _init_index(
+    def _init_index(
         self
     ) -> IndexManager:
         index_manager = IndexManager()
         save_local = True
         if not save_local:
             graph = Graph.build_from_file(
                 "openfinance/datacenter/knowledge/schema.md"
```

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/base.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/industry/base.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/industry/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/industry/output_parser.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/industry/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/macro/base.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/macro/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/macro/output_parser.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/macro/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/stock/base.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/stock/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/stock/output_parser.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/stock/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/strategy/base.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/strategy/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/strategy/output_parser.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/strategy/output_parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/qa_search/test_intent_search.py` & `openfinance-3.3.3/openfinance/searchhub/task/qa_search/test_intent_search.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/role/role_task.py` & `openfinance-3.3.3/openfinance/searchhub/task/role/role_task.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/role/test_charcter.py` & `openfinance-3.3.3/openfinance/searchhub/task/role/test_charcter.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/search/search_task.py` & `openfinance-3.3.3/openfinance/searchhub/task/search/search_task.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/search_sql/search_sql_task.py` & `openfinance-3.3.3/openfinance/searchhub/task/search_sql/search_sql_task.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/searchhub/task/task_manager.py` & `openfinance-3.3.3/openfinance/searchhub/task/task_manager.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/auth/login.py` & `openfinance-3.3.3/openfinance/service/auth/login.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/base.py` & `openfinance-3.3.3/openfinance/service/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/chat_http_server.py` & `openfinance-3.3.3/openfinance/service/chat_http_server.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/chat_socket_server.py` & `openfinance-3.3.3/openfinance/service/chat_socket_server.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/easy_embedding_service.py` & `openfinance-3.3.3/openfinance/service/easy_embedding_service.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/easy_quant.py` & `openfinance-3.3.3/openfinance/service/easy_quant.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/embedding_service.py` & `openfinance-3.3.3/openfinance/service/embedding_service.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/error.py` & `openfinance-3.3.3/openfinance/service/error.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/finance_service.py` & `openfinance-3.3.3/openfinance/service/finance_service.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/homepage_server.py` & `openfinance-3.3.3/openfinance/service/homepage_server.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/service/push_data_service.py` & `openfinance-3.3.3/openfinance/service/push_data_service.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/base.py` & `openfinance-3.3.3/openfinance/strategy/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/data_storage/company_storage.py` & `openfinance-3.3.3/openfinance/strategy/data_storage/company_storage.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/data_storage/market_storage.py` & `openfinance-3.3.3/openfinance/strategy/data_storage/market_storage.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/base.py` & `openfinance-3.3.3/openfinance/strategy/feature/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/company/__init__.py` & `openfinance-3.3.3/openfinance/strategy/feature/company/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/company/divident_mean.py` & `openfinance-3.3.3/openfinance/strategy/feature/company/divident_mean.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/company/divident_stability.py` & `openfinance-3.3.3/openfinance/strategy/feature/company/divident_stability.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/company/news_sentiment.py` & `openfinance-3.3.3/openfinance/strategy/feature/company/news_sentiment.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/company/win_cost_distribution.py` & `openfinance-3.3.3/openfinance/strategy/feature/company/win_cost_distribution.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/data_adaptor.py` & `openfinance-3.3.3/openfinance/strategy/feature/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/macro/vix.py` & `openfinance-3.3.3/openfinance/strategy/feature/macro/vix.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/market/__init__.py` & `openfinance-3.3.3/openfinance/strategy/feature/market/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/market/market_volume.py` & `openfinance-3.3.3/openfinance/strategy/feature/market/market_volume.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/market/north_moneyflow.py` & `openfinance-3.3.3/openfinance/strategy/feature/market/north_moneyflow.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/market/north_moneyflow_position.py` & `openfinance-3.3.3/openfinance/strategy/feature/market/north_moneyflow_position.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/feature/market/vix.py` & `openfinance-3.3.3/openfinance/strategy/feature/market/vix.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/model/base.py` & `openfinance-3.3.3/openfinance/strategy/model/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/model/index_sort.py` & `openfinance-3.3.3/openfinance/strategy/model/index_sort.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/model/linear_regression.py` & `openfinance-3.3.3/openfinance/strategy/model/linear_regression.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/__init__.py` & `openfinance-3.3.3/openfinance/strategy/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/acc.py` & `openfinance-3.3.3/openfinance/strategy/operator/acc.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/base.py` & `openfinance-3.3.3/openfinance/strategy/operator/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/coefficient_variance.py` & `openfinance-3.3.3/openfinance/strategy/operator/coefficient_variance.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/hist.py` & `openfinance-3.3.3/openfinance/strategy/operator/hist.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/latest_position_index.py` & `openfinance-3.3.3/openfinance/strategy/operator/latest_position_index.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/macd.py` & `openfinance-3.3.3/openfinance/strategy/operator/macd.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/mean.py` & `openfinance-3.3.3/openfinance/strategy/operator/mean.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/moving_average.py` & `openfinance-3.3.3/openfinance/strategy/operator/moving_average.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/obv.py` & `openfinance-3.3.3/openfinance/strategy/operator/obv.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/operator/rsi.py` & `openfinance-3.3.3/openfinance/strategy/operator/rsi.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/policy/base.py` & `openfinance-3.3.3/openfinance/strategy/policy/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/policy/company_ranker.py` & `openfinance-3.3.3/openfinance/strategy/policy/company_ranker.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/policy/lr_ranker.py` & `openfinance-3.3.3/openfinance/strategy/policy/lr_ranker.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/policy/market_danger.py` & `openfinance-3.3.3/openfinance/strategy/policy/market_danger.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/policy/market_sentiment.py` & `openfinance-3.3.3/openfinance/strategy/policy/market_sentiment.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/third_party/eastmoney_pool.py` & `openfinance-3.3.3/openfinance/strategy/third_party/eastmoney_pool.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/strategy/third_party/ths_em_pool.py` & `openfinance-3.3.3/openfinance/strategy/third_party/ths_em_pool.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/embeddings/embedding_manager.py` & `openfinance-3.3.3/openfinance/utils/embeddings/embedding_manager.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/embeddings/huggingface_embedding.py` & `openfinance-3.3.3/openfinance/utils/embeddings/huggingface_embedding.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/embeddings/sentence_transformers.py` & `openfinance-3.3.3/openfinance/utils/embeddings/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/embeddings/sentence_transformers_cn.py` & `openfinance-3.3.3/openfinance/utils/embeddings/sentence_transformers_cn.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/log.py` & `openfinance-3.3.3/openfinance/utils/log.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/recall/base.py` & `openfinance-3.3.3/openfinance/utils/recall/base.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/recall/es.py` & `openfinance-3.3.3/openfinance/utils/recall/es.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
         docs: Dict[str, Any]
     ):
         """
             docs: {'id': { 'title': 'new_value1', 'doc': 'new_value2'} },
         """
         """批量写入"""
         actions = []
-        for sid, docs in docs.items():
+        for sid, doc in docs.items():
             action = {
                 "_index": self.name,
                 "_type": "_doc",
                 "_id": sid,
-                "_source": docs
+                "_source": doc
             }
             # print(index)
             actions.append(action)
         ret = helpers.bulk(self.client, actions)
         # print(ret)
         return ret
```

### Comparing `openfinance-3.3.2/openfinance/utils/recall/faiss.py` & `openfinance-3.3.3/openfinance/utils/recall/faiss.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/redis/redis_tools.py` & `openfinance-3.3.3/openfinance/utils/redis/redis_tools.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance/utils/string_tools/parser.py` & `openfinance-3.3.3/openfinance/utils/string_tools/parser.py`

 * *Files identical despite different names*

### Comparing `openfinance-3.3.2/openfinance.egg-info/PKG-INFO` & `openfinance-3.3.3/openfinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfinance
-Version: 3.3.2
+Version: 3.3.3
 Summary: an open financial agent framework powered by llm
 Home-page: 
 Author: Bin ZHU
 Author-email: zhubin_n@outlook.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openfinance-3.3.2/openfinance.egg-info/SOURCES.txt` & `openfinance-3.3.3/openfinance.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 openfinance/agents/role/prompts/catherine_wood.py
 openfinance/agents/role/prompts/elon_musk.py
 openfinance/agents/role/prompts/growth_investor.py
 openfinance/agents/role/prompts/quant_investor.py
 openfinance/agents/role/prompts/ray_dalio.py
 openfinance/agents/role/prompts/valuation_investor.py
 openfinance/agents/role/prompts/warren_buffett.py
+openfinance/agents/skill/__init__.py
+openfinance/agents/skill/analysis.py
 openfinance/agents/third_party/__init__.py
 openfinance/agents/tool/__init__.py
 openfinance/agents/tool/factor_search.py
 openfinance/agents/tool/search.py
 openfinance/config/__init__.py
 openfinance/config/config.py
 openfinance/datacenter/__init__.py
@@ -189,15 +191,14 @@
 openfinance/searchhub/page_manage/__init__.py
 openfinance/searchhub/page_manage/base.py
 openfinance/searchhub/page_manage/company.py
 openfinance/searchhub/page_manage/factor.py
 openfinance/searchhub/page_manage/model.py
 openfinance/searchhub/page_manage/role.py
 openfinance/searchhub/page_manage/user.py
-openfinance/searchhub/page_rank/__init__.py
 openfinance/searchhub/query_understand/__init__.py
 openfinance/searchhub/query_understand/base.py
 openfinance/searchhub/recall/__init__.py
 openfinance/searchhub/recall/base.py
 openfinance/searchhub/recall/channel/__init__.py
 openfinance/searchhub/recall/channel/analysis.py
 openfinance/searchhub/recall/channel/search.py
```

### Comparing `openfinance-3.3.2/setup.py` & `openfinance-3.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="openfinance",
-    version="3.3.2",
+    version="3.3.3",
     author="Bin ZHU",
     author_email="zhubin_n@outlook.com",
     description="an open financial agent framework powered by llm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```


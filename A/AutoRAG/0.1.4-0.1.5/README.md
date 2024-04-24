# Comparing `tmp/autorag-0.1.4.tar.gz` & `tmp/autorag-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.1.4.tar", last modified: Mon Apr 22 06:04:28 2024, max compression
+gzip compressed data, was "autorag-0.1.5.tar", last modified: Wed Apr 24 16:52:39 2024, max compression
```

## Comparing `autorag-0.1.4.tar` & `autorag-0.1.5.tar`

### file list

```diff
@@ -1,499 +1,514 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.186767 autorag-0.1.4/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.067275 autorag-0.1.4/.github/
--rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.4/.github/dependabot.yml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.067903 autorag-0.1.4/.github/workflows/
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.4/.github/workflows/sphinx.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-22 05:42:18.000000 autorag-0.1.4/.github/workflows/test.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.4/.gitignore
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.185949 autorag-0.1.4/AutoRAG.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    19139 2024-04-22 06:04:28.000000 autorag-0.1.4/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      512 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-22 05:42:18.000000 autorag-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-22 05:42:18.000000 autorag-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.4/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-22 06:04:28.186490 autorag-0.1.4/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.4/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.071310 autorag-0.1.4/autorag/
--rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-22 06:00:49.000000 autorag-0.1.4/autorag/VERSION
--rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.4/autorag/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/cli.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.071520 autorag-0.1.4/autorag/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.4/autorag/data/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.072262 autorag-0.1.4/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.4/autorag/data/corpus/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1625 2024-03-22 05:41:56.000000 autorag-0.1.4/autorag/data/corpus/langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2834 2024-03-22 04:27:08.000000 autorag-0.1.4/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.073794 autorag-0.1.4/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.4/autorag/data/qacreation/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/data/qacreation/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-17 13:38:02.000000 autorag-0.1.4/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.4/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/data/qacreation/ragas.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.074130 autorag-0.1.4/autorag/data/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/data/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/data/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.4/autorag/deploy.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.075680 autorag-0.1.4/autorag/evaluate/
--rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.4/autorag/evaluate/generation.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.077004 autorag-0.1.4/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.4/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.078055 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/evaluate/metric/generation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 autorag-0.1.4/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 autorag-0.1.4/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/metric/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.4/autorag/evaluate/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    17273 2024-04-12 13:21:55.000000 autorag-0.1.4/autorag/evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/node_line.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.078404 autorag-0.1.4/autorag/nodes/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.079594 autorag-0.1.4/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.4/autorag/nodes/generator/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.4/autorag/nodes/generator/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.4/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.4/autorag/nodes/generator/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.4/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.081205 autorag-0.1.4/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.4/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.4/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.4/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.082746 autorag-0.1.4/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.4/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2476 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3955 2024-04-10 13:46:46.000000 autorag-0.1.4/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.087030 autorag-0.1.4/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.4/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3936 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2612 2024-04-22 05:42:18.000000 autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2373 2024-04-22 05:42:18.000000 autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.4/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.4/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-19 15:05:28.000000 autorag-0.1.4/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.4/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.4/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4167 2024-04-10 13:46:46.000000 autorag-0.1.4/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.087897 autorag-0.1.4/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3864 2024-04-22 05:42:18.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 autorag-0.1.4/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.089208 autorag-0.1.4/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.4/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.4/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.4/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.4/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.090776 autorag-0.1.4/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.4/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.4/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.4/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.4/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.4/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.4/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.093188 autorag-0.1.4/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.4/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    10780 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 autorag-0.1.4/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.094165 autorag-0.1.4/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/schema/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/schema/module.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/schema/node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3985 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/support.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.094604 autorag-0.1.4/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)      161 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2611 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/utils/preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11345 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.4/autorag/web.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-19 08:38:15.000000 autorag-0.1.4/dev_requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.095404 autorag-0.1.4/docs/
--rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.4/docs/Makefile
--rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.4/docs/make.bat
--rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-19 08:38:15.000000 autorag-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.097257 autorag-0.1.4/docs/source/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.104281 autorag-0.1.4/docs/source/_static/
--rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/data_creation.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/data_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_line_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_line_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_lines.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.4/docs/source/_static/project_folder_example.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/project_folders.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.108275 autorag-0.1.4/docs/source/_static/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.4/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/trial_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/trial_json.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/trial_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.4/docs/source/_static/web_interface.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.112935 autorag-0.1.4/docs/source/api_spec/
--rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.4/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.4/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     3229 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1688 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      432 2024-04-10 13:46:46.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.4/docs/source/api_spec/autorag.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.4/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.4/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.4/docs/source/api_spec/modules.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-19 08:38:15.000000 autorag-0.1.4/docs/source/conf.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.113728 autorag-0.1.4/docs/source/data_creation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.4/docs/source/data_creation/data_format.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/data_creation/ragas.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.4/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.114364 autorag-0.1.4/docs/source/deploy/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.4/docs/source/deploy/web.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/index.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.4/docs/source/install.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/local_model.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.114606 autorag-0.1.4/docs/source/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.115360 autorag-0.1.4/docs/source/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.4/docs/source/nodes/generator/generator.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.4/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/index.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.116044 autorag-0.1.4/docs/source/nodes/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.116986 autorag-0.1.4/docs/source/nodes/passage_filter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.4/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.120224 autorag-0.1.4/docs/source/nodes/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.121020 autorag-0.1.4/docs/source/nodes/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.4/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.4/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.121526 autorag-0.1.4/docs/source/nodes/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.4/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.123164 autorag-0.1.4/docs/source/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.124265 autorag-0.1.4/docs/source/optimization/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.4/docs/source/optimization/custom_config.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/optimization/folder_structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.4/docs/source/optimization/optimization.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.124486 autorag-0.1.4/docs/source/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.4/docs/source/troubleshooting.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.4/docs/source/tutorial.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 autorag-0.1.4/pyproject.toml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1149 2024-04-12 13:21:50.000000 autorag-0.1.4/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.126343 autorag-0.1.4/sample_config/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.4/sample_config/compact_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.4/sample_config/compact_openai.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.4/sample_config/config_korean.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.4/sample_config/extracted_sample.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     4448 2024-04-15 08:09:03.000000 autorag-0.1.4/sample_config/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.4/sample_config/simple_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.4/sample_config/simple_openai.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.126595 autorag-0.1.4/sample_dataset/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.4/sample_dataset/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.126959 autorag-0.1.4/sample_dataset/eli5/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.4/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.127211 autorag-0.1.4/sample_dataset/msmarco/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.4/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.127503 autorag-0.1.4/sample_dataset/triviaqa/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.4/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-22 06:04:28.186829 autorag-0.1.4/setup.cfg
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.128222 autorag-0.1.4/tests/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.129881 autorag-0.1.4/tests/autorag/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.060481 autorag-0.1.4/tests/autorag/data/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.130777 autorag-0.1.4/tests/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.4/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      642 2024-03-22 04:29:59.000000 autorag-0.1.4/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      977 2024-03-25 07:44:05.000000 autorag-0.1.4/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.131780 autorag-0.1.4/tests/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.132712 autorag-0.1.4/tests/autorag/evaluate/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.133391 autorag-0.1.4/tests/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.4/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1569 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.4/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.061334 autorag-0.1.4/tests/autorag/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.134396 autorag-0.1.4/tests/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.135823 autorag-0.1.4/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.137371 autorag-0.1.4/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3799 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.141569 autorag-0.1.4/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      795 2024-03-17 04:13:16.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-08 12:04:54.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1078 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1524 2024-04-06 14:23:40.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1795 2024-04-05 03:16:26.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1120 2024-04-08 08:26:20.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      963 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.142186 autorag-0.1.4/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.143336 autorag-0.1.4/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.145475 autorag-0.1.4/tests/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.146442 autorag-0.1.4/tests/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.4/tests/autorag/test_cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/test_deploy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/test_evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/test_strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/test_support.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.4/tests/autorag/test_web.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.147040 autorag-0.1.4/tests/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2491 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9696 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/utils/test_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/conftest.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/delete_tests.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.4/tests/mock.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.149649 autorag-0.1.4/tests/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.4/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.061800 autorag-0.1.4/tests/resources/data_creation/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.150554 autorag-0.1.4/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.4/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.4/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.4/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.4/tests/resources/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.4/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.151376 autorag-0.1.4/tests/resources/qa_gen_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.4/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.4/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.152210 autorag-0.1.4/tests/resources/result_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.152692 autorag-0.1.4/tests/resources/result_project/0/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.153001 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.155530 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.156533 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.156765 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.158056 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.158184 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.159101 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.160483 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.161889 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.4/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.162261 autorag-0.1.4/tests/resources/result_project/1/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.162840 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.164411 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.063587 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.164577 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.165637 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.167245 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.167489 autorag-0.1.4/tests/resources/result_project/2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.063845 autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.167724 autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.168306 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.169746 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.169898 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.170546 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.173426 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.175403 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.175618 autorag-0.1.4/tests/resources/result_project/3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.4/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.176421 autorag-0.1.4/tests/resources/result_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.176727 autorag-0.1.4/tests/resources/result_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.176981 autorag-0.1.4/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.183652 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/trial.json
--rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.065081 autorag-0.1.4/tests/resources/sample_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.184630 autorag-0.1.4/tests/resources/sample_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.4/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.4/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.184991 autorag-0.1.4/tests/resources/sample_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.4/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/resources/simple.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.4/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.229396 autorag-0.1.5/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.109232 autorag-0.1.5/.github/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.5/.github/dependabot.yml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.109813 autorag-0.1.5/.github/workflows/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.5/.github/workflows/sphinx.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-22 05:42:18.000000 autorag-0.1.5/.github/workflows/test.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.5/.gitignore
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.228604 autorag-0.1.5/AutoRAG.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19810 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      512 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-24 16:52:39.000000 autorag-0.1.5/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-22 05:42:18.000000 autorag-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-22 05:42:18.000000 autorag-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.5/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-24 16:52:39.229115 autorag-0.1.5/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.5/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.113097 autorag-0.1.5/autorag/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-24 15:34:10.000000 autorag-0.1.5/autorag/VERSION
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.5/autorag/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/cli.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.113300 autorag-0.1.5/autorag/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.5/autorag/data/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.113843 autorag-0.1.5/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.5/autorag/data/corpus/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1538 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/data/corpus/langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3645 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.115334 autorag-0.1.5/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.5/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/data/qacreation/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-17 13:38:02.000000 autorag-0.1.5/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.5/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.115656 autorag-0.1.5/autorag/data/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/data/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/data/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.5/autorag/deploy.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.116859 autorag-0.1.5/autorag/evaluate/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.5/autorag/evaluate/generation.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.118028 autorag-0.1.5/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.5/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.119256 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-19 08:38:15.000000 autorag-0.1.5/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 autorag-0.1.5/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 autorag-0.1.5/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/metric/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.5/autorag/evaluate/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    17273 2024-04-12 13:21:55.000000 autorag-0.1.5/autorag/evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/node_line.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.119411 autorag-0.1.5/autorag/nodes/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.120387 autorag-0.1.5/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.5/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.5/autorag/nodes/generator/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.5/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.5/autorag/nodes/generator/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.5/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.121567 autorag-0.1.5/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      112 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4688 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      388 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3387 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.123015 autorag-0.1.5/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.5/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.5/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.5/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.124582 autorag-0.1.5/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.5/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.5/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2399 2024-04-24 16:50:09.000000 autorag-0.1.5/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3951 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.128761 autorag-0.1.5/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.5/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3625 2024-04-24 15:33:34.000000 autorag-0.1.5/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2722 2024-04-24 07:39:51.000000 autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2397 2024-04-24 07:39:51.000000 autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.5/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.5/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-19 15:05:28.000000 autorag-0.1.5/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.5/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.5/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4167 2024-04-10 13:46:46.000000 autorag-0.1.5/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-19 08:38:15.000000 autorag-0.1.5/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.129544 autorag-0.1.5/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3832 2024-04-23 11:22:32.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.5/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 autorag-0.1.5/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.130803 autorag-0.1.5/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.5/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.5/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.5/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.5/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.132248 autorag-0.1.5/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.5/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.5/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.5/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.5/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.5/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.5/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.134794 autorag-0.1.5/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.5/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    10780 2024-04-11 14:29:33.000000 autorag-0.1.5/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 autorag-0.1.5/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.135655 autorag-0.1.5/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/schema/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/schema/module.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/schema/node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.5/autorag/strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4202 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/support.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.136515 autorag-0.1.5/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      177 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3314 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/utils/preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11592 2024-04-23 11:20:05.000000 autorag-0.1.5/autorag/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.5/autorag/web.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-19 08:38:15.000000 autorag-0.1.5/dev_requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.137354 autorag-0.1.5/docs/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.5/docs/Makefile
+-rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.5/docs/make.bat
+-rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-19 08:38:15.000000 autorag-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.138956 autorag-0.1.5/docs/source/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.146987 autorag-0.1.5/docs/source/_static/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/data_creation.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/data_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_lines.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/node_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.5/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/project_folders.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.150528 autorag-0.1.5/docs/source/_static/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.5/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/trial_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/trial_json.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/_static/trial_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.5/docs/source/_static/web_interface.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.155380 autorag-0.1.5/docs/source/api_spec/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.5/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.5/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.5/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      864 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3434 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1896 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      466 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.5/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.5/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.5/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.5/docs/source/api_spec/modules.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-19 08:38:15.000000 autorag-0.1.5/docs/source/conf.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.156438 autorag-0.1.5/docs/source/data_creation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.5/docs/source/data_creation/data_format.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/data_creation/ragas.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.5/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.156995 autorag-0.1.5/docs/source/deploy/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.5/docs/source/deploy/web.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/index.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.5/docs/source/install.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/local_model.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.157210 autorag-0.1.5/docs/source/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.157845 autorag-0.1.5/docs/source/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.5/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.5/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/index.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.158205 autorag-0.1.5/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1591 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      727 2024-04-23 11:20:05.000000 autorag-0.1.5/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.158750 autorag-0.1.5/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.159879 autorag-0.1.5/docs/source/nodes/passage_filter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.5/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.162697 autorag-0.1.5/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.163486 autorag-0.1.5/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.5/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.5/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.164037 autorag-0.1.5/docs/source/nodes/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.5/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.165410 autorag-0.1.5/docs/source/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.5/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.166363 autorag-0.1.5/docs/source/optimization/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.5/docs/source/optimization/custom_config.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.5/docs/source/optimization/optimization.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.166578 autorag-0.1.5/docs/source/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.5/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.5/docs/source/structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.5/docs/source/troubleshooting.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.5/docs/source/tutorial.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 autorag-0.1.5/pyproject.toml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1149 2024-04-12 13:21:50.000000 autorag-0.1.5/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168158 autorag-0.1.5/sample_config/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.5/sample_config/compact_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.5/sample_config/compact_openai.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.5/sample_config/config_korean.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.5/sample_config/extracted_sample.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4769 2024-04-23 11:20:05.000000 autorag-0.1.5/sample_config/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.5/sample_config/simple_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.5/sample_config/simple_openai.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168353 autorag-0.1.5/sample_dataset/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.5/sample_dataset/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168592 autorag-0.1.5/sample_dataset/eli5/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.5/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.168768 autorag-0.1.5/sample_dataset/msmarco/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.5/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.169050 autorag-0.1.5/sample_dataset/triviaqa/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.5/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-24 16:52:39.229444 autorag-0.1.5/setup.cfg
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.169871 autorag-0.1.5/tests/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.171394 autorag-0.1.5/tests/autorag/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.103562 autorag-0.1.5/tests/autorag/data/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.172491 autorag-0.1.5/tests/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.5/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      646 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1317 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.173594 autorag-0.1.5/tests/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.174416 autorag-0.1.5/tests/autorag/evaluate/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.175060 autorag-0.1.5/tests/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.5/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1569 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.5/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.104392 autorag-0.1.5/tests/autorag/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.176256 autorag-0.1.5/tests/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.5/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.177237 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      751 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2594 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3080 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.178536 autorag-0.1.5/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.180550 autorag-0.1.5/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4380 2024-04-24 16:50:09.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.184156 autorag-0.1.5/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1160 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1994 2024-04-24 07:39:51.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2213 2024-04-24 07:39:51.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1407 2024-04-23 11:22:32.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2230 2024-04-24 15:33:34.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1604 2024-04-23 11:22:32.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-04-23 11:22:32.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 autorag-0.1.5/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.185071 autorag-0.1.5/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.186362 autorag-0.1.5/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.188935 autorag-0.1.5/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 autorag-0.1.5/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.189404 autorag-0.1.5/tests/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.5/tests/autorag/test_cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/autorag/test_deploy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-19 08:38:15.000000 autorag-0.1.5/tests/autorag/test_evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/test_strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.5/tests/autorag/test_support.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.5/tests/autorag/test_web.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.189880 autorag-0.1.5/tests/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2788 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9696 2024-04-12 13:21:50.000000 autorag-0.1.5/tests/autorag/utils/test_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/conftest.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.5/tests/delete_tests.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.5/tests/mock.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.192654 autorag-0.1.5/tests/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/README.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.5/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.104743 autorag-0.1.5/tests/resources/data_creation/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.194028 autorag-0.1.5/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.5/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.5/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.5/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.5/tests/resources/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.5/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.194786 autorag-0.1.5/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.5/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.5/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.195398 autorag-0.1.5/tests/resources/result_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.195865 autorag-0.1.5/tests/resources/result_project/0/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.196074 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.198778 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.199769 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.200011 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.201350 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.201500 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.202401 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.203909 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.205377 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.5/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.205623 autorag-0.1.5/tests/resources/result_project/1/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.205897 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.208020 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.106328 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.208168 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.209169 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.210786 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.211077 autorag-0.1.5/tests/resources/result_project/2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.106523 autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.211273 autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.211870 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.213603 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.213749 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.214427 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.216199 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.217974 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.218190 autorag-0.1.5/tests/resources/result_project/3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.5/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.219120 autorag-0.1.5/tests/resources/result_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.219375 autorag-0.1.5/tests/resources/result_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.5/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.219631 autorag-0.1.5/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.226159 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.5/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.5/tests/resources/result_project/trial.json
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.5/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.107437 autorag-0.1.5/tests/resources/sample_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.227275 autorag-0.1.5/tests/resources/sample_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   115302 2024-04-23 11:20:05.000000 autorag-0.1.5/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.5/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-24 16:52:39.227775 autorag-0.1.5/tests/resources/sample_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.5/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.5/tests/resources/simple.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.5/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.1.4/.github/workflows/sphinx.yml` & `autorag-0.1.5/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/.github/workflows/test.yml` & `autorag-0.1.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/.gitignore` & `autorag-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/AutoRAG.egg-info/PKG-INFO` & `autorag-0.1.5/AutoRAG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.4
+Version: 0.1.5
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.1.4/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.1.5/AutoRAG.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
 autorag/nodes/__init__.py
 autorag/nodes/generator/__init__.py
 autorag/nodes/generator/base.py
 autorag/nodes/generator/llama_index_llm.py
 autorag/nodes/generator/run.py
 autorag/nodes/generator/vllm.py
+autorag/nodes/passageaugmenter/__init__.py
+autorag/nodes/passageaugmenter/base.py
+autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+autorag/nodes/passageaugmenter/prev_next_augmenter.py
+autorag/nodes/passageaugmenter/run.py
 autorag/nodes/passagecompressor/__init__.py
 autorag/nodes/passagecompressor/base.py
 autorag/nodes/passagecompressor/pass_compressor.py
 autorag/nodes/passagecompressor/refine.py
 autorag/nodes/passagecompressor/run.py
 autorag/nodes/passagecompressor/tree_summarize.py
 autorag/nodes/passagefilter/__init__.py
@@ -148,14 +153,15 @@
 docs/source/api_spec/autorag.data.corpus.rst
 docs/source/api_spec/autorag.data.qacreation.rst
 docs/source/api_spec/autorag.data.rst
 docs/source/api_spec/autorag.data.utils.rst
 docs/source/api_spec/autorag.evaluate.metric.rst
 docs/source/api_spec/autorag.evaluate.rst
 docs/source/api_spec/autorag.nodes.generator.rst
+docs/source/api_spec/autorag.nodes.passageaugmenter.rst
 docs/source/api_spec/autorag.nodes.passagecompressor.rst
 docs/source/api_spec/autorag.nodes.passagefilter.rst
 docs/source/api_spec/autorag.nodes.passagereranker.rst
 docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
 docs/source/api_spec/autorag.nodes.promptmaker.rst
 docs/source/api_spec/autorag.nodes.queryexpansion.rst
 docs/source/api_spec/autorag.nodes.retrieval.rst
@@ -169,14 +175,16 @@
 docs/source/data_creation/tutorial.md
 docs/source/deploy/api_endpoint.md
 docs/source/deploy/web.md
 docs/source/nodes/index.md
 docs/source/nodes/generator/generator.md
 docs/source/nodes/generator/llama_index_llm.md
 docs/source/nodes/generator/vllm.md
+docs/source/nodes/passage_augmenter/passage_augmenter.md
+docs/source/nodes/passage_augmenter/prev_next_augmenter.md
 docs/source/nodes/passage_compressor/passage_compressor.md
 docs/source/nodes/passage_compressor/refine.md
 docs/source/nodes/passage_compressor/tree_summarize.md
 docs/source/nodes/passage_filter/passage_filter.md
 docs/source/nodes/passage_filter/recency_filter.md
 docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
 docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
@@ -245,14 +253,18 @@
 tests/autorag/evaluate/metric/test_generation_metric.py
 tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
 tests/autorag/evaluate/metric/test_retrieval_metric.py
 tests/autorag/nodes/generator/test_generator_base.py
 tests/autorag/nodes/generator/test_llama_index_llm.py
 tests/autorag/nodes/generator/test_run_generator_node.py
 tests/autorag/nodes/generator/test_vllm.py
+tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
 tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
 tests/autorag/nodes/passagecompressor/test_pass_compressor.py
 tests/autorag/nodes/passagecompressor/test_refine.py
 tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
 tests/autorag/nodes/passagecompressor/test_tree_summarize.py
 tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
 tests/autorag/nodes/passagefilter/test_passage_filter_base.py
```

### Comparing `autorag-0.1.4/AutoRAG.egg-info/requires.txt` & `autorag-0.1.5/AutoRAG.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/CODE_OF_CONDUCT.md` & `autorag-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/CONTRIBUTING.md` & `autorag-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/LICENSE` & `autorag-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/PKG-INFO` & `autorag-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.4
+Version: 0.1.5
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.1.4/README.md` & `autorag-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/__init__.py` & `autorag-0.1.5/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/cli.py` & `autorag-0.1.5/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/data/corpus/langchain.py` & `autorag-0.1.5/autorag/data/corpus/langchain.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,17 +21,18 @@
     :param output_filepath: Optional filepath to save the parquet file.
         If None, the function will return the processed_data as pd.DataFrame, but do not save as parquet.
         File directory must exist. File extension must be .parquet
     :param upsert: If true, the function will overwrite the existing file if it exists.
         Default is False.
     :return: Corpus data as pd.DataFrame
     """
-    corpus_df = pd.DataFrame({
-        'doc_id': [str(uuid.uuid4()) for _ in range(len(langchain_documents))],
-        'contents': list(map(lambda doc: doc.page_content, langchain_documents)),
-        'metadata': list(map(lambda doc: add_essential_metadata(doc.metadata), langchain_documents)),
-    })
+
+    corpus_df = pd.DataFrame(list(map(lambda doc: {
+        'doc_id': str(uuid.uuid4()),
+        'contents': doc.page_content,
+        'metadata': add_essential_metadata(doc.metadata)
+    }, langchain_documents)))
 
     if output_filepath is not None:
         save_parquet_safe(corpus_df, output_filepath, upsert=upsert)
 
     return corpus_df
```

### Comparing `autorag-0.1.4/autorag/data/qacreation/base.py` & `autorag-0.1.5/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/data/qacreation/llama_index.py` & `autorag-0.1.5/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.1.5/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/data/qacreation/ragas.py` & `autorag-0.1.5/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/data/qacreation/simple.py` & `autorag-0.1.5/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/data/utils/util.py` & `autorag-0.1.5/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/deploy.py` & `autorag-0.1.5/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/generation.py` & `autorag-0.1.5/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.1.5/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/metric/generation.py` & `autorag-0.1.5/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/metric/retrieval.py` & `autorag-0.1.5/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.1.5/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/retrieval.py` & `autorag-0.1.5/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/retrieval_contents.py` & `autorag-0.1.5/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluate/util.py` & `autorag-0.1.5/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/evaluator.py` & `autorag-0.1.5/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/node_line.py` & `autorag-0.1.5/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/generator/base.py` & `autorag-0.1.5/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.1.5/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/generator/run.py` & `autorag-0.1.5/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/generator/vllm.py` & `autorag-0.1.5/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagecompressor/base.py` & `autorag-0.1.5/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagecompressor/refine.py` & `autorag-0.1.5/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagecompressor/run.py` & `autorag-0.1.5/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.1.5/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagefilter/base.py` & `autorag-0.1.5/autorag/nodes/passagefilter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.1.5/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagefilter/recency.py` & `autorag-0.1.5/autorag/nodes/passagefilter/recency.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 import logging
-from datetime import datetime
-from typing import List, Tuple
+from datetime import datetime, date
+from typing import List, Tuple, Union
 
 from autorag.nodes.passagefilter.base import passage_filter_node
 
 logger = logging.getLogger("AutoRAG")
 
 
 @passage_filter_node
 def recency_filter(contents_list: List[List[str]],
                    scores_list: List[List[float]], ids_list: List[List[str]],
                    time_list: List[List[datetime]],
-                   threshold: str,
+                   threshold: Union[datetime, date],
                    ) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     """
     Filter out the contents that are below the threshold datetime.
     If all contents are filtered, keep the only one recency content.
     If the threshold date format is incorrect, return the original contents.
 
     :param contents_list: The list of lists of contents to filter
     :param scores_list: The list of lists of scores retrieved
     :param ids_list: The list of lists of ids retrieved
     :param time_list: The list of lists of datetime retrieved
     :param threshold: The threshold to cut off
     :return: Tuple of lists containing the filtered contents, ids, and scores
     """
+    if not (isinstance(threshold, datetime) or isinstance(threshold, date)):
+        raise ValueError(f"Threshold should be a datetime object, but got {type(threshold)}")
+
+    if not isinstance(threshold, datetime):
+        threshold = datetime.combine(threshold, datetime.min.time())
+
+    time_list = [
+        list(map(lambda t: datetime.combine(t, datetime.min.time()) if not isinstance(t, datetime) else t, time))
+        for time in time_list
+    ]
 
     def sort_row(contents, scores, ids, time, _datetime_threshold):
         combined = list(zip(contents, scores, ids, time))
         combined_filtered = [item for item in combined if item[3] >= _datetime_threshold]
 
         if combined_filtered:
             remain_contents, remain_scores, remain_ids, _ = zip(*combined_filtered)
         else:
             combined.sort(key=lambda x: x[3], reverse=True)
             remain_contents, remain_scores, remain_ids, _ = zip(*combined[:1])
 
         return list(remain_contents), list(remain_ids), list(remain_scores)
 
-    def parse_threshold(threshold_str):
-        for fmt in ("%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M", "%Y-%m-%d"):
-            try:
-                return datetime.strptime(threshold_str, fmt)
-            except ValueError:
-                continue
-        logger.info("threshold date format is incorrect, "
-                    "should be YYYY-MM-DD or YYYY-MM-DD HH:MM:SS or YYYY-MM-DD HH:MM")
-        return None
-
-    datetime_threshold = parse_threshold(threshold)
-    if datetime_threshold is None:
-        return contents_list, ids_list, scores_list
-
     remain_contents_list, remain_ids_list, remain_scores_list = zip(
-        *map(sort_row, contents_list, scores_list, ids_list, time_list, [datetime_threshold] * len(contents_list)))
+        *map(sort_row, contents_list, scores_list, ids_list, time_list, [threshold] * len(contents_list)))
 
     return remain_contents_list, remain_ids_list, remain_scores_list
```

### Comparing `autorag-0.1.4/autorag/nodes/passagefilter/run.py` & `autorag-0.1.5/autorag/nodes/passagefilter/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     :param modules: Passage filter modules to run.
     :param module_params: Passage filter module parameters.
     :param previous_result: Previous result dataframe.
         Could be retrieval, reranker, passage filter modules result.
         It means it must contain 'query', 'retrieved_contents', 'retrieved_ids', 'retrieve_scores' columns.
     :param node_line_dir: This node line's directory.
-    :param strategies: Strategies for passage reranker node.
+    :param strategies: Strategies for passage filter node.
         In this node, we use 'retrieval_f1', 'retrieval_recall' and 'retrieval_precision'.
         You can skip evaluation when you use only one module and a module parameter.
     :return: The best result dataframe with previous result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
@@ -34,15 +34,15 @@
 
     results, execution_times = zip(*map(lambda task: measure_speed(
         task[0], project_dir=project_dir, previous_result=previous_result, **task[1]), zip(modules, module_params)))
     average_times = list(map(lambda x: x / len(results[0]), execution_times))
 
     # run metrics before filtering
     if strategies.get('metrics') is None:
-        raise ValueError("You must at least one metrics for passage_reranker evaluation.")
+        raise ValueError("You must at least one metrics for passage_filter evaluation.")
     results = list(map(lambda x: evaluate_retrieval_node(x, retrieval_gt, strategies.get('metrics')), results))
 
     # save results to folder
     save_dir = os.path.join(node_line_dir, "passage_filter")  # node name
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
     filepaths = list(map(lambda x: os.path.join(save_dir, f'{x}.parquet'), range(len(modules))))
```

### Comparing `autorag-0.1.4/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.1.5/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/base.py` & `autorag-0.1.5/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/cohere.py` & `autorag-0.1.5/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/colbert.py` & `autorag-0.1.5/autorag/nodes/passagereranker/jina.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,82 @@
-from typing import List, Tuple
+import asyncio
+import os
+from typing import List, Tuple, Optional
 
-import pandas as pd
-import torch
-from transformers import AutoModel, AutoTokenizer
+import aiohttp
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
-from autorag.utils.util import make_batch, select_top_k, flatten_apply, sort_by_scores
+from autorag.utils.util import process_batch
+
+JINA_API_URL = "https://api.jina.ai/v1/rerank"
 
 
 @passage_reranker_node
-def colbert_reranker(queries: List[str], contents_list: List[List[str]],
-                     scores_list: List[List[float]], ids_list: List[List[str]],
-                     top_k: int, batch: int = 64,
-                     model_name: str = "colbert-ir/colbertv2.0",
-                     ) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+def jina_reranker(queries: List[str], contents_list: List[List[str]],
+                  scores_list: List[List[float]], ids_list: List[List[str]],
+                  top_k: int, api_key: Optional[str] = None,
+                  model: str = "jina-reranker-v1-base-en",
+                  batch: int = 8
+                  ) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     """
-    Rerank a list of contents with Colbert rerank models.
-    You can get more information about a Colbert model at https://huggingface.co/colbert-ir/colbertv2.0.
-    It uses BERT-based model, so recommend using CUDA gpu for faster reranking.
+    Rerank a list of contents with Jina rerank models.
+    You can get the API key from https://jina.ai/reranker and set it in the environment variable JINAAI_API_KEY.
 
     :param queries: The list of queries to use for reranking
     :param contents_list: The list of lists of contents to rerank
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
+    :param api_key: The API key for Jina rerank.
+        You can set it in the environment variable JINAAI_API_KEY.
+        Or, you can directly set it on the config YAML file using this parameter.
+        Default is env variable "JINAAI_API_KEY".
+    :param model: The model name for Cohere rerank.
+        You can choose between "jina-reranker-v1-base-en" and "jina-colbert-v1-en".
+        Default is "jina-reranker-v1-base-en".
     :param batch: The number of queries to be processed in a batch
-        Default is 64.
-    :param model_name: The model name for Colbert rerank.
-        You can choose colbert model for reranking.
-        Default is "colbert-ir/colbertv2.0".
     :return: Tuple of lists containing the reranked contents, ids, and scores
     """
-    device = "cuda" if torch.cuda.is_available() else "cpu"
-    model = AutoModel.from_pretrained(model_name).to(device)
-    tokenizer = AutoTokenizer.from_pretrained(model_name)
-
-    nested_list = [list(map(lambda x: [query, x], content_list)) for query, content_list in zip(queries, contents_list)]
-
-    rerank_scores = flatten_apply(colbert_run_model, nested_list, model=model,
-                                  tokenizer=tokenizer, batch_size=batch, device=device)
-    df = pd.DataFrame({
-        'contents': contents_list,
-        'ids': ids_list,
-        'scores': rerank_scores,
-    })
-    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
-    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
-
-    del model
-    if torch.cuda.is_available():
-        torch.cuda.empty_cache()
-
-    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
-
-
-def colbert_run_model(contents_list, model, tokenizer, device, batch_size: int):
-    batch_contents_list = make_batch(contents_list, batch_size)
-    results = []
-
-    for batch_contents in batch_contents_list:
-        flattened_batch_queries, flattened_batch_contents = map(list, zip(*batch_contents))
-
-        # Tokenize both queries and contents together
-        feature = tokenizer(flattened_batch_queries, flattened_batch_contents, padding=True, truncation=True,
-                            return_tensors="pt").to(device)
-
-        # Process the combined feature through the model in one go
-        outputs = model(**feature)
-        last_hidden_state = outputs.last_hidden_state
-
-        # Split the embeddings back into query and content parts
-        num_queries = len(flattened_batch_queries)
-        query_embedding, content_embedding = last_hidden_state.split(
-            [num_queries, last_hidden_state.size(1) - num_queries], dim=1)
-
-        # Calculate cosine similarity between query and content embeddings
-        sim_matrix = torch.nn.functional.cosine_similarity(
-            query_embedding.unsqueeze(2), content_embedding.unsqueeze(1), dim=-1
-        )
-
-        # Take the maximum similarity for each query token (across all document tokens)
-        max_sim_scores, _ = torch.max(sim_matrix, dim=2)
-        results.extend(torch.mean(max_sim_scores, dim=1))
+    if api_key is None:
+        api_key = os.getenv("JINAAI_API_KEY", None)
+        if api_key is None:
+            raise ValueError("API key is not provided."
+                             "You can set it as an argument or as an environment variable 'JINAAI_API_KEY'")
+
+    tasks = [jina_reranker_pure(query, contents, scores, ids, top_k=top_k, api_key=api_key, model=model) for
+             query, contents, scores, ids in
+             zip(queries, contents_list, scores_list, ids_list)]
+    loop = asyncio.get_event_loop()
+    results = loop.run_until_complete(process_batch(tasks, batch))
+
+    content_result, id_result, score_result = zip(*results)
+
+    return list(content_result), list(id_result), list(score_result)
+
+
+async def jina_reranker_pure(query: str, contents: List[str],
+                             scores: List[float], ids: List[str],
+                             top_k: int, api_key: str,
+                             model: str = "jina-reranker-v1-base-en") -> Tuple[List[str], List[str], List[float]]:
+    session = aiohttp.ClientSession()
+    session.headers.update({"Authorization": f"Bearer {api_key}", "Accept-Encoding": "identity"})
+    async with session.post(
+            JINA_API_URL,
+            json={
+                "query": query,
+                "documents": contents,
+                "model": model,
+                "top_n": top_k,
+            },
+    ) as resp:
+        resp_json = await resp.json()
+        if 'results' not in resp_json:
+            raise RuntimeError(f"Invalid response from Jina API: {resp_json['detail']}")
+
+        results = resp_json['results']
+        indices = list(map(lambda x: x['index'], results))
+        score_result = list(map(lambda x: x['relevance_score'], results))
+        id_result = list(map(lambda x: ids[x], indices))
+        content_result = list(map(lambda x: contents[x], indices))
 
-    return list(map(float, results))
+        await session.close()
+        return content_result, id_result, score_result
```

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 
     :param queries: The list of queries to use for reranking
     :param contents_list: The list of lists of contents to rerank
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
     :param batch: The number of queries to be processed in a batch
+        Default is 64.
     :param use_fp16: Whether to use fp16 for inference
     :param model_name: The name of the BAAI Reranker normal-model name.
         Default is "BAAI/bge-reranker-large"
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
+
     model = FlagReranker(
         model_name_or_path=model_name, use_fp16=use_fp16
     )
     nested_list = [list(map(lambda x: [query, x], content_list)) for query, content_list in zip(queries, contents_list)]
     rerank_scores = flatten_apply(flag_embedding_run_model, nested_list, model=model, batch_size=batch)
 
     df = pd.DataFrame({
@@ -51,9 +53,12 @@
 
 def flag_embedding_run_model(input_texts, model, batch_size: int):
     batch_input_texts = make_batch(input_texts, batch_size)
     results = []
     for batch_texts in batch_input_texts:
         with torch.no_grad():
             pred_scores = model.compute_score(sentence_pairs=batch_texts)
-        results.extend(pred_scores)
+        if batch_size == 1:
+            results.append(pred_scores)
+        else:
+            results.extend(pred_scores)
     return results
```

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.1.5/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,21 @@
 
     :param queries: The list of queries to use for reranking
     :param contents_list: The list of lists of contents to rerank
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
     :param batch: The number of queries to be processed in a batch
+        Default is 64.
     :param use_fp16: Whether to use fp16 for inference
     :param model_name: The name of the BAAI Reranker LLM-based-model name.
         Default is "BAAI/bge-reranker-v2-gemma"
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
+
     model = FlagLLMReranker(
         model_name_or_path=model_name, use_fp16=use_fp16
     )
     nested_list = [list(map(lambda x: [query, x], content_list)) for query, content_list in zip(queries, contents_list)]
     rerank_scores = flatten_apply(flag_embedding_run_model, nested_list, model=model, batch_size=batch)
 
     df = pd.DataFrame({
```

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.1.5/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/monot5.py` & `autorag-0.1.5/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.1.5/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.1.5/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/run.py` & `autorag-0.1.5/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.1.5/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.1.5/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.1.5/autorag/nodes/passagereranker/tart/tart.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,20 +59,20 @@
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
     return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
 
 def tart_run_model(input_texts, contents_list, model, batch_size: int, tokenizer, device):
-    batch_input_texts = make_batch(input_texts, batch_size)
-    batch_contents_list = make_batch(contents_list, batch_size)
+    flattened_texts = list(chain.from_iterable(input_texts))
+    flattened_contents = list(chain.from_iterable(contents_list))
+    batch_input_texts = make_batch(flattened_texts, batch_size)
+    batch_contents_list = make_batch(flattened_contents, batch_size)
     results = []
     for batch_texts, batch_contents in zip(batch_input_texts, batch_contents_list):
-        flattened_batch_texts = list(chain.from_iterable(batch_texts))
-        flattened_batch_contents = list(chain.from_iterable(batch_contents))
-        feature = tokenizer(flattened_batch_texts, flattened_batch_contents, padding=True, truncation=True,
+        feature = tokenizer(batch_texts, batch_contents, padding=True, truncation=True,
                             return_tensors="pt").to(device)
         with torch.no_grad():
             pred_scores = model(**feature).logits
             normalized_scores = [float(score[1]) for score in F.softmax(pred_scores, dim=1)]
         results.extend(normalized_scores)
     return results
```

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.1.5/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.1.5/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/passagereranker/upr.py` & `autorag-0.1.5/autorag/nodes/passagereranker/upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/promptmaker/base.py` & `autorag-0.1.5/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/promptmaker/fstring.py` & `autorag-0.1.5/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.1.5/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/promptmaker/run.py` & `autorag-0.1.5/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/queryexpansion/base.py` & `autorag-0.1.5/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.1.5/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.1.5/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/queryexpansion/run.py` & `autorag-0.1.5/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/base.py` & `autorag-0.1.5/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/bm25.py` & `autorag-0.1.5/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.1.5/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.1.5/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.1.5/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.1.5/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/run.py` & `autorag-0.1.5/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/nodes/retrieval/vectordb.py` & `autorag-0.1.5/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/schema/module.py` & `autorag-0.1.5/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/schema/node.py` & `autorag-0.1.5/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/strategy.py` & `autorag-0.1.5/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/autorag/support.py` & `autorag-0.1.5/autorag/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         # retrieval
         'bm25': ('autorag.nodes.retrieval', 'bm25'),
         'vectordb': ('autorag.nodes.retrieval', 'vectordb'),
         'hybrid_rrf': ('autorag.nodes.retrieval', 'hybrid_rrf'),
         'hybrid_cc': ('autorag.nodes.retrieval', 'hybrid_cc'),
         'hybrid_rsf': ('autorag.nodes.retrieval', 'hybrid_rsf'),
         'hybrid_dbsf': ('autorag.nodes.retrieval', 'hybrid_dbsf'),
+        # passage_augmenter
+        'prev_next_augmenter': ('autorag.nodes.passageaugmenter', 'prev_next_augmenter'),
         # passage_reranker
         'monot5': ('autorag.nodes.passagereranker', 'monot5'),
         'tart': ('autorag.nodes.passagereranker', 'tart'),
         'upr': ('autorag.nodes.passagereranker', 'upr'),
         'koreranker': ('autorag.nodes.passagereranker', 'koreranker'),
         'pass_reranker': ('autorag.nodes.passagereranker', 'pass_reranker'),
         'cohere_reranker': ('autorag.nodes.passagereranker', 'cohere_reranker'),
@@ -63,9 +65,10 @@
         'query_expansion': ('autorag.nodes.queryexpansion.run', 'run_query_expansion_node'),
         'retrieval': ('autorag.nodes.retrieval.run', 'run_retrieval_node'),
         'generator': ('autorag.nodes.generator.run', 'run_generator_node'),
         'prompt_maker': ('autorag.nodes.promptmaker.run', 'run_prompt_maker_node'),
         'passage_filter': ('autorag.nodes.passagefilter.run', 'run_passage_filter_node'),
         'passage_compressor': ('autorag.nodes.passagecompressor.run', 'run_passage_compressor_node'),
         'passage_reranker': ('autorag.nodes.passagereranker.run', 'run_passage_reranker_node'),
+        'passage_augmenter': ('autorag.nodes.passageaugmenter.run', 'run_passage_augmenter_node'),
     }
     return dynamically_find_function(node_name, support_nodes)
```

### Comparing `autorag-0.1.4/autorag/utils/preprocess.py` & `autorag-0.1.5/autorag/utils/preprocess.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,8 +65,23 @@
 
     df['metadata'] = df['metadata'].apply(make_datetime_metadata)
 
     # check every metadata have a datetime key
     assert sum(df['metadata'].apply(lambda x: x.get('last_modified_datetime') is not None)) == len(df), \
         "Every metadata must have a datetime key."
 
+    def make_prev_next_id_metadata(x, id_type: str):
+        if x is None or x == {}:
+            return {id_type: None}
+        elif x.get(id_type) is None:
+            return {**x, id_type: None}
+        else:
+            return x
+
+    df['metadata'] = df['metadata'].apply(lambda x: make_prev_next_id_metadata(x, 'prev_id'))
+    df['metadata'] = df['metadata'].apply(lambda x: make_prev_next_id_metadata(x, 'next_id'))
+
+    # check every metadata have a prev_id, next_id key
+    assert all('prev_id' in metadata for metadata in df['metadata']), "Every metadata must have a prev_id key."
+    assert all('next_id' in metadata for metadata in df['metadata']), "Every metadata must have a next_id key."
+
     return df
```

### Comparing `autorag-0.1.4/autorag/utils/util.py` & `autorag-0.1.5/autorag/utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,7 +312,17 @@
     return list(reranked_contents), list(reranked_ids), list(reranked_scores)
 
 
 def select_top_k(df, column_names: List[str], top_k: int):
     for column_name in column_names:
         df[column_name] = df[column_name].apply(lambda x: x[:top_k])
     return df
+
+
+def filter_dict_keys(dict_, keys: List[str]):
+    result = {}
+    for key in keys:
+        if key in dict_:
+            result[key] = dict_[key]
+        else:
+            raise KeyError(f"Key '{key}' not found in dictionary.")
+    return result
```

### Comparing `autorag-0.1.4/autorag/web.py` & `autorag-0.1.5/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/Makefile` & `autorag-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/make.bat` & `autorag-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/data_creation.png` & `autorag-0.1.5/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/data_folder.png` & `autorag-0.1.5/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/node_folder.png` & `autorag-0.1.5/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/node_line_folder.png` & `autorag-0.1.5/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/node_line_summary.png` & `autorag-0.1.5/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/node_lines.png` & `autorag-0.1.5/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/node_summary.png` & `autorag-0.1.5/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/project_folder_example.png` & `autorag-0.1.5/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/project_folders.png` & `autorag-0.1.5/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/resources_folder.png` & `autorag-0.1.5/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.1.5/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.1.5/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/roadmap/cycle.png` & `autorag-0.1.5/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/roadmap/merger.png` & `autorag-0.1.5/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.1.5/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/roadmap/policy.png` & `autorag-0.1.5/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.1.5/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/trial_folder.png` & `autorag-0.1.5/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/trial_json.png` & `autorag-0.1.5/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/trial_summary.png` & `autorag-0.1.5/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/_static/web_interface.png` & `autorag-0.1.5/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagefilter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,22 @@
 -----------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.jina
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passagereranker.just\_lab module
+----------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.just_lab
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passagereranker.koreranker module
 -----------------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.koreranker
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,22 @@
 ------------------------------------------
 
 .. automodule:: autorag.nodes.retrieval.hybrid_rsf
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.retrieval.recursive\_chunk module
+-----------------------------------------------
+
+.. automodule:: autorag.nodes.retrieval.recursive_chunk
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.retrieval.run module
 ----------------------------------
 
 .. automodule:: autorag.nodes.retrieval.run
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.4/docs/source/api_spec/autorag.rst` & `autorag-0.1.5/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/conf.py` & `autorag-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/data_creation/data_format.md` & `autorag-0.1.5/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/data_creation/ragas.md` & `autorag-0.1.5/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/data_creation/tutorial.md` & `autorag-0.1.5/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/deploy/api_endpoint.md` & `autorag-0.1.5/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/deploy/web.md` & `autorag-0.1.5/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/index.rst` & `autorag-0.1.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/install.md` & `autorag-0.1.5/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/local_model.md` & `autorag-0.1.5/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/generator/generator.md` & `autorag-0.1.5/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.1.5/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/generator/vllm.md` & `autorag-0.1.5/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.1.5/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.1.5/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.1.5/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.1.5/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.1.5/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.1.5/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.1.5/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.1.5/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.1.5/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.1.5/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.1.5/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.1.5/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.1.5/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.1.5/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/retrieval/bm25.md` & `autorag-0.1.5/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.1.5/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.1.5/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.1.5/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/optimization/custom_config.md` & `autorag-0.1.5/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/optimization/folder_structure.md` & `autorag-0.1.5/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/optimization/optimization.md` & `autorag-0.1.5/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/optimization/sample_full_config.yaml` & `autorag-0.1.5/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/roadmap/modular_rag.md` & `autorag-0.1.5/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/structure.md` & `autorag-0.1.5/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/troubleshooting.md` & `autorag-0.1.5/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/docs/source/tutorial.md` & `autorag-0.1.5/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/pyproject.toml` & `autorag-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/requirements.txt` & `autorag-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_config/compact_local.yaml` & `autorag-0.1.5/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_config/compact_openai.yaml` & `autorag-0.1.5/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_config/config_korean.yaml` & `autorag-0.1.5/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_config/extracted_sample.yaml` & `autorag-0.1.5/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_config/full.yaml` & `autorag-0.1.5/sample_config/full.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,24 @@
             - (0.7, 0.3)
         - module_type: hybrid_dbsf
           target_modules: ('bm25', 'vectordb')
           weights:
             - (0.5, 0.5)
             - (0.3, 0.7)
             - (0.7, 0.3)
+    - node_type: passage_augmenter
+      strategy:
+        metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+        speed_threshold: 5
+      top_k: 5
+      embedding_model: openai
+      modules:
+        - module_type: pass_passage_augmenter
+        - module_type: prev_next_augmenter
+          mode: next
     - node_type: passage_reranker
       strategy:
         metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
         speed_threshold: 10
       top_k: 5
       modules:
         - module_type: pass_reranker
```

### Comparing `autorag-0.1.4/sample_config/simple_local.yaml` & `autorag-0.1.5/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_config/simple_openai.yaml` & `autorag-0.1.5/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_dataset/README.md` & `autorag-0.1.5/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.1.5/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.1.5/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.1.5/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/data/corpus/test_base.py` & `autorag-0.1.5/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.1.5/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import tempfile
 
 import pytest
 from llama_index.core import Document
-from llama_index.core.schema import TextNode
+from llama_index.core.schema import TextNode, NodeRelationship, RelatedNodeInfo
 
 from autorag.data.corpus import llama_documents_to_parquet, llama_text_node_to_parquet
 from tests.autorag.data.corpus.test_base import validate_corpus
 
 
 @pytest.fixture
 def parquet_filepath():
     with tempfile.NamedTemporaryFile(suffix='.parquet') as temp_file:
         yield temp_file.name
 
 
 def test_llama_documents_to_parquet(parquet_filepath):
-    documents = [Document(text='test text', metadata={'key': 'value'}) for _ in range(5)]
+    documents = [Document(text='test text', metadata={'key': 'value'},
+                          ) for _ in range(5)]
     result_df = llama_documents_to_parquet(documents, parquet_filepath, upsert=True)
     validate_corpus(result_df, 5, parquet_filepath)
 
 
 def test_llama_text_node_to_parquet(parquet_filepath):
-    text_nodes = [TextNode(text='test text', metadata={'key': 'value'}) for _ in range(5)]
+    sample_text_node = TextNode(text='test text',
+                                metadata={'key': 'value'},
+                                relationships={NodeRelationship.PREVIOUS: RelatedNodeInfo(node_id='0'),
+                                               NodeRelationship.NEXT: RelatedNodeInfo(node_id='2')})
+    text_nodes = [sample_text_node for _ in range(5)]
     result_df = llama_text_node_to_parquet(text_nodes, parquet_filepath, upsert=True)
     validate_corpus(result_df, 5, parquet_filepath)
```

### Comparing `autorag-0.1.4/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.1.5/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.1.5/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.1.5/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.1.5/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.1.5/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.1.5/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.1.5/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.1.5/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.1.5/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.1.5/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.1.5/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.1.5/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.1.5/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.1.5/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.1.5/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.1.5/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,11 +8,20 @@
     top_k = 3
     original_cohere_reranker = cohere_reranker.__wrapped__
     contents_result, id_result, score_result \
         = original_cohere_reranker(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
+def test_cohere_reranker_batch_one():
+    top_k = 3
+    batch = 1
+    original_cohere_reranker = cohere_reranker.__wrapped__
+    contents_result, id_result, score_result \
+        = original_cohere_reranker(queries_example, contents_example, scores_example, ids_example, top_k, batch=batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
 def test_cohere_node():
     top_k = 1
     result_df = cohere_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 import pytest
 
-from autorag.nodes.passagereranker import flag_embedding_llm_reranker
+from autorag.nodes.passagereranker import flag_embedding_reranker
 from tests.autorag.nodes.passagereranker.test_passage_reranker_base import queries_example, contents_example, \
     scores_example, ids_example, base_reranker_test, project_dir, previous_result, base_reranker_node_test
 from tests.delete_tests import is_github_action
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_flag_embedding_llm_reranker():
+def test_flag_embedding_reranker():
     top_k = 3
-    original_flag_embedding_llm = flag_embedding_llm_reranker.__wrapped__
+    original_flag_embedding = flag_embedding_reranker.__wrapped__
     contents_result, id_result, score_result \
-        = original_flag_embedding_llm(queries_example, contents_example, scores_example, ids_example, top_k,
-                                      use_fp16=True)
+        = original_flag_embedding(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_flag_embedding_llm_reranker_node():
+def test_flag_embedding_reranker_batch_one():
+    top_k = 3
+    batch = 1
+    original_flag_embedding = flag_embedding_reranker.__wrapped__
+    contents_result, id_result, score_result \
+        = original_flag_embedding(queries_example, contents_example, scores_example, ids_example, top_k, batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_flag_embedding_reranker_batch():
+    top_k = 3
+    batch = 2
+    original_flag_embedding = flag_embedding_reranker.__wrapped__
+    contents_result, id_result, score_result \
+        = original_flag_embedding(queries_example, contents_example, scores_example, ids_example, top_k, batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_flag_embedding_reranker_node():
     top_k = 1
-    result_df = flag_embedding_llm_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
+    result_df = flag_embedding_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,11 +28,20 @@
     top_k = 3
     original_jina_reranker = jina_reranker.__wrapped__
     contents_result, id_result, score_result \
         = original_jina_reranker(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
+def test_jina_reranker_batch_one():
+    top_k = 3
+    batch = 1
+    original_jina_reranker = jina_reranker.__wrapped__
+    contents_result, id_result, score_result \
+        = original_jina_reranker(queries_example, contents_example, scores_example, ids_example, top_k, batch=batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
 def test_jina_reranker_node():
     top_k = 1
     result_df = jina_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,11 +13,21 @@
     original_monot5 = monot5.__wrapped__
     contents_result, id_result, score_result \
         = original_monot5(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_monot5_batch_one():
+    top_k = 1
+    batch = 1
+    original_monot5 = monot5.__wrapped__
+    contents_result, id_result, score_result \
+        = original_monot5(queries_example, contents_example, scores_example, ids_example, top_k, batch=batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
 def test_monot5_node():
     top_k = 1
     result_df = monot5(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,24 @@
     original_rankgpt_reranker = rankgpt.__wrapped__
     contents_result, id_result, score_result \
         = original_rankgpt_reranker(queries_example, contents_example, scores_example, ids_example, top_k,
                                     llm=OpenAI(model="gpt-3.5-turbo-16k"))
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
+def test_rankgpt_reranker_batch_one():
+    top_k = 3
+    batch = 1
+    original_rankgpt_reranker = rankgpt.__wrapped__
+    contents_result, id_result, score_result \
+        = original_rankgpt_reranker(queries_example, contents_example, scores_example, ids_example, top_k,
+                                    llm=OpenAI(model="gpt-3.5-turbo-16k"), batch=batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
 def test_rankgpt_node():
     top_k = 1
     result_df = rankgpt(project_dir=project_dir, previous_result=previous_result, top_k=top_k,
                         llm='openai', model='gpt-3.5-turbo', temperature=0.5, batch=8, verbose=True)
     base_reranker_node_test(result_df, top_k)
 
     top_k = 2
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,11 +12,21 @@
     original_sentence_transformer = sentence_transformer_reranker.__wrapped__
     contents_result, id_result, score_result \
         = original_sentence_transformer(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_sentence_transformer_reranker_batch_one():
+    top_k = 3
+    batch = 1
+    original_sentence_transformer = sentence_transformer_reranker.__wrapped__
+    contents_result, id_result, score_result \
+        = original_sentence_transformer(queries_example, contents_example, scores_example, ids_example, top_k, batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
 def test_sentence_transformer_reranker_node():
     top_k = 1
     result_df = sentence_transformer_reranker(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pytest
 
-from autorag.nodes.passagereranker import tart
+from autorag.nodes.passagereranker import upr
 from tests.autorag.nodes.passagereranker.test_passage_reranker_base import base_reranker_test, queries_example, \
     contents_example, scores_example, ids_example, base_reranker_node_test, project_dir, previous_result
 from tests.delete_tests import is_github_action
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_tart():
+def test_upr():
     top_k = 1
-    original_tart = tart.__wrapped__
+    original_upr = upr.__wrapped__
     contents_result, id_result, score_result \
-        = original_tart(queries_example, contents_example, scores_example, ids_example, top_k)
+        = original_upr(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_tart_node():
+def test_upr_node():
     top_k = 1
-    result_df = tart(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
+    result_df = upr(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.1.5/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import pytest
 
-from autorag.nodes.passagereranker import upr
+from autorag.nodes.passagereranker import tart
 from tests.autorag.nodes.passagereranker.test_passage_reranker_base import base_reranker_test, queries_example, \
     contents_example, scores_example, ids_example, base_reranker_node_test, project_dir, previous_result
 from tests.delete_tests import is_github_action
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_upr():
+def test_tart():
     top_k = 1
-    original_upr = upr.__wrapped__
+    original_tart = tart.__wrapped__
     contents_result, id_result, score_result \
-        = original_upr(queries_example, contents_example, scores_example, ids_example, top_k)
+        = original_tart(queries_example, contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
-def test_upr_node():
+def test_tart_batch_one():
     top_k = 1
-    result_df = upr(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
+    batch = 1
+    original_tart = tart.__wrapped__
+    contents_result, id_result, score_result \
+        = original_tart(queries_example, contents_example, scores_example, ids_example, top_k, batch=batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k)
+
+
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_tart_node():
+    top_k = 1
+    result_df = tart(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k)
```

### Comparing `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.1.5/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.1.5/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.1.5/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/schema/test_module_schema.py` & `autorag-0.1.5/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/schema/test_node_schema.py` & `autorag-0.1.5/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/test_cli.py` & `autorag-0.1.5/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/test_deploy.py` & `autorag-0.1.5/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/test_evaluator.py` & `autorag-0.1.5/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/test_strategy.py` & `autorag-0.1.5/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/test_web.py` & `autorag-0.1.5/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/autorag/utils/test_preprocess.py` & `autorag-0.1.5/tests/autorag/utils/test_preprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 
-import pytest
 import pandas as pd
+import pytest
 
 from autorag.utils import validate_qa_dataset, validate_corpus_dataset, cast_qa_dataset, cast_corpus_dataset
 
 
 @pytest.fixture
 def qa_df():
     return pd.DataFrame({
@@ -18,15 +18,16 @@
 
 # Fixture for corpus dataset
 @pytest.fixture
 def corpus_df():
     return pd.DataFrame({
         'doc_id': ['doc1', 'doc2', 'doc3'],
         'contents': ['content1', 'content2', 'content3'],
-        'metadata': [{}, {'test_key': 'test_value'}, {'last_modified_datetime': datetime(2022, 12, 1, 3, 4, 5)}]
+        'metadata': [{'prev_id': None, 'next_id': 'doc2'}, {'test_key': 'test_value'},
+                     {'last_modified_datetime': datetime(2022, 12, 1, 3, 4, 5)}]
     })
 
 
 # Test validate_qa_dataset
 def test_validate_qa_dataset(qa_df):
     # This should pass as the qa_df fixture contains the required columns
     validate_qa_dataset(qa_df)
@@ -64,9 +65,13 @@
 
 
 # Test cast_corpus_dataset
 def test_cast_corpus_dataset(corpus_df):
     # Cast the dataset and check for a datetime key in metadata
     casted_df = cast_corpus_dataset(corpus_df)
     assert all('last_modified_datetime' in x for x in casted_df['metadata'])
+    assert casted_df['metadata'].iloc[0]['prev_id'] is None
+    assert casted_df['metadata'].iloc[0]['next_id'] == 'doc2'
     assert casted_df['metadata'].iloc[1]['test_key'] == 'test_value'
+    assert casted_df['metadata'].iloc[1]['prev_id'] is None
+    assert casted_df['metadata'].iloc[1]['next_id'] is None
     assert casted_df['metadata'].iloc[2]['last_modified_datetime'] == datetime(2022, 12, 1, 3, 4, 5)
```

### Comparing `autorag-0.1.4/tests/autorag/utils/test_util.py` & `autorag-0.1.5/tests/autorag/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/delete_tests.py` & `autorag-0.1.5/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/mock.py` & `autorag-0.1.5/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/README.md` & `autorag-0.1.5/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/corpus_data_sample.parquet` & `autorag-0.1.5/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.1.5/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.1.5/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.1.5/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/full.yaml` & `autorag-0.1.5/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/qa_data_sample.parquet` & `autorag-0.1.5/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/qa_test_data_sample.parquet` & `autorag-0.1.5/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/config.yaml` & `autorag-0.1.5/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.1.5/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/0/summary.csv` & `autorag-0.1.5/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/config.yaml` & `autorag-0.1.5/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/config.yaml` & `autorag-0.1.5/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.5/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/3/config.yaml` & `autorag-0.1.5/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/best.yaml` & `autorag-0.1.5/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/data/corpus.parquet` & `autorag-0.1.5/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/data/qa.parquet` & `autorag-0.1.5/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.1.5/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.1.5/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.1.5/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/sample_contents_nqa.csv` & `autorag-0.1.5/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.1.5/tests/resources/sample_project/data/corpus.parquet`

 * *Files 8% similar despite different names*

```diff
@@ -6856,141 +6856,352 @@
 0001ac70: b10d 1c15 0419 3500 0610 1928 086d 6574  ......5....(.met
 0001ac80: 6164 6174 6116 6c61 7374 5f6d 6f64 6966  adata.last_modif
 0001ac90: 6965 645f 6461 7465 7469 6d65 1502 163c  ied_datetime...<
 0001aca0: 16b2 0516 e403 26a6 b00d 26f8 ad0d 1c18  ......&...&.....
 0001acb0: 08be 6307 3ed4 0e06 0018 080c 6307 3ed4  ..c.>.......c.>.
 0001acc0: 0e06 0016 0028 08be 6307 3ed4 0e06 0018  .....(..c.>.....
 0001acd0: 080c 6307 3ed4 0e06 0000 192c 1504 1500  ..c.>......,....
-0001ace0: 1502 0015 0015 1015 0200 0000 1504 195c  ...............\
-0001acf0: 3500 1806 7363 6865 6d61 1506 0015 0c25  5...schema.....%
-0001ad00: 0218 0863 6f6e 7465 6e74 7325 004c 1c00  ...contents%.L..
-0001ad10: 0000 150c 2502 1806 646f 635f 6964 2500  ....%...doc_id%.
-0001ad20: 4c1c 0000 0035 0218 086d 6574 6164 6174  L....5...metadat
-0001ad30: 6115 0200 1504 2502 1816 6c61 7374 5f6d  a.....%...last_m
-0001ad40: 6f64 6966 6965 645f 6461 7465 7469 6d65  odified_datetime
-0001ad50: 2514 4c8c 121c 2c00 0000 0000 163c 191c  %.L...,......<..
-0001ad60: 193c 26e0 950d 1c15 0c19 3500 0610 1918  .<&.......5.....
-0001ad70: 0863 6f6e 7465 6e74 7315 0216 3c16 ae95  .contents...<...
-0001ad80: 1516 d895 0d26 fa94 0d26 081c 3600 0019  .....&...&..6...
-0001ad90: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-0001ada0: 0026 e6ab 0d1c 150c 1935 0006 1019 1806  .&.......5......
-0001adb0: 646f 635f 6964 1502 163c 16fa 1416 8815  doc_id...<......
-0001adc0: 26e8 a90d 26de 960d 1c36 0028 2466 6262  &...&....6.($fbb
-0001add0: 3865 3434 342d 6234 3837 2d34 6261 372d  8e444-b487-4ba7-
-0001ade0: 3964 3062 2d37 3562 3234 3366 6436 3636  9d0b-75b243fd666
-0001adf0: 6218 2431 3931 6335 3464 662d 3730 3361  b.$191c54df-703a
-0001ae00: 2d34 3737 642d 3836 6236 2d39 3931 3833  -477d-86b6-99183
-0001ae10: 6632 3534 3739 3900 192c 1504 1500 1502  f254799..,......
-0001ae20: 0015 0015 1015 0200 0000 26dc b10d 1c15  ..........&.....
-0001ae30: 0419 3500 0610 1928 086d 6574 6164 6174  ..5....(.metadat
-0001ae40: 6116 6c61 7374 5f6d 6f64 6966 6965 645f  a.last_modified_
-0001ae50: 6461 7465 7469 6d65 1502 163c 16b2 0516  datetime...<....
-0001ae60: e403 26a6 b00d 26f8 ad0d 1c18 08be 6307  ..&...&.......c.
-0001ae70: 3ed4 0e06 0018 080c 6307 3ed4 0e06 0016  >.......c.>.....
-0001ae80: 0028 08be 6307 3ed4 0e06 0018 080c 6307  .(..c.>.......c.
-0001ae90: 3ed4 0e06 0000 192c 1504 1500 1502 0015  >......,........
-0001aea0: 0015 1015 0200 0000 16da af15 163c 2608  .............<&.
-0001aeb0: 16c4 ae0d 1400 0019 2c18 0670 616e 6461  ........,..panda
-0001aec0: 7318 e203 7b22 696e 6465 785f 636f 6c75  s...{"index_colu
-0001aed0: 6d6e 7322 3a20 5b5d 2c20 2263 6f6c 756d  mns": [], "colum
-0001aee0: 6e5f 696e 6465 7865 7322 3a20 5b5d 2c20  n_indexes": [], 
-0001aef0: 2263 6f6c 756d 6e73 223a 205b 7b22 6e61  "columns": [{"na
-0001af00: 6d65 223a 2022 636f 6e74 656e 7473 222c  me": "contents",
-0001af10: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-0001af20: 636f 6e74 656e 7473 222c 2022 7061 6e64  contents", "pand
-0001af30: 6173 5f74 7970 6522 3a20 2275 6e69 636f  as_type": "unico
-0001af40: 6465 222c 2022 6e75 6d70 795f 7479 7065  de", "numpy_type
-0001af50: 223a 2022 6f62 6a65 6374 222c 2022 6d65  ": "object", "me
-0001af60: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
-0001af70: 7b22 6e61 6d65 223a 2022 646f 635f 6964  {"name": "doc_id
-0001af80: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-0001af90: 2022 646f 635f 6964 222c 2022 7061 6e64   "doc_id", "pand
-0001afa0: 6173 5f74 7970 6522 3a20 2275 6e69 636f  as_type": "unico
-0001afb0: 6465 222c 2022 6e75 6d70 795f 7479 7065  de", "numpy_type
-0001afc0: 223a 2022 6f62 6a65 6374 222c 2022 6d65  ": "object", "me
-0001afd0: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
-0001afe0: 7b22 6e61 6d65 223a 2022 6d65 7461 6461  {"name": "metada
-0001aff0: 7461 222c 2022 6669 656c 645f 6e61 6d65  ta", "field_name
-0001b000: 223a 2022 6d65 7461 6461 7461 222c 2022  ": "metadata", "
-0001b010: 7061 6e64 6173 5f74 7970 6522 3a20 226f  pandas_type": "o
-0001b020: 626a 6563 7422 2c20 226e 756d 7079 5f74  bject", "numpy_t
-0001b030: 7970 6522 3a20 226f 626a 6563 7422 2c20  ype": "object", 
-0001b040: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-0001b050: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
-0001b060: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
-0001b070: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
-0001b080: 2022 3134 2e30 2e32 227d 2c20 2270 616e   "14.0.2"}, "pan
-0001b090: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
-0001b0a0: 2e31 2e34 227d 0018 0c41 5252 4f57 3a73  .1.4"}...ARROW:s
-0001b0b0: 6368 656d 6118 cc08 2f2f 2f2f 2f7a 4144  chema.../////zAD
-0001b0c0: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
-0001b0d0: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
-0001b0e0: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
-0001b0f0: 4141 4145 4141 6741 4367 4141 4142 6743  AAAEAAgACgAAABgC
-0001b100: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
-0001b110: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
-0001b120: 4141 4477 4151 4141 4241 4141 414f 4942  AADwAQAABAAAAOIB
-0001b130: 4141 4237 496d 6c75 5a47 5634 5832 4e76  AAB7ImluZGV4X2Nv
-0001b140: 6248 5674 626e 4d69 4f69 4262 5853 7767  bHVtbnMiOiBbXSwg
-0001b150: 496d 4e76 6248 5674 626c 3970 626d 526c  ImNvbHVtbl9pbmRl
-0001b160: 6547 567a 496a 6f67 5731 3073 4943 4a6a  eGVzIjogW10sICJj
-0001b170: 6232 7831 6257 357a 496a 6f67 5733 7369  b2x1bW5zIjogW3si
-0001b180: 626d 4674 5a53 4936 4943 4a6a 6232 3530  bmFtZSI6ICJjb250
-0001b190: 5a57 3530 6379 4973 4943 4a6d 6157 5673  ZW50cyIsICJmaWVs
-0001b1a0: 5a46 3975 5957 316c 496a 6f67 496d 4e76  ZF9uYW1lIjogImNv
-0001b1b0: 626e 526c 626e 527a 4969 7767 496e 4268  bnRlbnRzIiwgInBh
-0001b1c0: 626d 5268 6331 3930 6558 426c 496a 6f67  bmRhc190eXBlIjog
-0001b1d0: 496e 5675 6157 4e76 5a47 5569 4c43 4169  InVuaWNvZGUiLCAi
-0001b1e0: 626e 5674 6348 6c66 6448 6c77 5a53 4936  bnVtcHlfdHlwZSI6
-0001b1f0: 4943 4a76 596d 706c 5933 5169 4c43 4169  ICJvYmplY3QiLCAi
-0001b200: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
-0001b210: 6457 7873 6653 7767 6579 4a75 5957 316c  dWxsfSwgeyJuYW1l
-0001b220: 496a 6f67 496d 5276 5931 3970 5a43 4973  IjogImRvY19pZCIs
-0001b230: 4943 4a6d 6157 5673 5a46 3975 5957 316c  ICJmaWVsZF9uYW1l
-0001b240: 496a 6f67 496d 5276 5931 3970 5a43 4973  IjogImRvY19pZCIs
-0001b250: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
-0001b260: 5a53 4936 4943 4a31 626d 6c6a 6232 526c  ZSI6ICJ1bmljb2Rl
-0001b270: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
-0001b280: 6347 5569 4f69 4169 6232 4a71 5a57 4e30  cGUiOiAib2JqZWN0
-0001b290: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-0001b2a0: 496a 6f67 626e 5673 6248 3073 4948 7369  IjogbnVsbH0sIHsi
-0001b2b0: 626d 4674 5a53 4936 4943 4a74 5a58 5268  bmFtZSI6ICJtZXRh
-0001b2c0: 5a47 4630 5953 4973 4943 4a6d 6157 5673  ZGF0YSIsICJmaWVs
-0001b2d0: 5a46 3975 5957 316c 496a 6f67 496d 316c  ZF9uYW1lIjogIm1l
-0001b2e0: 6447 466b 5958 5268 4969 7767 496e 4268  dGFkYXRhIiwgInBh
-0001b2f0: 626d 5268 6331 3930 6558 426c 496a 6f67  bmRhc190eXBlIjog
-0001b300: 496d 3969 616d 566a 6443 4973 4943 4a75  Im9iamVjdCIsICJu
-0001b310: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
-0001b320: 496d 3969 616d 566a 6443 4973 4943 4a74  Im9iamVjdCIsICJt
-0001b330: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
-0001b340: 6247 7839 5853 7767 496d 4e79 5a57 4630  bGx9XSwgImNyZWF0
-0001b350: 6233 4969 4f69 4237 496d 7870 596e 4a68  b3IiOiB7ImxpYnJh
-0001b360: 636e 6b69 4f69 4169 6348 6c68 636e 4a76  cnkiOiAicHlhcnJv
-0001b370: 6479 4973 4943 4a32 5a58 4a7a 6157 3975  dyIsICJ2ZXJzaW9u
-0001b380: 496a 6f67 496a 4530 4c6a 4175 4d69 4a39  IjogIjE0LjAuMiJ9
-0001b390: 4c43 4169 6347 4675 5a47 467a 5833 5a6c  LCAicGFuZGFzX3Zl
-0001b3a0: 636e 4e70 6232 3469 4f69 4169 4d69 3478  cnNpb24iOiAiMi4x
-0001b3b0: 4c6a 5169 6651 4141 4267 4141 4148 4268  LjQifQAABgAAAHBh
-0001b3c0: 626d 5268 6377 4141 4177 4141 414c 6741  bmRhcwAAAwAAALgA
-0001b3d0: 4141 4238 4141 4141 4241 4141 4147 542f  AAB8AAAABAAAAGT/
-0001b3e0: 2f2f 3841 4141 454e 4641 4141 4143 4141  //8AAAENFAAAACAA
-0001b3f0: 4141 4145 4141 4141 4151 4141 4142 6741  AAAEAAAAAQAAABgA
-0001b400: 4141 4149 4141 4141 6257 5630 5957 5268  AAAIAAAAbWV0YWRh
-0001b410: 6447 4541 4141 4141 5750 2f2f 2f35 542f  dGEAAAAAWP///5T/
-0001b420: 2f2f 3841 4141 454b 4541 4141 4144 4141  //8AAAEKEAAAADAA
-0001b430: 4141 4145 4141 4141 4141 4141 4142 5941  AAAEAAAAAAAAABYA
-0001b440: 4141 4273 5958 4e30 5832 3176 5a47 6c6d  AABsYXN0X21vZGlm
-0001b450: 6157 566b 5832 5268 6447 5630 6157 316c  aWVkX2RhdGV0aW1l
-0001b460: 4141 4141 4141 5941 4341 4147 4141 5941  AAAAAAYACAAGAAYA
-0001b470: 4141 4141 4141 4941 3250 2f2f 2f77 4141  AAAAAAIA2P///wAA
-0001b480: 4151 5551 4141 4141 4741 4141 4141 5141  AQUQAAAAGAAAAAQA
-0001b490: 4141 4141 4141 4141 4267 4141 4147 5276  AAAAAAAABgAAAGRv
-0001b4a0: 5931 3970 5a41 4141 7850 2f2f 2f78 4141  Y19pZAAAxP///xAA
-0001b4b0: 4641 4149 4141 5941 4277 414d 4141 4141  FAAIAAYABwAMAAAA
-0001b4c0: 4541 4151 4141 4141 4141 4142 4252 4141  EAAQAAAAAAABBRAA
-0001b4d0: 4141 4167 4141 4141 4241 4141 4141 4141  AAAgAAAABAAAAAAA
-0001b4e0: 4141 4149 4141 4141 5932 3975 6447 5675  AAAIAAAAY29udGVu
-0001b4f0: 6448 4d41 4141 4141 4241 4145 4141 5141  dHMAAAAABAAEAAQA
-0001b500: 4141 413d 0018 2070 6172 7175 6574 2d63  AAA=.. parquet-c
-0001b510: 7070 2d61 7272 6f77 2076 6572 7369 6f6e  pp-arrow version
-0001b520: 2031 342e 302e 3219 3c1c 0000 1c00 001c   14.0.2.<.......
-0001b530: 0000 0047 0800 0050 4152 31              ...G...PAR1
+0001ace0: 1502 0015 0015 1015 0200 0000 1504 1590  ................
+0001acf0: 1215 9a12 4c15 3a15 0012 0000 8809 f04f  ....L.:........O
+0001ad00: 2400 0000 6239 6164 3631 3161 2d65 3630  $...b9ad611a-e60
+0001ad10: 362d 3465 3739 2d38 3835 612d 3766 3830  6-4e79-885a-7f80
+0001ad20: 3333 6634 3235 3132 2400 0000 3265 6335  33f42512$...2ec5
+0001ad30: 3131 3231 2d33 3634 302d 3433 6437 2d38  1121-3640-43d7-8
+0001ad40: 3564 622d 3132 3539 6364 6461 6134 6339  5db-1259cddaa4c9
+0001ad50: 0150 f433 0431 3931 6335 3464 662d 3730  .P.3.191c54df-70
+0001ad60: 3361 2d34 3737 642d 3836 6236 2d39 3931  3a-477d-86b6-991
+0001ad70: 3833 6632 3534 3739 3924 0000 0036 6632  83f254799$...6f2
+0001ad80: 3061 6637 302d 3438 6237 2d34 3137 312d  0af70-48b7-4171-
+0001ad90: 6138 6437 2d39 3637 6561 3538 3361 3539  a8d7-967ea583a59
+0001ada0: 3524 0000 0064 6335 6463 3664 352d 6235  5$...dc5dc6d5-b5
+0001adb0: 3366 2d34 6130 382d 3838 3864 2d32 6436  3f-4a08-888d-2d6
+0001adc0: 6535 6338 3563 6634 6224 0000 0037 6264  e5c85cf4b$...7bd
+0001add0: 6237 6465 382d 3633 3532 2d34 3365 352d  b7de8-6352-43e5-
+0001ade0: 6134 3934 2d64 3233 3534 3534 3339 6466  a494-d23545439df
+0001adf0: 3024 0000 0062 6661 3463 3737 612d 3333  0$...bfa4c77a-33
+0001ae00: 3939 2d34 6236 612d 3966 3837 2d37 3233  99-4b6a-9f87-723
+0001ae10: 3932 3835 3139 3739 3824 0000 0036 3961  928519798$...69a
+0001ae20: 3037 6537 302d 3137 3637 2d34 3638 652d  07e70-1767-468e-
+0001ae30: 3965 6231 2d30 3130 6538 6230 6636 3164  9eb1-010e8b0f61d
+0001ae40: 3024 0000 0064 6230 3032 3031 392d 3533  0$...db002019-53
+0001ae50: 6461 2d34 3936 382d 6132 3866 2d31 3061  da-4968-a28f-10a
+0001ae60: 3561 3763 6662 6633 3124 0000 0037 6163  5a7cfbf31$...7ac
+0001ae70: 3332 6535 362d 6236 3539 2d34 3366 322d  32e56-b659-43f2-
+0001ae80: 6131 3861 2d64 3133 3861 3039 3733 6535  a18a-d138a0973e5
+0001ae90: 6624 0000 0038 6238 6330 3135 392d 3965  f$...8b8c0159-9e
+0001aea0: 6666 2d34 3635 632d 3839 3362 2d32 3933  ff-465c-893b-293
+0001aeb0: 3835 6666 3438 3366 3924 0000 0066 6262  85ff483f9$...fbb
+0001aec0: 3865 3434 342d 6234 3837 2d34 6261 372d  8e444-b487-4ba7-
+0001aed0: 3964 3062 2d37 3562 3234 3366 6436 3636  9d0b-75b243fd666
+0001aee0: 6224 0000 0032 6230 3834 3565 372d 3832  b$...2b0845e7-82
+0001aef0: 3136 2d34 3862 612d 6136 3130 2d33 3563  16-48ba-a610-35c
+0001af00: 3830 3166 6435 6135 3824 0000 0034 6133  801fd5a58$...4a3
+0001af10: 6133 6436 662d 3361 6432 2d34 3937 342d  a3d6f-3ad2-4974-
+0001af20: 3930 6639 2d62 3964 6161 6537 3432 3832  90f9-b9daae74282
+0001af30: 3324 0000 0061 6261 3832 3933 642d 3265  3$...aba8293d-2e
+0001af40: 6239 2d34 6133 352d 3862 6461 2d65 3663  b9-4a35-8bda-e6c
+0001af50: 3837 3739 3463 3238 6424 0000 0038 3562  87794c28d$...85b
+0001af60: 3764 6335 362d 6335 6263 2d34 3231 622d  7dc56-c5bc-421b-
+0001af70: 6264 6436 2d63 3932 6637 3339 3961 6637  bdd6-c92f7399af7
+0001af80: 3124 0000 0033 6565 3138 3736 342d 3930  1$...3ee18764-90
+0001af90: 6532 2d34 6564 372d 3837 6535 2d37 3665  e2-4ed7-87e5-76e
+0001afa0: 3966 3931 3736 3465 6524 0000 0033 3232  9f91764ee$...322
+0001afb0: 3037 3837 322d 6465 6535 2d34 3631 332d  07872-dee5-4613-
+0001afc0: 3838 3765 2d62 3734 6662 3563 3336 3435  887e-b74fb5c3645
+0001afd0: 3724 0000 0062 3166 6563 3038 342d 3134  7$...b1fec084-14
+0001afe0: 3435 2d34 3836 342d 6236 3439 2d32 3662  45-4864-b649-26b
+0001aff0: 3464 3161 6133 6636 6524 0000 0035 6566  4d1aa3f6e$...5ef
+0001b000: 6233 6163 382d 3034 6636 2d34 3138 342d  b3ac8-04f6-4184-
+0001b010: 3934 6233 2d36 3163 6263 6530 3830 6538  94b3-61cbce080e8
+0001b020: 3624 0000 0062 3332 3862 6261 652d 6132  6$...b328bbae-a2
+0001b030: 3666 2d34 6632 632d 3938 3061 2d35 6535  6f-4f2c-980a-5e5
+0001b040: 3466 3332 6237 3537 3524 0000 0039 3064  4f32b7575$...90d
+0001b050: 6264 3635 312d 6631 3663 2d34 3839 352d  bd651-f16c-4895-
+0001b060: 3861 3364 2d62 3664 3732 3135 6530 6563  8a3d-b6d7215e0ec
+0001b070: 6524 0000 0032 6439 3434 6239 352d 3739  e$...2d944b95-79
+0001b080: 6333 2d34 6262 622d 6136 3033 2d30 6532  c3-4bbb-a603-0e2
+0001b090: 3461 3237 6464 6461 3524 0000 0062 6137  4a27ddda5$...ba7
+0001b0a0: 3033 3262 662d 6665 3965 2d34 3061 612d  032bf-fe9e-40aa-
+0001b0b0: 6132 3037 2d37 6132 3131 6438 3137 3330  a207-7a211d81730
+0001b0c0: 3924 0000 0035 3033 6532 3566 652d 6664  9$...503e25fe-fd
+0001b0d0: 3039 2d34 3666 652d 3931 3838 2d66 3036  09-46fe-9188-f06
+0001b0e0: 3563 3430 3636 3238 6524 0000 0065 6566  5c406628e$...eef
+0001b0f0: 3966 3137 612d 6138 3532 2d34 3630 302d  9f17a-a852-4600-
+0001b100: 3961 6235 2d34 6266 6263 6131 3763 3732  9ab5-4bfbca17c72
+0001b110: 3824 0000 0035 3638 3662 3462 372d 3138  8$...5686b4b7-18
+0001b120: 3730 2d34 3437 312d 6237 6662 2d66 6462  70-4471-b7fb-fdb
+0001b130: 6633 3166 3361 6637 3424 0000 0039 3966  f31f3af74$...99f
+0001b140: 3065 3664 662d 3366 3033 2d34 6264 622d  0e6df-3f03-4bdb-
+0001b150: 6261 3234 2d38 6633 3837 6137 3833 6335  ba24-8f387a783c5
+0001b160: 3524 0000 0031 3935 3063 3565 362d 6565  5$...1950c5e6-ee
+0001b170: 3533 2d34 6230 662d 3962 3332 2d65 3031  53-4b0f-9b32-e01
+0001b180: 6439 3164 3663 6539 6315 0015 3c15 402c  d91d6ce9c...<.@,
+0001b190: 153c 1510 1506 1506 1c36 0228 2466 6262  .<.......6.($fbb
+0001b1a0: 3865 3434 342d 6234 3837 2d34 6261 372d  8e444-b487-4ba7-
+0001b1b0: 3964 3062 2d37 3562 3234 3366 6436 3636  9d0b-75b243fd666
+0001b1c0: 6218 2431 3931 6335 3464 662d 3730 3361  b.$191c54df-703a
+0001b1d0: 2d34 3737 642d 3836 6236 2d39 3931 3833  -477d-86b6-99183
+0001b1e0: 6632 3534 3739 3900 0000 1e74 0400 0000  f254799....t....
+0001b1f0: 3a02 0201 0509 2088 418a 3928 a9c5 9a7b  :..... .A.9(...{
+0001b200: 30ca 49ab bd38 ebcd 0100 2694 c80d 1c15  0.I..8....&.....
+0001b210: 0c19 3500 0610 1928 086d 6574 6164 6174  ..5....(.metadat
+0001b220: 6107 6e65 7874 5f69 6415 0216 3c16 ae14  a.next_id...<...
+0001b230: 16bc 1426 92c6 0d26 d8b3 0d1c 3602 2824  ...&...&....6.($
+0001b240: 6662 6238 6534 3434 2d62 3438 372d 3462  fbb8e444-b487-4b
+0001b250: 6137 2d39 6430 622d 3735 6232 3433 6664  a7-9d0b-75b243fd
+0001b260: 3636 3662 1824 3139 3163 3534 6466 2d37  666b.$191c54df-7
+0001b270: 3033 612d 3437 3764 2d38 3662 362d 3939  03a-477d-86b6-99
+0001b280: 3138 3366 3235 3437 3939 0019 2c15 0415  183f254799..,...
+0001b290: 0015 0200 1500 1510 1502 0000 0015 0415  ................
+0001b2a0: 9012 159a 124c 153a 1500 1200 0088 09f0  .....L.:........
+0001b2b0: 4f24 0000 0035 6239 3537 3739 312d 3363  O$...5b957791-3c
+0001b2c0: 3762 2d34 6632 392d 6134 3130 2d38 6430  7b-4f29-a410-8d0
+0001b2d0: 3035 6135 3338 3835 3524 0000 0062 3961  05a538855$...b9a
+0001b2e0: 6436 3131 612d 6536 3036 2d34 6537 392d  d611a-e606-4e79-
+0001b2f0: 3838 3561 2d37 6638 3033 3366 3432 3531  885a-7f8033f4251
+0001b300: 3201 50f4 3304 3265 6335 3131 3231 2d33  2.P.3.2ec51121-3
+0001b310: 3634 302d 3433 6437 2d38 3564 622d 3132  640-43d7-85db-12
+0001b320: 3539 6364 6461 6134 6339 2400 0000 3139  59cddaa4c9$...19
+0001b330: 3163 3534 6466 2d37 3033 612d 3437 3764  1c54df-703a-477d
+0001b340: 2d38 3662 362d 3939 3138 3366 3235 3437  -86b6-99183f2547
+0001b350: 3939 2400 0000 3666 3230 6166 3730 2d34  99$...6f20af70-4
+0001b360: 3862 372d 3431 3731 2d61 3864 372d 3936  8b7-4171-a8d7-96
+0001b370: 3765 6135 3833 6135 3935 2400 0000 6463  7ea583a595$...dc
+0001b380: 3564 6336 6435 2d62 3533 662d 3461 3038  5dc6d5-b53f-4a08
+0001b390: 2d38 3838 642d 3264 3665 3563 3835 6366  -888d-2d6e5c85cf
+0001b3a0: 3462 2400 0000 3762 6462 3764 6538 2d36  4b$...7bdb7de8-6
+0001b3b0: 3335 322d 3433 6535 2d61 3439 342d 6432  352-43e5-a494-d2
+0001b3c0: 3335 3435 3433 3964 6630 2400 0000 6266  3545439df0$...bf
+0001b3d0: 6134 6337 3761 2d33 3339 392d 3462 3661  a4c77a-3399-4b6a
+0001b3e0: 2d39 6638 372d 3732 3339 3238 3531 3937  -9f87-7239285197
+0001b3f0: 3938 2400 0000 3639 6130 3765 3730 2d31  98$...69a07e70-1
+0001b400: 3736 372d 3436 3865 2d39 6562 312d 3031  767-468e-9eb1-01
+0001b410: 3065 3862 3066 3631 6430 2400 0000 6462  0e8b0f61d0$...db
+0001b420: 3030 3230 3139 2d35 3364 612d 3439 3638  002019-53da-4968
+0001b430: 2d61 3238 662d 3130 6135 6137 6366 6266  -a28f-10a5a7cfbf
+0001b440: 3331 2400 0000 3761 6333 3265 3536 2d62  31$...7ac32e56-b
+0001b450: 3635 392d 3433 6632 2d61 3138 612d 6431  659-43f2-a18a-d1
+0001b460: 3338 6130 3937 3365 3566 2400 0000 3862  38a0973e5f$...8b
+0001b470: 3863 3031 3539 2d39 6566 662d 3436 3563  8c0159-9eff-465c
+0001b480: 2d38 3933 622d 3239 3338 3566 6634 3833  -893b-29385ff483
+0001b490: 6639 2400 0000 6662 6238 6534 3434 2d62  f9$...fbb8e444-b
+0001b4a0: 3438 372d 3462 6137 2d39 6430 622d 3735  487-4ba7-9d0b-75
+0001b4b0: 6232 3433 6664 3636 3662 2400 0000 3262  b243fd666b$...2b
+0001b4c0: 3038 3435 6537 2d38 3231 362d 3438 6261  0845e7-8216-48ba
+0001b4d0: 2d61 3631 302d 3335 6338 3031 6664 3561  -a610-35c801fd5a
+0001b4e0: 3538 2400 0000 3461 3361 3364 3666 2d33  58$...4a3a3d6f-3
+0001b4f0: 6164 322d 3439 3734 2d39 3066 392d 6239  ad2-4974-90f9-b9
+0001b500: 6461 6165 3734 3238 3233 2400 0000 6162  daae742823$...ab
+0001b510: 6138 3239 3364 2d32 6562 392d 3461 3335  a8293d-2eb9-4a35
+0001b520: 2d38 6264 612d 6536 6338 3737 3934 6332  -8bda-e6c87794c2
+0001b530: 3864 2400 0000 3835 6237 6463 3536 2d63  8d$...85b7dc56-c
+0001b540: 3562 632d 3432 3162 2d62 6464 362d 6339  5bc-421b-bdd6-c9
+0001b550: 3266 3733 3939 6166 3731 2400 0000 3365  2f7399af71$...3e
+0001b560: 6531 3837 3634 2d39 3065 322d 3465 6437  e18764-90e2-4ed7
+0001b570: 2d38 3765 352d 3736 6539 6639 3137 3634  -87e5-76e9f91764
+0001b580: 6565 2400 0000 3332 3230 3738 3732 2d64  ee$...32207872-d
+0001b590: 6565 352d 3436 3133 2d38 3837 652d 6237  ee5-4613-887e-b7
+0001b5a0: 3466 6235 6333 3634 3537 2400 0000 6231  4fb5c36457$...b1
+0001b5b0: 6665 6330 3834 2d31 3434 352d 3438 3634  fec084-1445-4864
+0001b5c0: 2d62 3634 392d 3236 6234 6431 6161 3366  -b649-26b4d1aa3f
+0001b5d0: 3665 2400 0000 3565 6662 3361 6338 2d30  6e$...5efb3ac8-0
+0001b5e0: 3466 362d 3431 3834 2d39 3462 332d 3631  4f6-4184-94b3-61
+0001b5f0: 6362 6365 3038 3065 3836 2400 0000 6233  cbce080e86$...b3
+0001b600: 3238 6262 6165 2d61 3236 662d 3466 3263  28bbae-a26f-4f2c
+0001b610: 2d39 3830 612d 3565 3534 6633 3262 3735  -980a-5e54f32b75
+0001b620: 3735 2400 0000 3930 6462 6436 3531 2d66  75$...90dbd651-f
+0001b630: 3136 632d 3438 3935 2d38 6133 642d 6236  16c-4895-8a3d-b6
+0001b640: 6437 3231 3565 3065 6365 2400 0000 3264  d7215e0ece$...2d
+0001b650: 3934 3462 3935 2d37 3963 332d 3462 6262  944b95-79c3-4bbb
+0001b660: 2d61 3630 332d 3065 3234 6132 3764 6464  -a603-0e24a27ddd
+0001b670: 6135 2400 0000 6261 3730 3332 6266 2d66  a5$...ba7032bf-f
+0001b680: 6539 652d 3430 6161 2d61 3230 372d 3761  e9e-40aa-a207-7a
+0001b690: 3231 3164 3831 3733 3039 2400 0000 3530  211d817309$...50
+0001b6a0: 3365 3235 6665 2d66 6430 392d 3436 6665  3e25fe-fd09-46fe
+0001b6b0: 2d39 3138 382d 6630 3635 6334 3036 3632  -9188-f065c40662
+0001b6c0: 3865 2400 0000 6565 6639 6631 3761 2d61  8e$...eef9f17a-a
+0001b6d0: 3835 322d 3436 3030 2d39 6162 352d 3462  852-4600-9ab5-4b
+0001b6e0: 6662 6361 3137 6337 3238 2400 0000 3536  fbca17c728$...56
+0001b6f0: 3836 6234 6237 2d31 3837 302d 3434 3731  86b4b7-1870-4471
+0001b700: 2d62 3766 622d 6664 6266 3331 6633 6166  -b7fb-fdbf31f3af
+0001b710: 3734 2400 0000 3939 6630 6536 6466 2d33  74$...99f0e6df-3
+0001b720: 6630 332d 3462 6462 2d62 6132 342d 3866  f03-4bdb-ba24-8f
+0001b730: 3338 3761 3738 3363 3535 1500 153e 1542  387a783c55...>.B
+0001b740: 2c15 3c15 1015 0615 061c 3602 2824 6662  ,.<.......6.($fb
+0001b750: 6238 6534 3434 2d62 3438 372d 3462 6137  b8e444-b487-4ba7
+0001b760: 2d39 6430 622d 3735 6232 3433 6664 3636  -9d0b-75b243fd66
+0001b770: 3662 1824 3139 3163 3534 6466 2d37 3033  6b.$191c54df-703
+0001b780: 612d 3437 3764 2d38 3662 362d 3939 3138  a-477d-86b6-9918
+0001b790: 3366 3235 3437 3939 0000 001f 7805 0000  3f254799....x...
+0001b7a0: 0003 a9aa 2c02 0509 2088 418a 3928 a9c5  ....,... .A.9(..
+0001b7b0: 9a7b 30ca 49ab bd38 ebcd 0100 26f8 de0d  .{0.I..8....&...
+0001b7c0: 1c15 0c19 3500 0610 1928 086d 6574 6164  ....5....(.metad
+0001b7d0: 6174 6107 7072 6576 5f69 6415 0216 3c16  ata.prev_id...<.
+0001b7e0: b014 16be 1426 f4dc 0d26 baca 0d1c 3602  .....&...&....6.
+0001b7f0: 2824 6662 6238 6534 3434 2d62 3438 372d  ($fbb8e444-b487-
+0001b800: 3462 6137 2d39 6430 622d 3735 6232 3433  4ba7-9d0b-75b243
+0001b810: 6664 3636 3662 1824 3139 3163 3534 6466  fd666b.$191c54df
+0001b820: 2d37 3033 612d 3437 3764 2d38 3662 362d  -703a-477d-86b6-
+0001b830: 3939 3138 3366 3235 3437 3939 0019 2c15  99183f254799..,.
+0001b840: 0415 0015 0200 1500 1510 1502 0000 0015  ................
+0001b850: 0419 7c35 0018 0673 6368 656d 6115 0600  ..|5...schema...
+0001b860: 150c 2502 1808 636f 6e74 656e 7473 2500  ..%...contents%.
+0001b870: 4c1c 0000 0015 0c25 0218 0664 6f63 5f69  L......%...doc_i
+0001b880: 6425 004c 1c00 0000 3502 1808 6d65 7461  d%.L....5...meta
+0001b890: 6461 7461 1506 0015 0425 0218 166c 6173  data.....%...las
+0001b8a0: 745f 6d6f 6469 6669 6564 5f64 6174 6574  t_modified_datet
+0001b8b0: 696d 6525 144c 8c12 1c2c 0000 0000 0015  ime%.L...,......
+0001b8c0: 0c25 0218 076e 6578 745f 6964 2500 4c1c  .%...next_id%.L.
+0001b8d0: 0000 0015 0c25 0218 0770 7265 765f 6964  .....%...prev_id
+0001b8e0: 2500 4c1c 0000 0016 3c19 1c19 5c26 e095  %.L.....<...\&..
+0001b8f0: 0d1c 150c 1935 0006 1019 1808 636f 6e74  .....5......cont
+0001b900: 656e 7473 1502 163c 16ae 9515 16d8 950d  ents...<........
+0001b910: 26fa 940d 2608 1c36 0000 192c 1504 1500  &...&..6...,....
+0001b920: 1502 0015 0015 1015 0200 0000 26e6 ab0d  ............&...
+0001b930: 1c15 0c19 3500 0610 1918 0664 6f63 5f69  ....5......doc_i
+0001b940: 6415 0216 3c16 fa14 1688 1526 e8a9 0d26  d...<......&...&
+0001b950: de96 0d1c 3600 2824 6662 6238 6534 3434  ....6.($fbb8e444
+0001b960: 2d62 3438 372d 3462 6137 2d39 6430 622d  -b487-4ba7-9d0b-
+0001b970: 3735 6232 3433 6664 3636 3662 1824 3139  75b243fd666b.$19
+0001b980: 3163 3534 6466 2d37 3033 612d 3437 3764  1c54df-703a-477d
+0001b990: 2d38 3662 362d 3939 3138 3366 3235 3437  -86b6-99183f2547
+0001b9a0: 3939 0019 2c15 0415 0015 0200 1500 1510  99..,...........
+0001b9b0: 1502 0000 0026 dcb1 0d1c 1504 1935 0006  .....&.......5..
+0001b9c0: 1019 2808 6d65 7461 6461 7461 166c 6173  ..(.metadata.las
+0001b9d0: 745f 6d6f 6469 6669 6564 5f64 6174 6574  t_modified_datet
+0001b9e0: 696d 6515 0216 3c16 b205 16e4 0326 a6b0  ime...<......&..
+0001b9f0: 0d26 f8ad 0d1c 1808 be63 073e d40e 0600  .&.......c.>....
+0001ba00: 1808 0c63 073e d40e 0600 1600 2808 be63  ...c.>......(..c
+0001ba10: 073e d40e 0600 1808 0c63 073e d40e 0600  .>.......c.>....
+0001ba20: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+0001ba30: 0000 0026 94c8 0d1c 150c 1935 0006 1019  ...&.......5....
+0001ba40: 2808 6d65 7461 6461 7461 076e 6578 745f  (.metadata.next_
+0001ba50: 6964 1502 163c 16ae 1416 bc14 2692 c60d  id...<......&...
+0001ba60: 26d8 b30d 1c36 0228 2466 6262 3865 3434  &....6.($fbb8e44
+0001ba70: 342d 6234 3837 2d34 6261 372d 3964 3062  4-b487-4ba7-9d0b
+0001ba80: 2d37 3562 3234 3366 6436 3636 6218 2431  -75b243fd666b.$1
+0001ba90: 3931 6335 3464 662d 3730 3361 2d34 3737  91c54df-703a-477
+0001baa0: 642d 3836 6236 2d39 3931 3833 6632 3534  d-86b6-99183f254
+0001bab0: 3739 3900 192c 1504 1500 1502 0015 0015  799..,..........
+0001bac0: 1015 0200 0000 26f8 de0d 1c15 0c19 3500  ......&.......5.
+0001bad0: 0610 1928 086d 6574 6164 6174 6107 7072  ...(.metadata.pr
+0001bae0: 6576 5f69 6415 0216 3c16 b014 16be 1426  ev_id...<......&
+0001baf0: f4dc 0d26 baca 0d1c 3602 2824 6662 6238  ...&....6.($fbb8
+0001bb00: 6534 3434 2d62 3438 372d 3462 6137 2d39  e444-b487-4ba7-9
+0001bb10: 6430 622d 3735 6232 3433 6664 3636 3662  d0b-75b243fd666b
+0001bb20: 1824 3139 3163 3534 6466 2d37 3033 612d  .$191c54df-703a-
+0001bb30: 3437 3764 2d38 3662 362d 3939 3138 3366  477d-86b6-99183f
+0001bb40: 3235 3437 3939 0019 2c15 0415 0015 0200  254799..,.......
+0001bb50: 1500 1510 1502 0000 0016 b8d8 1516 3c26  ..............<&
+0001bb60: 0816 bed7 0d14 0000 192c 1806 7061 6e64  .........,..pand
+0001bb70: 6173 18e2 037b 2269 6e64 6578 5f63 6f6c  as...{"index_col
+0001bb80: 756d 6e73 223a 205b 5d2c 2022 636f 6c75  umns": [], "colu
+0001bb90: 6d6e 5f69 6e64 6578 6573 223a 205b 5d2c  mn_indexes": [],
+0001bba0: 2022 636f 6c75 6d6e 7322 3a20 5b7b 226e   "columns": [{"n
+0001bbb0: 616d 6522 3a20 2263 6f6e 7465 6e74 7322  ame": "contents"
+0001bbc0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+0001bbd0: 2263 6f6e 7465 6e74 7322 2c20 2270 616e  "contents", "pan
+0001bbe0: 6461 735f 7479 7065 223a 2022 756e 6963  das_type": "unic
+0001bbf0: 6f64 6522 2c20 226e 756d 7079 5f74 7970  ode", "numpy_typ
+0001bc00: 6522 3a20 226f 626a 6563 7422 2c20 226d  e": "object", "m
+0001bc10: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+0001bc20: 207b 226e 616d 6522 3a20 2264 6f63 5f69   {"name": "doc_i
+0001bc30: 6422 2c20 2266 6965 6c64 5f6e 616d 6522  d", "field_name"
+0001bc40: 3a20 2264 6f63 5f69 6422 2c20 2270 616e  : "doc_id", "pan
+0001bc50: 6461 735f 7479 7065 223a 2022 756e 6963  das_type": "unic
+0001bc60: 6f64 6522 2c20 226e 756d 7079 5f74 7970  ode", "numpy_typ
+0001bc70: 6522 3a20 226f 626a 6563 7422 2c20 226d  e": "object", "m
+0001bc80: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+0001bc90: 207b 226e 616d 6522 3a20 226d 6574 6164   {"name": "metad
+0001bca0: 6174 6122 2c20 2266 6965 6c64 5f6e 616d  ata", "field_nam
+0001bcb0: 6522 3a20 226d 6574 6164 6174 6122 2c20  e": "metadata", 
+0001bcc0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
+0001bcd0: 6f62 6a65 6374 222c 2022 6e75 6d70 795f  object", "numpy_
+0001bce0: 7479 7065 223a 2022 6f62 6a65 6374 222c  type": "object",
+0001bcf0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+0001bd00: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
+0001bd10: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
+0001bd20: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
+0001bd30: 3a20 2231 352e 302e 3022 7d2c 2022 7061  : "15.0.0"}, "pa
+0001bd40: 6e64 6173 5f76 6572 7369 6f6e 223a 2022  ndas_version": "
+0001bd50: 322e 322e 3022 7d00 180c 4152 524f 573a  2.2.0"}...ARROW:
+0001bd60: 7363 6865 6d61 18c0 092f 2f2f 2f2f 3467  schema.../////4g
+0001bd70: 4441 4141 5141 4141 4141 4141 4b41 4134  DAAAQAAAAAAAKAA4
+0001bd80: 4142 6741 4641 4167 4143 6741 4141 4141  ABgAFAAgACgAAAAA
+0001bd90: 4242 4141 5141 4141 4141 4141 4b41 4177  BBAAQAAAAAAAKAAw
+0001bda0: 4141 4141 4541 4167 4143 6741 4141 4267  AAAAEAAgACgAAABg
+0001bdb0: 4341 4141 4541 4141 4141 5141 4141 4177  CAAAEAAAAAQAAAAw
+0001bdc0: 4141 4141 4941 4177 4142 4141 4941 4167  AAAAIAAwABAAIAAg
+0001bdd0: 4141 4144 7741 5141 4142 4141 4141 4f49  AAADwAQAABAAAAOI
+0001bde0: 4241 4142 3749 6d6c 755a 4756 3458 324e  BAAB7ImluZGV4X2N
+0001bdf0: 7662 4856 7462 6e4d 694f 6942 6258 5377  vbHVtbnMiOiBbXSw
+0001be00: 6749 6d4e 7662 4856 7462 6c39 7062 6d52  gImNvbHVtbl9pbmR
+0001be10: 6c65 4756 7a49 6a6f 6757 3130 7349 434a  leGVzIjogW10sICJ
+0001be20: 6a62 3278 3162 5735 7a49 6a6f 6757 3373  jb2x1bW5zIjogW3s
+0001be30: 6962 6d46 745a 5349 3649 434a 6a62 3235  ibmFtZSI6ICJjb25
+0001be40: 305a 5735 3063 7949 7349 434a 6d61 5756  0ZW50cyIsICJmaWV
+0001be50: 735a 4639 7559 5731 6c49 6a6f 6749 6d4e  sZF9uYW1lIjogImN
+0001be60: 7662 6e52 6c62 6e52 7a49 6977 6749 6e42  vbnRlbnRzIiwgInB
+0001be70: 6862 6d52 6863 3139 3065 5842 6c49 6a6f  hbmRhc190eXBlIjo
+0001be80: 6749 6e56 7561 574e 765a 4755 694c 4341  gInVuaWNvZGUiLCA
+0001be90: 6962 6e56 7463 486c 6664 486c 775a 5349  ibnVtcHlfdHlwZSI
+0001bea0: 3649 434a 7659 6d70 6c59 3351 694c 4341  6ICJvYmplY3QiLCA
+0001beb0: 6962 5756 3059 5752 6864 4745 694f 6942  ibWV0YWRhdGEiOiB
+0001bec0: 7564 5778 7366 5377 6765 794a 7559 5731  udWxsfSwgeyJuYW1
+0001bed0: 6c49 6a6f 6749 6d52 7659 3139 705a 4349  lIjogImRvY19pZCI
+0001bee0: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
+0001bef0: 6c49 6a6f 6749 6d52 7659 3139 705a 4349  lIjogImRvY19pZCI
+0001bf00: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
+0001bf10: 775a 5349 3649 434a 3162 6d6c 6a62 3252  wZSI6ICJ1bmljb2R
+0001bf20: 6c49 6977 6749 6d35 3162 5842 3558 3352  lIiwgIm51bXB5X3R
+0001bf30: 3563 4755 694f 6941 6962 324a 715a 574e  5cGUiOiAib2JqZWN
+0001bf40: 3049 6977 6749 6d31 6c64 4746 6b59 5852  0IiwgIm1ldGFkYXR
+0001bf50: 6849 6a6f 6762 6e56 7362 4830 7349 4873  hIjogbnVsbH0sIHs
+0001bf60: 6962 6d46 745a 5349 3649 434a 745a 5852  ibmFtZSI6ICJtZXR
+0001bf70: 685a 4746 3059 5349 7349 434a 6d61 5756  hZGF0YSIsICJmaWV
+0001bf80: 735a 4639 7559 5731 6c49 6a6f 6749 6d31  sZF9uYW1lIjogIm1
+0001bf90: 6c64 4746 6b59 5852 6849 6977 6749 6e42  ldGFkYXRhIiwgInB
+0001bfa0: 6862 6d52 6863 3139 3065 5842 6c49 6a6f  hbmRhc190eXBlIjo
+0001bfb0: 6749 6d39 6961 6d56 6a64 4349 7349 434a  gIm9iamVjdCIsICJ
+0001bfc0: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
+0001bfd0: 6749 6d39 6961 6d56 6a64 4349 7349 434a  gIm9iamVjdCIsICJ
+0001bfe0: 745a 5852 685a 4746 3059 5349 3649 4735  tZXRhZGF0YSI6IG5
+0001bff0: 3162 4778 3958 5377 6749 6d4e 795a 5746  1bGx9XSwgImNyZWF
+0001c000: 3062 3349 694f 6942 3749 6d78 7059 6e4a  0b3IiOiB7ImxpYnJ
+0001c010: 6863 6e6b 694f 6941 6963 486c 6863 6e4a  hcnkiOiAicHlhcnJ
+0001c020: 7664 7949 7349 434a 325a 584a 7a61 5739  vdyIsICJ2ZXJzaW9
+0001c030: 7549 6a6f 6749 6a45 314c 6a41 754d 434a  uIjogIjE1LjAuMCJ
+0001c040: 394c 4341 6963 4746 755a 4746 7a58 335a  9LCAicGFuZGFzX3Z
+0001c050: 6c63 6e4e 7062 3234 694f 6941 694d 6934  lcnNpb24iOiAiMi4
+0001c060: 794c 6a41 6966 5141 4142 6741 4141 4842  yLjAifQAABgAAAHB
+0001c070: 6862 6d52 6863 7741 4141 7741 4141 4241  hbmRhcwAAAwAAABA
+0001c080: 4241 4144 5541 4141 4142 4141 4141 417a  BAADUAAAABAAAAAz
+0001c090: 2f2f 2f38 4141 4145 4e48 4141 4141 4367  ///8AAAENHAAAACg
+0001c0a0: 4141 4141 4541 4141 4141 7741 4141 4841  AAAAEAAAAAwAAAHA
+0001c0b0: 4141 4142 4541 4141 4147 4141 4141 4167  AAABEAAAAGAAAAAg
+0001c0c0: 4141 4142 745a 5852 685a 4746 3059 5141  AAABtZXRhZGF0YQA
+0001c0d0: 4141 4141 492f 2f2f 2f52 502f 2f2f 7741  AAAAI////RP///wA
+0001c0e0: 4141 5155 5141 4141 4147 4141 4141 4151  AAQUQAAAAGAAAAAQ
+0001c0f0: 4141 4141 4141 4141 4142 7741 4141 4842  AAAAAAAAABwAAAHB
+0001c100: 795a 585a 6661 5751 414d 502f 2f2f 327a  yZXZfaWQAMP///2z
+0001c110: 2f2f 2f38 4141 4145 4645 4141 4141 4267  ///8AAAEFEAAAABg
+0001c120: 4141 4141 4541 4141 4141 4141 4141 4163  AAAAEAAAAAAAAAAc
+0001c130: 4141 4142 755a 5868 3058 326c 6b41 466a  AAABuZXh0X2lkAFj
+0001c140: 2f2f 2f2b 552f 2f2f 2f41 4141 4243 6841  ///+U////AAABChA
+0001c150: 4141 4141 7741 4141 4142 4141 4141 4141  AAAAwAAAABAAAAAA
+0001c160: 4141 4141 5741 4141 4162 4746 7a64 4639  AAAAWAAAAbGFzdF9
+0001c170: 7462 3252 705a 6d6c 6c5a 4639 6b59 5852  tb2RpZmllZF9kYXR
+0001c180: 6c64 476c 745a 5141 4141 4141 4741 4167  ldGltZQAAAAAGAAg
+0001c190: 4142 6741 4741 4141 4141 4141 4341 4e6a  ABgAGAAAAAAACANj
+0001c1a0: 2f2f 2f38 4141 4145 4645 4141 4141 4267  ///8AAAEFEAAAABg
+0001c1b0: 4141 4141 4541 4141 4141 4141 4141 4159  AAAAEAAAAAAAAAAY
+0001c1c0: 4141 4142 6b62 324e 6661 5751 4141 4d54  AAABkb2NfaWQAAMT
+0001c1d0: 2f2f 2f38 5141 4251 4143 4141 4741 4163  ///8QABQACAAGAAc
+0001c1e0: 4144 4141 4141 4241 4145 4141 4141 4141  ADAAAABAAEAAAAAA
+0001c1f0: 4141 5155 5141 4141 4149 4141 4141 4151  AAQUQAAAAIAAAAAQ
+0001c200: 4141 4141 4141 4141 4143 4141 4141 474e  AAAAAAAAACAAAAGN
+0001c210: 7662 6e52 6c62 6e52 7a41 4141 4141 4151  vbnRlbnRzAAAAAAQ
+0001c220: 4142 4141 4541 4141 4100 1820 7061 7271  ABAAEAAAA.. parq
+0001c230: 7565 742d 6370 702d 6172 726f 7720 7665  uet-cpp-arrow ve
+0001c240: 7273 696f 6e20 3135 2e30 2e30 195c 1c00  rsion 15.0.0.\..
+0001c250: 001c 0000 1c00 001c 0000 1c00 0000 0f0a  ................
+0001c260: 0000 5041 5231                           ..PAR1
```

### Comparing `autorag-0.1.4/tests/resources/sample_project/data/qa.parquet` & `autorag-0.1.5/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/sample_project/resources/bm25.pkl` & `autorag-0.1.5/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/simple.yaml` & `autorag-0.1.5/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.4/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.1.5/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*


# Comparing `tmp/swarmauri-0.1.80.tar.gz` & `tmp/swarmauri-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmauri-0.1.80.tar", last modified: Wed Apr 24 03:29:09 2024, max compression
+gzip compressed data, was "swarmauri-0.1.9.tar", last modified: Thu Mar  7 03:38:55 2024, max compression
```

## Comparing `swarmauri-0.1.80.tar` & `swarmauri-0.1.9.tar`

### file list

```diff
@@ -1,486 +1,405 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.153468 swarmauri-0.1.80/
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-24 03:29:09.153468 swarmauri-0.1.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-24 03:28:49.000000 swarmauri-0.1.80/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:29:09.153468 swarmauri-0.1.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-24 03:28:49.000000 swarmauri-0.1.80/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.077468 swarmauri-0.1.80/swarmauri/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.077468 swarmauri-0.1.80/swarmauri/community/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/retrievers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/retrievers/base/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/retrievers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/retrievers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/retrievers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/community/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/DownloadPdfTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/EntityRecognitionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/GmailReadTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/GmailSendTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/PaCMAP.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/WebScrapingTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/ZapierHookTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/community/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.081468 swarmauri-0.1.80/swarmauri/core/agent_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agent_apis/IAgentCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agent_apis/IAgentRouterCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agent_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.085469 swarmauri-0.1.80/swarmauri/core/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agent_factories/IAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agent_factories/IExportConf.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.085469 swarmauri-0.1.80/swarmauri/core/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/IAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/IAgentConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/IAgentName.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/IAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/IAgentRetriever.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/IAgentToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/IAgentVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.085469 swarmauri-0.1.80/swarmauri/core/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/chains/ICallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/chains/IChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/chains/IChainFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/chains/IChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.085469 swarmauri-0.1.80/swarmauri/core/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/chunkers/IChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.085469 swarmauri-0.1.80/swarmauri/core/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/conversations/IConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/conversations/IMaxSize.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/conversations/ISystemContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.089469 swarmauri-0.1.80/swarmauri/core/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/distances/IDistanceSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.089469 swarmauri-0.1.80/swarmauri/core/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/document_stores/IDocumentRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/document_stores/IDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.089469 swarmauri-0.1.80/swarmauri/core/documents/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/documents/IDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/documents/IEmbed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/documents/IExperimentDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.089469 swarmauri-0.1.80/swarmauri/core/experiment_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/experiment_stores/IExperimentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/experiment_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.089469 swarmauri-0.1.80/swarmauri/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/messages/IMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.089469 swarmauri-0.1.80/swarmauri/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/metrics/IAggMeasurements.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/metrics/ICalculateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/metrics/IMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/metrics/IThreshold.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.089469 swarmauri-0.1.80/swarmauri/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/models/IFit.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/models/IModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/models/IPredict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.093469 swarmauri-0.1.80/swarmauri/core/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/parsers/IParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.093469 swarmauri-0.1.80/swarmauri/core/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/prompts/IPrompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/prompts/ITemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.093469 swarmauri-0.1.80/swarmauri/core/swarm_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarm_apis/ISwarmAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarm_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.093469 swarmauri-0.1.80/swarmauri/core/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarms/ISwarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarms/ISwarmAgentRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarms/ISwarmChainCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarms/ISwarmComponent.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarms/ISwarmConfigurationExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarms/ISwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.093469 swarmauri-0.1.80/swarmauri/core/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/toolkits/IToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.093469 swarmauri-0.1.80/swarmauri/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/tools/IParameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/tools/ITool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.097468 swarmauri-0.1.80/swarmauri/core/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/tracing/IChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/tracing/ITraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/tracing/ITracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.097468 swarmauri-0.1.80/swarmauri/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/utils/ITransactional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.097468 swarmauri-0.1.80/swarmauri/core/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IAngleBetweenVectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IDecompose.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IDivergence.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IGradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IOrthogonalProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IReflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/ISaveLoadStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/ISimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/ISimiliarityQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorArithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorBasisCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorLinearCombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorNorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorRotate.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorSpan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.101468 swarmauri-0.1.80/swarmauri/core/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectorizers/IFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectorizers/ISaveModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectorizers/IVectorize.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.101468 swarmauri-0.1.80/swarmauri/core/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectors/IVector.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectors/IVectorMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectors/IVectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectors/IVectorTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/core/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.101468 swarmauri-0.1.80/swarmauri/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.101468 swarmauri-0.1.80/swarmauri/experimental/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/ChainOrderStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/ChainOrderStrategyBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/ChainProcessingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/ChainProcessingStrategyBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/IChainOrderStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/IChainProcessingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/MatrixOrderStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/MatrixProcessingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.101468 swarmauri-0.1.80/swarmauri/experimental/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/conversations/SemanticConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.105468 swarmauri-0.1.80/swarmauri/experimental/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/CanberraDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/ChebyshevDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/HaversineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/ManhattanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/MinkowskiDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/SSASimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/SSIVSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/ScannVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/SorensenDiceDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/SquaredEuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.105468 swarmauri-0.1.80/swarmauri/experimental/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/document_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/document_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.105468 swarmauri-0.1.80/swarmauri/experimental/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/models/HierarchicalAttentionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/models/SageMaker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.105468 swarmauri-0.1.80/swarmauri/experimental/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/parsers/PDFToTextParser.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/experimental/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tools/CypherQueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tools/FileDownloaderTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tools/LinkedInArticleTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tools/OutlookSendMailTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tools/SQLite3QueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tools/TwitterPostTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/experimental/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tracing/RemoteTrace.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/utils/ISerializable.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/utils/get_last_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/utils/log_prompt_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/utils/save_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/experimental/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/vector_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/experimental/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/vectorizers/DGLVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/experimental/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/standard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/standard/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/standard/agent_factories/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agent_factories/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.109468 swarmauri-0.1.80/swarmauri/standard/agent_factories/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agent_factories/concrete/AgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agent_factories/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/agents/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/agents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/base/AgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/base/ConversationAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/base/NamedAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/base/ToolAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/base/VectorStoreAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/agents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/GenerativeRagAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/RagAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/SingleCommandAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/ToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/agents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/apis/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/apis/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/apis/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/apis/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.113469 swarmauri-0.1.80/swarmauri/standard/chains/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/base/ChainBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/base/ChainStepBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/chains/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/concrete/CallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/concrete/ChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/concrete/StateChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chains/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/chunkers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/conversations/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/base/ConversationBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/base/SystemContextBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/conversations/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/concrete/SharedConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/concrete/SimpleConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/conversations/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/distances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.117468 swarmauri-0.1.80/swarmauri/standard/distances/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/distances/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/concrete/ChiSquaredDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/concrete/CosineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/concrete/EuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/concrete/JaccardIndexDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/concrete/LevenshteinDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/distances/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/document_stores/base/DocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/documents/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/documents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/documents/base/DocumentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/documents/base/EmbeddedBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/documents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/documents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/documents/concrete/Document.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/documents/concrete/EmbeddedDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/documents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.121468 swarmauri-0.1.80/swarmauri/standard/messages/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/base/MessageBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.125468 swarmauri-0.1.80/swarmauri/standard/messages/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/concrete/AgentMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/concrete/FunctionMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/concrete/HumanMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/concrete/SystemMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/messages/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.125468 swarmauri-0.1.80/swarmauri/standard/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.125468 swarmauri-0.1.80/swarmauri/standard/metrics/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/base/AggregateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/base/CalculateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/base/MetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/base/ThresholdMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.125468 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/HitRateAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/ImpressionAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/MeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/StaticValueMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/ZeroMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/metrics/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.125468 swarmauri-0.1.80/swarmauri/standard/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.125468 swarmauri-0.1.80/swarmauri/standard/models/base/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/base/ModelBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.129468 swarmauri-0.1.80/swarmauri/standard/models/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/concrete/AzureGPT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/concrete/OpenAIModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/concrete/OpenAIToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/models/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.129468 swarmauri-0.1.80/swarmauri/standard/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.129468 swarmauri-0.1.80/swarmauri/standard/parsers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.129468 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/CSVParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/MarkdownParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/PythonParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/RegExParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/TFIDFParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/URLExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/XMLParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/parsers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.129468 swarmauri-0.1.80/swarmauri/standard/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/prompts/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/prompts/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/prompts/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/prompts/concrete/Prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/prompts/concrete/PromptGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/prompts/concrete/PromptTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/prompts/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/states/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/states/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/states/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/states/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/swarms/base/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/swarms/base/SwarmComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/swarms/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/swarms/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/swarms/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/toolkits/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/toolkits/base/ToolkitBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/toolkits/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/toolkits/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/toolkits/concrete/Toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/toolkits/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.133468 swarmauri-0.1.80/swarmauri/standard/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/base/ToolBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.137468 swarmauri-0.1.80/swarmauri/standard/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/concrete/AdditionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/concrete/Parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/concrete/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/concrete/WeatherTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.137468 swarmauri-0.1.80/swarmauri/standard/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.137468 swarmauri-0.1.80/swarmauri/standard/tracing/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.137468 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/CallableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/ChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/SimpleTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/TracedVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/VariableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/tracing/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.137468 swarmauri-0.1.80/swarmauri/standard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/utils/load_documents_from_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.137468 swarmauri-0.1.80/swarmauri/standard/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.137468 swarmauri-0.1.80/swarmauri/standard/vector_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri/standard/vector_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vector_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri/standard/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri/standard/vectorizers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri/standard/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri/standard/vectors/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectors/base/VectorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectors/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri/standard/vectors/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectors/concrete/SimpleVector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectors/concrete/VectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:28:49.000000 swarmauri-0.1.80/swarmauri/standard/vectors/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:29:09.141468 swarmauri-0.1.80/swarmauri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-24 03:29:09.000000 swarmauri-0.1.80/swarmauri.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17552 2024-04-24 03:29:09.000000 swarmauri-0.1.80/swarmauri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:29:09.000000 swarmauri-0.1.80/swarmauri.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 03:29:09.000000 swarmauri-0.1.80/swarmauri.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 03:29:09.000000 swarmauri-0.1.80/swarmauri.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.960000 swarmauri-0.1.9/
+-rw-rw-rw-   0        0        0     3496 2024-03-07 03:38:56.000000 swarmauri-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2024-03-03 14:10:52.000000 swarmauri-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-07 03:38:56.000000 swarmauri-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2170 2024-03-04 21:18:48.000000 swarmauri-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.970000 swarmauri-0.1.9/swarmauri/
+-rw-rw-rw-   0        0        0       21 2024-03-06 12:54:10.000000 swarmauri-0.1.9/swarmauri/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.970000 swarmauri-0.1.9/swarmauri/community/
+-rw-rw-rw-   0        0        0        0 2024-03-01 11:37:30.000000 swarmauri-0.1.9/swarmauri/community/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/document_stores/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/document_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/document_stores/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/document_stores/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/document_stores/concrete/
+-rw-rw-rw-   0        0        0     2873 2024-02-27 22:23:48.000000 swarmauri-0.1.9/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/document_stores/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/retrievers/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/community/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.990000 swarmauri-0.1.9/swarmauri/community/retrievers/base/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/community/retrievers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.990000 swarmauri-0.1.9/swarmauri/community/retrievers/concrete/
+-rw-rw-rw-   0        0        0     2087 2024-02-27 19:40:22.000000 swarmauri-0.1.9/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/community/retrievers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.990000 swarmauri-0.1.9/swarmauri/community/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.000000 swarmauri-0.1.9/swarmauri/community/tools/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/tools/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/
+-rw-rw-rw-   0        0        0     2477 2024-02-26 12:20:58.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/DownloadPdfTool.py
+-rw-rw-rw-   0        0        0     1159 2024-02-25 00:17:10.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/EntityRecognitionTool.py
+-rw-rw-rw-   0        0        0     4073 2024-02-25 00:17:14.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailReadTool.py
+-rw-rw-rw-   0        0        0     4081 2024-03-03 17:06:56.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailSendTool.py
+-rw-rw-rw-   0        0        0     2491 2024-02-27 06:54:54.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/PaCMAP.py
+-rw-rw-rw-   0        0        0      888 2024-02-25 00:17:56.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
+-rw-rw-rw-   0        0        0     2098 2024-02-26 10:14:00.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/WebScrapingTool.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.000000 swarmauri-0.1.9/swarmauri/core/
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:23:40.000000 swarmauri-0.1.9/swarmauri/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.010000 swarmauri-0.1.9/swarmauri/core/agent_apis/
+-rw-rw-rw-   0        0        0     2067 2024-02-29 07:10:06.000000 swarmauri-0.1.9/swarmauri/core/agent_apis/IAgentCommands.py
+-rw-rw-rw-   0        0        0     1786 2024-02-29 07:10:32.000000 swarmauri-0.1.9/swarmauri/core/agent_apis/IAgentRouterCRUD.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/agent_apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.010000 swarmauri-0.1.9/swarmauri/core/agents/
+-rw-rw-rw-   0        0        0      477 2024-03-06 13:34:16.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentConversation.py
+-rw-rw-rw-   0        0        0      317 2024-03-06 13:37:18.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentDocument.py
+-rw-rw-rw-   0        0        0      355 2024-03-06 14:06:14.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentName.py
+-rw-rw-rw-   0        0        0      303 2024-03-06 13:37:54.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentParser.py
+-rw-rw-rw-   0        0        0      327 2024-03-06 13:37:14.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentRetriever.py
+-rw-rw-rw-   0        0        0      317 2024-03-06 13:33:32.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentToolkit.py
+-rw-rw-rw-   0        0        0      638 2024-03-06 13:34:38.000000 swarmauri-0.1.9/swarmauri/core/agents/ISwarmAgent.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.010000 swarmauri-0.1.9/swarmauri/core/chains/
+-rw-rw-rw-   0        0        0      511 2024-03-06 07:13:14.000000 swarmauri-0.1.9/swarmauri/core/chains/ICallableChain.py
+-rw-rw-rw-   0        0        0     1228 2024-03-07 03:38:28.000000 swarmauri-0.1.9/swarmauri/core/chains/IChain.py
+-rw-rw-rw-   0        0        0      960 2024-03-06 22:31:24.000000 swarmauri-0.1.9/swarmauri/core/chains/IChainStep.py
+-rw-rw-rw-   0        0        0       63 2024-03-06 07:46:14.000000 swarmauri-0.1.9/swarmauri/core/chains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.020000 swarmauri-0.1.9/swarmauri/core/chunkers/
+-rw-rw-rw-   0        0        0     1134 2024-03-06 09:41:16.000000 swarmauri-0.1.9/swarmauri/core/chunkers/IChunker.py
+-rw-rw-rw-   0        0        0       93 2024-02-29 02:35:28.000000 swarmauri-0.1.9/swarmauri/core/chunkers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.020000 swarmauri-0.1.9/swarmauri/core/conversations/
+-rw-rw-rw-   0        0        0     1165 2024-02-24 21:26:54.000000 swarmauri-0.1.9/swarmauri/core/conversations/IConversation.py
+-rw-rw-rw-   0        0        0      307 2024-02-24 19:48:48.000000 swarmauri-0.1.9/swarmauri/core/conversations/IMaxSize.py
+-rw-rw-rw-   0        0        0      871 2024-02-24 21:28:08.000000 swarmauri-0.1.9/swarmauri/core/conversations/ISystemContext.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/conversations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.020000 swarmauri-0.1.9/swarmauri/core/document_stores/
+-rw-rw-rw-   0        0        0     2179 2024-02-25 01:07:04.000000 swarmauri-0.1.9/swarmauri/core/document_stores/IDocumentStore.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/document_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/documents/
+-rw-rw-rw-   0        0        0     1597 2024-02-29 23:27:20.000000 swarmauri-0.1.9/swarmauri/core/documents/IDocument.py
+-rw-rw-rw-   0        0        0      486 2024-03-04 22:09:54.000000 swarmauri-0.1.9/swarmauri/core/documents/IEmbed.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/documents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/messages/
+-rw-rw-rw-   0        0        0      722 2024-02-22 03:01:56.000000 swarmauri-0.1.9/swarmauri/core/messages/IMessage.py
+-rw-rw-rw-   0        0        0       30 2024-02-24 21:26:46.000000 swarmauri-0.1.9/swarmauri/core/messages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/models/
+-rw-rw-rw-   0        0        0      298 2024-02-29 03:14:00.000000 swarmauri-0.1.9/swarmauri/core/models/IFit.py
+-rw-rw-rw-   0        0        0      485 2024-02-29 03:15:00.000000 swarmauri-0.1.9/swarmauri/core/models/IModel.py
+-rw-rw-rw-   0        0        0      311 2024-02-29 03:13:40.000000 swarmauri-0.1.9/swarmauri/core/models/IPredict.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/parsers/
+-rw-rw-rw-   0        0        0      778 2024-02-24 21:26:38.000000 swarmauri-0.1.9/swarmauri/core/parsers/IParser.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.040000 swarmauri-0.1.9/swarmauri/core/prompts/
+-rw-rw-rw-   0        0        0      556 2024-02-24 19:59:22.000000 swarmauri-0.1.9/swarmauri/core/prompts/IPrompt.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/prompts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.040000 swarmauri-0.1.9/swarmauri/core/retrievers/
+-rw-rw-rw-   0        0        0      904 2024-02-24 21:27:04.000000 swarmauri-0.1.9/swarmauri/core/retrievers/IRetriever.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:23:58.000000 swarmauri-0.1.9/swarmauri/core/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.040000 swarmauri-0.1.9/swarmauri/core/swarm_apis/
+-rw-rw-rw-   0        0        0     2306 2024-02-29 07:15:38.000000 swarmauri-0.1.9/swarmauri/core/swarm_apis/IAgentRegistration.py
+-rw-rw-rw-   0        0        0     1140 2024-03-03 14:20:54.000000 swarmauri-0.1.9/swarmauri/core/swarm_apis/ISwarmAPI.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/swarm_apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.050000 swarmauri-0.1.9/swarmauri/core/swarms/
+-rw-rw-rw-   0        0        0        0 2024-02-23 03:51:40.000000 swarmauri-0.1.9/swarmauri/core/swarms/ISwarm.py
+-rw-rw-rw-   0        0        0      331 2024-03-06 22:32:50.000000 swarmauri-0.1.9/swarmauri/core/swarms/ISwarmComponent.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/swarms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.050000 swarmauri-0.1.9/swarmauri/core/toolkits/
+-rw-rw-rw-   0        0        0     1635 2024-02-24 21:26:30.000000 swarmauri-0.1.9/swarmauri/core/toolkits/IToolkit.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/toolkits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.060000 swarmauri-0.1.9/swarmauri/core/tools/
+-rw-rw-rw-   0        0        0     2042 2024-02-24 20:06:46.000000 swarmauri-0.1.9/swarmauri/core/tools/IParameter.py
+-rw-rw-rw-   0        0        0      516 2024-03-03 17:27:50.000000 swarmauri-0.1.9/swarmauri/core/tools/ITool.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.060000 swarmauri-0.1.9/swarmauri/core/tracing/
+-rw-rw-rw-   0        0        0     1058 2024-03-06 05:25:36.000000 swarmauri-0.1.9/swarmauri/core/tracing/IChainTracer.py
+-rw-rw-rw-   0        0        0      804 2024-03-02 05:02:52.000000 swarmauri-0.1.9/swarmauri/core/tracing/ITraceContext.py
+-rw-rw-rw-   0        0        0     1606 2024-03-06 00:14:54.000000 swarmauri-0.1.9/swarmauri/core/tracing/ITracer.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/tracing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.060000 swarmauri-0.1.9/swarmauri/core/utils/
+-rw-rw-rw-   0        0        0      637 2024-02-27 19:34:00.000000 swarmauri-0.1.9/swarmauri/core/utils/ITransactional.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.070000 swarmauri-0.1.9/swarmauri/core/vector_stores/
+-rw-rw-rw-   0        0        0      800 2024-02-29 05:59:20.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IAngleBetweenVectors.py
+-rw-rw-rw-   0        0        0     1054 2024-02-29 06:51:34.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IDecompose.py
+-rw-rw-rw-   0        0        0     1676 2024-03-01 22:46:34.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IDistanceSimilarity.py
+-rw-rw-rw-   0        0        0      702 2024-02-29 06:17:22.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IDivergence.py
+-rw-rw-rw-   0        0        0      828 2024-02-29 06:15:56.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IGradient.py
+-rw-rw-rw-   0        0        0      721 2024-02-29 05:46:12.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IOrthogonalProject.py
+-rw-rw-rw-   0        0        0      619 2024-02-29 05:46:38.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IProject.py
+-rw-rw-rw-   0        0        0      661 2024-02-29 06:12:02.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IReflect.py
+-rw-rw-rw-   0        0        0      939 2024-02-29 04:08:20.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/ISimilarity.py
+-rw-rw-rw-   0        0        0      848 2024-02-27 19:35:06.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/ISimiliarityQuery.py
+-rw-rw-rw-   0        0        0      888 2024-02-29 05:28:14.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorArithmetic.py
+-rw-rw-rw-   0        0        0      588 2024-02-29 06:55:40.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorBasisCheck.py
+-rw-rw-rw-   0        0        0      711 2024-02-29 06:44:38.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorLinearCombination.py
+-rw-rw-rw-   0        0        0     1362 2024-02-29 04:54:00.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorNorm.py
+-rw-rw-rw-   0        0        0     2108 2024-02-29 05:40:54.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorProduct.py
+-rw-rw-rw-   0        0        0      757 2024-02-29 06:25:06.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorRotate.py
+-rw-rw-rw-   0        0        0      672 2024-02-29 06:40:18.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorSpan.py
+-rw-rw-rw-   0        0        0     1924 2024-02-29 22:26:24.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorStore.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:24:08.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/core/vectorizers/
+-rw-rw-rw-   0        0        0      624 2024-03-01 10:44:28.000000 swarmauri-0.1.9/swarmauri/core/vectorizers/IVectorize.py
+-rw-rw-rw-   0        0        0        1 2024-02-29 23:57:16.000000 swarmauri-0.1.9/swarmauri/core/vectorizers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/core/vectors/
+-rw-rw-rw-   0        0        0      578 2024-03-01 23:23:06.000000 swarmauri-0.1.9/swarmauri/core/vectors/IVector.py
+-rw-rw-rw-   0        0        0      900 2024-02-29 04:09:42.000000 swarmauri-0.1.9/swarmauri/core/vectors/IVectorMeta.py
+-rw-rw-rw-   0        0        0     1312 2024-02-29 22:50:46.000000 swarmauri-0.1.9/swarmauri/core/vectors/IVectorTransform.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:24:16.000000 swarmauri-0.1.9/swarmauri/core/vectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/experimental/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/experimental/chains/
+-rw-rw-rw-   0        0        0      628 2024-03-06 23:57:40.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainOrderStrategy.py
+-rw-rw-rw-   0        0        0      516 2024-03-06 22:36:46.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainOrderStrategyBase.py
+-rw-rw-rw-   0        0        0      842 2024-03-06 23:53:50.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainProcessingStrategy.py
+-rw-rw-rw-   0        0        0      603 2024-03-06 23:48:40.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainProcessingStrategyBase.py
+-rw-rw-rw-   0        0        0      299 2024-03-06 22:32:20.000000 swarmauri-0.1.9/swarmauri/experimental/chains/IChainOrderStrategy.py
+-rw-rw-rw-   0        0        0      585 2024-03-06 22:32:10.000000 swarmauri-0.1.9/swarmauri/experimental/chains/IChainProcessingStrategy.py
+-rw-rw-rw-   0        0        0      725 2024-03-07 01:54:34.000000 swarmauri-0.1.9/swarmauri/experimental/chains/MatrixOrderStrategy.py
+-rw-rw-rw-   0        0        0     1073 2024-03-07 00:47:16.000000 swarmauri-0.1.9/swarmauri/experimental/chains/MatrixProcessingStrategy.py
+-rw-rw-rw-   0        0        0     4481 2024-03-06 12:26:20.000000 swarmauri-0.1.9/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+-rw-rw-rw-   0        0        0        1 2024-03-07 03:35:10.000000 swarmauri-0.1.9/swarmauri/experimental/chains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.090000 swarmauri-0.1.9/swarmauri/experimental/conversations/
+-rw-rw-rw-   0        0        0     3471 2024-03-04 00:27:10.000000 swarmauri-0.1.9/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
+-rw-rw-rw-   0        0        0     2219 2024-02-24 23:03:58.000000 swarmauri-0.1.9/swarmauri/experimental/conversations/SemanticConversation.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:51:08.000000 swarmauri-0.1.9/swarmauri/experimental/conversations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.090000 swarmauri-0.1.9/swarmauri/experimental/models/
+-rw-rw-rw-   0        0        0     3556 2024-03-03 14:27:12.000000 swarmauri-0.1.9/swarmauri/experimental/models/HierarchicalAttentionModel.py
+-rw-rw-rw-   0        0        0     1846 2024-02-24 23:05:02.000000 swarmauri-0.1.9/swarmauri/experimental/models/SageMaker.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 05:01:34.000000 swarmauri-0.1.9/swarmauri/experimental/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.090000 swarmauri-0.1.9/swarmauri/experimental/parsers/
+-rw-rw-rw-   0        0        0     1508 2024-02-29 02:42:10.000000 swarmauri-0.1.9/swarmauri/experimental/parsers/PDFToTextParser.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.100000 swarmauri-0.1.9/swarmauri/experimental/tools/
+-rw-rw-rw-   0        0        0     1414 2024-02-29 02:47:28.000000 swarmauri-0.1.9/swarmauri/experimental/tools/CypherQueryTool.py
+-rw-rw-rw-   0        0        0     1237 2024-02-29 02:49:12.000000 swarmauri-0.1.9/swarmauri/experimental/tools/FileDownloaderTool.py
+-rw-rw-rw-   0        0        0     3466 2024-02-24 23:06:28.000000 swarmauri-0.1.9/swarmauri/experimental/tools/LinkedInArticleTool.py
+-rw-rw-rw-   0        0        0     2918 2024-02-27 18:57:56.000000 swarmauri-0.1.9/swarmauri/experimental/tools/OutlookSendMailTool.py
+-rw-rw-rw-   0        0        0     1357 2024-02-29 02:51:04.000000 swarmauri-0.1.9/swarmauri/experimental/tools/SQLite3QueryTool.py
+-rw-rw-rw-   0        0        0     1511 2024-02-24 23:06:52.000000 swarmauri-0.1.9/swarmauri/experimental/tools/TwitterPostTool.py
+-rw-rw-rw-   0        0        0       27 2024-02-27 18:55:30.000000 swarmauri-0.1.9/swarmauri/experimental/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.110000 swarmauri-0.1.9/swarmauri/experimental/utils/
+-rw-rw-rw-   0        0        0      973 2024-02-27 19:36:04.000000 swarmauri-0.1.9/swarmauri/experimental/utils/ISerializable.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/utils/__init__.py
+-rw-rw-rw-   0        0        0      655 2024-02-23 08:24:16.000000 swarmauri-0.1.9/swarmauri/experimental/utils/get_last_frame.py
+-rw-rw-rw-   0        0        0     2141 2024-02-23 08:34:46.000000 swarmauri-0.1.9/swarmauri/experimental/utils/save_schema.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.110000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/
+-rw-rw-rw-   0        0        0     2854 2024-03-03 14:29:14.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/CanberraDistance.py
+-rw-rw-rw-   0        0        0     1875 2024-03-03 14:30:48.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/ChebyshevDistance.py
+-rw-rw-rw-   0        0        0     2024 2024-03-03 14:31:04.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/HaversineDistance.py
+-rw-rw-rw-   0        0        0     2347 2024-03-03 14:31:12.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/ManhattanDistance.py
+-rw-rw-rw-   0        0        0     2866 2024-03-03 14:35:10.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/MinkowskiDistance.py
+-rw-rw-rw-   0        0        0     2057 2024-02-29 09:06:24.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSASimilarity.py
+-rw-rw-rw-   0        0        0     2643 2024-02-29 09:07:00.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSIVSimilarity.py
+-rw-rw-rw-   0        0        0     7058 2024-03-03 09:40:08.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/ScannVectorStore.py
+-rw-rw-rw-   0        0        0     2213 2024-03-03 14:31:54.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SorensenDiceDistance.py
+-rw-rw-rw-   0        0        0     1989 2024-03-03 14:31:30.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.110000 swarmauri-0.1.9/swarmauri/standard/
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:33:08.000000 swarmauri-0.1.9/swarmauri/standard/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.120000 swarmauri-0.1.9/swarmauri/standard/agents/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.120000 swarmauri-0.1.9/swarmauri/standard/agents/base/
+-rw-rw-rw-   0        0        0     1650 2024-03-06 14:58:36.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/AgentBase.py
+-rw-rw-rw-   0        0        0      913 2024-03-06 15:05:42.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/ConversationAgentBase.py
+-rw-rw-rw-   0        0        0      546 2024-03-06 14:31:00.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/NamedAgentBase.py
+-rw-rw-rw-   0        0        0     1061 2024-03-06 15:05:50.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/ToolAgentBase.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.120000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/
+-rw-rw-rw-   0        0        0     1688 2024-03-06 14:42:14.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
+-rw-rw-rw-   0        0        0     2101 2024-03-06 15:05:58.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
+-rw-rw-rw-   0        0        0     3847 2024-03-06 15:06:02.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
+-rw-rw-rw-   0        0        0      925 2024-03-06 14:55:40.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
+-rw-rw-rw-   0        0        0      569 2024-03-06 14:55:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/SingleCommandAgent.py
+-rw-rw-rw-   0        0        0     3451 2024-03-06 14:00:52.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/ToolAgent.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.130000 swarmauri-0.1.9/swarmauri/standard/apis/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.130000 swarmauri-0.1.9/swarmauri/standard/apis/base/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/apis/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.130000 swarmauri-0.1.9/swarmauri/standard/apis/concrete/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/apis/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.150000 swarmauri-0.1.9/swarmauri/standard/chains/
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:46:30.000000 swarmauri-0.1.9/swarmauri/standard/chains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.150000 swarmauri-0.1.9/swarmauri/standard/chains/base/
+-rw-rw-rw-   0        0        0     2007 2024-03-07 03:22:46.000000 swarmauri-0.1.9/swarmauri/standard/chains/base/ChainBase.py
+-rw-rw-rw-   0        0        0     1050 2024-03-06 23:41:32.000000 swarmauri-0.1.9/swarmauri/standard/chains/base/ChainStepBase.py
+-rw-rw-rw-   0        0        0        1 2024-03-06 07:27:50.000000 swarmauri-0.1.9/swarmauri/standard/chains/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.150000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/
+-rw-rw-rw-   0        0        0     1262 2024-03-06 10:26:28.000000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/CallableChain.py
+-rw-rw-rw-   0        0        0     1594 2024-03-06 23:53:24.000000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/Chain.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:46:36.000000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.160000 swarmauri-0.1.9/swarmauri/standard/chunkers/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.160000 swarmauri-0.1.9/swarmauri/standard/chunkers/base/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.160000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/
+-rw-rw-rw-   0        0        0     1935 2024-03-03 14:28:00.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
+-rw-rw-rw-   0        0        0     1477 2024-03-03 14:27:50.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
+-rw-rw-rw-   0        0        0     2164 2024-03-06 09:27:14.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
+-rw-rw-rw-   0        0        0     1198 2024-03-05 00:05:40.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
+-rw-rw-rw-   0        0        0     1605 2024-03-03 14:27:52.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.170000 swarmauri-0.1.9/swarmauri/standard/conversations/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.180000 swarmauri-0.1.9/swarmauri/standard/conversations/base/
+-rw-rw-rw-   0        0        0     1129 2024-02-26 07:54:40.000000 swarmauri-0.1.9/swarmauri/standard/conversations/base/ConversationBase.py
+-rw-rw-rw-   0        0        0     1615 2024-02-26 08:46:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/base/SystemContextBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.180000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/
+-rw-rw-rw-   0        0        0     1355 2024-02-24 22:46:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
+-rw-rw-rw-   0        0        0     3621 2024-02-26 07:48:40.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
+-rw-rw-rw-   0        0        0     4703 2024-03-03 21:57:50.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/SharedConversation.py
+-rw-rw-rw-   0        0        0      349 2024-02-25 00:13:18.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/SimpleConversation.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.190000 swarmauri-0.1.9/swarmauri/standard/document_stores/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.190000 swarmauri-0.1.9/swarmauri/standard/document_stores/base/
+-rw-rw-rw-   0        0        0     2465 2024-02-27 13:13:34.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/base/DocumentStoreBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.200000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/
+-rw-rw-rw-   0        0        0     2598 2024-03-05 01:36:40.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/Doc2VecDocumentStore.py
+-rw-rw-rw-   0        0        0     2781 2024-03-05 03:23:04.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/TFIDFDocumentStore.py
+-rw-rw-rw-   0        0        0     3898 2024-03-04 23:55:32.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/Word2VecDocumentStore.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.200000 swarmauri-0.1.9/swarmauri/standard/documents/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/documents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.200000 swarmauri-0.1.9/swarmauri/standard/documents/base/
+-rw-rw-rw-   0        0        0     1615 2024-03-05 00:27:00.000000 swarmauri-0.1.9/swarmauri/standard/documents/base/DocumentBase.py
+-rw-rw-rw-   0        0        0      538 2024-03-04 23:27:36.000000 swarmauri-0.1.9/swarmauri/standard/documents/base/EmbeddedBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/documents/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.210000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/
+-rw-rw-rw-   0        0        0      132 2024-03-05 01:42:48.000000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/Document.py
+-rw-rw-rw-   0        0        0      469 2024-03-04 23:01:20.000000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/EmbeddedDocument.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.220000 swarmauri-0.1.9/swarmauri/standard/messages/
+-rw-rw-rw-   0        0        0        0 2024-02-24 22:27:04.000000 swarmauri-0.1.9/swarmauri/standard/messages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.220000 swarmauri-0.1.9/swarmauri/standard/messages/base/
+-rw-rw-rw-   0        0        0     1628 2024-02-26 05:35:02.000000 swarmauri-0.1.9/swarmauri/standard/messages/base/MessageBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-24 22:28:22.000000 swarmauri-0.1.9/swarmauri/standard/messages/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.230000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/
+-rw-rw-rw-   0        0        0      309 2024-02-24 23:56:56.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/AgentMessage.py
+-rw-rw-rw-   0        0        0      836 2024-02-24 23:57:04.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/FunctionMessage.py
+-rw-rw-rw-   0        0        0      761 2024-02-24 23:57:02.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/HumanMessage.py
+-rw-rw-rw-   0        0        0      536 2024-02-24 23:57:08.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/SystemMessage.py
+-rw-rw-rw-   0        0        0      166 2024-02-24 22:27:54.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.230000 swarmauri-0.1.9/swarmauri/standard/models/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.240000 swarmauri-0.1.9/swarmauri/standard/models/base/
+-rw-rw-rw-   0        0        0      770 2024-02-29 03:23:18.000000 swarmauri-0.1.9/swarmauri/standard/models/base/ModelBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/models/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.240000 swarmauri-0.1.9/swarmauri/standard/models/concrete/
+-rw-rw-rw-   0        0        0     2387 2024-02-29 03:27:06.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/AzureGPT.py
+-rw-rw-rw-   0        0        0     1565 2024-02-29 03:27:20.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
+-rw-rw-rw-   0        0        0     2105 2024-02-29 03:25:52.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIModel.py
+-rw-rw-rw-   0        0        0      825 2024-03-03 21:05:02.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIToolModel.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.240000 swarmauri-0.1.9/swarmauri/standard/parsers/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.250000 swarmauri-0.1.9/swarmauri/standard/parsers/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/parsers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.250000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/
+-rw-rw-rw-   0        0        0     2357 2024-03-01 04:56:04.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
+-rw-rw-rw-   0        0        0     1785 2024-02-29 23:28:16.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/CSVParser.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 23:28:30.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
+-rw-rw-rw-   0        0        0     1275 2024-02-29 23:28:38.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
+-rw-rw-rw-   0        0        0     1925 2024-02-29 23:28:44.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
+-rw-rw-rw-   0        0        0     1723 2024-02-29 23:28:50.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/MarkdownParser.py
+-rw-rw-rw-   0        0        0     1938 2024-02-29 23:28:54.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
+-rw-rw-rw-   0        0        0     1576 2024-02-29 23:28:58.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
+-rw-rw-rw-   0        0        0     2118 2024-02-29 23:29:02.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PythonParser.py
+-rw-rw-rw-   0        0        0     1645 2024-02-29 23:29:10.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/RegExParser.py
+-rw-rw-rw-   0        0        0     1857 2024-02-29 23:29:14.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
+-rw-rw-rw-   0        0        0     1386 2024-02-29 23:29:36.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
+-rw-rw-rw-   0        0        0      829 2024-02-29 23:29:42.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TfidfParser.py
+-rw-rw-rw-   0        0        0     1661 2024-02-29 23:29:48.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/URLExtractorParser.py
+-rw-rw-rw-   0        0        0     1952 2024-02-29 23:29:54.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/XMLParser.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.260000 swarmauri-0.1.9/swarmauri/standard/prompts/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/prompts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.260000 swarmauri-0.1.9/swarmauri/standard/prompts/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/prompts/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.270000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/
+-rw-rw-rw-   0        0        0     1522 2024-02-24 22:55:06.000000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/Prompt.py
+-rw-rw-rw-   0        0        0     2082 2024-02-24 22:55:20.000000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/PromptTemplate.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.270000 swarmauri-0.1.9/swarmauri/standard/retrievers/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.280000 swarmauri-0.1.9/swarmauri/standard/retrievers/base/
+-rw-rw-rw-   0        0        0     1525 2024-02-27 13:25:48.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/base/DocumentRetrieverBase.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.280000 swarmauri-0.1.9/swarmauri/standard/retrievers/concrete/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.290000 swarmauri-0.1.9/swarmauri/standard/states/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/states/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.290000 swarmauri-0.1.9/swarmauri/standard/states/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/states/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.300000 swarmauri-0.1.9/swarmauri/standard/states/concrete/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/states/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.300000 swarmauri-0.1.9/swarmauri/standard/swarms/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/swarms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.300000 swarmauri-0.1.9/swarmauri/standard/swarms/base/
+-rw-rw-rw-   0        0        0      553 2024-03-06 22:40:40.000000 swarmauri-0.1.9/swarmauri/standard/swarms/base/SwarmComponentBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/swarms/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.310000 swarmauri-0.1.9/swarmauri/standard/swarms/concrete/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/swarms/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.320000 swarmauri-0.1.9/swarmauri/standard/toolkits/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.320000 swarmauri-0.1.9/swarmauri/standard/toolkits/base/
+-rw-rw-rw-   0        0        0     2430 2024-02-25 00:14:18.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/base/ToolkitBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.320000 swarmauri-0.1.9/swarmauri/standard/toolkits/concrete/
+-rw-rw-rw-   0        0        0      510 2024-02-25 00:14:40.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/concrete/Toolkit.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tools/base/
+-rw-rw-rw-   0        0        0     2351 2024-03-03 17:48:26.000000 swarmauri-0.1.9/swarmauri/standard/tools/base/ToolBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/tools/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/
+-rw-rw-rw-   0        0        0     1021 2024-02-29 03:53:26.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/AdditionTool.py
+-rw-rw-rw-   0        0        0     3181 2024-02-25 00:22:04.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/Parameter.py
+-rw-rw-rw-   0        0        0      981 2024-02-24 22:57:00.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/TestTool.py
+-rw-rw-rw-   0        0        0     1121 2024-02-24 22:57:12.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/WeatherTool.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tracing/
+-rw-rw-rw-   0        0        0        1 2024-03-02 03:57:38.000000 swarmauri-0.1.9/swarmauri/standard/tracing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.340000 swarmauri-0.1.9/swarmauri/standard/tracing/base/
+-rw-rw-rw-   0        0        0        1 2024-03-02 03:57:44.000000 swarmauri-0.1.9/swarmauri/standard/tracing/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.340000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/
+-rw-rw-rw-   0        0        0     1424 2024-03-06 07:31:36.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/CallableTracer.py
+-rw-rw-rw-   0        0        0     2115 2024-03-06 05:51:12.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/ChainTracer.py
+-rw-rw-rw-   0        0        0      715 2024-03-06 07:30:20.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
+-rw-rw-rw-   0        0        0     1660 2024-03-06 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/SimpleTracer.py
+-rw-rw-rw-   0        0        0     1126 2024-03-06 00:57:18.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/TracedVariable.py
+-rw-rw-rw-   0        0        0     1042 2024-03-06 07:31:20.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/VariableTracer.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:46:20.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.360000 swarmauri-0.1.9/swarmauri/standard/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.360000 swarmauri-0.1.9/swarmauri/standard/vector_stores/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.370000 swarmauri-0.1.9/swarmauri/standard/vector_stores/base/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.380000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/
+-rw-rw-rw-   0        0        0     1504 2024-03-03 14:30:54.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/ChiSquaredDistance.py
+-rw-rw-rw-   0        0        0     2682 2024-03-04 23:27:58.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/CosineDistance.py
+-rw-rw-rw-   0        0        0     1998 2024-03-03 14:29:58.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/EuclideanDistance.py
+-rw-rw-rw-   0        0        0     3527 2024-03-01 03:38:10.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/FaissVectorStore.py
+-rw-rw-rw-   0        0        0     2769 2024-03-03 14:31:06.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/JaccardIndexDistance.py
+-rw-rw-rw-   0        0        0     3242 2024-03-03 14:30:12.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/LevenshteinDistance.py
+-rw-rw-rw-   0        0        0     1429 2024-03-01 10:02:22.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/VectorProduct.py
+-rw-rw-rw-   0        0        0     1542 2024-03-03 14:31:34.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/WeaviateVectorStore.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.380000 swarmauri-0.1.9/swarmauri/standard/vectorizers/
+-rw-rw-rw-   0        0        0        1 2024-03-01 00:01:54.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.400000 swarmauri-0.1.9/swarmauri/standard/vectorizers/base/
+-rw-rw-rw-   0        0        0        1 2024-03-01 00:02:00.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.410000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/
+-rw-rw-rw-   0        0        0     2285 2024-03-01 10:45:14.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/BERTEmbeddingVectorizer.py
+-rw-rw-rw-   0        0        0     2369 2024-03-01 10:43:42.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
+-rw-rw-rw-   0        0        0        1 2024-03-01 00:01:54.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.420000 swarmauri-0.1.9/swarmauri/standard/vectors/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.420000 swarmauri-0.1.9/swarmauri/standard/vectors/base/
+-rw-rw-rw-   0        0        0      751 2024-03-01 23:28:40.000000 swarmauri-0.1.9/swarmauri/standard/vectors/base/VectorBase.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vectors/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.430000 swarmauri-0.1.9/swarmauri/standard/vectors/concrete/
+-rw-rw-rw-   0        0        0      211 2024-03-01 04:52:48.000000 swarmauri-0.1.9/swarmauri/standard/vectors/concrete/SimpleVector.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vectors/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.970000 swarmauri-0.1.9/swarmauri.egg-info/
+-rw-rw-rw-   0        0        0     3496 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14135 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      576 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/top_level.txt
```

### Comparing `swarmauri-0.1.80/README.md` & `swarmauri-0.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-# SwarmaURI SDK
-This repository includes core interfaces, standard ABCs, and standard concrete references of the SwarmaURI Framework.
-
-## Steps to compile python package from source
-```bash
-pip install swarmauri[full]
-```
-## ./combined
-This includes convenience outputs to enable conversations with GPTs.
-
-## ./dist
-This includes SwarmaURI python package builds. This will eventually be excluded from this directory in favor of pypi.
-
-## ./scripts
-This includes convenience scripts that are nother included with the SwarmaURI SDK.
-#### /scripts/combine_files.py
-```bash
-#This script generates the convenience outputs found in ./combined
-python ./combine_files.py
-```
-
-## ./swarmauri
-This includes the libaries for the SwarmaURI python package.
-
-## ./tests
-This includes test cases for the SwarmaURI python  package.
+# SwarmaURI SDK
+This repository includes core interfaces, standard ABCs, and standard concrete references of the SwarmaURI Framework.
+
+## Steps to compile python package from source
+```bash
+git clone https://github.com/cobycloud/swarmauri
+cd swarmauri
+python -m build
+pip install ./dist/swarmauri-0.1.tar.gz --force-reinstall
+```
+## ./combined
+This includes convenience outputs to enable conversations with GPTs.
+
+## ./dist
+This includes SwarmaURI python package builds. This will eventually be excluded from this directory in favor of pypi.
+
+## ./scripts
+This includes convenience scripts that are nother included with the SwarmaURI SDK.
+#### /scripts/combine_files.py
+```bash
+#This script generates the convenience outputs found in ./combined
+python ./combine_files.py
+```
+
+## ./swamauri
+This includes the libaries for the SwarmaURI python package.
+
+## ./tests
+This includes test cases for the SwarmaURI python  package.
```

### Comparing `swarmauri-0.1.80/swarmauri/community/document_stores/concrete/RedisDocumentStore.py` & `swarmauri-0.1.9/swarmauri/community/document_stores/concrete/RedisDocumentStore.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from typing import List, Optional
-from ....standard.document_stores.base.DocumentStoreBase import DocumentStoreBase
-from ....core.documents.IDocument import IDocument
-import redis
-import json
-from redis.commands.search.field import TextField, NumericField, TagField
-from redis.commands.search.indexDefinition import IndexDefinition, IndexType
-
-
-class RedisDocumentStore(DocumentStoreBase):
-    def __init__(self, host, password, port, db):
-        """Store connection details without initializing the Redis client."""
-        self._host = host
-        self._password = password
-        self._port = port
-        self._db = db
-        self._redis_client = None  # Delayed initialization
-
-    @property
-    def redis_client(self):
-        """Lazily initialize and return the Redis client using a factory method."""
-        if self._redis_client is None:
-            print('here')
-            self._redis_client = redis.Redis(host=self._host, 
-                                             password=self._password, 
-                                             port=self._port, 
-                                             db=self._db)
-            print('there')
-        return self._redis_client
-
-    def add_document(self, document: IDocument) -> None:
-        
-        data = document.as_dict()
-        doc_id = data['id'] 
-        del data['id']
-        self.redis_client.json().set(doc_id, '$', json.dumps(data))
-
-    def add_documents(self, documents: List[IDocument]) -> None:
-        with self.redis_client.pipeline() as pipe:
-            for document in documents:
-                pipe.set(document.doc_id, document)
-            pipe.execute()
-
-    def get_document(self, doc_id: str) -> Optional[IDocument]:
-        result = self.redis_client.json().get(doc_id)
-        if result:
-            return json.loads(result)
-        return None
-
-    def get_all_documents(self) -> List[IDocument]:
-        keys = self.redis_client.keys('*')
-        documents = []
-        for key in keys:
-            document_data = self.redis_client.get(key)
-            if document_data:
-                documents.append(json.loads(document_data))
-        return documents
-
-    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
-        self.add_document(updated_document)
-
-    def delete_document(self, doc_id: str) -> None:
-        self.redis_client.delete(doc_id)
-    
-    def __getstate__(self):
-        """Return the object state for serialization, excluding the Redis client."""
-        state = self.__dict__.copy()
-        state['_redis_client'] = None  # Exclude Redis client from serialization
-        return state
-
-    def __setstate__(self, state):
-        """Restore the object state after serialization, reinitializing the Redis client."""
+from typing import List, Optional
+from ....standard.document_stores.base.DocumentStoreBase import DocumentStoreBase
+from ....core.documents.IDocument import IDocument
+import redis
+import json
+from redis.commands.search.field import TextField, NumericField, TagField
+from redis.commands.search.indexDefinition import IndexDefinition, IndexType
+
+
+class RedisDocumentStore(DocumentStoreBase):
+    def __init__(self, host, password, port, db):
+        """Store connection details without initializing the Redis client."""
+        self._host = host
+        self._password = password
+        self._port = port
+        self._db = db
+        self._redis_client = None  # Delayed initialization
+
+    @property
+    def redis_client(self):
+        """Lazily initialize and return the Redis client using a factory method."""
+        if self._redis_client is None:
+            print('here')
+            self._redis_client = redis.Redis(host=self._host, 
+                                             password=self._password, 
+                                             port=self._port, 
+                                             db=self._db)
+            print('there')
+        return self._redis_client
+
+    def add_document(self, document: IDocument) -> None:
+        
+        data = document.as_dict()
+        doc_id = data['id'] 
+        del data['id']
+        self.redis_client.json().set(doc_id, '$', json.dumps(data))
+
+    def add_documents(self, documents: List[IDocument]) -> None:
+        with self.redis_client.pipeline() as pipe:
+            for document in documents:
+                pipe.set(document.doc_id, document)
+            pipe.execute()
+
+    def get_document(self, doc_id: str) -> Optional[IDocument]:
+        result = self.redis_client.json().get(doc_id)
+        if result:
+            return json.loads(result)
+        return None
+
+    def get_all_documents(self) -> List[IDocument]:
+        keys = self.redis_client.keys('*')
+        documents = []
+        for key in keys:
+            document_data = self.redis_client.get(key)
+            if document_data:
+                documents.append(json.loads(document_data))
+        return documents
+
+    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
+        self.add_document(updated_document)
+
+    def delete_document(self, doc_id: str) -> None:
+        self.redis_client.delete(doc_id)
+    
+    def __getstate__(self):
+        """Return the object state for serialization, excluding the Redis client."""
+        state = self.__dict__.copy()
+        state['_redis_client'] = None  # Exclude Redis client from serialization
+        return state
+
+    def __setstate__(self, state):
+        """Restore the object state after serialization, reinitializing the Redis client."""
         self.__dict__.update(state)
```

### Comparing `swarmauri-0.1.80/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py` & `swarmauri-0.1.9/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from typing import List
-from redisearch import Client, Query
-from ....core.documents.IDocument import IDocument
-from ....standard.document_stores.concrete.ConcreteDocument import ConcreteDocument
-from ....standard.retrievers.base.DocumentRetrieverBase import DocumentRetrieverBase
-
-class RedisDocumentRetriever(DocumentRetrieverBase):
-    """
-    A document retriever that fetches documents from a Redis store.
-    """
-    
-    def __init__(self, redis_idx_name, redis_host, redis_port):
-        """
-        Initializes a new instance of RedisDocumentRetriever.
-
-        Args:
-            redis_client (Redis): An instance of the Redis client.
-        """
-        self._redis_client = None
-        self._redis_idx_name = redis_idx_name
-        self._redis_host = redis_host
-        self._redis_port = redis_port
-
-    @property
-    def redis_client(self):
-        """Lazily initialize and return the Redis client using a factory method."""
-        if self._redis_client is None:
-            self._redis_client = Client(self.redis_idx_name, host=self.redis_host, port=self.redis_port)
-        return self._redis_client
-    
-    def retrieve(self, query: str, top_k: int = 5) -> List[IDocument]:
-        """
-        Retrieve the most relevant documents based on the given query.
-        
-        Args:
-            query (str): The query string used for document retrieval.
-            top_k (int, optional): The number of top relevant documents to retrieve. Defaults to 5.
-        
-        Returns:
-            List[IDocument]: A list of the top_k most relevant documents.
-        """
-        query_result = self.redis_client.search(Query(query).paging(0, top_k))
-        
-        documents = [
-            ConcreteDocument(
-                doc_id=doc.id,
-                content=doc.text,  # Note: Adjust 'text' based on actual Redis document schema
-                metadata=doc.__dict__  # Including full document fields and values in metadata
-            )
-            for doc in query_result.docs
-        ]
-
-        return documents
+from typing import List
+from redisearch import Client, Query
+from ....core.documents.IDocument import IDocument
+from ....standard.document_stores.concrete.ConcreteDocument import ConcreteDocument
+from ....standard.retrievers.base.DocumentRetrieverBase import DocumentRetrieverBase
+
+class RedisDocumentRetriever(DocumentRetrieverBase):
+    """
+    A document retriever that fetches documents from a Redis store.
+    """
+    
+    def __init__(self, redis_idx_name, redis_host, redis_port):
+        """
+        Initializes a new instance of RedisDocumentRetriever.
+
+        Args:
+            redis_client (Redis): An instance of the Redis client.
+        """
+        self._redis_client = None
+        self._redis_idx_name = redis_idx_name
+        self._redis_host = redis_host
+        self._redis_port = redis_port
+
+    @property
+    def redis_client(self):
+        """Lazily initialize and return the Redis client using a factory method."""
+        if self._redis_client is None:
+            self._redis_client = Client(self.redis_idx_name, host=self.redis_host, port=self.redis_port)
+        return self._redis_client
+    
+    def retrieve(self, query: str, top_k: int = 5) -> List[IDocument]:
+        """
+        Retrieve the most relevant documents based on the given query.
+        
+        Args:
+            query (str): The query string used for document retrieval.
+            top_k (int, optional): The number of top relevant documents to retrieve. Defaults to 5.
+        
+        Returns:
+            List[IDocument]: A list of the top_k most relevant documents.
+        """
+        query_result = self.redis_client.search(Query(query).paging(0, top_k))
+        
+        documents = [
+            ConcreteDocument(
+                doc_id=doc.id,
+                content=doc.text,  # Note: Adjust 'text' based on actual Redis document schema
+                metadata=doc.__dict__  # Including full document fields and values in metadata
+            )
+            for doc in query_result.docs
+        ]
+
+        return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/community/tools/concrete/DownloadPdfTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/DownloadPdfTool.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import requests
-from typing import Dict
-from pathlib import Path
-from ...standard.tools.base.ToolBase import ToolBase
-from ...standard.tools.concrete.Parameter import Parameter
-
-class DownloadPDFTool(ToolBase):
-    def __init__(self):
-        parameters = [
-            Parameter(
-                name="url",
-                type="string",
-                description="The URL of the PDF file to download",
-                required=True
-            ),
-            Parameter(
-                name="destination",
-                type="string",
-                description="The path where the PDF file will be saved",
-                required=True
-            )
-        ]
-        
-        super().__init__(name="DownloadPDFTool",
-                         description="Downloads a PDF from a specified URL and saves it to a specified path.",
-                         parameters=parameters)
-
-    def __call__(self, url: str, destination: str) -> Dict[str, str]:
-        """
-        Download the PDF from the specified URL and saves it to the given destination path.
-
-        Parameters:
-        - url (str): The URL from where to download the PDF.
-        - destination (str): The local file path where the PDF should be saved.
-        
-        Returns:
-        - Dict[str, str]: A dictionary containing the result message and the destination path.
-        """
-        try:
-            # Send a GET request to the specified URL
-            response = requests.get(url, stream=True)
-
-            # Raise an HTTPError if the status code is not 200 (OK)
-            response.raise_for_status()
-
-            # Ensure destination directory exists
-            Path(destination).parent.mkdir(parents=True, exist_ok=True)
-
-            # Open a file at the specified destination path and write the content of the response to it
-            with open(Path(destination), 'wb') as file:
-                for chunk in response.iter_content(chunk_size=8192):
-                    file.write(chunk)
-            
-            return {
-                "message": "PDF downloaded successfully.",
-                "destination": destination
-            }
-
-        except requests.exceptions.RequestException as e:
-            # Handle requests-related errors
-            return {"error": f"Failed to download PDF: {e}"}
-        except IOError as e:
-            # Handle file I/O errors
+import requests
+from typing import Dict
+from pathlib import Path
+from ...standard.tools.base.ToolBase import ToolBase
+from ...standard.tools.concrete.Parameter import Parameter
+
+class DownloadPDFTool(ToolBase):
+    def __init__(self):
+        parameters = [
+            Parameter(
+                name="url",
+                type="string",
+                description="The URL of the PDF file to download",
+                required=True
+            ),
+            Parameter(
+                name="destination",
+                type="string",
+                description="The path where the PDF file will be saved",
+                required=True
+            )
+        ]
+        
+        super().__init__(name="DownloadPDFTool",
+                         description="Downloads a PDF from a specified URL and saves it to a specified path.",
+                         parameters=parameters)
+
+    def __call__(self, url: str, destination: str) -> Dict[str, str]:
+        """
+        Download the PDF from the specified URL and saves it to the given destination path.
+
+        Parameters:
+        - url (str): The URL from where to download the PDF.
+        - destination (str): The local file path where the PDF should be saved.
+        
+        Returns:
+        - Dict[str, str]: A dictionary containing the result message and the destination path.
+        """
+        try:
+            # Send a GET request to the specified URL
+            response = requests.get(url, stream=True)
+
+            # Raise an HTTPError if the status code is not 200 (OK)
+            response.raise_for_status()
+
+            # Ensure destination directory exists
+            Path(destination).parent.mkdir(parents=True, exist_ok=True)
+
+            # Open a file at the specified destination path and write the content of the response to it
+            with open(Path(destination), 'wb') as file:
+                for chunk in response.iter_content(chunk_size=8192):
+                    file.write(chunk)
+            
+            return {
+                "message": "PDF downloaded successfully.",
+                "destination": destination
+            }
+
+        except requests.exceptions.RequestException as e:
+            # Handle requests-related errors
+            return {"error": f"Failed to download PDF: {e}"}
+        except IOError as e:
+            # Handle file I/O errors
             return {"error": f"Failed to save PDF: {e}"}
```

### Comparing `swarmauri-0.1.80/swarmauri/community/tools/concrete/EntityRecognitionTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/EntityRecognitionTool.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import json
-from transformers import pipeline, logging as hf_logging
-from ....standard.tools.base.ToolBase import ToolBase
-from ....standard.tools.concrete.Parameter import Parameter
-
-hf_logging.set_verbosity_error()
-
-class EntityRecognitionTool(ToolBase):
-    def __init__(self):
-        parameters = [
-            Parameter("text","string","The text for entity recognition",True)
-        ]
-        super().__init__(name="EntityRecognitionTool", 
-                         description="Extracts named entities from text", 
-                         parameters=parameters)
-        
-
-    def __call__(self, text: str) -> dict:
-        try:
-            self.nlp = pipeline("ner")
-            entities = self.nlp(text)
-            organized_entities = {}
-            for entity in entities:
-                if entity['entity'] not in organized_entities:
-                    organized_entities[entity['entity']] = []
-                organized_entities[entity['entity']].append(entity['word'])
-            return json.dumps(organized_entities)
-        except Exception as e:
-            raise e
-        finally:
+import json
+from transformers import pipeline, logging as hf_logging
+from ....standard.tools.base.ToolBase import ToolBase
+from ....standard.tools.concrete.Parameter import Parameter
+
+hf_logging.set_verbosity_error()
+
+class EntityRecognitionTool(ToolBase):
+    def __init__(self):
+        parameters = [
+            Parameter("text","string","The text for entity recognition",True)
+        ]
+        super().__init__(name="EntityRecognitionTool", 
+                         description="Extracts named entities from text", 
+                         parameters=parameters)
+        
+
+    def __call__(self, text: str) -> dict:
+        try:
+            self.nlp = pipeline("ner")
+            entities = self.nlp(text)
+            organized_entities = {}
+            for entity in entities:
+                if entity['entity'] not in organized_entities:
+                    organized_entities[entity['entity']] = []
+                organized_entities[entity['entity']].append(entity['word'])
+            return json.dumps(organized_entities)
+        except Exception as e:
+            raise e
+        finally:
             del self.nlp
```

### Comparing `swarmauri-0.1.80/swarmauri/community/tools/concrete/GmailReadTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailReadTool.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import os
-import base64
-import json
-from googleapiclient import discovery
-from google.oauth2 import service_account
-from googleapiclient.discovery import build
-from ....standard.tools.base.ToolBase import ToolBase
-from ....standard.tools.concrete.Parameter import Parameter
-
-class GmailReadTool(ToolBase):
-    SCOPES = ['https://www.googleapis.com/auth/gmail.readonly']
-
-    def __init__(self, credentials_path: str, sender_email: str):
-        """
-        Initializes the GmailReadTool with a path to the credentials JSON file.
-
-        Parameters:
-        credentials_path (str): The path to the Gmail service JSON file.
-        """
-        
-        parameters = [
-            Parameter(
-                name="query",
-                type="string",
-                description='''The query to filter emails. For example, "is:unread" or "from:example@gmail.com" or "from:sender@company.com"''',
-                required=True
-            ),
-            Parameter(
-                name="max_results",
-                type="integer",
-                description='''The number of emails to return. Defaults to 10.'''
-            )
-        ]
-        
-        
-        super().__init__(name="GmailReadTool", 
-                         description="Read emails from a Gmail account.", 
-                         parameters = parameters)
-        self.credentials_path = credentials_path
-        self.sender_email = sender_email
-        
-
-    def authenticate(self):
-        """
-        Authenticates the user and creates a Gmail API service.
-        """
-        credentials = service_account.Credentials.from_service_account_file(
-                self.credentials_path, scopes=self.SCOPES)
-        
-        delegated_credentials = credentials.with_subject(self.sender_email)
-        self.service = discovery.build('gmail', 'v1', credentials=delegated_credentials)
-
-
-
-    def __call__(self, query='', max_results=10):
-        """
-        Fetches emails from the authenticated Gmail account based on the given query.
-
-        Parameters:
-        query (str): The query to filter emails. For example, "is:unread".
-        max_results (int): The maximum number of email messages to fetch.
-
-        Returns:
-        list: A list of email messages.
-        """
-        self.authenticate()
-        try:
-            # Call the Gmail API
-            
-            gmail_messages = self.service.users().messages()
-            results = gmail_messages.list(userId='me', q=query, maxResults=max_results).execute()
-            messages = results.get('messages', [])
-            message_data = ""
-            for message in messages:
-                
-                msg = gmail_messages.get(userId='me', id=message['threadId'], format="full").execute()
-                headers = msg['payload']['headers']
-                
-                sender = next(header['value'] for header in headers if header['name'] == 'From')
-                subject = next(header['value'] for header in headers if header['name'] == 'Subject')
-                reply_to = next((header['value'] for header in headers if header['name'] == 'Reply-To'), subject)
-                date_time = next(header['value'] for header in headers if header['name'] == 'Date')
-                
-                #part = msg['payload']['parts'][0]
-                #data = part['body']['data']
-                #decoded_data = base64.urlsafe_b64decode(data.encode('ASCII'))
-
-                formatted_msg = f"\nsender:{sender} reply-to:{reply_to} subject: {subject} date_time:{date_time}"
-                
-                message_data += formatted_msg
-                
-            
-            return message_data
-        
-        
-        
-        except Exception as e:
-            print(f"An error occurred: {e}")
-            return []
-        
-        finally:
-            del self.service
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
+import os
+import base64
+import json
+from googleapiclient import discovery
+from google.oauth2 import service_account
+from googleapiclient.discovery import build
+from ....standard.tools.base.ToolBase import ToolBase
+from ....standard.tools.concrete.Parameter import Parameter
+
+class GmailReadTool(ToolBase):
+    SCOPES = ['https://www.googleapis.com/auth/gmail.readonly']
+
+    def __init__(self, credentials_path: str, sender_email: str):
+        """
+        Initializes the GmailReadTool with a path to the credentials JSON file.
+
+        Parameters:
+        credentials_path (str): The path to the Gmail service JSON file.
+        """
+        
+        parameters = [
+            Parameter(
+                name="query",
+                type="string",
+                description='''The query to filter emails. For example, "is:unread" or "from:example@gmail.com" or "from:sender@company.com"''',
+                required=True
+            ),
+            Parameter(
+                name="max_results",
+                type="integer",
+                description='''The number of emails to return. Defaults to 10.'''
+            )
+        ]
+        
+        
+        super().__init__(name="GmailReadTool", 
+                         description="Read emails from a Gmail account.", 
+                         parameters = parameters)
+        self.credentials_path = credentials_path
+        self.sender_email = sender_email
+        
+
+    def authenticate(self):
+        """
+        Authenticates the user and creates a Gmail API service.
+        """
+        credentials = service_account.Credentials.from_service_account_file(
+                self.credentials_path, scopes=self.SCOPES)
+        
+        delegated_credentials = credentials.with_subject(self.sender_email)
+        self.service = discovery.build('gmail', 'v1', credentials=delegated_credentials)
+
+
+
+    def __call__(self, query='', max_results=10):
+        """
+        Fetches emails from the authenticated Gmail account based on the given query.
+
+        Parameters:
+        query (str): The query to filter emails. For example, "is:unread".
+        max_results (int): The maximum number of email messages to fetch.
+
+        Returns:
+        list: A list of email messages.
+        """
+        self.authenticate()
+        try:
+            # Call the Gmail API
+            
+            gmail_messages = self.service.users().messages()
+            results = gmail_messages.list(userId='me', q=query, maxResults=max_results).execute()
+            messages = results.get('messages', [])
+            message_data = ""
+            for message in messages:
+                
+                msg = gmail_messages.get(userId='me', id=message['threadId'], format="full").execute()
+                headers = msg['payload']['headers']
+                
+                sender = next(header['value'] for header in headers if header['name'] == 'From')
+                subject = next(header['value'] for header in headers if header['name'] == 'Subject')
+                reply_to = next((header['value'] for header in headers if header['name'] == 'Reply-To'), subject)
+                date_time = next(header['value'] for header in headers if header['name'] == 'Date')
+                
+                #part = msg['payload']['parts'][0]
+                #data = part['body']['data']
+                #decoded_data = base64.urlsafe_b64decode(data.encode('ASCII'))
+
+                formatted_msg = f"\nsender:{sender} reply-to:{reply_to} subject: {subject} date_time:{date_time}"
+                
+                message_data += formatted_msg
+                
+            
+            return message_data
+        
+        
+        
+        except Exception as e:
+            print(f"An error occurred: {e}")
+            return []
+        
+        finally:
+            del self.service
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+
```

### Comparing `swarmauri-0.1.80/swarmauri/community/tools/concrete/GmailSendTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailSendTool.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import base64
-import json
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
-from googleapiclient import discovery
-from google.oauth2 import service_account
-from googleapiclient.discovery import build
-from swarmauri.standard.tools.base.ToolBase import ToolBase
-from swarmauri.standard.tools.concrete.Parameter import Parameter
-
-class GmailSendTool(ToolBase):
-    SCOPES = ['https://www.googleapis.com/auth/gmail.send']
-
-    def __init__(self, credentials_path: str, sender_email: str):
-        """
-        Initializes the GmailSendTool with a path to the credentials JSON file and the sender email.
-
-        Parameters:
-        credentials_path (str): The path to the Gmail service JSON file.
-        sender_email (str): The email address being used to send emails.
-        """
-        
-        parameters = [
-            Parameter(
-                name="recipients",
-                type="string",
-                description="The email addresses of the recipients, separated by commas",
-                required=True
-            ),
-            Parameter(
-                name="subject",
-                type="string",
-                description="The subject of the email",
-                required=True
-            ),
-            Parameter(
-                name="htmlMsg",
-                type="string",
-                description="The HTML message to be sent as the email body",
-                required=True
-            )
-        ]
-        
-        super().__init__(name="GmailSendTool", 
-                         description="Sends an email using the Gmail API.",
-                         parameters=parameters)
-        self.credentials_path = credentials_path
-        self.sender_email = sender_email
-        
-
-    def authenticate(self):
-        """
-        Authenticates the user and creates a Gmail API service for sending emails.
-        """
-        credentials = service_account.Credentials.from_service_account_file(
-                self.credentials_path, scopes=self.SCOPES)
-        
-        delegated_credentials = credentials.with_subject(self.sender_email)
-        self.service = build('gmail', 'v1', credentials=delegated_credentials)
-
-    def create_message(self, to: str, subject: str, message_text: str):
-        """
-        Create a MIMEText message for sending an email.
-
-        Parameters:
-        sender (str): The email address of the sender.
-        to (str): The email address of the recipient.
-        subject (str): The subject of the email.
-        message_text (str): The HTML body of the email.
-
-        Returns:
-        The created MIMEText message.
-        """
-        message = MIMEMultipart('alternative')
-        message['from'] = self.sender_email
-        message['to'] = to
-        message['subject'] = subject
-        mime_text = MIMEText(message_text, 'html')
-        message.attach(mime_text)
-        raw_message = base64.urlsafe_b64encode(message.as_string().encode('utf-8'))
-        return {'raw': raw_message.decode('utf-8')}
-
-    def __call__(self, recipients, subject, htmlMsg):
-        """
-        Sends an email to the specified recipients with the given subject and HTML message.
-        
-        Parameters:
-        sender (str): The email address of the sender.
-        recipients (str): The email address of the recipients, separated by commas.
-        subject (str): The subject of the email.
-        htmlMsg (str): The HTML content of the email body.
-
-        Returns:
-        The result of sending the email or an error message if the operation fails.
-        """
-        self.authenticate()
-        try:
-            message = self.create_message(recipients, subject, htmlMsg)
-            sent_message = (self.service.users().messages().send(userId='me', body=message).execute())
-            return f"Email sent successfully to {recipients}"
-
-        except Exception as e:
-            return f"An error occurred in sending the email: {e}"
-        finally:
+import base64
+import json
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+from googleapiclient import discovery
+from google.oauth2 import service_account
+from googleapiclient.discovery import build
+from swarmauri.standard.tools.base.ToolBase import ToolBase
+from swarmauri.standard.tools.concrete.Parameter import Parameter
+
+class GmailSendTool(ToolBase):
+    SCOPES = ['https://www.googleapis.com/auth/gmail.send']
+
+    def __init__(self, credentials_path: str, sender_email: str):
+        """
+        Initializes the GmailSendTool with a path to the credentials JSON file and the sender email.
+
+        Parameters:
+        credentials_path (str): The path to the Gmail service JSON file.
+        sender_email (str): The email address being used to send emails.
+        """
+        
+        parameters = [
+            Parameter(
+                name="recipients",
+                type="string",
+                description="The email addresses of the recipients, separated by commas",
+                required=True
+            ),
+            Parameter(
+                name="subject",
+                type="string",
+                description="The subject of the email",
+                required=True
+            ),
+            Parameter(
+                name="htmlMsg",
+                type="string",
+                description="The HTML message to be sent as the email body",
+                required=True
+            )
+        ]
+        
+        super().__init__(name="GmailSendTool", 
+                         description="Sends an email using the Gmail API.",
+                         parameters=parameters)
+        self.credentials_path = credentials_path
+        self.sender_email = sender_email
+        
+
+    def authenticate(self):
+        """
+        Authenticates the user and creates a Gmail API service for sending emails.
+        """
+        credentials = service_account.Credentials.from_service_account_file(
+                self.credentials_path, scopes=self.SCOPES)
+        
+        delegated_credentials = credentials.with_subject(self.sender_email)
+        self.service = build('gmail', 'v1', credentials=delegated_credentials)
+
+    def create_message(self, to: str, subject: str, message_text: str):
+        """
+        Create a MIMEText message for sending an email.
+
+        Parameters:
+        sender (str): The email address of the sender.
+        to (str): The email address of the recipient.
+        subject (str): The subject of the email.
+        message_text (str): The HTML body of the email.
+
+        Returns:
+        The created MIMEText message.
+        """
+        message = MIMEMultipart('alternative')
+        message['from'] = self.sender_email
+        message['to'] = to
+        message['subject'] = subject
+        mime_text = MIMEText(message_text, 'html')
+        message.attach(mime_text)
+        raw_message = base64.urlsafe_b64encode(message.as_string().encode('utf-8'))
+        return {'raw': raw_message.decode('utf-8')}
+
+    def __call__(self, recipients, subject, htmlMsg):
+        """
+        Sends an email to the specified recipients with the given subject and HTML message.
+        
+        Parameters:
+        sender (str): The email address of the sender.
+        recipients (str): The email address of the recipients, separated by commas.
+        subject (str): The subject of the email.
+        htmlMsg (str): The HTML content of the email body.
+
+        Returns:
+        The result of sending the email or an error message if the operation fails.
+        """
+        self.authenticate()
+        try:
+            message = self.create_message(recipients, subject, htmlMsg)
+            sent_message = (self.service.users().messages().send(userId='me', body=message).execute())
+            return f"Email sent successfully to {recipients}"
+
+        except Exception as e:
+            return f"An error occurred in sending the email: {e}"
+        finally:
             del self.service
```

### Comparing `swarmauri-0.1.80/swarmauri/community/tools/concrete/PaCMAP.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/PaCMAP.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from ....core.tools.ITool import ITool
-from ....standard.tools.concrete.Parameter import Parameter  # Update import path as necessary
-import numpy as np
-import pacmap  # Ensure pacmap is installed
-
-class PaCMAPTool(ITool):
-    """
-    A tool for applying the PaCMAP method for dimensionality reduction.
-    """
-
-    def __init__(self):
-        parameters = [
-            Parameter(
-                name="X",
-                type="object",
-                description="X (np.ndarray): The high-dimensional data points to reduce.",
-                required=True
-            ),
-            Parameter(
-                name="n_neighbors",
-                type="integer",
-                description="The size of local neighborhood (in terms of number of neighboring data points) used for manifold approximation.",
-                required=False
-            ),
-            Parameter(
-                name="n_components",
-                type="integer",
-                description="The dimension of the space into which to embed the data.",
-                required=True
-            ),
-            Parameter(
-                name="n_iterations",
-                type="integer",
-                description="The number of iterations used for optimization.",
-                required=False
-            )
-        ]
-        
-        super().__init__(name="PaCMAPTool", 
-                         description="Applies PaCMAP for dimensionality reduction.", 
-                         parameters=parameters)
-
-    def __call__(self, **kwargs) -> np.ndarray:
-        """
-        Applies the PaCMAP algorithm on the provided dataset.
-
-        Parameters:
-        - kwargs: Additional keyword arguments for the PaCMAP algorithm.
-
-        Returns:
-        - np.ndarray: The reduced dimension data points.
-        """
-        # Set default values for any unspecified parameters
-        X = kwargs.get('X')
-        n_neighbors = kwargs.get('n_neighbors', 30)
-        n_components = kwargs.get('n_components', 2)
-        n_iterations = kwargs.get('n_iterations', 500)
-        
-        # Instantiate the PaCMAP instance with specified parameters
-        embedder = pacmap.PaCMAP(n_neighbors=n_neighbors, n_components=n_components, 
-                                 n_iters=n_iterations, **kwargs)
-                                 
-        # Fit the model and transform the data
-        X_reduced = embedder.fit_transform(X)
-
+from ....core.tools.ITool import ITool
+from ....standard.tools.concrete.Parameter import Parameter  # Update import path as necessary
+import numpy as np
+import pacmap  # Ensure pacmap is installed
+
+class PaCMAPTool(ITool):
+    """
+    A tool for applying the PaCMAP method for dimensionality reduction.
+    """
+
+    def __init__(self):
+        parameters = [
+            Parameter(
+                name="X",
+                type="object",
+                description="X (np.ndarray): The high-dimensional data points to reduce.",
+                required=True
+            ),
+            Parameter(
+                name="n_neighbors",
+                type="integer",
+                description="The size of local neighborhood (in terms of number of neighboring data points) used for manifold approximation.",
+                required=False
+            ),
+            Parameter(
+                name="n_components",
+                type="integer",
+                description="The dimension of the space into which to embed the data.",
+                required=True
+            ),
+            Parameter(
+                name="n_iterations",
+                type="integer",
+                description="The number of iterations used for optimization.",
+                required=False
+            )
+        ]
+        
+        super().__init__(name="PaCMAPTool", 
+                         description="Applies PaCMAP for dimensionality reduction.", 
+                         parameters=parameters)
+
+    def __call__(self, **kwargs) -> np.ndarray:
+        """
+        Applies the PaCMAP algorithm on the provided dataset.
+
+        Parameters:
+        - kwargs: Additional keyword arguments for the PaCMAP algorithm.
+
+        Returns:
+        - np.ndarray: The reduced dimension data points.
+        """
+        # Set default values for any unspecified parameters
+        X = kwargs.get('X')
+        n_neighbors = kwargs.get('n_neighbors', 30)
+        n_components = kwargs.get('n_components', 2)
+        n_iterations = kwargs.get('n_iterations', 500)
+        
+        # Instantiate the PaCMAP instance with specified parameters
+        embedder = pacmap.PaCMAP(n_neighbors=n_neighbors, n_components=n_components, 
+                                 n_iters=n_iterations, **kwargs)
+                                 
+        # Fit the model and transform the data
+        X_reduced = embedder.fit_transform(X)
+
         return X_reduced
```

### Comparing `swarmauri-0.1.80/swarmauri/community/tools/concrete/SentimentAnalysisTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/SentimentAnalysisTool.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from transformers import pipeline
-from transformers import logging as hf_logging
-
-from ....standard.tools.base.ToolBase import ToolBase
-from ....standard.tools.concrete.Parameter import Parameter
-
-hf_logging.set_verbosity_error()
-
-class SentimentAnalysisTool(ToolBase):
-    def __init__(self):
-        super().__init__("SentimentAnalysisTool", 
-                         "Analyzes the sentiment of the given text.", 
-                         parameters=[
-                             Parameter("text", "string", "The text for sentiment analysis", True)
-                         ])
-        
-
-    def __call__(self, text: str) -> str:
-        try:
-            self.analyzer = pipeline("sentiment-analysis")
-            result = self.analyzer(text)
-            return result[0]['label']
-        except:
-            raise
-        finally:
+from transformers import pipeline
+from transformers import logging as hf_logging
+
+from ....standard.tools.base.ToolBase import ToolBase
+from ....standard.tools.concrete.Parameter import Parameter
+
+hf_logging.set_verbosity_error()
+
+class SentimentAnalysisTool(ToolBase):
+    def __init__(self):
+        super().__init__("SentimentAnalysisTool", 
+                         "Analyzes the sentiment of the given text.", 
+                         parameters=[
+                             Parameter("text", "string", "The text for sentiment analysis", True)
+                         ])
+        
+
+    def __call__(self, text: str) -> str:
+        try:
+            self.analyzer = pipeline("sentiment-analysis")
+            result = self.analyzer(text)
+            return result[0]['label']
+        except:
+            raise
+        finally:
             del self.analyzer
```

### Comparing `swarmauri-0.1.80/swarmauri/community/tools/concrete/WebScrapingTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/WebScrapingTool.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import requests
-from bs4 import BeautifulSoup
-from ....standard.tools.base.ToolBase import ToolBase
-from ....standard.tools.concrete.Parameter import Parameter
-
-class WebScrapingTool(ToolBase):
-    def __init__(self):
-        parameters = [
-            Parameter(
-                name="url",
-                type="string",
-                description="URL of the link, website, webpage, etc... to scrape",
-                required=True
-            ),
-            Parameter(
-                name="selector",
-                type="string",
-                description="CSS selector to target specific elements",
-                required=True
-            )
-        ]
-        
-        super().__init__(name="WebScrapingTool", 
-                         description="This is a web scraping tool that you can utilize to scrape links, websites, webpages, etc... This tool uses python's requests and BeautifulSoup libraries to parse a URL using a CSS to target specific elements.", 
-                         parameters=parameters)
-
-    def __call__(self, url: str, selector: str) -> str:
-        """
-        Fetches content from the specified URL and extracts elements based on the provided CSS selector.
-        
-        Args:
-            url (str): The URL of the webpage to scrape.
-            selector (str): CSS selector to target specific elements in the webpage.
-
-        Returns:
-            str: Extracted text from the selector or an error message.
-        """
-        try:
-            response = requests.get(url)
-            response.raise_for_status()  # Raises HTTPError for bad requests (4xx or 5xx)
-
-            html_content = response.content
-            soup = BeautifulSoup(html_content, 'html.parser')
-
-            elements = soup.select(selector)
-            extracted_text = '\n'.join([element.text for element in elements])
-            return extracted_text
-        except requests.RequestException as e:
-            return f"Request Exception: {str(e)}"
-        except Exception as e:
+import requests
+from bs4 import BeautifulSoup
+from ....standard.tools.base.ToolBase import ToolBase
+from ....standard.tools.concrete.Parameter import Parameter
+
+class WebScrapingTool(ToolBase):
+    def __init__(self):
+        parameters = [
+            Parameter(
+                name="url",
+                type="string",
+                description="URL of the link, website, webpage, etc... to scrape",
+                required=True
+            ),
+            Parameter(
+                name="selector",
+                type="string",
+                description="CSS selector to target specific elements",
+                required=True
+            )
+        ]
+        
+        super().__init__(name="WebScrapingTool", 
+                         description="This is a web scraping tool that you can utilize to scrape links, websites, webpages, etc... This tool uses python's requests and BeautifulSoup libraries to parse a URL using a CSS to target specific elements.", 
+                         parameters=parameters)
+
+    def __call__(self, url: str, selector: str) -> str:
+        """
+        Fetches content from the specified URL and extracts elements based on the provided CSS selector.
+        
+        Args:
+            url (str): The URL of the webpage to scrape.
+            selector (str): CSS selector to target specific elements in the webpage.
+
+        Returns:
+            str: Extracted text from the selector or an error message.
+        """
+        try:
+            response = requests.get(url)
+            response.raise_for_status()  # Raises HTTPError for bad requests (4xx or 5xx)
+
+            html_content = response.content
+            soup = BeautifulSoup(html_content, 'html.parser')
+
+            elements = soup.select(selector)
+            extracted_text = '\n'.join([element.text for element in elements])
+            return extracted_text
+        except requests.RequestException as e:
+            return f"Request Exception: {str(e)}"
+        except Exception as e:
             return f"Unexpected error: {str(e)}"
```

### Comparing `swarmauri-0.1.80/swarmauri/core/agent_apis/IAgentRouterCRUD.py` & `swarmauri-0.1.9/swarmauri/core/agent_apis/IAgentRouterCRUD.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from abc import ABC, abstractmethod
-from typing import Callable, Any, Dict
-
-class IAgentRouterCRUD(ABC):
-    """
-    Interface for managing API routes within a SwarmAgent.
-    """
-    
-    @abstractmethod
-    def create_route(self, path: str, method: str, handler: Callable[[Any], Any]) -> None:
-        """
-        Create a new route for the API.
-        
-        Parameters:
-        - path (str): The URL path for the route.
-        - method (str): The HTTP method (e.g., 'GET', 'POST').
-        - handler (Callable[[Any], Any]): The function that handles requests to this route.
-        """
-        pass
-    
-    @abstractmethod
-    def read_route(self, path: str, method: str) -> Dict:
-        """
-        Retrieve information about a specific route.
-        
-        Parameters:
-        - path (str): The URL path for the route.
-        - method (str): The HTTP method.
-        
-        Returns:
-        - Dict: Information about the route, including path, method, and handler.
-        """
-        pass
-    
-    @abstractmethod
-    def update_route(self, path: str, method: str, new_handler: Callable[[Any], Any]) -> None:
-        """
-        Update the handler function for an existing route.
-        
-        Parameters:
-        - path (str): The URL path for the route.
-        - method (str): The HTTP method.
-        - new_handler (Callable[[Any], Any]): The new function that handles requests to this route.
-        """
-        pass
-    
-    @abstractmethod
-    def delete_route(self, path: str, method: str) -> None:
-        """
-        Delete a specific route from the API.
-        
-        Parameters:
-        - path (str): The URL path for the route.
-        - method (str): The HTTP method.
-        """
+from abc import ABC, abstractmethod
+from typing import Callable, Any, Dict
+
+class IAgentRouterCRUD(ABC):
+    """
+    Interface for managing API routes within a SwarmAgent.
+    """
+    
+    @abstractmethod
+    def create_route(self, path: str, method: str, handler: Callable[[Any], Any]) -> None:
+        """
+        Create a new route for the API.
+        
+        Parameters:
+        - path (str): The URL path for the route.
+        - method (str): The HTTP method (e.g., 'GET', 'POST').
+        - handler (Callable[[Any], Any]): The function that handles requests to this route.
+        """
+        pass
+    
+    @abstractmethod
+    def read_route(self, path: str, method: str) -> Dict:
+        """
+        Retrieve information about a specific route.
+        
+        Parameters:
+        - path (str): The URL path for the route.
+        - method (str): The HTTP method.
+        
+        Returns:
+        - Dict: Information about the route, including path, method, and handler.
+        """
+        pass
+    
+    @abstractmethod
+    def update_route(self, path: str, method: str, new_handler: Callable[[Any], Any]) -> None:
+        """
+        Update the handler function for an existing route.
+        
+        Parameters:
+        - path (str): The URL path for the route.
+        - method (str): The HTTP method.
+        - new_handler (Callable[[Any], Any]): The new function that handles requests to this route.
+        """
+        pass
+    
+    @abstractmethod
+    def delete_route(self, path: str, method: str) -> None:
+        """
+        Delete a specific route from the API.
+        
+        Parameters:
+        - path (str): The URL path for the route.
+        - method (str): The HTTP method.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/chains/IChainStep.py` & `swarmauri-0.1.9/swarmauri/core/chains/IChainStep.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from typing import List, Dict, Any, Callable
-
-class IChainStep:
-    """
-    Represents a single step within an execution chain.
-    """
-    def __init__(self, 
-        key: str, 
-        method: Callable, 
-        args: List[Any] = None, 
-        kwargs: Dict[str, Any] = None, 
-        ref: str = None):
-        """
-        Initialize a chain step.
-
-        Args:
-            key (str): Unique key or identifier for the step.
-            method (Callable): The callable object (function or method) to execute in this step.
-            args (List[Any], optional): Positional arguments for the callable.
-            kwargs (Dict[str, Any], optional): Keyword arguments for the callable.
-            ref (str, optional): Reference to another component or context variable, if applicable.
-        """
-        self.key = key
-        self.method = method
-        self.args = args if args is not None else []
-        self.kwargs = kwargs if kwargs is not None else {}
+from typing import List, Dict, Any, Callable
+
+class IChainStep:
+    """
+    Represents a single step within an execution chain.
+    """
+    def __init__(self, key: str, method: Callable, args: List[Any] = None, kwargs: Dict[str, Any] = None, ref: str = None):
+        """
+        Initialize a chain step.
+
+        Args:
+            key (str): Unique key or identifier for the step.
+            method (Callable): The callable object (function or method) to execute in this step.
+            args (List[Any], optional): Positional arguments for the callable.
+            kwargs (Dict[str, Any], optional): Keyword arguments for the callable.
+            ref (str, optional): Reference to another component or context variable, if applicable.
+        """
+        self.key = key
+        self.method = method
+        self.args = args if args is not None else []
+        self.kwargs = kwargs if kwargs is not None else {}
         self.ref = ref
```

### Comparing `swarmauri-0.1.80/swarmauri/core/conversations/IConversation.py` & `swarmauri-0.1.9/swarmauri/core/conversations/IConversation.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from abc import ABC, abstractmethod
-from typing import List, Optional
-from ..messages.IMessage import IMessage
-
-class IConversation(ABC):
-    """
-    Interface for managing conversations, defining abstract methods for
-    adding messages, retrieving the latest message, getting all messages, and clearing history.
-    """
-
-    @property
-    def history(self) -> List[IMessage]:
-        """
-        Provides read-only access to the conversation history.
-        """
-        pass
-
-    @abstractmethod
-    def add_message(self, message: IMessage):
-        """
-        Adds a message to the conversation history.
-        """
-        pass
-
-    @abstractmethod
-    def get_last(self) -> Optional[IMessage]:
-        """
-        Retrieves the latest message from the conversation history.
-        """
-        pass
-
-    @abstractmethod
-    def clear_history(self) -> None:
-        """
-        Clears the conversation history.
-        """
-        pass
-
-    @abstractmethod
-    def as_dict(self) -> List[dict]:
-        """
-        Returns all messages from the conversation history as a list of dictionaries.
-        """
+from abc import ABC, abstractmethod
+from typing import List, Optional
+from ..messages.IMessage import IMessage
+
+class IConversation(ABC):
+    """
+    Interface for managing conversations, defining abstract methods for
+    adding messages, retrieving the latest message, getting all messages, and clearing history.
+    """
+
+    @property
+    def history(self) -> List[IMessage]:
+        """
+        Provides read-only access to the conversation history.
+        """
+        pass
+
+    @abstractmethod
+    def add_message(self, message: IMessage):
+        """
+        Adds a message to the conversation history.
+        """
+        pass
+
+    @abstractmethod
+    def get_last(self) -> Optional[IMessage]:
+        """
+        Retrieves the latest message from the conversation history.
+        """
+        pass
+
+    @abstractmethod
+    def clear_history(self) -> None:
+        """
+        Clears the conversation history.
+        """
+        pass
+
+    @abstractmethod
+    def as_dict(self) -> List[dict]:
+        """
+        Returns all messages from the conversation history as a list of dictionaries.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/conversations/ISystemContext.py` & `swarmauri-0.1.9/swarmauri/core/conversations/ISystemContext.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from abc import ABC, abstractmethod
-from typing import Optional
-from ..messages.IMessage import IMessage
-
-class ISystemContext(ABC):
-
-    @property
-    @abstractmethod
-    def system_context(self) -> Optional[IMessage]:
-        """
-        An abstract property to get the system context message.
-        Subclasses must provide an implementation for storing and retrieving system context.
-        """
-        pass
-
-    @system_context.setter
-    @abstractmethod
-    def system_context(self, new_system_message: Optional[IMessage]) -> None:
-        """
-        An abstract property setter to update the system context.
-        Subclasses must provide an implementation for how the system context is updated.
-        This might be a direct string, which is converted to an IMessage instance, or directly an IMessage instance.
-        """
+from abc import ABC, abstractmethod
+from typing import Optional
+from ..messages.IMessage import IMessage
+
+class ISystemContext(ABC):
+
+    @property
+    @abstractmethod
+    def system_context(self) -> Optional[IMessage]:
+        """
+        An abstract property to get the system context message.
+        Subclasses must provide an implementation for storing and retrieving system context.
+        """
+        pass
+
+    @system_context.setter
+    @abstractmethod
+    def system_context(self, new_system_message: Optional[IMessage]) -> None:
+        """
+        An abstract property setter to update the system context.
+        Subclasses must provide an implementation for how the system context is updated.
+        This might be a direct string, which is converted to an IMessage instance, or directly an IMessage instance.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/distances/IDistanceSimilarity.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IDistanceSimilarity.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from abc import ABC, abstractmethod
-from typing import List
-from ..vectors.IVector import IVector
-
-class IDistanceSimilarity(ABC):
-    """
-    Interface for computing distances and similarities between high-dimensional data vectors. This interface
-    abstracts the method for calculating the distance and similarity, allowing for the implementation of various 
-    distance metrics such as Euclidean, Manhattan, Cosine similarity, etc.
-    """
-
-    @abstractmethod
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the distance between two vectors.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            float: The computed distance between vector_a and vector_b.
-        """
-        pass
-    
-
-    @abstractmethod
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> float:
-        pass
-
-
-    @abstractmethod
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Compute the similarity between two vectors. The definition of similarity (e.g., cosine similarity)
-        should be implemented in concrete classes.
-
-        Args:
-            vector_a (IVector): The first vector.
-            vector_b (IVector): The second vector to compare with the first vector.
-
-        Returns:
-            float: A similarity score between vector_a and vector_b.
-        """
-        pass
-
-    @abstractmethod
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> float:
-        pass
+from abc import ABC, abstractmethod
+from typing import List
+from ..vectors.IVector import IVector
+
+class IDistanceSimilarity(ABC):
+    """
+    Interface for computing distances and similarities between high-dimensional data vectors. This interface
+    abstracts the method for calculating the distance and similarity, allowing for the implementation of various 
+    distance metrics such as Euclidean, Manhattan, Cosine similarity, etc.
+    """
+
+    @abstractmethod
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the distance between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The computed distance between vector_a and vector_b.
+        """
+        pass
+    
+
+    @abstractmethod
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> float:
+        pass
+
+
+    @abstractmethod
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Compute the similarity between two vectors. The definition of similarity (e.g., cosine similarity)
+        should be implemented in concrete classes.
+
+        Args:
+            vector_a (IVector): The first vector.
+            vector_b (IVector): The second vector to compare with the first vector.
+
+        Returns:
+            float: A similarity score between vector_a and vector_b.
+        """
+        pass
+
+    @abstractmethod
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> float:
+        pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/document_stores/IDocumentRetrieve.py` & `swarmauri-0.1.9/swarmauri/core/retrievers/IRetriever.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from abc import ABC, abstractmethod
-from typing import List
-from swarmauri.core.documents.IDocument import IDocument
-
-class IDocumentRetrieve(ABC):
-    """
-    Abstract base class for document retrieval operations.
-    
-    This class defines the interface for retrieving documents based on a query or other criteria.
-    Implementations may use various indexing or search technologies to fulfill these retrievals.
-    """
-
-    @abstractmethod
-    def retrieve(self, query: str, top_k: int = 5) -> List[IDocument]:
-        """
-        Retrieve the most relevant documents based on the given query.
-        
-        Parameters:
-            query (str): The query string used for document retrieval.
-            top_k (int): The number of top relevant documents to retrieve.
-            
-        Returns:
-            List[Document]: A list of the top_k most relevant documents.
-        """
+from abc import ABC, abstractmethod
+from typing import List
+from ..documents.IDocument import IDocument
+
+class IRetriever(ABC):
+    """
+    Abstract base class for document retrieval operations.
+    
+    This class defines the interface for retrieving documents based on a query or other criteria.
+    Implementations may use various indexing or search technologies to fulfill these retrievals.
+    """
+
+    @abstractmethod
+    def retrieve(self, query: str, top_k: int = 5) -> List[IDocument]:
+        """
+        Retrieve the most relevant documents based on the given query.
+        
+        Parameters:
+            query (str): The query string used for document retrieval.
+            top_k (int): The number of top relevant documents to retrieve.
+            
+        Returns:
+            List[Document]: A list of the top_k most relevant documents.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/document_stores/IDocumentStore.py` & `swarmauri-0.1.9/swarmauri/standard/document_stores/base/DocumentStoreBase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,76 @@
-from abc import ABC, abstractmethod
-from typing import List, Union
-from swarmauri.core.documents.IDocument import IDocument
-
-class IDocumentStore(ABC):
-    """
-    Interface for a Document Store responsible for storing, indexing, and retrieving documents.
-    """
-
-    @abstractmethod
-    def add_document(self, document: IDocument) -> None:
-        """
-        Stores a single document in the document store.
-
-        Parameters:
-        - document (IDocument): The document to store.
-        """
-        pass
-
-    @abstractmethod
-    def add_documents(self, documents: List[IDocument]) -> None:
-        """
-        Stores multiple documents in the document store.
-
-        Parameters:
-        - documents (List[IDocument]): The list of documents to store.
-        """
-        pass
-
-    @abstractmethod
-    def get_document(self, doc_id: str) -> Union[IDocument, None]:
-        """
-        Retrieves a document by its ID.
-
-        Parameters:
-        - doc_id (str): The unique identifier for the document.
-
-        Returns:
-        - Union[IDocument, None]: The requested document, or None if not found.
-        """
-        pass
-
-    @abstractmethod
-    def get_all_documents(self) -> List[IDocument]:
-        """
-        Retrieves all documents stored in the document store.
-
-        Returns:
-        - List[IDocument]: A list of all documents.
-        """
-        pass
-
-    @abstractmethod
-    def delete_document(self, doc_id: str) -> None:
-        """
-        Deletes a document from the document store by its ID.
-
-        Parameters:
-        - doc_id (str): The unique identifier of the document to delete.
-        """
-        pass
-
-
-    @abstractmethod
-    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
-        """
-        Updates a document in the document store.
-
-        Parameters:
-        - doc_id (str): The unique identifier for the document to update.
-        - updated_document (IDocument): The updated document object.
-
-        Note: It's assumed that the updated_document will retain the same doc_id but may have different content or metadata.
-        """
-        pass
-
-    @abstractmethod
-    def document_count(self) -> int:
+from abc import ABC, abstractmethod
+from typing import List, Union, Optional
+from ....core.documents.IDocument import IDocument
+from ....core.document_stores.IDocumentStore import IDocumentStore
+
+class DocumentStoreBase(IDocumentStore, ABC):
+    """
+    Abstract base class for document stores, implementing the IDocumentStore interface.
+
+    This class provides a standard API for adding, updating, getting, and deleting documents in a store.
+    The specifics of storing (e.g., in a database, in-memory, or file system) are to be implemented by concrete subclasses.
+    """
+
+    @abstractmethod
+    def add_document(self, document: IDocument) -> None:
+        """
+        Add a single document to the document store.
+
+        Parameters:
+        - document (IDocument): The document to be added to the store.
+        """
+        pass
+
+    @abstractmethod
+    def add_documents(self, documents: List[IDocument]) -> None:
+        """
+        Add multiple documents to the document store in a batch operation.
+
+        Parameters:
+        - documents (List[IDocument]): A list of documents to be added to the store.
+        """
+        pass
+
+    @abstractmethod
+    def get_document(self, doc_id: str) -> Optional[IDocument]:
+        """
+        Retrieve a single document by its identifier.
+
+        Parameters:
+        - doc_id (str): The unique identifier of the document to retrieve.
+
+        Returns:
+        - Optional[IDocument]: The requested document if found; otherwise, None.
+        """
+        pass
+
+    @abstractmethod
+    def get_all_documents(self) -> List[IDocument]:
+        """
+        Retrieve all documents stored in the document store.
+
+        Returns:
+        - List[IDocument]: A list of all documents in the store.
+        """
+        pass
+
+    @abstractmethod
+    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
+        """
+        Update a document in the document store.
+
+        Parameters:
+        - doc_id (str): The unique identifier of the document to update.
+        - updated_document (IDocument): The updated document instance.
+        """
+        pass
+
+    @abstractmethod
+    def delete_document(self, doc_id: str) -> None:
+        """
+        Delete a document from the document store by its identifier.
+
+        Parameters:
+        - doc_id (str): The unique identifier of the document to delete.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/messages/IMessage.py` & `swarmauri-0.1.9/swarmauri/core/messages/IMessage.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from abc import ABC, abstractmethod
-
-class IMessage(ABC):
-    """
-    An abstract interface representing a general message structure.
-
-    This interface defines the basic attributes that all
-    messages should have, including type, name, and content, 
-    and requires subclasses to implement representation and formatting methods.
-    """
-    @property
-    @abstractmethod
-    def role(self) -> str:
-        pass
-    
-    @property
-    @abstractmethod
-    def content(self) -> str:
-        pass
-
-    @abstractmethod
-    def as_dict(self) -> dict:
-        """
-        An abstract method that subclasses must implement to return a dictionary representation of the object.
-        """
+from abc import ABC, abstractmethod
+
+class IMessage(ABC):
+    """
+    An abstract interface representing a general message structure.
+
+    This interface defines the basic attributes that all
+    messages should have, including type, name, and content, 
+    and requires subclasses to implement representation and formatting methods.
+    """
+    @property
+    @abstractmethod
+    def role(self) -> str:
+        pass
+    
+    @property
+    @abstractmethod
+    def content(self) -> str:
+        pass
+
+    @abstractmethod
+    def as_dict(self) -> dict:
+        """
+        An abstract method that subclasses must implement to return a dictionary representation of the object.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/parsers/IParser.py` & `swarmauri-0.1.9/swarmauri/core/parsers/IParser.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from abc import ABC, abstractmethod
-from typing import List, Union, Any
-from ..documents.IDocument import IDocument
-
-class IParser(ABC):
-    """
-    Abstract base class for parsers. It defines a public method to parse input data (str or Message) into documents,
-    and relies on subclasses to implement the specific parsing logic through protected and private methods.
-    """
-
-    @abstractmethod
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Public method to parse input data (either a str or a Message) into a list of Document instances.
-        
-        This method leverages the abstract _parse_data method which must be
-        implemented by subclasses to define specific parsing logic.
-        """
-        pass
-
+from abc import ABC, abstractmethod
+from typing import List, Union, Any
+from ..documents.IDocument import IDocument
+
+class IParser(ABC):
+    """
+    Abstract base class for parsers. It defines a public method to parse input data (str or Message) into documents,
+    and relies on subclasses to implement the specific parsing logic through protected and private methods.
+    """
+
+    @abstractmethod
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Public method to parse input data (either a str or a Message) into a list of Document instances.
+        
+        This method leverages the abstract _parse_data method which must be
+        implemented by subclasses to define specific parsing logic.
+        """
+        pass
+
```

### Comparing `swarmauri-0.1.80/swarmauri/core/toolkits/IToolkit.py` & `swarmauri-0.1.9/swarmauri/core/toolkits/IToolkit.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from typing import Dict
-from abc import ABC, abstractmethod
-from ..tools.ITool import ITool  # Ensure Tool is correctly imported from your tools package
-
-class IToolkit(ABC):
-    """
-    A class representing a toolkit used by Swarm Agents.
-    Tools are maintained in a dictionary keyed by the tool's name.
-    """
-
-    @property
-    @abstractmethod
-    def tools(self) -> Dict[str, ITool]:
-        """
-        An abstract property that should be implemented by subclasses to return the tools dictionary
-        """
-        pass
-
-    @abstractmethod
-    def add_tools(self, tools: Dict[str, ITool]):
-        """
-        An abstract method that should be implemented by subclasses to add multiple tools to the toolkit.
-        """
-        pass
-
-    @abstractmethod
-    def add_tool(self, tool: ITool):
-        """
-        An abstract method that should be implemented by subclasses to add a single tool to the toolkit.
-        """
-        pass
-
-    @abstractmethod
-    def remove_tool(self, tool_name: str):
-        """
-        An abstract method that should be implemented by subclasses to remove a tool from the toolkit by name.
-        """
-        pass
-
-    @abstractmethod
-    def get_tool_by_name(self, tool_name: str) -> ITool:
-        """
-        An abstract method that should be implemented by subclasses to retrieve a tool from the toolkit by name.
-        """
-        pass
-
-    @abstractmethod
-    def __len__(self) -> int:
-        """
-        An abstract method that should be implemented by subclasses to return the number of tools in the toolkit.
-        """
+from typing import Dict
+from abc import ABC, abstractmethod
+from ..tools.ITool import ITool  # Ensure Tool is correctly imported from your tools package
+
+class IToolkit(ABC):
+    """
+    A class representing a toolkit used by Swarm Agents.
+    Tools are maintained in a dictionary keyed by the tool's name.
+    """
+
+    @property
+    @abstractmethod
+    def tools(self) -> Dict[str, ITool]:
+        """
+        An abstract property that should be implemented by subclasses to return the tools dictionary
+        """
+        pass
+
+    @abstractmethod
+    def add_tools(self, tools: Dict[str, ITool]):
+        """
+        An abstract method that should be implemented by subclasses to add multiple tools to the toolkit.
+        """
+        pass
+
+    @abstractmethod
+    def add_tool(self, tool: ITool):
+        """
+        An abstract method that should be implemented by subclasses to add a single tool to the toolkit.
+        """
+        pass
+
+    @abstractmethod
+    def remove_tool(self, tool_name: str):
+        """
+        An abstract method that should be implemented by subclasses to remove a tool from the toolkit by name.
+        """
+        pass
+
+    @abstractmethod
+    def get_tool_by_name(self, tool_name: str) -> ITool:
+        """
+        An abstract method that should be implemented by subclasses to retrieve a tool from the toolkit by name.
+        """
+        pass
+
+    @abstractmethod
+    def __len__(self) -> int:
+        """
+        An abstract method that should be implemented by subclasses to return the number of tools in the toolkit.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/tools/IParameter.py` & `swarmauri-0.1.9/swarmauri/core/tools/IParameter.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from abc import ABC, abstractmethod
-from typing import Optional, List, Any
-
-class IParameter(ABC):
-    """
-    An abstract class to represent a parameter for a tool.
-    """
-
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """
-        Abstract property for getting the name of the parameter.
-        """
-        pass
-
-    @name.setter
-    @abstractmethod
-    def name(self, value: str):
-        """
-        Abstract setter for setting the name of the parameter.
-        """
-        pass
-
-    @property
-    @abstractmethod
-    def type(self) -> str:
-        """
-        Abstract property for getting the type of the parameter.
-        """
-        pass
-
-    @type.setter
-    @abstractmethod
-    def type(self, value: str):
-        """
-        Abstract setter for setting the type of the parameter.
-        """
-        pass
-
-    @property
-    @abstractmethod
-    def description(self) -> str:
-        """
-        Abstract property for getting the description of the parameter.
-        """
-        pass
-
-    @description.setter
-    @abstractmethod
-    def description(self, value: str):
-        """
-        Abstract setter for setting the description of the parameter.
-        """
-        pass
-
-    @property
-    @abstractmethod
-    def required(self) -> bool:
-        """
-        Abstract property for getting the required status of the parameter.
-        """
-        pass
-
-    @required.setter
-    @abstractmethod
-    def required(self, value: bool):
-        """
-        Abstract setter for setting the required status of the parameter.
-        """
-        pass
-
-    @property
-    @abstractmethod
-    def enum(self) -> Optional[List[Any]]:
-        """
-        Abstract property for getting the enum list of the parameter.
-        """
-        pass
-
-    @enum.setter
-    @abstractmethod
-    def enum(self, value: Optional[List[Any]]):
-        """
-        Abstract setter for setting the enum list of the parameter.
-        """
+from abc import ABC, abstractmethod
+from typing import Optional, List, Any
+
+class IParameter(ABC):
+    """
+    An abstract class to represent a parameter for a tool.
+    """
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """
+        Abstract property for getting the name of the parameter.
+        """
+        pass
+
+    @name.setter
+    @abstractmethod
+    def name(self, value: str):
+        """
+        Abstract setter for setting the name of the parameter.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def type(self) -> str:
+        """
+        Abstract property for getting the type of the parameter.
+        """
+        pass
+
+    @type.setter
+    @abstractmethod
+    def type(self, value: str):
+        """
+        Abstract setter for setting the type of the parameter.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def description(self) -> str:
+        """
+        Abstract property for getting the description of the parameter.
+        """
+        pass
+
+    @description.setter
+    @abstractmethod
+    def description(self, value: str):
+        """
+        Abstract setter for setting the description of the parameter.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def required(self) -> bool:
+        """
+        Abstract property for getting the required status of the parameter.
+        """
+        pass
+
+    @required.setter
+    @abstractmethod
+    def required(self, value: bool):
+        """
+        Abstract setter for setting the required status of the parameter.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def enum(self) -> Optional[List[Any]]:
+        """
+        Abstract property for getting the enum list of the parameter.
+        """
+        pass
+
+    @enum.setter
+    @abstractmethod
+    def enum(self, value: Optional[List[Any]]):
+        """
+        Abstract setter for setting the enum list of the parameter.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/tracing/IChainTracer.py` & `swarmauri-0.1.9/swarmauri/core/tracing/IChainTracer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from abc import ABC, abstractmethod
-from typing import Callable, List, Tuple, Dict, Any
-
-class IChainTracer(ABC):
-    """
-    Interface for a tracer supporting method chaining through a list of tuples.
-    Each tuple in the list contains: trace context, function, args, and kwargs.
-    """
-
-    @abstractmethod
-    def process_chain(self, chain: List[Tuple[Any, Callable[..., Any], List[Any], Dict[str, Any]]]) -> "IChainTracer":
-        """
-        Processes a sequence of operations defined in a chain.
-
-        Args:
-            chain (List[Tuple[Any, Callable[..., Any], List[Any], Dict[str, Any]]]): A list where each tuple contains:
-                - The trace context or reference required by the function.
-                - The function (method of IChainTracer) to execute.
-                - A list of positional arguments for the function.
-                - A dictionary of keyword arguments for the function.
-
-        Returns:
-            IChainTracer: Returns self to allow further method chaining.
-        """
+from abc import ABC, abstractmethod
+from typing import Callable, List, Tuple, Dict, Any
+
+class IChainTracer(ABC):
+    """
+    Interface for a tracer supporting method chaining through a list of tuples.
+    Each tuple in the list contains: trace context, function, args, and kwargs.
+    """
+
+    @abstractmethod
+    def process_chain(self, chain: List[Tuple[Any, Callable[..., Any], List[Any], Dict[str, Any]]]) -> "IChainTracer":
+        """
+        Processes a sequence of operations defined in a chain.
+
+        Args:
+            chain (List[Tuple[Any, Callable[..., Any], List[Any], Dict[str, Any]]]): A list where each tuple contains:
+                - The trace context or reference required by the function.
+                - The function (method of IChainTracer) to execute.
+                - A list of positional arguments for the function.
+                - A dictionary of keyword arguments for the function.
+
+        Returns:
+            IChainTracer: Returns self to allow further method chaining.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/tracing/ITraceContext.py` & `swarmauri-0.1.9/swarmauri/core/tracing/ITraceContext.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from abc import ABC, abstractmethod
-from typing import Any
-
-class ITraceContext(ABC):
-    """
-    Interface for a trace context, representing a single trace instance.
-    This context carries the state and metadata of the trace across different system components.
-    """
-
-    @abstractmethod
-    def get_trace_id(self) -> str:
-        """
-        Retrieves the unique identifier for this trace.
-
-        Returns:
-            str: The unique trace identifier.
-        """
-        pass
-
-    @abstractmethod
-    def add_attribute(self, key: str, value: Any):
-        """
-        Adds or updates an attribute associated with this trace.
-
-        Args:
-            key (str): The attribute key or name.
-            value (Any): The value of the attribute.
-        """
+from abc import ABC, abstractmethod
+from typing import Any
+
+class ITraceContext(ABC):
+    """
+    Interface for a trace context, representing a single trace instance.
+    This context carries the state and metadata of the trace across different system components.
+    """
+
+    @abstractmethod
+    def get_trace_id(self) -> str:
+        """
+        Retrieves the unique identifier for this trace.
+
+        Returns:
+            str: The unique trace identifier.
+        """
+        pass
+
+    @abstractmethod
+    def add_attribute(self, key: str, value: Any):
+        """
+        Adds or updates an attribute associated with this trace.
+
+        Args:
+            key (str): The attribute key or name.
+            value (Any): The value of the attribute.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/tracing/ITracer.py` & `swarmauri-0.1.9/swarmauri/core/tracing/ITracer.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from swarmauri.core.tracing.ITraceContext import ITraceContext
-from abc import ABC, abstractmethod
-from typing import Optional, Dict, Any
-
-
-class ITracer(ABC):
-    """
-    Interface for implementing distributed tracing across different components of the system.
-    """
-
-    @abstractmethod
-    def start_trace(self, name: str, initial_attributes: Optional[Dict[str, Any]] = None) -> ITraceContext:
-        """
-        Starts a new trace with a given name and optional initial attributes.
-
-        Args:
-            name (str): Name of the trace, usually represents the operation being traced.
-            initial_attributes (Optional[Dict[str, Any]]): Key-value pairs to be attached to the trace initially.
-
-        Returns:
-            ITraceContext: A context object representing this particular trace instance.
-        """
-        pass
-
-    @abstractmethod
-    def end_trace(self, trace_context: ITraceContext):
-        """
-        Marks the end of a trace, completing its lifecycle and recording its details.
-
-        Args:
-            trace_context (ITraceContext): The trace context to be ended.
-        """
-        pass
-
-    @abstractmethod
-    def annotate_trace(self, trace_context: ITraceContext, key: str, value: Any):
-        """
-        Adds an annotation to an existing trace, enriching it with more detailed information.
-
-        Args:
-            trace_context (ITraceContext): The trace context to annotate.
-            key (str): The key or name of the annotation.
-            value (Any): The value of the annotation.
-        """
+from swarmauri.core.tracing.ITraceContext import ITraceContext
+from abc import ABC, abstractmethod
+from typing import Optional, Dict, Any
+
+
+class ITracer(ABC):
+    """
+    Interface for implementing distributed tracing across different components of the system.
+    """
+
+    @abstractmethod
+    def start_trace(self, name: str, initial_attributes: Optional[Dict[str, Any]] = None) -> ITraceContext:
+        """
+        Starts a new trace with a given name and optional initial attributes.
+
+        Args:
+            name (str): Name of the trace, usually represents the operation being traced.
+            initial_attributes (Optional[Dict[str, Any]]): Key-value pairs to be attached to the trace initially.
+
+        Returns:
+            ITraceContext: A context object representing this particular trace instance.
+        """
+        pass
+
+    @abstractmethod
+    def end_trace(self, trace_context: ITraceContext):
+        """
+        Marks the end of a trace, completing its lifecycle and recording its details.
+
+        Args:
+            trace_context (ITraceContext): The trace context to be ended.
+        """
+        pass
+
+    @abstractmethod
+    def annotate_trace(self, trace_context: ITraceContext, key: str, value: Any):
+        """
+        Adds an annotation to an existing trace, enriching it with more detailed information.
+
+        Args:
+            trace_context (ITraceContext): The trace context to annotate.
+            key (str): The key or name of the annotation.
+            value (Any): The value of the annotation.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IDecompose.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IDecompose.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from abc import ABC, abstractmethod
-from typing import Tuple, List
-from swarmauri.core.vectors.IVector import IVector  # Assuming there's a base IVector interface for vector representations
-
-class IDecompose(ABC):
-    """
-    Interface for decomposing a vector into components along specified basis vectors.
-    This operation is essential in expressing a vector in different coordinate systems or reference frames.
-    """
-
-    @abstractmethod
-    def decompose(self, vector: IVector, basis_vectors: List[IVector]) -> List[IVector]:
-        """
-        Decompose the given vector into components along the specified basis vectors.
-
-        Parameters:
-        - vector (IVector): The vector to be decomposed.
-        - basis_vectors (List[IVector]): A list of basis vectors along which to decompose the given vector.
-
-        Returns:
-        - List[IVector]: A list of vectors, each representing the component of the decomposed vector along 
-                         the corresponding basis vector in the `basis_vectors` list.
-        """
+from abc import ABC, abstractmethod
+from typing import Tuple, List
+from .IVector import IVector  # Assuming there's a base IVector interface for vector representations
+
+class IDecompose(ABC):
+    """
+    Interface for decomposing a vector into components along specified basis vectors.
+    This operation is essential in expressing a vector in different coordinate systems or reference frames.
+    """
+
+    @abstractmethod
+    def decompose(self, vector: IVector, basis_vectors: List[IVector]) -> List[IVector]:
+        """
+        Decompose the given vector into components along the specified basis vectors.
+
+        Parameters:
+        - vector (IVector): The vector to be decomposed.
+        - basis_vectors (List[IVector]): A list of basis vectors along which to decompose the given vector.
+
+        Returns:
+        - List[IVector]: A list of vectors, each representing the component of the decomposed vector along 
+                         the corresponding basis vector in the `basis_vectors` list.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IDivergence.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IDivergence.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from abc import ABC, abstractmethod
-from typing import List
-
-class IDivergence(ABC):
-    """
-    Interface for calculating the divergence of a vector field.
-    """
-
-    @abstractmethod
-    def calculate_divergence(self, vector_field: List[List[float]], point: List[float]) -> float:
-        """
-        Calculate the divergence of a vector field at a specific point.
-
-        Parameters:
-        - vector_field (List[List[float]]): A representation of the vector field as a list of vectors.
-        - point (List[float]): The point at which the divergence is to be calculated.
-
-        Returns:
-        - float: The divergence value at the specified point.
-        """
+from abc import ABC, abstractmethod
+from typing import List
+
+class IDivergence(ABC):
+    """
+    Interface for calculating the divergence of a vector field.
+    """
+
+    @abstractmethod
+    def calculate_divergence(self, vector_field: List[List[float]], point: List[float]) -> float:
+        """
+        Calculate the divergence of a vector field at a specific point.
+
+        Parameters:
+        - vector_field (List[List[float]]): A representation of the vector field as a list of vectors.
+        - point (List[float]): The point at which the divergence is to be calculated.
+
+        Returns:
+        - float: The divergence value at the specified point.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IOrthogonalProject.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IProject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from abc import ABC, abstractmethod
-from typing import List
-
-class IOrthogonalProject(ABC):
-    """
-    Interface for calculating the orthogonal projection of one vector onto another.
-    """
-
-    @abstractmethod
-    def orthogonal_project(self, vector_a: List[float], vector_b: List[float]) -> List[float]:
-        """
-        Calculates the orthogonal projection of vector_a onto vector_b.
-        
-        Args:
-            vector_a (List[float]): The vector to be projected.
-            vector_b (List[float]): The vector onto which vector_a is orthogonally projected.
-        
-        Returns:
-            List[float]: The orthogonal projection of vector_a onto vector_b.
-        """
-        pass
+from abc import ABC, abstractmethod
+from typing import List
+
+class IProject(ABC):
+    """
+    Interface for projecting one vector onto another.
+    """
+
+    @abstractmethod
+    def project(self, vector_a: List[float], vector_b: List[float]) -> List[float]:
+        """
+        Projects vector_a onto vector_b.
+        
+        Args:
+            vector_a (List[float]): The vector to be projected.
+            vector_b (List[float]): The vector onto which vector_a is projected.
+        
+        Returns:
+            List[float]: The projection of vector_a onto vector_b.
+        """
+        pass
+
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IProject.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IOrthogonalProject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from abc import ABC, abstractmethod
-from typing import List
-
-class IProject(ABC):
-    """
-    Interface for projecting one vector onto another.
-    """
-
-    @abstractmethod
-    def project(self, vector_a: List[float], vector_b: List[float]) -> List[float]:
-        """
-        Projects vector_a onto vector_b.
-        
-        Args:
-            vector_a (List[float]): The vector to be projected.
-            vector_b (List[float]): The vector onto which vector_a is projected.
-        
-        Returns:
-            List[float]: The projection of vector_a onto vector_b.
-        """
-        pass
-
+from abc import ABC, abstractmethod
+from typing import List
+
+class IOrthogonalProject(ABC):
+    """
+    Interface for calculating the orthogonal projection of one vector onto another.
+    """
+
+    @abstractmethod
+    def orthogonal_project(self, vector_a: List[float], vector_b: List[float]) -> List[float]:
+        """
+        Calculates the orthogonal projection of vector_a onto vector_b.
+        
+        Args:
+            vector_a (List[float]): The vector to be projected.
+            vector_b (List[float]): The vector onto which vector_a is orthogonally projected.
+        
+        Returns:
+            List[float]: The orthogonal projection of vector_a onto vector_b.
+        """
+        pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IReflect.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IReflect.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from abc import ABC, abstractmethod
-from typing import List
-
-class IReflect(ABC):
-    """
-    Interface for reflecting a vector across a specified plane or axis.
-    """
-
-    @abstractmethod
-    def reflect_vector(self, vector: List[float], normal: List[float]) -> List[float]:
-        """
-        Reflects a vector across a plane or axis defined by a normal vector.
-
-        Parameters:
-        - vector (List[float]): The vector to be reflected.
-        - normal (List[float]): The normal vector of the plane across which the vector will be reflected.
-
-        Returns:
-        - List[float]: The reflected vector.
-        """
+from abc import ABC, abstractmethod
+from typing import List
+
+class IReflect(ABC):
+    """
+    Interface for reflecting a vector across a specified plane or axis.
+    """
+
+    @abstractmethod
+    def reflect_vector(self, vector: List[float], normal: List[float]) -> List[float]:
+        """
+        Reflects a vector across a plane or axis defined by a normal vector.
+
+        Parameters:
+        - vector (List[float]): The vector to be reflected.
+        - normal (List[float]): The normal vector of the plane across which the vector will be reflected.
+
+        Returns:
+        - List[float]: The reflected vector.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorArithmetic.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorArithmetic.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from abc import ABC, abstractmethod
-from typing import List
-
-class IVectorArithmetic(ABC):
-    @abstractmethod
-    def add(self, vector1: List[float], vector2: List[float]) -> List[float]:
-        """
-        Vector addition of 'vector1' and 'vector2'.
-        """
-        pass
-        
-    @abstractmethod
-    def subtract(self, vector1: List[float], vector2: List[float]) -> List[float]:
-        """
-        Vector subtraction of 'vector1' - 'vector2'.
-        """
-        pass
-   
-    @abstractmethod
-    def multiply(self, vector: List[float], scalar: float) -> List[float]:
-        """
-        Scalar multiplication of 'vector' by 'scalar'.
-        """
-        pass
-        
-    @abstractmethod
-    def divide(self, vector: List[float], scalar: float) -> List[float]:
-        """
-        Scalar division of 'vector' by 'scalar'.
-        """
+from abc import ABC, abstractmethod
+from typing import List
+
+class IVectorArithmetic(ABC):
+    @abstractmethod
+    def add(self, vector1: List[float], vector2: List[float]) -> List[float]:
+        """
+        Vector addition of 'vector1' and 'vector2'.
+        """
+        pass
+        
+    @abstractmethod
+    def subtract(self, vector1: List[float], vector2: List[float]) -> List[float]:
+        """
+        Vector subtraction of 'vector1' - 'vector2'.
+        """
+        pass
+   
+    @abstractmethod
+    def multiply(self, vector: List[float], scalar: float) -> List[float]:
+        """
+        Scalar multiplication of 'vector' by 'scalar'.
+        """
+        pass
+        
+    @abstractmethod
+    def divide(self, vector: List[float], scalar: float) -> List[float]:
+        """
+        Scalar division of 'vector' by 'scalar'.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorNorm.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorNorm.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# core/vectors/IVectorNorm.py
-
-from abc import ABC, abstractmethod
-from typing import List, Union
-
-class IVectorNorm(ABC):
-    """
-    Interface for calculating vector norms.
-    Supports L1 norm, L2 norm, and Max norm calculations.
-    """
-
-    @abstractmethod
-    def l1_norm(self, vector: List[Union[int, float]]) -> float:
-        """
-        Calculate the L1 norm (Manhattan norm) of a vector.
-
-        Parameters:
-        - vector (List[Union[int, float]]): The vector for which to calculate the L1 norm.
-
-        Returns:
-        - float: The L1 norm of the vector.
-        """
-        pass
-
-    @abstractmethod
-    def l2_norm(self, vector: List[Union[int, float]]) -> float:
-        """
-        Calculate the L2 norm (Euclidean norm) of a vector.
-
-        Parameters:
-        - vector (List[Union[int, float]]): The vector for which to calculate the L2 norm.
-
-        Returns:
-        - float: The L2 norm of the vector.
-        """
-        pass
-
-    @abstractmethod
-    def max_norm(self, vector: List[Union[int, float]]) -> float:
-        """
-        Calculate the Max norm (infinity norm) of a vector.
-
-        Parameters:
-        - vector (List[Union[int, float]]): The vector for which to calculate the Max norm.
-
-        Returns:
-        - float: The Max norm of the vector.
-        """
+# core/vectors/IVectorNorm.py
+
+from abc import ABC, abstractmethod
+from typing import List, Union
+
+class IVectorNorm(ABC):
+    """
+    Interface for calculating vector norms.
+    Supports L1 norm, L2 norm, and Max norm calculations.
+    """
+
+    @abstractmethod
+    def l1_norm(self, vector: List[Union[int, float]]) -> float:
+        """
+        Calculate the L1 norm (Manhattan norm) of a vector.
+
+        Parameters:
+        - vector (List[Union[int, float]]): The vector for which to calculate the L1 norm.
+
+        Returns:
+        - float: The L1 norm of the vector.
+        """
+        pass
+
+    @abstractmethod
+    def l2_norm(self, vector: List[Union[int, float]]) -> float:
+        """
+        Calculate the L2 norm (Euclidean norm) of a vector.
+
+        Parameters:
+        - vector (List[Union[int, float]]): The vector for which to calculate the L2 norm.
+
+        Returns:
+        - float: The L2 norm of the vector.
+        """
+        pass
+
+    @abstractmethod
+    def max_norm(self, vector: List[Union[int, float]]) -> float:
+        """
+        Calculate the Max norm (infinity norm) of a vector.
+
+        Parameters:
+        - vector (List[Union[int, float]]): The vector for which to calculate the Max norm.
+
+        Returns:
+        - float: The Max norm of the vector.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorRotate.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorRotate.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from abc import ABC, abstractmethod
-from typing import List
-
-class IRotate(ABC):
-    """
-    Interface for rotating a vector.
-    """
-    
-    @abstractmethod
-    def rotate(self, vector: List[float], angle: float, axis: List[float] = None) -> List[float]:
-        """
-        Rotate the given vector by a specified angle around an axis (for 3D) or in a plane (for 2D).
-
-        For 2D vectors, the axis parameter can be omitted.
-
-        Args:
-            vector (List[float]): The vector to rotate.
-            angle (float): The angle of rotation in degrees.
-            axis (List[float], optional): The axis of rotation (applicable in 3D).
-
-        Returns:
-            List[float]: The rotated vector.
-        """
-        pass
+from abc import ABC, abstractmethod
+from typing import List
+
+class IRotate(ABC):
+    """
+    Interface for rotating a vector.
+    """
+    
+    @abstractmethod
+    def rotate(self, vector: List[float], angle: float, axis: List[float] = None) -> List[float]:
+        """
+        Rotate the given vector by a specified angle around an axis (for 3D) or in a plane (for 2D).
+
+        For 2D vectors, the axis parameter can be omitted.
+
+        Args:
+            vector (List[float]): The vector to rotate.
+            angle (float): The angle of rotation in degrees.
+            axis (List[float], optional): The axis of rotation (applicable in 3D).
+
+        Returns:
+            List[float]: The rotated vector.
+        """
+        pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorSpan.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorSpan.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from abc import ABC, abstractmethod
-from typing import List, Any
-
-class IVectorSpan(ABC):
-    """
-    Interface for determining if a vector is within the span of a set of vectors.
-    """
-
-    @abstractmethod
-    def in_span(self, vector: Any, basis_vectors: List[Any]) -> bool:
-        """
-        Checks if the given vector is in the span of the provided basis vectors.
-
-        Parameters:
-        - vector (Any): The vector to check.
-        - basis_vectors (List[Any]): A list of vectors that might span the vector.
-
-        Returns:
-        - bool: True if the vector is in the span of the basis_vectors, False otherwise.
-        """
+from abc import ABC, abstractmethod
+from typing import List, Any
+
+class IVectorSpan(ABC):
+    """
+    Interface for determining if a vector is within the span of a set of vectors.
+    """
+
+    @abstractmethod
+    def in_span(self, vector: Any, basis_vectors: List[Any]) -> bool:
+        """
+        Checks if the given vector is in the span of the provided basis vectors.
+
+        Parameters:
+        - vector (Any): The vector to check.
+        - basis_vectors (List[Any]): A list of vectors that might span the vector.
+
+        Returns:
+        - bool: True if the vector is in the span of the basis_vectors, False otherwise.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vector_stores/IVectorStore.py` & `swarmauri-0.1.9/swarmauri/core/document_stores/IDocumentStore.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,75 @@
-from abc import ABC, abstractmethod
-from typing import List, Dict, Union
-from swarmauri.core.vectors.IVector import IVector
-from swarmauri.core.documents.IDocument import IDocument
-
-class IVectorStore(ABC):
-    """
-    Interface for a Document Store responsible for storing, indexing, and retrieving documents.
-    """
-
-    @abstractmethod
-    def add_document(self, document: IDocument) -> None:
-        """
-        Stores a single document in the document store.
-
-        Parameters:
-        - document (IDocument): The document to store.
-        """
-        pass
-
-    @abstractmethod
-    def add_documents(self, documents: List[IDocument]) -> None:
-        """
-        Stores multiple documents in the document store.
-
-        Parameters:
-        - documents (List[IDocument]): The list of documents to store.
-        """
-        pass
-
-    @abstractmethod
-    def get_document(self, doc_id: str) -> Union[IDocument, None]:
-        """
-        Retrieves a document by its ID.
-
-        Parameters:
-        - doc_id (str): The unique identifier for the document.
-
-        Returns:
-        - Union[IDocument, None]: The requested document, or None if not found.
-        """
-        pass
-
-    @abstractmethod
-    def get_all_documents(self) -> List[IDocument]:
-        """
-        Retrieves all documents stored in the document store.
-
-        Returns:
-        - List[IDocument]: A list of all documents.
-        """
-        pass
-
-    @abstractmethod
-    def delete_document(self, doc_id: str) -> None:
-        """
-        Deletes a document from the document store by its ID.
-
-        Parameters:
-        - doc_id (str): The unique identifier of the document to delete.
-        """
-        pass
-
-
-    @abstractmethod
-    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
-        """
-        Updates a document in the document store.
-
-        Parameters:
-        - doc_id (str): The unique identifier for the document to update.
-        - updated_document (IDocument): The updated document object.
-
-        Note: It's assumed that the updated_document will retain the same doc_id but may have different content or metadata.
-        """
-        pass
-
-    @abstractmethod
-    def document_count(self) -> int:
-        pass 
+from abc import ABC, abstractmethod
+from typing import List, Union
+from ..documents.IDocument import IDocument
+
+class IDocumentStore(ABC):
+    """
+    Interface for a Document Store responsible for storing, indexing, and retrieving documents.
+    """
+
+    @abstractmethod
+    def add_document(self, document: IDocument) -> None:
+        """
+        Stores a single document in the document store.
+
+        Parameters:
+        - document (IDocument): The document to store.
+        """
+        pass
+
+    @abstractmethod
+    def add_documents(self, documents: List[IDocument]) -> None:
+        """
+        Stores multiple documents in the document store.
+
+        Parameters:
+        - documents (List[IDocument]): The list of documents to store.
+        """
+        pass
+
+    @abstractmethod
+    def get_document(self, doc_id: str) -> Union[IDocument, None]:
+        """
+        Retrieves a document by its ID.
+
+        Parameters:
+        - doc_id (str): The unique identifier for the document.
+
+        Returns:
+        - Union[IDocument, None]: The requested document, or None if not found.
+        """
+        pass
+
+    @abstractmethod
+    def get_all_documents(self) -> List[IDocument]:
+        """
+        Retrieves all documents stored in the document store.
+
+        Returns:
+        - List[IDocument]: A list of all documents.
+        """
+        pass
+
+    @abstractmethod
+    def delete_document(self, doc_id: str) -> None:
+        """
+        Deletes a document from the document store by its ID.
+
+        Parameters:
+        - doc_id (str): The unique identifier of the document to delete.
+        """
+        pass
+
+
+    @abstractmethod
+    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
+        """
+        Updates a document in the document store.
+
+        Parameters:
+        - doc_id (str): The unique identifier for the document to update.
+        - updated_document (IDocument): The updated document object.
+
+        Note: It's assumed that the updated_document will retain the same doc_id but may have different content or metadata.
+        """
+        pass
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vectorizers/IVectorize.py` & `swarmauri-0.1.9/swarmauri/core/vectors/IVector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-from abc import ABC, abstractmethod
-from typing import List, Union, Any
-from swarmauri.core.vectors.IVector import IVector
-
-class IVectorize(ABC):
-    """
-    Interface for converting text to vectors. 
-    Implementations of this interface transform input text into numerical 
-    vectors that can be used in machine learning models, similarity calculations, 
-    and other vector-based operations.
-    """
-    @abstractmethod
-    def fit(self, data: Union[str, Any]) -> List[IVector]:
-        pass
-    
-    @abstractmethod
-    def transform(self, data: Union[str, Any]) -> List[IVector]:
-        pass
-
-    @abstractmethod
-    def fit_transform(self, data: Union[str, Any]) -> List[IVector]:
-        pass
-
-    @abstractmethod
-    def infer_vector(self, data: Union[str, Any], *args, **kwargs) -> IVector:
-        pass
+from abc import ABC, abstractmethod
+from typing import Any, Dict, List
+
+class IVector(ABC):
+    """
+    Interface for a high-dimensional data vector. This interface defines the
+    basic structure and operations for interacting with vectors in various applications,
+    such as machine learning, information retrieval, and similarity search.
+    """
+
+    @property
+    @abstractmethod
+    def data(self) -> List[float]:
+        """
+        The high-dimensional data that the vector represents. It is typically a list of float values.
+        """
+        pass
+
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vectors/IVectorMeta.py` & `swarmauri-0.1.9/swarmauri/core/vectors/IVectorMeta.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from abc import ABC, abstractmethod
-from typing import Any, Dict, List
-
-class IVectorMeta(ABC):
-    """
-    Interface for a high-dimensional data vector. This interface defines the
-    basic structure and operations for interacting with vectors in various applications,
-    such as machine learning, information retrieval, and similarity search.
-    """
-
-    @property
-    @abstractmethod
-    def id(self) -> str:
-        """
-        Unique identifier for the vector. This ID can be used to reference the vector
-        in a database or a vector store.
-        """
-        pass
-
-    @property
-    @abstractmethod
-    def metadata(self) -> Dict[str, Any]:
-        """
-        Optional metadata associated with the vector. Metadata can include additional information
-        useful for retrieval, categorization, or description of the vector data.
-        """
-        pass
-
+from abc import ABC, abstractmethod
+from typing import Any, Dict, List
+
+class IVectorMeta(ABC):
+    """
+    Interface for a high-dimensional data vector. This interface defines the
+    basic structure and operations for interacting with vectors in various applications,
+    such as machine learning, information retrieval, and similarity search.
+    """
+
+    @property
+    @abstractmethod
+    def id(self) -> str:
+        """
+        Unique identifier for the vector. This ID can be used to reference the vector
+        in a database or a vector store.
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def metadata(self) -> Dict[str, Any]:
+        """
+        Optional metadata associated with the vector. Metadata can include additional information
+        useful for retrieval, categorization, or description of the vector data.
+        """
+        pass
+
```

### Comparing `swarmauri-0.1.80/swarmauri/core/vectors/IVectorProduct.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorProduct.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from abc import ABC, abstractmethod
-from typing import List, Tuple
-
-class IVectorProduct(ABC):
-    """
-    Interface for various vector products including dot product, cross product,
-    and triple products (vector and scalar).
-    """
-
-    @abstractmethod
-    def dot_product(self, vector_a: List[float], vector_b: List[float]) -> float:
-        """
-        Calculate the dot product of two vectors.
-
-        Parameters:
-        - vector_a (List[float]): The first vector.
-        - vector_b (List[float]): The second vector.
-
-        Returns:
-        - float: The dot product of the two vectors.
-        """
-        pass
-
-    @abstractmethod
-    def cross_product(self, vector_a: List[float], vector_b: List[float]) -> List[float]:
-        """
-        Calculate the cross product of two vectors.
-
-        Parameters:
-        - vector_a (List[float]): The first vector.
-        - vector_b (List[float]): The second vector.
-
-        Returns:
-        - List[float]: The cross product as a new vector.
-        """
-        pass
-
-    @abstractmethod
-    def vector_triple_product(self, vector_a: List[float], vector_b: List[float], vector_c: List[float]) -> List[float]:
-        """
-        Calculate the vector triple product of three vectors.
-
-        Parameters:
-        - vector_a (List[float]): The first vector.
-        - vector_b (List[float]): The second vector.
-        - vector_c (List[float]): The third vector.
-
-        Returns:
-        - List[float]: The result of the vector triple product as a new vector.
-        """
-        pass
-
-    @abstractmethod
-    def scalar_triple_product(self, vector_a: List[float], vector_b: List[float], vector_c: List[float]) -> float:
-        """
-        Calculate the scalar triple product of three vectors.
-
-        Parameters:
-        - vector_a (List[float]): The first vector.
-        - vector_b (List[float]): The second vector.
-        - vector_c (List[float]): The third vector.
-
-        Returns:
-        - float: The scalar value result of the scalar triple product.
-        """
+from abc import ABC, abstractmethod
+from typing import List, Tuple
+
+class IVectorProduct(ABC):
+    """
+    Interface for various vector products including dot product, cross product,
+    and triple products (vector and scalar).
+    """
+
+    @abstractmethod
+    def dot_product(self, vector_a: List[float], vector_b: List[float]) -> float:
+        """
+        Calculate the dot product of two vectors.
+
+        Parameters:
+        - vector_a (List[float]): The first vector.
+        - vector_b (List[float]): The second vector.
+
+        Returns:
+        - float: The dot product of the two vectors.
+        """
+        pass
+
+    @abstractmethod
+    def cross_product(self, vector_a: List[float], vector_b: List[float]) -> List[float]:
+        """
+        Calculate the cross product of two vectors.
+
+        Parameters:
+        - vector_a (List[float]): The first vector.
+        - vector_b (List[float]): The second vector.
+
+        Returns:
+        - List[float]: The cross product as a new vector.
+        """
+        pass
+
+    @abstractmethod
+    def vector_triple_product(self, vector_a: List[float], vector_b: List[float], vector_c: List[float]) -> List[float]:
+        """
+        Calculate the vector triple product of three vectors.
+
+        Parameters:
+        - vector_a (List[float]): The first vector.
+        - vector_b (List[float]): The second vector.
+        - vector_c (List[float]): The third vector.
+
+        Returns:
+        - List[float]: The result of the vector triple product as a new vector.
+        """
+        pass
+
+    @abstractmethod
+    def scalar_triple_product(self, vector_a: List[float], vector_b: List[float], vector_c: List[float]) -> float:
+        """
+        Calculate the scalar triple product of three vectors.
+
+        Parameters:
+        - vector_a (List[float]): The first vector.
+        - vector_b (List[float]): The second vector.
+        - vector_c (List[float]): The third vector.
+
+        Returns:
+        - float: The scalar value result of the scalar triple product.
+        """
         pass
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/chains/ChainProcessingStrategy.py` & `swarmauri-0.1.9/swarmauri/experimental/chains/ChainProcessingStrategy.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import List, Any
-from swarmauri.core.chains.IChainProcessingStrategy import IChainProcessingStrategy
-from swarmauri.core.chains.IChainStep import IChainStep
-
-class ChainProcessingStrategy(IChainProcessingStrategy):
-    def execute_steps(self, steps: List[IChainStep]) -> Any:
-        """
-        Executes the given list of ordered chain steps based on the specific strategy 
-        and collects their results.
-
-        Args:
-            steps (List[IChainStep]): The ordered list of chain steps to be executed.
-        
-        Returns:
-            Any: The result of executing the steps. This could be tailored as per requirement.
-        """
-        results = []
-        for step in steps:
-            result = step.method(*step.args, **step.kwargs)
-            results.append(result)
+from typing import List, Any
+from swarmauri.core.chains.IChainProcessingStrategy import IChainProcessingStrategy
+from swarmauri.core.chains.IChainStep import IChainStep
+
+class ChainProcessingStrategy(IChainProcessingStrategy):
+    def execute_steps(self, steps: List[IChainStep]) -> Any:
+        """
+        Executes the given list of ordered chain steps based on the specific strategy 
+        and collects their results.
+
+        Args:
+            steps (List[IChainStep]): The ordered list of chain steps to be executed.
+        
+        Returns:
+            Any: The result of executing the steps. This could be tailored as per requirement.
+        """
+        results = []
+        for step in steps:
+            result = step.method(*step.args, **step.kwargs)
+            results.append(result)
         return results
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/chains/ChainProcessingStrategyBase.py` & `swarmauri-0.1.9/swarmauri/experimental/chains/ChainProcessingStrategyBase.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List
-from swarmauri.core.chains.IChainProcessingStrategy import IChainProcessingStrategy
-from swarmauri.core.chains.IChainStep import IChainStep
-
-class ChainProcessingStrategyBase(IChainProcessingStrategy):
-    """
-    A base implementation of the IChainProcessingStrategy interface.
-    """
-    
-    def execute_steps(self, steps: List[IChainStep]):
-        """
-        Default implementation which should be overridden by specific processing strategies.
-        """
-        for step in steps:
-            print(step)
+from typing import List
+from swarmauri.core.chains.IChainProcessingStrategy import IChainProcessingStrategy
+from swarmauri.core.chains.IChainStep import IChainStep
+
+class ChainProcessingStrategyBase(IChainProcessingStrategy):
+    """
+    A base implementation of the IChainProcessingStrategy interface.
+    """
+    
+    def execute_steps(self, steps: List[IChainStep]):
+        """
+        Default implementation which should be overridden by specific processing strategies.
+        """
+        for step in steps:
+            print(step)
             step.method(*step.args, **step.kwargs)
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/chains/MatrixOrderStrategy.py` & `swarmauri-0.1.9/swarmauri/experimental/chains/MatrixOrderStrategy.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import List
-from swarmauri.core.chains.IChainOrderStrategy import IChainOrderStrategy
-from swarmauri.core.chains.IChainStep import IChainStep
-
-class MatrixOrderStrategy(IChainOrderStrategy):
-    def order_steps(self, steps: List[IChainStep]) -> List[IChainStep]:
-        # Assuming 'steps' are already organized in a matrix-like structure
-        ordered_steps = self.arrange_matrix(steps)
-        return ordered_steps
-
-    def arrange_matrix(self, steps_matrix):
-        # Implement the logic to arrange/order steps based on matrix positions.
-        # This is just a placeholder. The actual implementation would depend on the matrix specifications and task dependencies.
+from typing import List
+from swarmauri.core.chains.IChainOrderStrategy import IChainOrderStrategy
+from swarmauri.core.chains.IChainStep import IChainStep
+
+class MatrixOrderStrategy(IChainOrderStrategy):
+    def order_steps(self, steps: List[IChainStep]) -> List[IChainStep]:
+        # Assuming 'steps' are already organized in a matrix-like structure
+        ordered_steps = self.arrange_matrix(steps)
+        return ordered_steps
+
+    def arrange_matrix(self, steps_matrix):
+        # Implement the logic to arrange/order steps based on matrix positions.
+        # This is just a placeholder. The actual implementation would depend on the matrix specifications and task dependencies.
         return steps_matrix
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/chains/TypeAgnosticCallableChain.py` & `swarmauri-0.1.9/swarmauri/experimental/chains/TypeAgnosticCallableChain.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from typing import Any, Callable, List, Dict, Optional, Tuple, Union
-
-CallableDefinition = Tuple[Callable, List[Any], Dict[str, Any], Union[str, Callable, None]]
-
-class TypeAgnosticCallableChain:
-    def __init__(self, callables: Optional[List[CallableDefinition]] = None):
-        self.callables = callables if callables is not None else []
-
-    @staticmethod
-    def _ignore_previous(_previous_result, *args, **kwargs):
-        return args, kwargs
-
-    @staticmethod
-    def _use_first_arg(previous_result, *args, **kwargs):
-        return [previous_result] + list(args), kwargs
-
-    @staticmethod
-    def _use_all_previous_args_first(previous_result, *args, **kwargs):
-        if not isinstance(previous_result, (list, tuple)):
-            previous_result = [previous_result]
-        return list(previous_result) + list(args), kwargs
-
-    @staticmethod
-    def _use_all_previous_args_only(previous_result, *_args, **_kwargs):
-        if not isinstance(previous_result, (list, tuple)):
-            previous_result = [previous_result]
-        return list(previous_result), {}
-
-    @staticmethod
-    def _add_previous_kwargs_overwrite(previous_result, args, kwargs):
-        if not isinstance(previous_result, dict):
-            raise ValueError("Previous result is not a dictionary.")
-        return args, {**kwargs, **previous_result}
-
-    @staticmethod
-    def _add_previous_kwargs_no_overwrite(previous_result, args, kwargs):
-        if not isinstance(previous_result, dict):
-            raise ValueError("Previous result is not a dictionary.")
-        return args, {**previous_result, **kwargs}
-
-    @staticmethod
-    def _use_all_args_all_kwargs_overwrite(previous_result_args, previous_result_kwargs, *args, **kwargs):
-        combined_args = list(previous_result_args) + list(args) if isinstance(previous_result_args, (list, tuple)) else list(args)
-        combined_kwargs = previous_result_kwargs if isinstance(previous_result_kwargs, dict) else {}
-        combined_kwargs.update(kwargs)
-        return combined_args, combined_kwargs
-
-    @staticmethod
-    def _use_all_args_all_kwargs_no_overwrite(previous_result_args, previous_result_kwargs, *args, **kwargs):
-        combined_args = list(previous_result_args) + list(args) if isinstance(previous_result_args, (list, tuple)) else list(args)
-        combined_kwargs = kwargs if isinstance(kwargs, dict) else {}
-        combined_kwargs = {**combined_kwargs, **(previous_result_kwargs if isinstance(previous_result_kwargs, dict) else {})}
-        return combined_args, combined_kwargs
-
-    def add_callable(self, func: Callable, args: List[Any] = None, kwargs: Dict[str, Any] = None, input_handler: Union[str, Callable, None] = None) -> None:
-        if isinstance(input_handler, str):
-            # Map the string to the corresponding static method
-            input_handler_method = getattr(self, f"_{input_handler}", None)
-            if input_handler_method is None:
-                raise ValueError(f"Unknown input handler name: {input_handler}")
-            input_handler = input_handler_method
-        elif input_handler is None:
-            input_handler = self._ignore_previous
-        self.callables.append((func, args or [], kwargs or {}, input_handler))
-
-    def __call__(self, *initial_args, **initial_kwargs) -> Any:
-        result = None
-        for func, args, kwargs, input_handler in self.callables:
-            if isinstance(input_handler, str):
-                # Map the string to the corresponding static method
-                input_handler_method = getattr(self, f"_{input_handler}", None)
-                if input_handler_method is None:
-                    raise ValueError(f"Unknown input handler name: {input_handler}")
-                input_handler = input_handler_method
-            elif input_handler is None:
-                input_handler = self._ignore_previous
-                
-            args, kwargs = input_handler(result, *args, **kwargs) if result is not None else (args, kwargs)
-            result = func(*args, **kwargs)
-        return result
-
-    def __or__(self, other: "TypeAgnosticCallableChain") -> "TypeAgnosticCallableChain":
-        if not isinstance(other, TypeAgnosticCallableChain):
-            raise TypeError("Operand must be an instance of TypeAgnosticCallableChain")
-        
-        new_chain = TypeAgnosticCallableChain(self.callables + other.callables)
+from typing import Any, Callable, List, Dict, Optional, Tuple, Union
+
+CallableDefinition = Tuple[Callable, List[Any], Dict[str, Any], Union[str, Callable, None]]
+
+class TypeAgnosticCallableChain:
+    def __init__(self, callables: Optional[List[CallableDefinition]] = None):
+        self.callables = callables if callables is not None else []
+
+    @staticmethod
+    def _ignore_previous(_previous_result, *args, **kwargs):
+        return args, kwargs
+
+    @staticmethod
+    def _use_first_arg(previous_result, *args, **kwargs):
+        return [previous_result] + list(args), kwargs
+
+    @staticmethod
+    def _use_all_previous_args_first(previous_result, *args, **kwargs):
+        if not isinstance(previous_result, (list, tuple)):
+            previous_result = [previous_result]
+        return list(previous_result) + list(args), kwargs
+
+    @staticmethod
+    def _use_all_previous_args_only(previous_result, *_args, **_kwargs):
+        if not isinstance(previous_result, (list, tuple)):
+            previous_result = [previous_result]
+        return list(previous_result), {}
+
+    @staticmethod
+    def _add_previous_kwargs_overwrite(previous_result, args, kwargs):
+        if not isinstance(previous_result, dict):
+            raise ValueError("Previous result is not a dictionary.")
+        return args, {**kwargs, **previous_result}
+
+    @staticmethod
+    def _add_previous_kwargs_no_overwrite(previous_result, args, kwargs):
+        if not isinstance(previous_result, dict):
+            raise ValueError("Previous result is not a dictionary.")
+        return args, {**previous_result, **kwargs}
+
+    @staticmethod
+    def _use_all_args_all_kwargs_overwrite(previous_result_args, previous_result_kwargs, *args, **kwargs):
+        combined_args = list(previous_result_args) + list(args) if isinstance(previous_result_args, (list, tuple)) else list(args)
+        combined_kwargs = previous_result_kwargs if isinstance(previous_result_kwargs, dict) else {}
+        combined_kwargs.update(kwargs)
+        return combined_args, combined_kwargs
+
+    @staticmethod
+    def _use_all_args_all_kwargs_no_overwrite(previous_result_args, previous_result_kwargs, *args, **kwargs):
+        combined_args = list(previous_result_args) + list(args) if isinstance(previous_result_args, (list, tuple)) else list(args)
+        combined_kwargs = kwargs if isinstance(kwargs, dict) else {}
+        combined_kwargs = {**combined_kwargs, **(previous_result_kwargs if isinstance(previous_result_kwargs, dict) else {})}
+        return combined_args, combined_kwargs
+
+    def add_callable(self, func: Callable, args: List[Any] = None, kwargs: Dict[str, Any] = None, input_handler: Union[str, Callable, None] = None) -> None:
+        if isinstance(input_handler, str):
+            # Map the string to the corresponding static method
+            input_handler_method = getattr(self, f"_{input_handler}", None)
+            if input_handler_method is None:
+                raise ValueError(f"Unknown input handler name: {input_handler}")
+            input_handler = input_handler_method
+        elif input_handler is None:
+            input_handler = self._ignore_previous
+        self.callables.append((func, args or [], kwargs or {}, input_handler))
+
+    def __call__(self, *initial_args, **initial_kwargs) -> Any:
+        result = None
+        for func, args, kwargs, input_handler in self.callables:
+            if isinstance(input_handler, str):
+                # Map the string to the corresponding static method
+                input_handler_method = getattr(self, f"_{input_handler}", None)
+                if input_handler_method is None:
+                    raise ValueError(f"Unknown input handler name: {input_handler}")
+                input_handler = input_handler_method
+            elif input_handler is None:
+                input_handler = self._ignore_previous
+                
+            args, kwargs = input_handler(result, *args, **kwargs) if result is not None else (args, kwargs)
+            result = func(*args, **kwargs)
+        return result
+
+    def __or__(self, other: "TypeAgnosticCallableChain") -> "TypeAgnosticCallableChain":
+        if not isinstance(other, TypeAgnosticCallableChain):
+            raise TypeError("Operand must be an instance of TypeAgnosticCallableChain")
+        
+        new_chain = TypeAgnosticCallableChain(self.callables + other.callables)
         return new_chain
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/conversations/ConsensusBuildingConversation.py` & `swarmauri-0.1.9/swarmauri/experimental/conversations/ConsensusBuildingConversation.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from swarmauri.core.conversations.IConversation import IConversation
-from swarmauri.core.messages.IMessage import IMessage
-
-
-class ConsensusBuildingMessage(IMessage):
-    def __init__(self, sender_id: str, content: str, message_type: str):
-        self._sender_id = sender_id
-        self._content = content
-        self._role = 'consensus_message'
-        self._message_type = message_type
-
-    @property
-    def role(self) -> str:
-        return self._role
-
-    @property
-    def content(self) -> str:
-        return self._content
-
-    def as_dict(self) -> dict:
-        return {
-            "sender_id": self._sender_id,
-            "content": self._content,
-            "message_type": self._message_type
-        }
-
-
-class ConsensusBuildingConversation(IConversation):
-    def __init__(self, topic: str, participants: list):
-        self.topic = topic
-        self.participants = participants  # List of agent IDs
-        self._history = []  # Stores all messages exchanged in the conversation
-        self.proposal_votes = {}  # Tracks votes for each proposal
-
-    @property
-    def history(self) -> list:
-        return self._history
-
-    def add_message(self, message: IMessage):
-        if not isinstance(message, ConsensusBuildingMessage):
-            raise ValueError("Only instances of ConsensusBuildingMessage are accepted")
-        self._history.append(message)
-
-    def get_last(self) -> IMessage:
-        if self._history:
-            return self._history[-1]
-        return None
-
-    def clear_history(self) -> None:
-        self._history.clear()
-
-    def as_dict(self) -> list:
-        return [message.as_dict() for message in self._history]
-
-    def initiate_consensus(self, initiator_id: str, proposal=None):
-        """Starts the conversation with an initial proposal, if any."""
-        initiate_message = ConsensusBuildingMessage(initiator_id, proposal, "InitiateConsensusMessage")
-        self.add_message(initiate_message)
-
-    def add_proposal(self, sender_id: str, proposal: str):
-        """Adds a proposal to the conversation."""
-        proposal_message = ConsensusBuildingMessage(sender_id, proposal, "ProposalMessage")
-        self.add_message(proposal_message)
-
-    def add_comment(self, sender_id: str, comment: str):
-        """Adds a comment or feedback regarding a proposal."""
-        comment_message = ConsensusBuildingMessage(sender_id, comment, "CommentMessage")
-        self.add_message(comment_message)
-
-    def vote(self, sender_id: str, vote: str):
-        """Registers a vote for a given proposal."""
-        vote_message = ConsensusBuildingMessage(sender_id, vote, "VoteMessage")
-        self.add_message(vote_message)
-        # Count the vote
-        self.proposal_votes[vote] = self.proposal_votes.get(vote, 0) + 1
-
-    def check_agreement(self):
-        """
-        Checks if there is a consensus on any proposal.
-        A simple majority (>50% of the participants) is required for consensus.
-        """
-        consensus_threshold = len(self.participants) / 2  # Define consensus as a simple majority
-
-        for proposal, votes in self.proposal_votes.items():
-            if votes > consensus_threshold:
-                # A consensus has been reached
-                return True, f"Consensus reached on proposal: {proposal} with {votes} votes."
-
-        # If no consensus is reached
+from swarmauri.core.conversations.IConversation import IConversation
+from swarmauri.core.messages.IMessage import IMessage
+
+
+class ConsensusBuildingMessage(IMessage):
+    def __init__(self, sender_id: str, content: str, message_type: str):
+        self._sender_id = sender_id
+        self._content = content
+        self._role = 'consensus_message'
+        self._message_type = message_type
+
+    @property
+    def role(self) -> str:
+        return self._role
+
+    @property
+    def content(self) -> str:
+        return self._content
+
+    def as_dict(self) -> dict:
+        return {
+            "sender_id": self._sender_id,
+            "content": self._content,
+            "message_type": self._message_type
+        }
+
+
+class ConsensusBuildingConversation(IConversation):
+    def __init__(self, topic: str, participants: list):
+        self.topic = topic
+        self.participants = participants  # List of agent IDs
+        self._history = []  # Stores all messages exchanged in the conversation
+        self.proposal_votes = {}  # Tracks votes for each proposal
+
+    @property
+    def history(self) -> list:
+        return self._history
+
+    def add_message(self, message: IMessage):
+        if not isinstance(message, ConsensusBuildingMessage):
+            raise ValueError("Only instances of ConsensusBuildingMessage are accepted")
+        self._history.append(message)
+
+    def get_last(self) -> IMessage:
+        if self._history:
+            return self._history[-1]
+        return None
+
+    def clear_history(self) -> None:
+        self._history.clear()
+
+    def as_dict(self) -> list:
+        return [message.as_dict() for message in self._history]
+
+    def initiate_consensus(self, initiator_id: str, proposal=None):
+        """Starts the conversation with an initial proposal, if any."""
+        initiate_message = ConsensusBuildingMessage(initiator_id, proposal, "InitiateConsensusMessage")
+        self.add_message(initiate_message)
+
+    def add_proposal(self, sender_id: str, proposal: str):
+        """Adds a proposal to the conversation."""
+        proposal_message = ConsensusBuildingMessage(sender_id, proposal, "ProposalMessage")
+        self.add_message(proposal_message)
+
+    def add_comment(self, sender_id: str, comment: str):
+        """Adds a comment or feedback regarding a proposal."""
+        comment_message = ConsensusBuildingMessage(sender_id, comment, "CommentMessage")
+        self.add_message(comment_message)
+
+    def vote(self, sender_id: str, vote: str):
+        """Registers a vote for a given proposal."""
+        vote_message = ConsensusBuildingMessage(sender_id, vote, "VoteMessage")
+        self.add_message(vote_message)
+        # Count the vote
+        self.proposal_votes[vote] = self.proposal_votes.get(vote, 0) + 1
+
+    def check_agreement(self):
+        """
+        Checks if there is a consensus on any proposal.
+        A simple majority (>50% of the participants) is required for consensus.
+        """
+        consensus_threshold = len(self.participants) / 2  # Define consensus as a simple majority
+
+        for proposal, votes in self.proposal_votes.items():
+            if votes > consensus_threshold:
+                # A consensus has been reached
+                return True, f"Consensus reached on proposal: {proposal} with {votes} votes."
+
+        # If no consensus is reached
         return False, "No consensus reached."
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/conversations/SemanticConversation.py` & `swarmauri-0.1.9/swarmauri/experimental/conversations/SemanticConversation.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from abc import ABC, abstractmethod
-from typing import Callable, Dict, Union
-from ...core.messages.IMessage import IMessage
-from ...core.conversations.IConversation import IConversation
-
-class SemanticConversation(IConversation, ABC):
-    """
-    A concrete implementation of the Conversation class that includes semantic routing.
-    Semantic routing involves analyzing the content of messages to understand their intent
-    or category and then routing them to appropriate handlers based on that analysis.
-
-    This class requires subclasses to implement the _analyze_message method for semantic analysis.
-    """
-
-
-    @abstractmethod
-    def register_handler(self, category: str, handler: Callable[[IMessage], None]):
-        """
-        Registers a message handler for a specific semantic category.
-
-        Args:
-            category (str): The category of messages this handler should process.
-            handler (Callable[[Message], None]): The function to call for messages of the specified category.
-        """
-        pass
-
-    @abstractmethod
-    def add_message(self, message: IMessage):
-        """
-        Adds a message to the conversation history and routes it to the appropriate handler based on its semantic category.
-
-        Args:
-            message (Message): The message to be added and processed.
-        """
-        pass
-
-    @abstractmethod
-    def _analyze_message(self, message: IMessage) -> Union[str, None]:
-        """
-        Analyzes the content of a message to determine its semantic category.
-
-        This method must be implemented by subclasses to provide specific logic for semantic analysis.
-
-        Args:
-            message (Message): The message to analyze.
-
-        Returns:
-            Union[str, None]: The semantic category of the message, if determined; otherwise, None.
-
-        Raises:
-            NotImplementedError: If the method is not overridden in a subclass.
-        """
-        raise NotImplementedError("Subclasses must implement the _analyze_message method to provide semantic analysis.")
-
+from abc import ABC, abstractmethod
+from typing import Callable, Dict, Union
+from ...core.messages.IMessage import IMessage
+from ...core.conversations.IConversation import IConversation
+
+class SemanticConversation(IConversation, ABC):
+    """
+    A concrete implementation of the Conversation class that includes semantic routing.
+    Semantic routing involves analyzing the content of messages to understand their intent
+    or category and then routing them to appropriate handlers based on that analysis.
+
+    This class requires subclasses to implement the _analyze_message method for semantic analysis.
+    """
+
+
+    @abstractmethod
+    def register_handler(self, category: str, handler: Callable[[IMessage], None]):
+        """
+        Registers a message handler for a specific semantic category.
+
+        Args:
+            category (str): The category of messages this handler should process.
+            handler (Callable[[Message], None]): The function to call for messages of the specified category.
+        """
+        pass
+
+    @abstractmethod
+    def add_message(self, message: IMessage):
+        """
+        Adds a message to the conversation history and routes it to the appropriate handler based on its semantic category.
+
+        Args:
+            message (Message): The message to be added and processed.
+        """
+        pass
+
+    @abstractmethod
+    def _analyze_message(self, message: IMessage) -> Union[str, None]:
+        """
+        Analyzes the content of a message to determine its semantic category.
+
+        This method must be implemented by subclasses to provide specific logic for semantic analysis.
+
+        Args:
+            message (Message): The message to analyze.
+
+        Returns:
+            Union[str, None]: The semantic category of the message, if determined; otherwise, None.
+
+        Raises:
+            NotImplementedError: If the method is not overridden in a subclass.
+        """
+        raise NotImplementedError("Subclasses must implement the _analyze_message method to provide semantic analysis.")
+
     # Additional methods as needed for message retrieval, history management, etc., inherited from Conversation
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/CanberraDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/MinkowskiDistance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,68 @@
-import numpy as np
-from typing import List
-from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-
-class CanberraDistance(IDistanceSimilarity):
-    """
-    Concrete implementation of the IDistanceSimiliarity interface using the Canberra distance metric.
-    This class now processes IVector instances instead of raw lists.
-    """
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Canberra distance between two IVector instances.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            float: The computed Canberra distance between the vectors.
-        """
-        # Extract data from IVector
-        data_a = np.array(vector_a.data)
-        data_b = np.array(vector_b.data)
-
-        # Checking dimensions match
-        if data_a.shape != data_b.shape:
-            raise ValueError("Vectors must have the same dimensionality.")
-
-        # Computing Canberra distance
-        distance = np.sum(np.abs(data_a - data_b) / (np.abs(data_a) + np.abs(data_b)))
-        # Handling the case where both vectors have a zero value for the same dimension
-        distance = np.nan_to_num(distance)
-        return distance
-    
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Compute similarity using the Canberra distance. Since this distance metric isn't
-        directly interpretable as a similarity, a transformation is applied to map the distance
-        to a similarity score.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector to compare with the first vector.
-
-        Returns:
-            float: A similarity score between vector_a and vector_b.
-        """
-        # One way to derive a similarity from distance is through inversion or transformation.
-        # Here we use an exponential decay based on the computed distance. This is a placeholder
-        # that assumes closer vectors (smaller distance) are more similar.
-        distance = self.distance(vector_a, vector_b)
-
-        # Transform the distance into a similarity score
-        similarity = np.exp(-distance)
-
-        return similarity
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
+from typing import List
+from scipy.spatial.distance import minkowski
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+class MinkowskiDistance(IDistanceSimilarity):
+    """
+    Implementation of the IDistanceSimiliarity interface using the Minkowski distance metric.
+    Minkowski distance is a generalized metric form that includes Euclidean distance,
+    Manhattan distance, and others depending on the order (p) parameter.
+
+    The class provides methods to compute the Minkowski distance between two vectors.
+    """
+
+    def __init__(self, p: int = 2):
+        """
+        Initializes the MinkowskiDistance calculator with the specified order.
+
+        Parameters:
+        - p (int): The order of the Minkowski distance. p=2 corresponds to the Euclidean distance,
+                   while p=1 corresponds to the Manhattan distance. Default is 2.
+        """
+        self.p = p
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Minkowski distance between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The computed Minkowski distance between vector_a and vector_b.
+        """
+        # Check if both vectors have the same dimensionality
+        if vector_a.dimensions != vector_b.dimensions:
+            raise ValueError("Vectors must have the same dimensionality.")
+
+        # Extract data from IVector instances
+        data_a = vector_a.data
+        data_b = vector_b.data
+
+        # Calculate and return the Minkowski distance
+        return minkowski(data_a, data_b, p=self.p)
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Compute the similarity between two vectors based on the Minkowski distance.
+        The similarity is inversely related to the distance.
+
+        Args:
+            vector_a (IVector): The first vector to compare for similarity.
+            vector_b (IVector): The second vector to compare with the first vector.
+
+        Returns:
+            float: A similarity score between vector_a and vector_b.
+        """
+        dist = self.distance(vector_a, vector_b)
+        return 1 / (1 + dist)  # An example similarity score
+    
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
         return similarities
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/ChebyshevDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/EuclideanDistance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-from typing import List
-from swarmauri.core.vectors.IVector import IVector
-from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
-
-class ChebyshevDistance(IDistanceSimilarity):
-    """
-    Concrete implementation of the IDistanceSimiliarity interface using the Chebyshev distance metric.
-    Chebyshev distance is the maximum absolute distance between two vectors' elements.
-    """
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Chebyshev distance between two vectors.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            float: The computed Chebyshev distance between vector_a and vector_b.
-        """
-        max_distance = 0
-        for a, b in zip(vector_a.data, vector_b.data):
-            max_distance = max(max_distance, abs(a - b))
-        return max_distance
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the similarity between two vectors based on the Chebyshev distance.
-
-        Args:
-            vector_a (IVector): The first vector.
-            vector_b (IVector): The second vector.
-
-        Returns:
-            float: The similarity score between the two vectors.
-        """
-
-        return 1 / (1 + self.distance(vector_a, vector_b))
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
+from math import sqrt
+from typing import List
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+
+class EuclideanDistance(IDistanceSimilarity):
+    """
+    Class to compute the Euclidean distance between two vectors.
+    Implements the IDistanceSimiliarity interface.
+    """
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Euclidean distance between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The computed Euclidean distance between vector_a and vector_b.
+        """
+        if len(vector_a.data) != len(vector_b.data):
+            raise ValueError("Vectors do not have the same dimensionality.")
+        
+        distance = sqrt(sum((a - b) ** 2 for a, b in zip(vector_a.data, vector_b.data)))
+        return distance
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the similarity score as the inverse of the Euclidean distance between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The similarity score between vector_a and vector_b.
+        """
+        distance = self.distance(vector_a, vector_b)
+        return 1 / (1 + distance)
+    
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
         return similarities
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/HaversineDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/HaversineDistance.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from typing import List
-from math import radians, cos, sin, sqrt, atan2
-from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-
-class HaversineDistance(IDistanceSimilarity):
-    """
-    Concrete implementation of IDistanceSimiliarity interface using the Haversine formula.
-    
-    Haversine formula determines the great-circle distance between two points on a sphere given their 
-    longitudes and latitudes. This implementation is particularly useful for geo-spatial data.
-    """ 
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Haversine distance between two geo-spatial points.
-
-        Args:
-            vector_a (IVector): The first point in the format [latitude, longitude].
-            vector_b (IVector): The second point in the same format [latitude, longitude].
-
-        Returns:
-            float: The Haversine distance between vector_a and vector_b in kilometers.
-        """
-        # Earth radius in kilometers
-        R = 6371.0
-
-        lat1, lon1 = map(radians, vector_a.data)
-        lat2, lon2 = map(radians, vector_b.data)
-
-        dlat = lat2 - lat1
-        dlon = lon2 - lon1
-
-        # Haversine formula
-        a = sin(dlat / 2)**2 + cos(lat1) * cos(lat2) * sin(dlon / 2)**2
-        c = 2 * atan2(sqrt(a), sqrt(1 - a))
-        distance = R * c
-
-        return distance
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        raise NotImplementedError("Similarity not implemented for Haversine distance.")
-        
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+from typing import List
+from math import radians, cos, sin, sqrt, atan2
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+
+class HaversineDistance(IDistanceSimilarity):
+    """
+    Concrete implementation of IDistanceSimiliarity interface using the Haversine formula.
+    
+    Haversine formula determines the great-circle distance between two points on a sphere given their 
+    longitudes and latitudes. This implementation is particularly useful for geo-spatial data.
+    """ 
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Haversine distance between two geo-spatial points.
+
+        Args:
+            vector_a (IVector): The first point in the format [latitude, longitude].
+            vector_b (IVector): The second point in the same format [latitude, longitude].
+
+        Returns:
+            float: The Haversine distance between vector_a and vector_b in kilometers.
+        """
+        # Earth radius in kilometers
+        R = 6371.0
+
+        lat1, lon1 = map(radians, vector_a.data)
+        lat2, lon2 = map(radians, vector_b.data)
+
+        dlat = lat2 - lat1
+        dlon = lon2 - lon1
+
+        # Haversine formula
+        a = sin(dlat / 2)**2 + cos(lat1) * cos(lat2) * sin(dlon / 2)**2
+        c = 2 * atan2(sqrt(a), sqrt(1 - a))
+        distance = R * c
+
+        return distance
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        raise NotImplementedError("Similarity not implemented for Haversine distance.")
+        
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
         raise NotImplementedError("Similarity not implemented for Haversine distance.")
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/ManhattanDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/ManhattanDistance.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import List
-from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-class ManhattanDistance(IDistanceSimilarity):
-    """
-    Concrete implementation of the IDistanceSimiliarity interface using the Manhattan distance.
-    
-    The Manhattan distance between two points is the sum of the absolute differences of their Cartesian coordinates.
-    This is also known as L1 distance.
-    """
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Manhattan distance between two vectors.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            float: The Manhattan distance between vector_a and vector_b.
-        """
-        if vector_a.dimensions != vector_b.dimensions:
-            raise ValueError("Vectors must have the same dimensionality.")
-        
-        return sum(abs(a - b) for a, b in zip(vector_a.data, vector_b.data))
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        The similarity based on Manhattan distance can be inversely related to the distance for some applications,
-        but this method intentionally returns NotImplementedError to signal that Manhattan distance is typically
-        not directly converted to similarity in the conventional sense used in this context.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            NotImplementedError: This is intended as this distance metric doesn't directly offer a similarity measure.
-        """
-        raise NotImplementedError("ManhattanDistance does not directly provide a similarity measure.")
-        
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+from typing import List
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+class ManhattanDistance(IDistanceSimilarity):
+    """
+    Concrete implementation of the IDistanceSimiliarity interface using the Manhattan distance.
+    
+    The Manhattan distance between two points is the sum of the absolute differences of their Cartesian coordinates.
+    This is also known as L1 distance.
+    """
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Manhattan distance between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The Manhattan distance between vector_a and vector_b.
+        """
+        if vector_a.dimensions != vector_b.dimensions:
+            raise ValueError("Vectors must have the same dimensionality.")
+        
+        return sum(abs(a - b) for a, b in zip(vector_a.data, vector_b.data))
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        The similarity based on Manhattan distance can be inversely related to the distance for some applications,
+        but this method intentionally returns NotImplementedError to signal that Manhattan distance is typically
+        not directly converted to similarity in the conventional sense used in this context.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            NotImplementedError: This is intended as this distance metric doesn't directly offer a similarity measure.
+        """
+        raise NotImplementedError("ManhattanDistance does not directly provide a similarity measure.")
+        
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
         raise NotImplementedError("ManhattanDistance does not directly provide a similarity measure.")
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/MinkowskiDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/CanberraDistance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-from typing import List
-from scipy.spatial.distance import minkowski
-from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-class MinkowskiDistance(IDistanceSimilarity):
-    """
-    Implementation of the IDistanceSimiliarity interface using the Minkowski distance metric.
-    Minkowski distance is a generalized metric form that includes Euclidean distance,
-    Manhattan distance, and others depending on the order (p) parameter.
-
-    The class provides methods to compute the Minkowski distance between two vectors.
-    """
-
-    def __init__(self, p: int = 2):
-        """
-        Initializes the MinkowskiDistance calculator with the specified order.
-
-        Parameters:
-        - p (int): The order of the Minkowski distance. p=2 corresponds to the Euclidean distance,
-                   while p=1 corresponds to the Manhattan distance. Default is 2.
-        """
-        self.p = p
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Minkowski distance between two vectors.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            float: The computed Minkowski distance between vector_a and vector_b.
-        """
-        # Check if both vectors have the same dimensionality
-        if vector_a.dimensions != vector_b.dimensions:
-            raise ValueError("Vectors must have the same dimensionality.")
-
-        # Extract data from IVector instances
-        data_a = vector_a.data
-        data_b = vector_b.data
-
-        # Calculate and return the Minkowski distance
-        return minkowski(data_a, data_b, p=self.p)
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Compute the similarity between two vectors based on the Minkowski distance.
-        The similarity is inversely related to the distance.
-
-        Args:
-            vector_a (IVector): The first vector to compare for similarity.
-            vector_b (IVector): The second vector to compare with the first vector.
-
-        Returns:
-            float: A similarity score between vector_a and vector_b.
-        """
-        dist = self.distance(vector_a, vector_b)
-        return 1 / (1 + dist)  # An example similarity score
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
+import numpy as np
+from typing import List
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+
+class CanberraDistance(IDistanceSimilarity):
+    """
+    Concrete implementation of the IDistanceSimiliarity interface using the Canberra distance metric.
+    This class now processes IVector instances instead of raw lists.
+    """
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Canberra distance between two IVector instances.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The computed Canberra distance between the vectors.
+        """
+        # Extract data from IVector
+        data_a = np.array(vector_a.data)
+        data_b = np.array(vector_b.data)
+
+        # Checking dimensions match
+        if data_a.shape != data_b.shape:
+            raise ValueError("Vectors must have the same dimensionality.")
+
+        # Computing Canberra distance
+        distance = np.sum(np.abs(data_a - data_b) / (np.abs(data_a) + np.abs(data_b)))
+        # Handling the case where both vectors have a zero value for the same dimension
+        distance = np.nan_to_num(distance)
+        return distance
+    
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Compute similarity using the Canberra distance. Since this distance metric isn't
+        directly interpretable as a similarity, a transformation is applied to map the distance
+        to a similarity score.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector to compare with the first vector.
+
+        Returns:
+            float: A similarity score between vector_a and vector_b.
+        """
+        # One way to derive a similarity from distance is through inversion or transformation.
+        # Here we use an exponential decay based on the computed distance. This is a placeholder
+        # that assumes closer vectors (smaller distance) are more similar.
+        distance = self.distance(vector_a, vector_b)
+
+        # Transform the distance into a similarity score
+        similarity = np.exp(-distance)
+
+        return similarity
+    
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
         return similarities
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/SSASimilarity.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSASimilarity.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from typing import Set, List, Dict
-from ....core.vector_stores.ISimilarity import ISimilarity
-from ....core.vectors.IVector import IVector
-
-
-class SSASimilarity(ISimilarity):
-    """
-    Implements the State Similarity in Arity (SSA) similarity measure to
-    compare states (sets of variables) for their similarity.
-    """
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Calculate the SSA similarity between two documents by comparing their metadata,
-        assumed to represent states as sets of variables.
-
-        Args:
-        - vector_a (IDocument): The first document.
-        - vector_b (IDocument): The second document to compare with the first document.
-
-        Returns:
-        - float: The SSA similarity measure between vector_a and vector_b, ranging from 0 to 1
-                 where 0 represents no similarity and 1 represents identical states.
-        """
-        state_a = set(vector_a.metadata.keys())
-        state_b = set(vector_b.metadata.keys())
-
-        return self.calculate_ssa(state_a, state_b)
-
-    @staticmethod
-    def calculate_ssa(state_a: Set[str], state_b: Set[str]) -> float:
-        """
-        Calculate the State Similarity in Arity (SSA) between two states.
-
-        Parameters:
-        - state_a (Set[str]): A set of variables representing state A.
-        - state_b (Set[str]): A set of variables representing state B.
-
-        Returns:6
-        - float: The SSA similarity measure, ranging from 0 (no similarity) to 1 (identical states).
-        """
-        # Calculate the intersection (shared variables) between the two states
-        shared_variables = state_a.intersection(state_b)
-        
-        # Calculate the union (total unique variables) of the two states
-        total_variables = state_a.union(state_b)
-        
-        # Calculate the SSA measure as the ratio of shared to total variables
-        ssa = len(shared_variables) / len(total_variables) if total_variables else 1
-        
+from typing import Set, List, Dict
+from ....core.vector_stores.ISimilarity import ISimilarity
+from ....core.vectors.IVector import IVector
+
+
+class SSASimilarity(ISimilarity):
+    """
+    Implements the State Similarity in Arity (SSA) similarity measure to
+    compare states (sets of variables) for their similarity.
+    """
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Calculate the SSA similarity between two documents by comparing their metadata,
+        assumed to represent states as sets of variables.
+
+        Args:
+        - vector_a (IDocument): The first document.
+        - vector_b (IDocument): The second document to compare with the first document.
+
+        Returns:
+        - float: The SSA similarity measure between vector_a and vector_b, ranging from 0 to 1
+                 where 0 represents no similarity and 1 represents identical states.
+        """
+        state_a = set(vector_a.metadata.keys())
+        state_b = set(vector_b.metadata.keys())
+
+        return self.calculate_ssa(state_a, state_b)
+
+    @staticmethod
+    def calculate_ssa(state_a: Set[str], state_b: Set[str]) -> float:
+        """
+        Calculate the State Similarity in Arity (SSA) between two states.
+
+        Parameters:
+        - state_a (Set[str]): A set of variables representing state A.
+        - state_b (Set[str]): A set of variables representing state B.
+
+        Returns:6
+        - float: The SSA similarity measure, ranging from 0 (no similarity) to 1 (identical states).
+        """
+        # Calculate the intersection (shared variables) between the two states
+        shared_variables = state_a.intersection(state_b)
+        
+        # Calculate the union (total unique variables) of the two states
+        total_variables = state_a.union(state_b)
+        
+        # Calculate the SSA measure as the ratio of shared to total variables
+        ssa = len(shared_variables) / len(total_variables) if total_variables else 1
+        
         return ssa
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/SSIVSimilarity.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSIVSimilarity.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from typing import List, Dict, Set
-from ....core.vector_stores.ISimilarity import ISimilarity
-
-class SSIVSimilarity(ISimilarity):
-    """
-    Concrete class that implements ISimilarity interface using
-    State Similarity of Important Variables (SSIV) as the similarity measure.
-    """
-
-    def similarity(self, state_a: Set[str], state_b: Set[str], importance_a: Dict[str, float], importance_b: Dict[str, float]) -> float:
-        """
-        Calculate the SSIV between two states represented by sets of variables.
-
-        Parameters:
-        - state_a (Set[str]): A set of variables representing state A.
-        - state_b (Set[str]): A set of variables representing state B.
-        - importance_a (Dict[str, float]): A dictionary where keys are variables in state A and values are their importance weights.
-        - importance_b (Dict[str, float]): A dictionary where keys are variables in state B and values are their importance weights.
-
-        Returns:
-        - float: The SSIV similarity measure, ranging from 0 to 1.
-        """
-        return self.calculate_ssiv(state_a, state_b, importance_a, importance_b)
-
-    @staticmethod
-    def calculate_ssiv(state_a: Set[str], state_b: Set[str], importance_a: Dict[str, float], importance_b: Dict[str, float]) -> float:
-        """
-        Calculate the State Similarity of Important Variables (SSIV) between two states.
-
-        Parameters:
-        - state_a (Set[str]): A set of variables representing state A.
-        - state_b (Set[str]): A set of variables representing state B.
-        - importance_a (Dict[str, float]): A dictionary where keys are variables in state A and values are their importance weights.
-        - importance_b (Dict[str, float]): A dictionary where keys are variables in state B and values are their importance weights.
-
-        Returns:
-        - float: The SSIV similarity measure, ranging from 0 to 1.
-        
-        Note: It is assumed that the importance weights are non-negative.
-        """
-        shared_variables = state_a.intersection(state_b)
-        
-        # Calculate the summed importance of shared variables
-        shared_importance_sum = sum(importance_a[var] for var in shared_variables) + sum(importance_b[var] for var in shared_variables)
-        
-        # Calculate the total importance of all variables in both states
-        total_importance_sum = sum(importance_a.values()) + sum(importance_b.values())
-        
-        # Calculate and return the SSIV
-        ssiv = (2 * shared_importance_sum) / total_importance_sum if total_importance_sum != 0 else 0
-        return ssiv
+from typing import List, Dict, Set
+from ....core.vector_stores.ISimilarity import ISimilarity
+
+class SSIVSimilarity(ISimilarity):
+    """
+    Concrete class that implements ISimilarity interface using
+    State Similarity of Important Variables (SSIV) as the similarity measure.
+    """
+
+    def similarity(self, state_a: Set[str], state_b: Set[str], importance_a: Dict[str, float], importance_b: Dict[str, float]) -> float:
+        """
+        Calculate the SSIV between two states represented by sets of variables.
+
+        Parameters:
+        - state_a (Set[str]): A set of variables representing state A.
+        - state_b (Set[str]): A set of variables representing state B.
+        - importance_a (Dict[str, float]): A dictionary where keys are variables in state A and values are their importance weights.
+        - importance_b (Dict[str, float]): A dictionary where keys are variables in state B and values are their importance weights.
+
+        Returns:
+        - float: The SSIV similarity measure, ranging from 0 to 1.
+        """
+        return self.calculate_ssiv(state_a, state_b, importance_a, importance_b)
+
+    @staticmethod
+    def calculate_ssiv(state_a: Set[str], state_b: Set[str], importance_a: Dict[str, float], importance_b: Dict[str, float]) -> float:
+        """
+        Calculate the State Similarity of Important Variables (SSIV) between two states.
+
+        Parameters:
+        - state_a (Set[str]): A set of variables representing state A.
+        - state_b (Set[str]): A set of variables representing state B.
+        - importance_a (Dict[str, float]): A dictionary where keys are variables in state A and values are their importance weights.
+        - importance_b (Dict[str, float]): A dictionary where keys are variables in state B and values are their importance weights.
+
+        Returns:
+        - float: The SSIV similarity measure, ranging from 0 to 1.
+        
+        Note: It is assumed that the importance weights are non-negative.
+        """
+        shared_variables = state_a.intersection(state_b)
+        
+        # Calculate the summed importance of shared variables
+        shared_importance_sum = sum(importance_a[var] for var in shared_variables) + sum(importance_b[var] for var in shared_variables)
+        
+        # Calculate the total importance of all variables in both states
+        total_importance_sum = sum(importance_a.values()) + sum(importance_b.values())
+        
+        # Calculate and return the SSIV
+        ssiv = (2 * shared_importance_sum) / total_importance_sum if total_importance_sum != 0 else 0
+        return ssiv
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/SorensenDiceDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SorensenDiceDistance.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import numpy as np
-from typing import List
-from collections import Counter
-
-from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-class SorensenDiceDistance(IDistanceSimilarity):
-    """
-    Implementing a concrete Vector Store class for calculating Sörensen-Dice Index Distance.
-    The Sörensen-Dice Index, or Dice's coefficient, is a measure of the similarity between two sets.
-    """
-
-    def distance(self, vector_a: List[float], vector_b: List[float]) -> float:
-        """
-        Compute the Sörensen-Dice distance between two vectors.
-        
-        Args:
-            vector_a (List[float]): The first vector in the comparison.
-            vector_b (List[float]): The second vector in the comparison.
-        
-        Returns:
-            float: The computed Sörensen-Dice distance between vector_a and vector_b.
-        """
-        # Convert vectors to binary sets
-        set_a = set([i for i, val in enumerate(vector_a) if val])
-        set_b = set([i for i, val in enumerate(vector_b) if val])
-        
-        # Calculate the intersection size
-        intersection_size = len(set_a.intersection(set_b))
-        
-        # Sorensen-Dice Index calculation
-        try:
-            sorensen_dice_index = (2 * intersection_size) / (len(set_a) + len(set_b))
-        except ZeroDivisionError:
-            sorensen_dice_index = 0.0
-        
-        # Distance is inverse of similarity for Sörensen-Dice
-        distance = 1 - sorensen_dice_index
-        
-        return distance
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarity(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        raise NotImplementedError("Similarity calculation is not implemented for SorensenDiceDistance.")
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+import numpy as np
+from typing import List
+from collections import Counter
+
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+class SorensenDiceDistance(IDistanceSimilarity):
+    """
+    Implementing a concrete Vector Store class for calculating Sörensen-Dice Index Distance.
+    The Sörensen-Dice Index, or Dice's coefficient, is a measure of the similarity between two sets.
+    """
+
+    def distance(self, vector_a: List[float], vector_b: List[float]) -> float:
+        """
+        Compute the Sörensen-Dice distance between two vectors.
+        
+        Args:
+            vector_a (List[float]): The first vector in the comparison.
+            vector_b (List[float]): The second vector in the comparison.
+        
+        Returns:
+            float: The computed Sörensen-Dice distance between vector_a and vector_b.
+        """
+        # Convert vectors to binary sets
+        set_a = set([i for i, val in enumerate(vector_a) if val])
+        set_b = set([i for i, val in enumerate(vector_b) if val])
+        
+        # Calculate the intersection size
+        intersection_size = len(set_a.intersection(set_b))
+        
+        # Sorensen-Dice Index calculation
+        try:
+            sorensen_dice_index = (2 * intersection_size) / (len(set_a) + len(set_b))
+        except ZeroDivisionError:
+            sorensen_dice_index = 0.0
+        
+        # Distance is inverse of similarity for Sörensen-Dice
+        distance = 1 - sorensen_dice_index
+        
+        return distance
+    
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarity(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        raise NotImplementedError("Similarity calculation is not implemented for SorensenDiceDistance.")
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
         raise NotImplementedError("Similarity calculation is not implemented for SorensenDiceDistance.")
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/distances/SquaredEuclideanDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/CosineDistance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,63 @@
-from typing import List
-from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-class SquaredEuclideanDistance(IDistanceSimilarity):
-    """
-    A concrete class for computing the squared Euclidean distance between two vectors.
-    """
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the squared Euclidean distance between vectors `vector_a` and `vector_b`.
-
-        Parameters:
-        - vector_a (IVector): The first vector in the comparison.
-        - vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-        - float: The computed squared Euclidean distance between vector_a and vector_b.
-        """
-        if vector_a.dimensions != vector_b.dimensions:
-            raise ValueError("Vectors must be of the same dimensionality.")
-
-        squared_distance = sum((a - b) ** 2 for a, b in zip(vector_a.data, vector_b.data))
-        return squared_distance
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Squared Euclidean distance is not used for calculating similarity.
-        
-        Parameters:
-        - vector_a (IVector): The first vector.
-        - vector_b (IVector): The second vector.
-
-        Raises:
-        - NotImplementedError: Indicates that similarity calculation is not implemented.
-        """
-        raise NotImplementedError("Similarity calculation is not implemented for Squared Euclidean distance.")
-        
-        
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        raise NotImplementedError("Similarity calculation is not implemented for Squared Euclidean distance.")
+from numpy.linalg import norm
+from typing import List
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+from swarmauri.standard.vector_stores.concrete.VectorProduct import VectorProduct
+
+class CosineDistance(IDistanceSimilarity, VectorProduct):
+    """
+    Implements cosine distance calculation as an IDistanceSimiliarity interface.
+    Cosine distance measures the cosine of the angle between two non-zero vectors
+    of an inner product space, capturing the orientation rather than the magnitude 
+    of these vectors.
+    """
+       
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """ 
+        Computes the cosine distance between two vectors: 1 - cosine similarity.
+    
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+    
+        Returns:
+            float: The computed cosine distance between vector_a and vector_b.
+                   It ranges from 0 (completely similar) to 2 (completely dissimilar).
+        """
+        norm_a = norm(vector_a.data)
+        norm_b = norm(vector_b.data)
+    
+        # Check if either of the vector norms is close to zero
+        if norm_a < 1e-10 or norm_b < 1e-10:
+            return 1.0  # Return maximum distance for cosine which varies between -1 to 1, so 1 indicates complete dissimilarity
+    
+        # Compute the cosine similarity between the vectors
+        cos_sim = self.dot_product(vector_a.data, vector_b.data) / (norm_a * norm_b)
+    
+        # Covert cosine similarity to cosine distance
+        cos_distance = 1 - cos_sim
+    
+        return cos_distance
+    
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the cosine similarity between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The cosine similarity between vector_a and vector_b.
+        """
+        return 1 - self.distance(vector_a, vector_b)
+
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
+        print(similarities)
+        return similarities
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/document_stores/Word2VecDocumentStore.py` & `swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/Word2VecDocumentStore.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from typing import List, Union, Optional
-import numpy as np
-from gensim.models import Word2Vec
-from swarmauri.core.document_stores.IDocumentStore import IDocumentStore
-from swarmauri.core.retrievers.IRetriever import IRetriever
-from swarmauri.standard.documents.concrete.EmbeddedDocument import EmbeddedDocument
-from swarmauri.standard.vector_stores.concrete.CosineDistance import CosineDistance
-from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
-import gensim.downloader as api
-
-class Word2VecDocumentStore(IDocumentStore, IRetriever):
-    def __init__(self):
-        """
-        Initializes the Word2VecDocumentStore.
-
-        Parameters:
-        - word2vec_model_path (Optional[str]): File path to a pre-trained Word2Vec model. 
-                                               Leave None to use Gensim's pre-trained model.
-        - pre_trained (bool): If True, loads a pre-trained Word2Vec model. If False, an uninitialized model is used that requires further training.
-        """
-        self.model = Word2Vec(vector_size=100, window=5, min_count=1, workers=4)  # Example parameters; adjust as needed
-        self.documents = []
-        self.metric = CosineDistance()
-
-    def add_document(self, document: EmbeddedDocument) -> None:
-        # Check if the document already has an embedding, if not generate one using _average_word_vectors
-        if not hasattr(document, 'embedding') or document.embedding is None:
-            words = document.content.split()  # Simple tokenization, consider using a better tokenizer
-            embedding = self._average_word_vectors(words)
-            document.embedding = embedding
-            print(document.embedding)
-        self.documents.append(document)
-        
-    def add_documents(self, documents: List[EmbeddedDocument]) -> None:
-        self.documents.extend(documents)
-        
-    def get_document(self, doc_id: str) -> Union[EmbeddedDocument, None]:
-        for document in self.documents:
-            if document.id == doc_id:
-                return document
-        return None
-        
-    def get_all_documents(self) -> List[EmbeddedDocument]:
-        return self.documents
-        
-    def delete_document(self, doc_id: str) -> None:
-        self.documents = [doc for doc in self.documents if doc.id != doc_id]
-
-    def update_document(self, doc_id: str, updated_document: EmbeddedDocument) -> None:
-        for i, document in enumerate(self.documents):
-            if document.id == doc_id:
-                self.documents[i] = updated_document
-                break
-
-    def _average_word_vectors(self, words: List[str]) -> np.ndarray:
-        """
-        Generate document vector by averaging its word vectors.
-        """
-        word_vectors = [self.model.wv[word] for word in words if word in self.model.wv]
-        print(word_vectors)
-        if word_vectors:
-            return np.mean(word_vectors, axis=0)
-        else:
-            return np.zeros(self.model.vector_size)
-
-    def retrieve(self, query: str, top_k: int = 5) -> List[EmbeddedDocument]:
-        """
-        Retrieve documents similar to the query string based on Word2Vec embeddings.
-        """
-        query_vector = self._average_word_vectors(query.split())
-        print('query_vector', query_vector)
-        # Compute similarity scores between the query and each document's stored embedding
-        similarities = self.metric.similarities(SimpleVector(query_vector), [SimpleVector(doc.embedding) for doc in self.documents if doc.embedding])
-        print('similarities', similarities)
-        # Retrieve indices of top_k most similar documents
-        top_k_indices = sorted(range(len(similarities)), key=lambda i: similarities[i], reverse=True)[:top_k]
-        print('top_k_indices', top_k_indices)
+from typing import List, Union, Optional
+import numpy as np
+from gensim.models import Word2Vec
+from swarmauri.core.document_stores.IDocumentStore import IDocumentStore
+from swarmauri.core.retrievers.IRetriever import IRetriever
+from swarmauri.standard.documents.concrete.EmbeddedDocument import EmbeddedDocument
+from swarmauri.standard.vector_stores.concrete.CosineDistance import CosineDistance
+from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
+import gensim.downloader as api
+
+class Word2VecDocumentStore(IDocumentStore, IRetriever):
+    def __init__(self):
+        """
+        Initializes the Word2VecDocumentStore.
+
+        Parameters:
+        - word2vec_model_path (Optional[str]): File path to a pre-trained Word2Vec model. 
+                                               Leave None to use Gensim's pre-trained model.
+        - pre_trained (bool): If True, loads a pre-trained Word2Vec model. If False, an uninitialized model is used that requires further training.
+        """
+        self.model = Word2Vec(vector_size=100, window=5, min_count=1, workers=4)  # Example parameters; adjust as needed
+        self.documents = []
+        self.metric = CosineDistance()
+
+    def add_document(self, document: EmbeddedDocument) -> None:
+        # Check if the document already has an embedding, if not generate one using _average_word_vectors
+        if not hasattr(document, 'embedding') or document.embedding is None:
+            words = document.content.split()  # Simple tokenization, consider using a better tokenizer
+            embedding = self._average_word_vectors(words)
+            document.embedding = embedding
+            print(document.embedding)
+        self.documents.append(document)
+        
+    def add_documents(self, documents: List[EmbeddedDocument]) -> None:
+        self.documents.extend(documents)
+        
+    def get_document(self, doc_id: str) -> Union[EmbeddedDocument, None]:
+        for document in self.documents:
+            if document.id == doc_id:
+                return document
+        return None
+        
+    def get_all_documents(self) -> List[EmbeddedDocument]:
+        return self.documents
+        
+    def delete_document(self, doc_id: str) -> None:
+        self.documents = [doc for doc in self.documents if doc.id != doc_id]
+
+    def update_document(self, doc_id: str, updated_document: EmbeddedDocument) -> None:
+        for i, document in enumerate(self.documents):
+            if document.id == doc_id:
+                self.documents[i] = updated_document
+                break
+
+    def _average_word_vectors(self, words: List[str]) -> np.ndarray:
+        """
+        Generate document vector by averaging its word vectors.
+        """
+        word_vectors = [self.model.wv[word] for word in words if word in self.model.wv]
+        print(word_vectors)
+        if word_vectors:
+            return np.mean(word_vectors, axis=0)
+        else:
+            return np.zeros(self.model.vector_size)
+
+    def retrieve(self, query: str, top_k: int = 5) -> List[EmbeddedDocument]:
+        """
+        Retrieve documents similar to the query string based on Word2Vec embeddings.
+        """
+        query_vector = self._average_word_vectors(query.split())
+        print('query_vector', query_vector)
+        # Compute similarity scores between the query and each document's stored embedding
+        similarities = self.metric.similarities(SimpleVector(query_vector), [SimpleVector(doc.embedding) for doc in self.documents if doc.embedding])
+        print('similarities', similarities)
+        # Retrieve indices of top_k most similar documents
+        top_k_indices = sorted(range(len(similarities)), key=lambda i: similarities[i], reverse=True)[:top_k]
+        print('top_k_indices', top_k_indices)
         return [self.documents[i] for i in top_k_indices]
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/models/HierarchicalAttentionModel.py` & `swarmauri-0.1.9/swarmauri/experimental/models/HierarchicalAttentionModel.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import tensorflow as tf
-from swarmauri.core.models.IModel import IModel
-from typing import Any
-
-class HierarchicalAttentionModel(IModel):
-    def __init__(self, model_name: str):
-        self._model_name = model_name
-        self._model = None  # This will hold the TensorFlow model with attention
-
-    @property
-    def model_name(self) -> str:
-        return self._model_name
-
-    @model_name.setter
-    def model_name(self, value: str) -> None:
-        self._model_name = value
-
-    def load_model(self) -> None:
-        """
-        Here, we define and compile the TensorFlow model described earlier.
-        """
-        # The following code is adapted from the attention model example provided earlier
-        vocab_size = 10000  # Size of the vocabulary
-        embedding_dim = 256  # Dimension of the embedding layer
-        sentence_length = 100  # Max length of a sentence
-        num_sentences = 10  # Number of sentences in a document
-        units = 128  # Dimensionality of the output space of GRU
-        
-        # Word-level attention layer
-        word_input = tf.keras.layers.Input(shape=(sentence_length,), dtype='int32')
-        embedded_word = tf.keras.layers.Embedding(vocab_size, embedding_dim)(word_input)
-        word_gru = tf.keras.layers.Bidirectional(tf.keras.layers.GRU(units, return_sequences=True))(embedded_word)
-        word_attention_layer = tf.keras.layers.Attention(use_scale=True, return_attention_scores=True)
-        word_attention_output, word_attention_weights = word_attention_layer([word_gru, word_gru], return_attention_scores=True)
-        word_encoder_with_attention = tf.keras.Model(inputs=word_input, outputs=[word_attention_output, word_attention_weights])
-        
-        # Sentence-level attention layer
-        sentence_input = tf.keras.layers.Input(shape=(num_sentences, sentence_length), dtype='int32')
-        sentence_encoder_with_attention = tf.keras.layers.TimeDistributed(word_encoder_with_attention)(sentence_input)
-        sentence_gru = tf.keras.layers.Bidirectional(tf.keras.layers.GRU(units, return_sequences=True))(sentence_encoder_with_attention[0])
-        sentence_attention_layer = tf.keras.layers.Attention(use_scale=True, return_attention_scores=True)
-        sentence_attention_output, sentence_attention_weights = sentence_attention_layer([sentence_gru, sentence_gru], return_attention_scores=True)
-        doc_representation = tf.keras.layers.Dense(units, activation='tanh')(sentence_attention_output)
-        
-        # Classifier
-        classifier = tf.keras.layers.Dense(1, activation='sigmoid')(doc_representation)
-        
-        # The model
-        self._model = tf.keras.Model(inputs=sentence_input, outputs=[classifier, sentence_attention_weights])
-        self._model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
-
-    def predict(self, input_data: Any) -> Any:
-        """
-        Predict method to use the loaded model for making predictions.
-
-        This example assumes `input_data` is preprocessed appropriately for the model's expected input.
-        """
-        if self._model is None:
-            raise ValueError("Model is not loaded. Call `load_model` before prediction.")
-            
-        # Predicting with the model
-        predictions, attention_weights = self._model.predict(input_data)
-        
-        # Additional logic to handle and package the predictions and attention weights could be added here
-        
+import tensorflow as tf
+from swarmauri.core.models.IModel import IModel
+from typing import Any
+
+class HierarchicalAttentionModel(IModel):
+    def __init__(self, model_name: str):
+        self._model_name = model_name
+        self._model = None  # This will hold the TensorFlow model with attention
+
+    @property
+    def model_name(self) -> str:
+        return self._model_name
+
+    @model_name.setter
+    def model_name(self, value: str) -> None:
+        self._model_name = value
+
+    def load_model(self) -> None:
+        """
+        Here, we define and compile the TensorFlow model described earlier.
+        """
+        # The following code is adapted from the attention model example provided earlier
+        vocab_size = 10000  # Size of the vocabulary
+        embedding_dim = 256  # Dimension of the embedding layer
+        sentence_length = 100  # Max length of a sentence
+        num_sentences = 10  # Number of sentences in a document
+        units = 128  # Dimensionality of the output space of GRU
+        
+        # Word-level attention layer
+        word_input = tf.keras.layers.Input(shape=(sentence_length,), dtype='int32')
+        embedded_word = tf.keras.layers.Embedding(vocab_size, embedding_dim)(word_input)
+        word_gru = tf.keras.layers.Bidirectional(tf.keras.layers.GRU(units, return_sequences=True))(embedded_word)
+        word_attention_layer = tf.keras.layers.Attention(use_scale=True, return_attention_scores=True)
+        word_attention_output, word_attention_weights = word_attention_layer([word_gru, word_gru], return_attention_scores=True)
+        word_encoder_with_attention = tf.keras.Model(inputs=word_input, outputs=[word_attention_output, word_attention_weights])
+        
+        # Sentence-level attention layer
+        sentence_input = tf.keras.layers.Input(shape=(num_sentences, sentence_length), dtype='int32')
+        sentence_encoder_with_attention = tf.keras.layers.TimeDistributed(word_encoder_with_attention)(sentence_input)
+        sentence_gru = tf.keras.layers.Bidirectional(tf.keras.layers.GRU(units, return_sequences=True))(sentence_encoder_with_attention[0])
+        sentence_attention_layer = tf.keras.layers.Attention(use_scale=True, return_attention_scores=True)
+        sentence_attention_output, sentence_attention_weights = sentence_attention_layer([sentence_gru, sentence_gru], return_attention_scores=True)
+        doc_representation = tf.keras.layers.Dense(units, activation='tanh')(sentence_attention_output)
+        
+        # Classifier
+        classifier = tf.keras.layers.Dense(1, activation='sigmoid')(doc_representation)
+        
+        # The model
+        self._model = tf.keras.Model(inputs=sentence_input, outputs=[classifier, sentence_attention_weights])
+        self._model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
+
+    def predict(self, input_data: Any) -> Any:
+        """
+        Predict method to use the loaded model for making predictions.
+
+        This example assumes `input_data` is preprocessed appropriately for the model's expected input.
+        """
+        if self._model is None:
+            raise ValueError("Model is not loaded. Call `load_model` before prediction.")
+            
+        # Predicting with the model
+        predictions, attention_weights = self._model.predict(input_data)
+        
+        # Additional logic to handle and package the predictions and attention weights could be added here
+        
         return predictions, attention_weights
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/models/SageMaker.py` & `swarmauri-0.1.9/swarmauri/experimental/models/SageMaker.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import json
-import boto3
-from ...core.models.IModel import IModel
-
-
-class AWSSageMakerModel(IModel):
-    def __init__(self, access_key: str, secret_access_key: str, region_name: str, model_name: str):
-        """
-        Initialize the AWS SageMaker model with AWS credentials, region, and the model name.
-
-        Parameters:
-        - access_key (str): AWS access key ID.
-        - secret_access_key (str): AWS secret access key.
-        - region_name (str): The region where the SageMaker model is deployed.
-        - model_name (str): The name of the SageMaker model.
-        """
-        self.access_key = access_key
-        self.secret_access_key = secret_access_key
-        self.region_name = region_name
-        self.client = boto3.client('sagemaker-runtime',
-                                   aws_access_key_id=access_key,
-                                   aws_secret_access_key=secret_access_key,
-                                   region_name=region_name)
-        super().__init__(model_name)
-
-    def predict(self, payload: str, content_type: str='application/json') -> dict:
-        """
-        Generate predictions using the AWS SageMaker model.
-
-        Parameters:
-        - payload (str): Input data in JSON format.
-        - content_type (str): The MIME type of the input data (default: 'application/json').
-        
-        Returns:
-        - dict: The predictions returned by the model.
-        """
-        endpoint_name = self.model_name  # Assuming the model name is also the endpoint name
-        response = self.client.invoke_endpoint(EndpointName=endpoint_name,
-                                               Body=payload,
-                                               ContentType=content_type)
-        result = json.loads(response['Body'].read().decode())
+import json
+import boto3
+from ...core.models.IModel import IModel
+
+
+class AWSSageMakerModel(IModel):
+    def __init__(self, access_key: str, secret_access_key: str, region_name: str, model_name: str):
+        """
+        Initialize the AWS SageMaker model with AWS credentials, region, and the model name.
+
+        Parameters:
+        - access_key (str): AWS access key ID.
+        - secret_access_key (str): AWS secret access key.
+        - region_name (str): The region where the SageMaker model is deployed.
+        - model_name (str): The name of the SageMaker model.
+        """
+        self.access_key = access_key
+        self.secret_access_key = secret_access_key
+        self.region_name = region_name
+        self.client = boto3.client('sagemaker-runtime',
+                                   aws_access_key_id=access_key,
+                                   aws_secret_access_key=secret_access_key,
+                                   region_name=region_name)
+        super().__init__(model_name)
+
+    def predict(self, payload: str, content_type: str='application/json') -> dict:
+        """
+        Generate predictions using the AWS SageMaker model.
+
+        Parameters:
+        - payload (str): Input data in JSON format.
+        - content_type (str): The MIME type of the input data (default: 'application/json').
+        
+        Returns:
+        - dict: The predictions returned by the model.
+        """
+        endpoint_name = self.model_name  # Assuming the model name is also the endpoint name
+        response = self.client.invoke_endpoint(EndpointName=endpoint_name,
+                                               Body=payload,
+                                               ContentType=content_type)
+        result = json.loads(response['Body'].read().decode())
         return result
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/parsers/PDFToTextParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/RegExParser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-import fitz  # PyMuPDF
-from typing import List, Union, Any
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.ConcreteDocument import ConcreteDocument
-
-class PDFtoTextParser(IParser):
-    """
-    A parser to extract text from PDF files.
-    """
-
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses a PDF file and extracts its text content as Document instances.
-
-        Parameters:
-        - data (Union[str, Any]): The path to the PDF file.
-
-        Returns:
-        - List[IDocument]: A list with a single IDocument instance containing the extracted text.
-        """
-        # Ensure data is a valid str path to a PDF file
-        if not isinstance(data, str):
-            raise ValueError("PDFtoTextParser expects a file path in str format.")
-
-        try:
-            # Open the PDF file
-            doc = fitz.open(data)
-            text = ""
-
-            # Extract text from each page
-            for page_num in range(len(doc)):
-                page = doc.load_page(page_num)
-                text += page.get_text()
-
-            # Create a document with the extracted text
-            document = ConcreteDocument(doc_id=str(hash(data)), content=text, metadata={"source": data})
-            return [document]
-        
-        except Exception as e:
-            print(f"An error occurred while parsing the PDF: {e}")
-            return []
+import re
+from typing import List, Union, Any
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class RegExParser(IParser):
+    """
+    A parser that uses a regular expression to extract information from text.
+    """
+
+    def __init__(self, pattern: str):
+        """
+        Initializes the RegExParser with a specific regular expression pattern.
+
+        Parameters:
+        - pattern (str): The regular expression pattern used for parsing the text.
+        """
+        self.pattern = pattern
+
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses the input data using the specified regular expression pattern and
+        returns a list of IDocument instances containing the extracted information.
+
+        Parameters:
+        - data (Union[str, Any]): The input data to be parsed. It can be a string or any format 
+                                   that the concrete implementation can handle.
+
+        Returns:
+        - List[IDocument]: A list of IDocument instances containing the parsed information.
+        """
+        # Ensure data is a string
+        if not isinstance(data, str):
+            data = str(data)
+
+        # Use the regular expression pattern to find all matches in the text
+        matches = re.findall(self.pattern, data)
+
+        # Create a Document for each match and collect them into a list
+        documents = [Document(doc_id=str(i+1), content=match, metadata={}) for i, match in enumerate(matches)]
+
+        return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/tools/FileDownloaderTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/FileDownloaderTool.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import requests
-from ....core.tools.ToolBase import ToolBase
-from ....core.tools.Parameter import Parameter
-
-
-class FileDownloaderTool(ToolBase):
-    def __init__(self):
-        parameters = [
-            Parameter(
-                name="url",
-                type="string",
-                description="The URL of the file to download",
-                required=True
-            )
-        ]
-        
-        super().__init__(name="FileDownloaderTool",
-                         description="Downloads a file from a specified URL into memory.",
-                         parameters=parameters)
-    
-    def __call__(self, url: str) -> bytes:
-        """
-        Downloads a file from the given URL into memory.
-        
-        Parameters:
-        - url (str): The URL of the file to download.
-        
-        Returns:
-        - bytes: The content of the downloaded file.
-        """
-        try:
-            response = requests.get(url)
-            response.raise_for_status()  # Raises an HTTPError if the request resulted in an error
-            return response.content
-        except requests.RequestException as e:
+import requests
+from ....core.tools.ToolBase import ToolBase
+from ....core.tools.Parameter import Parameter
+
+
+class FileDownloaderTool(ToolBase):
+    def __init__(self):
+        parameters = [
+            Parameter(
+                name="url",
+                type="string",
+                description="The URL of the file to download",
+                required=True
+            )
+        ]
+        
+        super().__init__(name="FileDownloaderTool",
+                         description="Downloads a file from a specified URL into memory.",
+                         parameters=parameters)
+    
+    def __call__(self, url: str) -> bytes:
+        """
+        Downloads a file from the given URL into memory.
+        
+        Parameters:
+        - url (str): The URL of the file to download.
+        
+        Returns:
+        - bytes: The content of the downloaded file.
+        """
+        try:
+            response = requests.get(url)
+            response.raise_for_status()  # Raises an HTTPError if the request resulted in an error
+            return response.content
+        except requests.RequestException as e:
             raise RuntimeError(f"Failed to download file from '{url}'. Error: {e}")
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/tools/LinkedInArticleTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/LinkedInArticleTool.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import requests
-from ...standard.tools.base.ToolBase import ToolBase
-from ...standard.tools.concrete.Parameter import Parameter
-
-class LinkedInArticleTool(ToolBase):
-    """
-    A tool to post articles on LinkedIn using the LinkedIn API.
-    """
-    def __init__(self, access_token):
-        """
-        Initializes the LinkedInArticleTool with the necessary access token.
-        
-        Args:
-            access_token (str): The OAuth access token for authenticating with the LinkedIn API.
-        """
-        super().__init__(name="LinkedInArticleTool",
-                         description="A tool for posting articles on LinkedIn.",
-                         parameters=[
-                             Parameter(name="title", type="string", description="The title of the article", required=True),
-                             Parameter(name="text", type="string", description="The body text of the article", required=True),
-                             Parameter(name="visibility", type="string", description="The visibility of the article", required=True, enum=["anyone", "connectionsOnly"])
-                         ])
-        self.access_token = access_token
-        
-    def __call__(self, title: str, text: str, visibility: str = "anyone") -> str:
-        """
-        Posts an article on LinkedIn.
-
-        Args:
-            title (str): The title of the article.
-            text (str): The body text of the article.
-            visibility (str): The visibility of the article, either "anyone" or "connectionsOnly".
-
-        Returns:
-            str: A message indicating the success or failure of the post operation.
-        """
-        # Construct the request URL and payload according to LinkedIn API documentation
-        url = 'https://api.linkedin.com/v2/ugcPosts'
-        headers = {
-            'Authorization': f'Bearer {self.access_token}',
-            'X-Restli-Protocol-Version': '2.0.0',
-            'Content-Type': 'application/json'
-        }
-        
-        payload = {
-            "author": "urn:li:person:YOUR_PERSON_ID_HERE",
-            "lifecycleState": "PUBLISHED",
-            "specificContent": {
-                "com.linkedin.ugc.ShareContent": {
-                    "shareCommentary": {
-                        "text": text
-                    },
-                    "shareMediaCategory": "ARTICLE",
-                    "media": [
-                        {
-                            "status": "READY",
-                            "description": {
-                                "text": title
-                            },
-                            "originalUrl": "URL_OF_THE_ARTICLE_OR_IMAGE",
-                            "visibility": {
-                                "com.linkedin.ugc.MemberNetworkVisibility": visibility.upper()
-                            }
-                        }
-                    ]
-                }
-            },
-            "visibility": {
-                "com.linkedin.ugc.MemberNetworkVisibility": visibility.upper()
-            }
-        }
-     
-        # Make the POST request to LinkedIn's API
-        response = requests.post(url, headers=headers, json=payload)
-        
-        if response.status_code == 201:
-            return f"Article posted successfully: {response.json().get('id')}"
-        else:
+import requests
+from ...standard.tools.base.ToolBase import ToolBase
+from ...standard.tools.concrete.Parameter import Parameter
+
+class LinkedInArticleTool(ToolBase):
+    """
+    A tool to post articles on LinkedIn using the LinkedIn API.
+    """
+    def __init__(self, access_token):
+        """
+        Initializes the LinkedInArticleTool with the necessary access token.
+        
+        Args:
+            access_token (str): The OAuth access token for authenticating with the LinkedIn API.
+        """
+        super().__init__(name="LinkedInArticleTool",
+                         description="A tool for posting articles on LinkedIn.",
+                         parameters=[
+                             Parameter(name="title", type="string", description="The title of the article", required=True),
+                             Parameter(name="text", type="string", description="The body text of the article", required=True),
+                             Parameter(name="visibility", type="string", description="The visibility of the article", required=True, enum=["anyone", "connectionsOnly"])
+                         ])
+        self.access_token = access_token
+        
+    def __call__(self, title: str, text: str, visibility: str = "anyone") -> str:
+        """
+        Posts an article on LinkedIn.
+
+        Args:
+            title (str): The title of the article.
+            text (str): The body text of the article.
+            visibility (str): The visibility of the article, either "anyone" or "connectionsOnly".
+
+        Returns:
+            str: A message indicating the success or failure of the post operation.
+        """
+        # Construct the request URL and payload according to LinkedIn API documentation
+        url = 'https://api.linkedin.com/v2/ugcPosts'
+        headers = {
+            'Authorization': f'Bearer {self.access_token}',
+            'X-Restli-Protocol-Version': '2.0.0',
+            'Content-Type': 'application/json'
+        }
+        
+        payload = {
+            "author": "urn:li:person:YOUR_PERSON_ID_HERE",
+            "lifecycleState": "PUBLISHED",
+            "specificContent": {
+                "com.linkedin.ugc.ShareContent": {
+                    "shareCommentary": {
+                        "text": text
+                    },
+                    "shareMediaCategory": "ARTICLE",
+                    "media": [
+                        {
+                            "status": "READY",
+                            "description": {
+                                "text": title
+                            },
+                            "originalUrl": "URL_OF_THE_ARTICLE_OR_IMAGE",
+                            "visibility": {
+                                "com.linkedin.ugc.MemberNetworkVisibility": visibility.upper()
+                            }
+                        }
+                    ]
+                }
+            },
+            "visibility": {
+                "com.linkedin.ugc.MemberNetworkVisibility": visibility.upper()
+            }
+        }
+     
+        # Make the POST request to LinkedIn's API
+        response = requests.post(url, headers=headers, json=payload)
+        
+        if response.status_code == 201:
+            return f"Article posted successfully: {response.json().get('id')}"
+        else:
             return f"Failed to post the article. Status Code: {response.status_code} - {response.text}"
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/tools/SQLite3QueryTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/SQLite3QueryTool.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import sqlite3
-from ...base.ToolBase import ToolBase
-from ...concrete.Parameter import Parameter
-
-class SQLite3QueryTool(ToolBase):
-    def __init__(self, db_name: str):
-        parameters = [
-            Parameter(
-                name="query",
-                type="string",
-                description="SQL query to execute",
-                required=True
-            )
-        ]
-        super().__init__(name="SQLQueryTool", 
-                         description="Executes an SQL query and returns the results.", 
-                         parameters=parameters)
-        self.db_name = db_name
-
-    def __call__(self, query) -> str:
-        """
-        Execute the provided SQL query.
-
-        Parameters:
-        - query (str): The SQL query to execute.
-
-        Returns:
-        - str: The results of the SQL query as a string.
-        """
-        try:
-            connection = sqlite3.connect(self.db_name)  # Connect to the specific database file
-            cursor = connection.cursor()
-            
-            cursor.execute(query)
-            rows = cursor.fetchall()
-            result = "\n".join(str(row) for row in rows)
-        except Exception as e:
-            result = f"Error executing query: {e}"
-        finally:
-            connection.close()
-        
+import sqlite3
+from ...base.ToolBase import ToolBase
+from ...concrete.Parameter import Parameter
+
+class SQLite3QueryTool(ToolBase):
+    def __init__(self, db_name: str):
+        parameters = [
+            Parameter(
+                name="query",
+                type="string",
+                description="SQL query to execute",
+                required=True
+            )
+        ]
+        super().__init__(name="SQLQueryTool", 
+                         description="Executes an SQL query and returns the results.", 
+                         parameters=parameters)
+        self.db_name = db_name
+
+    def __call__(self, query) -> str:
+        """
+        Execute the provided SQL query.
+
+        Parameters:
+        - query (str): The SQL query to execute.
+
+        Returns:
+        - str: The results of the SQL query as a string.
+        """
+        try:
+            connection = sqlite3.connect(self.db_name)  # Connect to the specific database file
+            cursor = connection.cursor()
+            
+            cursor.execute(query)
+            rows = cursor.fetchall()
+            result = "\n".join(str(row) for row in rows)
+        except Exception as e:
+            result = f"Error executing query: {e}"
+        finally:
+            connection.close()
+        
         return f"Query Result:\n{result}"
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/utils/ISerializable.py` & `swarmauri-0.1.9/swarmauri/experimental/utils/ISerializable.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
-# class Serializable:
-#     def serialize(self):
-#         raise NotImplementedError("Serialization method not implemented")
-    
-#     @classmethod
-#     def deserialize(cls, data):
-#         raise NotImplementedError("Deserialization method not implemented")
-        
-        
-# class ToolAgent(Serializable):
-#     def serialize(self):
-#         # Simplified example, adapt according to actual attributes
-#         return {"type": self.__class__.__name__, "state": {"model_name": self.model.model_name}}
-
-#     @classmethod
-#     def deserialize(cls, data):
-#         # This method should instantiate the object based on the serialized state.
-#         # Example assumes the presence of model_name in the serialized state.
-#         model = OpenAIToolModel(api_key="api_key_placeholder", model_name=data["state"]["model_name"])
+
+# class Serializable:
+#     def serialize(self):
+#         raise NotImplementedError("Serialization method not implemented")
+    
+#     @classmethod
+#     def deserialize(cls, data):
+#         raise NotImplementedError("Deserialization method not implemented")
+        
+        
+# class ToolAgent(Serializable):
+#     def serialize(self):
+#         # Simplified example, adapt according to actual attributes
+#         return {"type": self.__class__.__name__, "state": {"model_name": self.model.model_name}}
+
+#     @classmethod
+#     def deserialize(cls, data):
+#         # This method should instantiate the object based on the serialized state.
+#         # Example assumes the presence of model_name in the serialized state.
+#         model = OpenAIToolModel(api_key="api_key_placeholder", model_name=data["state"]["model_name"])
 #         return cls(model=model, conversation=None, toolkit=None)  # Simplify, omit optional parameters for illustration
```

### Comparing `swarmauri-0.1.80/swarmauri/experimental/utils/get_last_frame.py` & `swarmauri-0.1.9/swarmauri/experimental/utils/get_last_frame.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import inspect
-
-def child_function(arg):
-    # Get the stack frame of the caller
-    caller_frame = inspect.currentframe().f_back
-    # Get the name of the caller function
-    caller_name = caller_frame.f_code.co_name
-    # Inspect the arguments of the caller function
-    args, _, _, values = inspect.getargvalues(caller_frame)
-    # Assuming the caller has only one argument for simplicity
-    arg_name = args[0]
-    arg_value = values[arg_name]
-    print(f"Caller Name: {caller_name}, Argument Name: {arg_name}, Argument Value: {arg_value}")
-
-def caller_function(l):
-    child_function(l)
-
-# Example usage
-caller_function("Hello")
-
+import inspect
+
+def child_function(arg):
+    # Get the stack frame of the caller
+    caller_frame = inspect.currentframe().f_back
+    # Get the name of the caller function
+    caller_name = caller_frame.f_code.co_name
+    # Inspect the arguments of the caller function
+    args, _, _, values = inspect.getargvalues(caller_frame)
+    # Assuming the caller has only one argument for simplicity
+    arg_name = args[0]
+    arg_value = values[arg_name]
+    print(f"Caller Name: {caller_name}, Argument Name: {arg_name}, Argument Value: {arg_value}")
+
+def caller_function(l):
+    child_function(l)
+
+# Example usage
+caller_function("Hello")
+
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/base/AgentBase.py` & `swarmauri-0.1.9/swarmauri/standard/agents/base/AgentBase.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import Any, Optional
-from abc import ABC
-from swarmauri.core.agents.IAgent import IAgent
-from swarmauri.core.models.IModel import IModel
-
-
-
-class AgentBase(IAgent, ABC):
-    def __init__(self, model: IModel):
-        self._model = model
-
-    def exec(self, input_str: Optional[Any]) -> Any:
-        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
-    
-    @property
-    def model(self) -> IModel:
-        return self._model
-    
-    @model.setter
-    def model(self, value) -> None:
-        self._model = value        
-
-    
-    def __getattr__(self, name):
-        # Example of transforming attribute name from simplified to internal naming convention
-        internal_name = f"_{name}"
-        if internal_name in self.__dict__:
-            return self.__dict__[internal_name]
-        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
-    
-    def __setattr__(self, name, value):
-        # Direct assignment to the __dict__ to bypass any potential infinite recursion
-        # from setting attributes that do not explicitly exist.
-        object.__setattr__(self, name, value) 
-        
-        
-    def __str__(self):
-        class_name = self.__class__.__name__
-        variables_str = ", ".join(f"{k}={v}" for k, v in self.__dict__.items())
-        return f"<{class_name} {variables_str}>"
-        
-    def __repr__(self):
-        class_name = self.__class__.__name__
-        variables_str = ", ".join(f"{k}={v}" for k, v in self.__dict__.items())
+from typing import Any, Optional
+from abc import ABC
+from swarmauri.core.agents.ISwarmAgent import ISwarmAgent
+from swarmauri.core.models.IModel import IModel
+
+
+
+class AgentBase(ISwarmAgent, ABC):
+    def __init__(self, model: IModel):
+        self._model = model
+
+    def exec(self, input_str: Optional[Any]) -> Any:
+        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
+    
+    @property
+    def model(self) -> IModel:
+        return self._model
+    
+    @model.setter
+    def model(self, value) -> None:
+        self._model = value        
+
+    
+    def __getattr__(self, name):
+        # Example of transforming attribute name from simplified to internal naming convention
+        internal_name = f"_{name}"
+        if internal_name in self.__dict__:
+            return self.__dict__[internal_name]
+        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
+    
+    def __setattr__(self, name, value):
+        # Direct assignment to the __dict__ to bypass any potential infinite recursion
+        # from setting attributes that do not explicitly exist.
+        object.__setattr__(self, name, value) 
+        
+        
+    def __str__(self):
+        class_name = self.__class__.__name__
+        variables_str = ", ".join(f"{k}={v}" for k, v in self.__dict__.items())
+        return f"<{class_name} {variables_str}>"
+        
+    def __repr__(self):
+        class_name = self.__class__.__name__
+        variables_str = ", ".join(f"{k}={v}" for k, v in self.__dict__.items())
         return f"{class_name} ({variables_str})"
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/base/ConversationAgentBase.py` & `swarmauri-0.1.9/swarmauri/standard/agents/base/ConversationAgentBase.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Any, Optional
-from abc import ABC
-
-from swarmauri.core.agents.IAgentConversation import IAgentConversation
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.conversations.IConversation import IConversation
-
-from swarmauri.standard.agents.base.AgentBase import AgentBase
-
-class ConversationAgentBase(AgentBase, IAgentConversation, ABC):
-    def __init__(self, model: IModel, conversation: IConversation):
-        AgentBase.__init__(self, model)
-        self._conversation = conversation
-
-    
-    def exec(self, input_str: Optional[Any]) -> Any:
-        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
-      
-
-    @property
-    def conversation(self) -> IConversation:
-        return self._conversation
-
-    @conversation.setter
-    def conversation(self, value) -> None:
-        self._conversation = value
-
+from typing import Any, Optional
+from abc import ABC
+
+from swarmauri.core.agents.IAgentConversation import IAgentConversation
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.conversations.IConversation import IConversation
+
+from swarmauri.standard.agents.base.AgentBase import AgentBase
+
+class ConversationAgentBase(AgentBase, IAgentConversation, ABC):
+    def __init__(self, model: IModel, conversation: IConversation):
+        AgentBase.__init__(self, model)
+        self._conversation = conversation
+
+    
+    def exec(self, input_str: Optional[Any]) -> Any:
+        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
+      
+
+    @property
+    def conversation(self) -> IConversation:
+        return self._conversation
+
+    @conversation.setter
+    def conversation(self, value) -> None:
+        self._conversation = value
+
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/base/NamedAgentBase.py` & `swarmauri-0.1.9/swarmauri/standard/agents/base/NamedAgentBase.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Optional
-from abc import ABC
-from swarmauri.core.agents.IAgentName import IAgentName
-
-
-class NamedAgentBase(IAgentName,ABC):
-    
-    def __init__(self, name: str):
-        self._name = name
-
-    def exec(self, input_str: Optional[Any]) -> Any:
-        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
-    
-    @property
-    def name(self) -> str:
-        return self._name
-    
-    @name.setter
-    def name(self, value) -> None:
+from typing import Any, Optional
+from abc import ABC
+from swarmauri.core.agents.IAgentName import IAgentName
+
+
+class NamedAgentBase(IAgentName,ABC):
+    
+    def __init__(self, name: str):
+        self._name = name
+
+    def exec(self, input_str: Optional[Any]) -> Any:
+        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
+    
+    @property
+    def name(self) -> str:
+        return self._name
+    
+    @name.setter
+    def name(self, value) -> None:
         self._name = value
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/base/ToolAgentBase.py` & `swarmauri-0.1.9/swarmauri/standard/agents/base/ToolAgentBase.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from abc import ABC
-from typing import Any, Optional
-from swarmauri.core.agents.IAgentConversation import IAgentConversation
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.conversations.IConversation import IConversation
-from swarmauri.core.toolkits.IToolkit import IToolkit
-from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
-
-
-class ToolAgentBase(ConversationAgentBase, IAgentConversation, ABC):
-    
-    def __init__(self, 
-                 model: IModel, 
-                 conversation: IConversation,
-                 toolkit: IToolkit):
-        ConversationAgentBase.__init__(self, model, conversation)
-        self._toolkit = toolkit
-
-    def exec(self, input_str: Optional[Any]) -> Any:
-        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
-    
-    @property
-    def toolkit(self) -> IToolkit:
-        return self._toolkit
-    
-    @toolkit.setter
-    def toolkit(self, value) -> None:
-        self._toolkit = value        
+from abc import ABC
+from typing import Any, Optional
+from swarmauri.core.agents.IAgentConversation import IAgentConversation
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.conversations.IConversation import IConversation
+from swarmauri.core.toolkits.IToolkit import IToolkit
+from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
+
+
+class ToolAgentBase(ConversationAgentBase, IAgentConversation, ABC):
+    
+    def __init__(self, 
+                 model: IModel, 
+                 conversation: IConversation,
+                 toolkit: IToolkit):
+        ConversationAgentBase.__init__(self, model, conversation)
+        self._toolkit = toolkit
+
+    def exec(self, input_str: Optional[Any]) -> Any:
+        raise NotImplementedError('The `exec` function has not been implemeneted on this class.')
+    
+    @property
+    def toolkit(self) -> IToolkit:
+        return self._toolkit
+    
+    @toolkit.setter
+    def toolkit(self, value) -> None:
+        self._toolkit = value
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/concrete/ChatSwarmAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/ChatSwarmAgent.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import Any, Optional, Union, Dict
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.messages import IMessage
-from swarmauri.core.conversations import IConversation
-from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
-from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
-
-class ChatSwarmAgent(ConversationAgentBase):
-    def __init__(self, model: IModel, conversation: IConversation):
-        super().__init__(model, conversation)
-
-    def exec(self, input_data: Union[str, IMessage], model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.conversation
-        model = self.model
-
-        # Check if the input is a string, then wrap it in a HumanMessage
-        if isinstance(input_data, str):
-            human_message = HumanMessage(input_data)
-        elif isinstance(input_data, IMessage):
-            human_message = input_data
-        else:
-            raise TypeError("Input data must be a string or an instance of Message.")
-
-        # Add the human message to the conversation
-        conversation.add_message(human_message)
-        
-        # Retrieve the conversation history and predict a response
-        messages = conversation.as_dict()
-        if model_kwargs:
-            prediction = model.predict(messages=messages, **model_kwargs)
-        else:
-            prediction = model.predict(messages=messages)
-        # Create an AgentMessage instance with the model's response and update the conversation
-        agent_message = AgentMessage(prediction)
-        conversation.add_message(agent_message)
-        
+from typing import Any, Optional, Union, Dict
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.messages import IMessage
+from swarmauri.core.conversations import IConversation
+from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
+
+class ChatSwarmAgent(ConversationAgentBase):
+    def __init__(self, model: IModel, conversation: IConversation):
+        super().__init__(model, conversation)
+
+    def exec(self, input_data: Union[str, IMessage], model_kwargs: Optional[Dict] = {}) -> Any:
+        conversation = self.conversation
+        model = self.model
+
+        # Check if the input is a string, then wrap it in a HumanMessage
+        if isinstance(input_data, str):
+            human_message = HumanMessage(input_data)
+        elif isinstance(input_data, IMessage):
+            human_message = input_data
+        else:
+            raise TypeError("Input data must be a string or an instance of Message.")
+
+        # Add the human message to the conversation
+        conversation.add_message(human_message)
+        
+        # Retrieve the conversation history and predict a response
+        messages = conversation.as_dict()
+        if model_kwargs:
+            prediction = model.predict(messages=messages, **model_kwargs)
+        else:
+            prediction = model.predict(messages=messages)
+        # Create an AgentMessage instance with the model's response and update the conversation
+        agent_message = AgentMessage(prediction)
+        conversation.add_message(agent_message)
+        
         return prediction
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Any, Optional, Union, Dict
-
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.messages import IMessage
-
-from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
-from swarmauri.standard.agents.base.NamedAgentBase import NamedAgentBase
-from swarmauri.standard.conversations.concrete.SharedConversation import SharedConversation
-from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
-
-class MultiPartyChatSwarmAgent(ConversationAgentBase, NamedAgentBase):
-    def __init__(self, 
-                 model: IModel, 
-                 conversation: SharedConversation,
-                 name: str):
-        ConversationAgentBase.__init__(self, model, conversation)
-        NamedAgentBase.__init__(self, name)
-
-    def exec(self, input_data: Union[str, IMessage] = "", model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.conversation
-        model = self.model
-
-        # Check if the input is a string, then wrap it in a HumanMessage
-        if isinstance(input_data, str):
-            human_message = HumanMessage(input_data)
-        elif isinstance(input_data, IMessage):
-            human_message = input_data
-        else:
-            raise TypeError("Input data must be a string or an instance of Message.")
-
-        if input_data != "":
-            # Add the human message to the conversation
-            conversation.add_message(human_message, sender_id=self.name)
-        
-        # Retrieve the conversation history and predict a response
-        messages = conversation.as_dict()
-
-        
-        if model_kwargs:
-            prediction = model.predict(messages=messages, **model_kwargs)
-        else:
-            prediction = model.predict(messages=messages)
-        # Create an AgentMessage instance with the model's response and update the conversation
-        if prediction != '':
-            agent_message = AgentMessage(prediction)
-            conversation.add_message(agent_message, sender_id=self.name)
-        
+from typing import Any, Optional, Union, Dict
+
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.messages import IMessage
+
+from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
+from swarmauri.standard.agents.base.NamedAgentBase import NamedAgentBase
+from swarmauri.standard.conversations.concrete.SharedConversation import SharedConversation
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
+
+class MultiPartyChatSwarmAgent(ConversationAgentBase, NamedAgentBase):
+    def __init__(self, 
+                 model: IModel, 
+                 conversation: SharedConversation,
+                 name: str):
+        ConversationAgentBase.__init__(self, model, conversation)
+        NamedAgentBase.__init__(self, name)
+
+    def exec(self, input_data: Union[str, IMessage] = "", model_kwargs: Optional[Dict] = {}) -> Any:
+        conversation = self.conversation
+        model = self.model
+
+        # Check if the input is a string, then wrap it in a HumanMessage
+        if isinstance(input_data, str):
+            human_message = HumanMessage(input_data)
+        elif isinstance(input_data, IMessage):
+            human_message = input_data
+        else:
+            raise TypeError("Input data must be a string or an instance of Message.")
+
+        if input_data != "":
+            # Add the human message to the conversation
+            conversation.add_message(human_message, sender_id=self.name)
+        
+        # Retrieve the conversation history and predict a response
+        messages = conversation.as_dict()
+
+        
+        if model_kwargs:
+            prediction = model.predict(messages=messages, **model_kwargs)
+        else:
+            prediction = model.predict(messages=messages)
+        # Create an AgentMessage instance with the model's response and update the conversation
+        if prediction != '':
+            agent_message = AgentMessage(prediction)
+            conversation.add_message(agent_message, sender_id=self.name)
+        
         return prediction
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from typing import Any, Optional, Union, Dict
-import json
-
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.toolkits.IToolkit import IToolkit
-from swarmauri.core.conversations.IConversation import IConversation
-from swarmauri.core.messages import IMessage
-
-from swarmauri.standard.agents.base.ToolAgentBase import ToolAgentBase
-from swarmauri.standard.agents.base.NamedAgentBase import NamedAgentBase
-from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage, FunctionMessage
-
-
-class MultiPartyToolAgent(ToolAgentBase, NamedAgentBase):
-    def __init__(self, 
-                 model: IModel, 
-                 conversation: IConversation, 
-                 toolkit: IToolkit,
-                 name: str):
-        ToolAgentBase.__init__(self, model, conversation, toolkit)
-        NamedAgentBase.__init__(self, name)
-
-    def exec(self, input_data: Union[str, IMessage], model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.conversation
-        model = self.model
-        toolkit = self.toolkit
-        
-
-        # Check if the input is a string, then wrap it in a HumanMessage
-        if isinstance(input_data, str):
-            human_message = HumanMessage(input_data)
-        elif isinstance(input_data, IMessage):
-            human_message = input_data
-        else:
-            raise TypeError("Input data must be a string or an instance of Message.")
-
-        if input_data != "":
-            # Add the human message to the conversation
-            conversation.add_message(human_message, sender_id=self.name)
-            
-        
-        # Retrieve the conversation history and predict a response
-        messages = conversation.as_dict()
-        
-
-        if model_kwargs:
-            prediction = model.predict(messages=messages, 
-                                   tools=toolkit.tools, 
-                                   tool_choice="auto",
-                                   **model_kwargs)
-        else:
-            prediction = model.predict(messages=messages)
-        
-        
-        prediction_message = prediction.choices[0].message
-        agent_response = prediction_message.content
-        
-        agent_message = AgentMessage(content=prediction_message.content, 
-                                     tool_calls=prediction_message.tool_calls)
-        conversation.add_message(agent_message, sender_id=self.name)
-        
-        tool_calls = prediction.choices[0].message.tool_calls
-        if tool_calls:
-        
-            for tool_call in tool_calls:
-                func_name = tool_call.function.name
-                
-                func_call = toolkit.get_tool_by_name(func_name)
-                func_args = json.loads(tool_call.function.arguments)
-                func_result = func_call(**func_args)
-                
-                func_message = FunctionMessage(func_result, 
-                                               name=func_name, 
-                                               tool_call_id=tool_call.id)
-                conversation.add_message(func_message, sender_id=self.name)
-            
-            
-            messages = conversation.as_dict()
-            rag_prediction = model.predict(messages=messages, 
-                                           tools=toolkit.tools, 
-                                           tool_choice="none")
-            
-            prediction_message = rag_prediction.choices[0].message
-            
-            agent_response = prediction_message.content
-            if agent_response != "":
-                agent_message = AgentMessage(agent_response)
-                conversation.add_message(agent_message, sender_id=self.name)
-            prediction = rag_prediction
-            
-        return agent_response 
+from typing import Any, Optional, Union, Dict
+import json
+
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.toolkits.IToolkit import IToolkit
+from swarmauri.core.conversations.IConversation import IConversation
+from swarmauri.core.messages import IMessage
+
+from swarmauri.standard.agents.base.ToolAgentBase import ToolAgentBase
+from swarmauri.standard.agents.base.NamedAgentBase import NamedAgentBase
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage, FunctionMessage
+
+
+class MultiPartyToolAgent(ToolAgentBase, NamedAgentBase):
+    def __init__(self, 
+                 model: IModel, 
+                 conversation: IConversation, 
+                 toolkit: IToolkit,
+                 name: str):
+        ToolAgentBase.__init__(self, model, conversation, toolkit)
+        NamedAgentBase.__init__(self, name)
+
+    def exec(self, input_data: Union[str, IMessage], model_kwargs: Optional[Dict] = {}) -> Any:
+        conversation = self.conversation
+        model = self.model
+        toolkit = self.toolkit
+        
+
+        # Check if the input is a string, then wrap it in a HumanMessage
+        if isinstance(input_data, str):
+            human_message = HumanMessage(input_data)
+        elif isinstance(input_data, IMessage):
+            human_message = input_data
+        else:
+            raise TypeError("Input data must be a string or an instance of Message.")
+
+        if input_data != "":
+            # Add the human message to the conversation
+            conversation.add_message(human_message, sender_id=self.name)
+            
+        
+        # Retrieve the conversation history and predict a response
+        messages = conversation.as_dict()
+        
+
+        if model_kwargs:
+            prediction = model.predict(messages=messages, 
+                                   tools=toolkit.tools, 
+                                   tool_choice="auto",
+                                   **model_kwargs)
+        else:
+            prediction = model.predict(messages=messages)
+        
+        
+        prediction_message = prediction.choices[0].message
+        agent_response = prediction_message.content
+        
+        agent_message = AgentMessage(content=prediction_message.content, 
+                                     tool_calls=prediction_message.tool_calls)
+        conversation.add_message(agent_message, sender_id=self.name)
+        
+        tool_calls = prediction.choices[0].message.tool_calls
+        if tool_calls:
+        
+            for tool_call in tool_calls:
+                func_name = tool_call.function.name
+                
+                func_call = toolkit.get_tool_by_name(func_name)
+                func_args = json.loads(tool_call.function.arguments)
+                func_result = func_call(**func_args)
+                
+                func_message = FunctionMessage(func_result, 
+                                               name=func_name, 
+                                               tool_call_id=tool_call.id)
+                conversation.add_message(func_message, sender_id=self.name)
+            
+            
+            messages = conversation.as_dict()
+            rag_prediction = model.predict(messages=messages, 
+                                           tools=toolkit.tools, 
+                                           tool_choice="none")
+            
+            prediction_message = rag_prediction.choices[0].message
+            
+            agent_response = prediction_message.content
+            if agent_response != "":
+                agent_message = AgentMessage(agent_response)
+                conversation.add_message(agent_message, sender_id=self.name)
+            prediction = rag_prediction
+            
+        return agent_response
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Any, Optional
-
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.conversations.IConversation import IConversation
-
-
-from swarmauri.standard.agents.base.SwarmAgentBase import AgentBase
-from swarmauri.standard.messages.concrete import HumanMessage
-
-class SimpleSwarmAgent(AgentBase):
-    def __init__(self, model: IModel, 
-                 conversation: IConversation):
-        super().__init__(model, conversation)
-
-    def exec(self, input_str: Optional[str] = None) -> Any:
-        conversation = self.conversation
-        model = self.model
-
-        # Construct a new human message (for example purposes)
-        if input_str:
-            human_message = HumanMessage(input_str)
-            conversation.add_message(human_message)
-        
-        messages = conversation.as_dict()
-        prediction = model.predict(messages=messages)
+from typing import Any, Optional
+
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.conversations.IConversation import IConversation
+
+
+from swarmauri.standard.agents.base.SwarmAgentBase import AgentBase
+from swarmauri.standard.messages.concrete import HumanMessage
+
+class SimpleSwarmAgent(AgentBase):
+    def __init__(self, model: IModel, 
+                 conversation: IConversation):
+        super().__init__(model, conversation)
+
+    def exec(self, input_str: Optional[str] = None) -> Any:
+        conversation = self.conversation
+        model = self.model
+
+        # Construct a new human message (for example purposes)
+        if input_str:
+            human_message = HumanMessage(input_str)
+            conversation.add_message(human_message)
+        
+        messages = conversation.as_dict()
+        prediction = model.predict(messages=messages)
         return prediction
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/concrete/SingleCommandAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/SingleCommandAgent.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Any, Optional
-
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.conversations.IConversation import IConversation
-
-from swarmauri.standard.agents.base.AgentBase import AgentBase
-
-class SingleCommandAgent(AgentBase):
-    def __init__(self, model: IModel, 
-                 conversation: IConversation):
-        super().__init__(model, conversation)
-
-    def exec(self, input_str: Optional[str] = None) -> Any:
-        model = self.model
-        prediction = model.predict(input_str)
-        
+from typing import Any, Optional
+
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.conversations.IConversation import IConversation
+
+from swarmauri.standard.agents.base.AgentBase import AgentBase
+
+class SingleCommandAgent(AgentBase):
+    def __init__(self, model: IModel, 
+                 conversation: IConversation):
+        super().__init__(model, conversation)
+
+    def exec(self, input_str: Optional[str] = None) -> Any:
+        model = self.model
+        prediction = model.predict(input_str)
+        
         return prediction
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/agents/concrete/ToolAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/ToolAgent.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from typing import Any, Optional, Union, Dict
-import json
-
-from swarmauri.core.models.IModel import IModel
-from swarmauri.core.toolkits.IToolkit import IToolkit
-from swarmauri.core.conversations.IConversation import IConversation
-from swarmauri.core.messages import IMessage
-
-from swarmauri.standard.agents.base.ToolAgentBase import ToolAgentBase
-from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage, FunctionMessage
-
-
-class ToolAgent(ToolAgentBase):
-    def __init__(self, 
-                 model: IModel, 
-                 conversation: IConversation, 
-                 toolkit: IToolkit):
-        super().__init__(model, conversation, toolkit)
-
-    def exec(self, input_data: Union[str, IMessage],  model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.conversation
-        model = self.model
-        toolkit = self.toolkit
-        
-
-        # Check if the input is a string, then wrap it in a HumanMessage
-        if isinstance(input_data, str):
-            human_message = HumanMessage(input_data)
-        elif isinstance(input_data, IMessage):
-            human_message = input_data
-        else:
-            raise TypeError("Input data must be a string or an instance of Message.")
-
-        # Add the human message to the conversation
-        conversation.add_message(human_message)
-
-            
-        
-        # Retrieve the conversation history and predict a response
-        messages = conversation.as_dict()
-        
-        prediction = model.predict(messages=messages, 
-                                   tools=toolkit.tools, 
-                                   tool_choice="auto", 
-                                   **model_kwargs)
-        
-        prediction_message = prediction.choices[0].message
-        
-        agent_response = prediction_message.content
-        
-        agent_message = AgentMessage(content=prediction_message.content, 
-                                     tool_calls=prediction_message.tool_calls)
-        conversation.add_message(agent_message)
-        
-        tool_calls = prediction.choices[0].message.tool_calls
-        if tool_calls:
-        
-            for tool_call in tool_calls:
-                func_name = tool_call.function.name
-                
-                func_call = toolkit.get_tool_by_name(func_name)
-                func_args = json.loads(tool_call.function.arguments)
-                func_result = func_call(**func_args)
-                
-                func_message = FunctionMessage(func_result, 
-                                               name=func_name, 
-                                               tool_call_id=tool_call.id)
-                conversation.add_message(func_message)
-            
-            
-            messages = conversation.as_dict()
-            rag_prediction = model.predict(messages=messages, 
-                                           tools=toolkit.tools, 
-                                           tool_choice="none",
-                                           **model_kwargs)
-            
-            prediction_message = rag_prediction.choices[0].message
-            
-            agent_response = prediction_message.content
-            agent_message = AgentMessage(agent_response)
-            conversation.add_message(agent_message)
-            prediction = rag_prediction
-            
-        return agent_response 
+from typing import Any, Optional, Union, Dict
+import json
+
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.toolkits.IToolkit import IToolkit
+from swarmauri.core.conversations.IConversation import IConversation
+from swarmauri.core.messages import IMessage
+
+from swarmauri.standard.agents.base.ToolAgentBase import ToolAgentBase
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage, FunctionMessage
+
+
+class ToolAgent(ToolAgentBase):
+    def __init__(self, 
+                 model: IModel, 
+                 conversation: IConversation, 
+                 toolkit: IToolkit):
+        super().__init__(model, conversation, toolkit)
+
+    def exec(self, input_data: Union[str, IMessage],  model_kwargs: Optional[Dict] = {}) -> Any:
+        conversation = self.conversation
+        model = self.model
+        toolkit = self.toolkit
+        
+
+        # Check if the input is a string, then wrap it in a HumanMessage
+        if isinstance(input_data, str):
+            human_message = HumanMessage(input_data)
+        elif isinstance(input_data, IMessage):
+            human_message = input_data
+        else:
+            raise TypeError("Input data must be a string or an instance of Message.")
+
+        # Add the human message to the conversation
+        conversation.add_message(human_message)
+
+            
+        
+        # Retrieve the conversation history and predict a response
+        messages = conversation.as_dict()
+        
+        prediction = model.predict(messages=messages, 
+                                   tools=toolkit.tools, 
+                                   tool_choice="auto", 
+                                   **model_kwargs)
+        
+        prediction_message = prediction.choices[0].message
+        
+        agent_response = prediction_message.content
+        
+        agent_message = AgentMessage(content=prediction_message.content, 
+                                     tool_calls=prediction_message.tool_calls)
+        conversation.add_message(agent_message)
+        
+        tool_calls = prediction.choices[0].message.tool_calls
+        if tool_calls:
+        
+            for tool_call in tool_calls:
+                func_name = tool_call.function.name
+                
+                func_call = toolkit.get_tool_by_name(func_name)
+                func_args = json.loads(tool_call.function.arguments)
+                func_result = func_call(**func_args)
+                
+                func_message = FunctionMessage(func_result, 
+                                               name=func_name, 
+                                               tool_call_id=tool_call.id)
+                conversation.add_message(func_message)
+            
+            
+            messages = conversation.as_dict()
+            rag_prediction = model.predict(messages=messages, 
+                                           tools=toolkit.tools, 
+                                           tool_choice="none",
+                                           **model_kwargs)
+            
+            prediction_message = rag_prediction.choices[0].message
+            
+            agent_response = prediction_message.content
+            agent_message = AgentMessage(agent_response)
+            conversation.add_message(agent_message)
+            prediction = rag_prediction
+            
+        return agent_response
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/chains/base/ChainStepBase.py` & `swarmauri-0.1.9/swarmauri/standard/chains/base/ChainStepBase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-from typing import Any, Callable, List, Dict
-from swarmauri.core.chains.IChainStep import IChainStep
-
-class ChainStepBase(IChainStep):
-    """
-    Represents a single step within an execution chain.
-    """
-    
-    def __init__(self, 
-        key: str, 
-        method: Callable, 
-        args: List[Any] = None, 
-        kwargs: Dict[str, Any] = None, 
-        ref: str = None):
-        """
-        Initialize a chain step.
-
-        Args:
-            key (str): Unique key or identifier for the step.
-            method (Callable): The callable object (function or method) to execute in this step.
-            args (List[Any], optional): Positional arguments for the callable.
-            kwargs (Dict[str, Any], optional): Keyword arguments for the callable.
-            ref (str, optional): Reference to another component or context variable, if applicable.
-        """
-        self.key = key
-        self.method = method
-        self.args = args if args is not None else []
-        self.kwargs = kwargs if kwargs is not None else {}
-        self.ref = ref
-        
+from typing import Any, Callable, List, Dict
+from swarmauri.core.chains.IChainStep import IChainStep
+
+class ChainStepBase(IChainStep):
+    """
+    Represents a single step within an execution chain.
+    """
+    
+    def __init__(self, key: str, method: Callable, args: List[Any] = None, kwargs: Dict[str, Any] = None, ref: str = None):
+        """
+        Initialize a chain step.
+
+        Args:
+            key (str): Unique key or identifier for the step.
+            method (Callable): The callable object (function or method) to execute in this step.
+            args (List[Any], optional): Positional arguments for the callable.
+            kwargs (Dict[str, Any], optional): Keyword arguments for the callable.
+            ref (str, optional): Reference to another component or context variable, if applicable.
+        """
+        self.key = key
+        self.method = method
+        self.args = args if args is not None else []
+        self.kwargs = kwargs if kwargs is not None else {}
+        self.ref = ref
+
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import List, Union, Any
-from swarmauri.core.chunkers.IChunker import IChunker
-
-class FixedLengthChunker(IChunker):
-    """
-    Concrete implementation of IChunker that divides text into fixed-length chunks.
-    
-    This chunker breaks the input text into chunks of a specified size, making sure 
-    that each chunk has exactly the number of characters specified by the chunk size, 
-    except for possibly the last chunk.
-    """
-
-    def __init__(self, chunk_size: int):
-        """
-        Initializes a new instance of the FixedLengthChunker class with a specific chunk size.
-
-        Parameters:
-        - chunk_size (int): The fixed size (number of characters) for each chunk.
-        """
-        self.chunk_size = chunk_size
-
-    def chunk_text(self, text: Union[str, Any], *args, **kwargs) -> List[str]:
-        """
-        Splits the input text into fixed-length chunks.
-
-        Parameters:
-        - text (Union[str, Any]): The input text to be chunked.
-        
-        Returns:
-        - List[str]: A list of text chunks, each of a specified fixed length.
-        """
-        # Check if the input is a string, if not, attempt to convert to a string.
-        if not isinstance(text, str):
-            text = str(text)
-        
-        # Using list comprehension to split text into chunks of fixed size
-        chunks = [text[i:i+self.chunk_size] for i in range(0, len(text), self.chunk_size)]
-        
+from swarmauri.core.chunkers import IChunker
+from typing import List, Union, Any
+
+class FixedLengthChunker(IChunker):
+    """
+    Concrete implementation of IChunker that divides text into fixed-length chunks.
+    
+    This chunker breaks the input text into chunks of a specified size, making sure 
+    that each chunk has exactly the number of characters specified by the chunk size, 
+    except for possibly the last chunk.
+    """
+
+    def __init__(self, chunk_size: int):
+        """
+        Initializes a new instance of the FixedLengthChunker class with a specific chunk size.
+
+        Parameters:
+        - chunk_size (int): The fixed size (number of characters) for each chunk.
+        """
+        self.chunk_size = chunk_size
+
+    def chunk_text(self, text: Union[str, Any], *args, **kwargs) -> List[str]:
+        """
+        Splits the input text into fixed-length chunks.
+
+        Parameters:
+        - text (Union[str, Any]): The input text to be chunked.
+        
+        Returns:
+        - List[str]: A list of text chunks, each of a specified fixed length.
+        """
+        # Check if the input is a string, if not, attempt to convert to a string.
+        if not isinstance(text, str):
+            text = str(text)
+        
+        # Using list comprehension to split text into chunks of fixed size
+        chunks = [text[i:i+self.chunk_size] for i in range(0, len(text), self.chunk_size)]
+        
         return chunks
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import List, Union, Any, Optional
-import re
-from swarmauri.core.chunkers.IChunker import IChunker
-
-class MdSnippetChunker(IChunker):
-    def __init__(self, language: Optional[str] = None):
-        """
-        Initializes the MdSnippetChunker with a specific programming language
-        to look for within Markdown fenced code blocks.
-        """
-        self.language = language
-    
-    def chunk_text(self, text: Union[str, Any], *args, **kwargs) -> List[tuple]:
-        """
-        Extracts paired comments and code blocks from Markdown content based on the 
-        specified programming language.
-        """
-        if self.language:
-            # If language is specified, directly extract the corresponding blocks
-            pattern = fr'```{self.language}\s*(.*?)```'
-            scripts = re.findall(pattern, text, re.DOTALL)
-            comments_temp = re.split(pattern, text, flags=re.DOTALL)
-        else:
-            # Extract blocks and languages dynamically if no specific language is provided
-            scripts = []
-            languages = []
-            for match in re.finditer(r'```(\w+)?\s*(.*?)```', text, re.DOTALL):
-                if match.group(1) is not None:  # Checks if a language identifier is present
-                    languages.append(match.group(1))
-                    scripts.append(match.group(2))
-                else:
-                    languages.append('')  # Default to an empty string if no language is found
-                    scripts.append(match.group(2))
-            comments_temp = re.split(r'```.*?```', text, flags=re.DOTALL)
-
-        comments = [comment.strip() for comment in comments_temp]
-
-        if text.strip().startswith('```'):
-            comments = [''] + comments
-        if text.strip().endswith('```'):
-            comments.append('')
-
-        if self.language:
-            structured_output = [(comments[i], self.language, scripts[i].strip()) for i in range(len(scripts))]
-        else:
-            structured_output = [(comments[i], languages[i], scripts[i].strip()) for i in range(len(scripts))]
-
-        return structured_output
+from typing import List, Union, Any, Optional
+import re
+from swarmauri.core.chunkers.IChunker import IChunker
+
+class MdSnippetChunker(IChunker):
+    def __init__(self, language: Optional[str] = None):
+        """
+        Initializes the MdSnippetChunker with a specific programming language
+        to look for within Markdown fenced code blocks.
+        """
+        self.language = language
+    
+    def chunk_text(self, text: Union[str, Any], *args, **kwargs) -> List[tuple]:
+        """
+        Extracts paired comments and code blocks from Markdown content based on the 
+        specified programming language.
+        """
+        if self.language:
+            # If language is specified, directly extract the corresponding blocks
+            pattern = fr'```{self.language}\s*(.*?)```'
+            scripts = re.findall(pattern, text, re.DOTALL)
+            comments_temp = re.split(pattern, text, flags=re.DOTALL)
+        else:
+            # Extract blocks and languages dynamically if no specific language is provided
+            scripts = []
+            languages = []
+            for match in re.finditer(r'```(\w+)?\s*(.*?)```', text, re.DOTALL):
+                if match.group(1) is not None:  # Checks if a language identifier is present
+                    languages.append(match.group(1))
+                    scripts.append(match.group(2))
+                else:
+                    languages.append('')  # Default to an empty string if no language is found
+                    scripts.append(match.group(2))
+            comments_temp = re.split(r'```.*?```', text, flags=re.DOTALL)
+
+        comments = [comment.strip() for comment in comments_temp]
+
+        if text.strip().startswith('```'):
+            comments = [''] + comments
+        if text.strip().endswith('```'):
+            comments.append('')
+
+        if self.language:
+            structured_output = [(comments[i], self.language, scripts[i].strip()) for i in range(len(scripts))]
+        else:
+            structured_output = [(comments[i], languages[i], scripts[i].strip()) for i in range(len(scripts))]
+
+        return structured_output
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import re
-from swarmauri.core.chunkers.IChunker import IChunker
-
-class SimpleSentenceChunker(IChunker):
-    """
-    A simple implementation of the IChunker interface to chunk text into sentences.
-    
-    This class uses basic punctuation marks (., !, and ?) as indicators for sentence boundaries.
-    """
-    
-    def chunk_text(self, text, *args, **kwargs):
-        """
-        Chunks the given text into sentences using basic punctuation.
-
-        Args:
-            text (str): The input text to be chunked into sentences.
-        
-        Returns:
-            List[str]: A list of sentence chunks.
-        """
-        # Split text using a simple regex pattern that looks for periods, exclamation marks, or question marks.
-        # Note: This is a very simple approach and might not work well with abbreviations or other edge cases.
-        sentence_pattern = r'(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|!)\s'
-        sentences = re.split(sentence_pattern, text)
-        
-        # Filter out any empty strings that may have resulted from the split operation
-        sentences = [sentence.strip() for sentence in sentences if sentence]
-        
+from swarmauri.core.chunkers.IChunker import IChunker
+import re
+
+class SimpleSentenceChunker(IChunker):
+    """
+    A simple implementation of the IChunker interface to chunk text into sentences.
+    
+    This class uses basic punctuation marks (., !, and ?) as indicators for sentence boundaries.
+    """
+    
+    def chunk_text(self, text, *args, **kwargs):
+        """
+        Chunks the given text into sentences using basic punctuation.
+
+        Args:
+            text (str): The input text to be chunked into sentences.
+        
+        Returns:
+            List[str]: A list of sentence chunks.
+        """
+        # Split text using a simple regex pattern that looks for periods, exclamation marks, or question marks.
+        # Note: This is a very simple approach and might not work well with abbreviations or other edge cases.
+        sentence_pattern = r'(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|!)\s'
+        sentences = re.split(sentence_pattern, text)
+        
+        # Filter out any empty strings that may have resulted from the split operation
+        sentences = [sentence.strip() for sentence in sentences if sentence]
+        
         return sentences
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/conversations/base/SystemContextBase.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/base/SystemContextBase.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from abc import ABC
-from typing import Optional, Union
-from swarmauri.core.conversations.ISystemContext import ISystemContext
-from swarmauri.standard.messages.concrete.SystemMessage import SystemMessage
-from swarmauri.standard.conversations.base.ConversationBase import ConversationBase
-
-class SystemContextBase(ConversationBase, ISystemContext, ABC):
-    def __init__(self, *args, system_message_content: Optional[SystemMessage] = None):
-        ConversationBase.__init__(self)
-        # Automatically handle both string and SystemMessage types for initializing system context
-        self._system_context = None  # Initialize with None
-        if system_message_content:
-            self.system_context = system_message_content
-    
-    @property
-    def system_context(self) -> Union[SystemMessage, None]:
-        """Get the system context message. Raises an error if it's not set."""
-        if self._system_context is None:
-            raise ValueError("System context has not been set.")
-        return self._system_context
-    
-    @system_context.setter
-    def system_context(self, new_system_message: Union[SystemMessage, str]) -> None:
-        """
-        Set a new system context message. The new system message can be a string or 
-        an instance of SystemMessage. If it's a string, it converts it to a SystemMessage.
-        """
-        if isinstance(new_system_message, SystemMessage):
-            self._system_context = new_system_message
-        elif isinstance(new_system_message, str):
-            self._system_context = SystemMessage(new_system_message)
-        else:
+from abc import ABC, abstractmethod
+from typing import Optional, Union
+from ....core.messages.IMessage import IMessage
+from ....core.conversations.ISystemContext import ISystemContext
+from ...messages.concrete.SystemMessage import SystemMessage
+
+class SystemContextBase(ISystemContext, ABC):
+    def __init__(self, *args, system_message_content: Optional[SystemMessage] = None):
+        # Automatically handle both string and SystemMessage types for initializing system context
+        self._system_context = None  # Initialize with None
+        if system_message_content:
+            self.system_context = system_message_content
+    
+    @property
+    def system_context(self) -> Union[SystemMessage, None]:
+        """Get the system context message. Raises an error if it's not set."""
+        if self._system_context is None:
+            raise ValueError("System context has not been set.")
+        return self._system_context
+    
+    @system_context.setter
+    def system_context(self, new_system_message: Union[SystemMessage, str]) -> None:
+        """
+        Set a new system context message. The new system message can be a string or 
+        an instance of SystemMessage. If it's a string, it converts it to a SystemMessage.
+        """
+        if isinstance(new_system_message, SystemMessage):
+            self._system_context = new_system_message
+        elif isinstance(new_system_message, str):
+            self._system_context = SystemMessage(new_system_message)
+        else:
             raise ValueError("System context must be a string or a SystemMessage instance.")
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from ..base.ConversationBase import ConversationBase
-from ....core.messages.IMessage import IMessage
-from ....core.conversations.IMaxSize import IMaxSize
-
-class LimitedSizeConversation(ConversationBase, IMaxSize):
-    def __init__(self, max_size: int):
-        super().__init__()
-        self._max_size = max_size
-        
-    @property
-    def max_size(self) -> int:
-        """
-        Provides read-only access to the conversation history.
-        """
-        return self._max_size
-    
-    @max_size.setter
-    def max_size(self, new_max_size: int) -> int:
-        """
-        Provides read-only access to the conversation history.
-        """
-        if new_max_size > 0:
-            self._max_size = int
-        else:
-            raise ValueError('Cannot set conversation size to 0.')
-
-
-    def add_message(self, message: IMessage):
-        """Adds a message and ensures the conversation does not exceed the max size."""
-        super().add_message(message)
-        self._enforce_max_size_limit()
-
-    def _enforce_max_size_limit(self):
-        """
-        Enforces the maximum size limit of the conversation history.
-        If the current history size exceeds the maximum size, the oldest messages are removed.
-        """
-        while len(self._history) > self.max_size:
+from ..base.ConversationBase import ConversationBase
+from ....core.messages.IMessage import IMessage
+from ....core.conversations.IMaxSize import IMaxSize
+
+class LimitedSizeConversation(ConversationBase, IMaxSize):
+    def __init__(self, max_size: int):
+        super().__init__()
+        self._max_size = max_size
+        
+    @property
+    def max_size(self) -> int:
+        """
+        Provides read-only access to the conversation history.
+        """
+        return self._max_size
+    
+    @max_size.setter
+    def max_size(self, new_max_size: int) -> int:
+        """
+        Provides read-only access to the conversation history.
+        """
+        if new_max_size > 0:
+            self._max_size = int
+        else:
+            raise ValueError('Cannot set conversation size to 0.')
+
+
+    def add_message(self, message: IMessage):
+        """Adds a message and ensures the conversation does not exceed the max size."""
+        super().add_message(message)
+        self._enforce_max_size_limit(self)
+
+    def _enforce_max_size_limit(self):
+        """
+        Enforces the maximum size limit of the conversation history.
+        If the current history size exceeds the maximum size, the oldest messages are removed.
+        """
+        while len(self._history) > self.max_size:
             self._history.pop(0)
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,87 @@
-from typing import Optional, Union, List
-from swarmauri.core.messages.IMessage import IMessage
-from swarmauri.core.conversations.IMaxSize import IMaxSize
-from swarmauri.standard.conversations.base.SystemContextBase import SystemContextBase
-from swarmauri.standard.messages.concrete.SystemMessage import SystemMessage
-
-class LimitedSystemContextConversation(SystemContextBase, IMaxSize):
-    def __init__(self, max_size: int, system_message_content: Optional[SystemMessage] = None):
-        """
-        Initializes the conversation with a system context message and a maximum history size.
-        
-        Parameters:
-            max_size (int): The maximum number of messages allowed in the conversation history.
-            system_message_content (Optional[str], optional): The initial system message content. Can be a string.
-        """
-        SystemContextBase.__init__(self, system_message_content=system_message_content if system_message_content else "")  # Initialize SystemContext with a SystemMessage
-        self._max_size = max_size  # Set the maximum size
-    
-    @property
-    def history(self) -> List[IMessage]:
-        """
-        Provides read-only access to the conversation history.
-        """
-        
-        
-        res = [] 
-        res.append(self.system_context)
-        res.extend(self._history)
-        return res
-        
-        
-    @property
-    def max_size(self) -> int:
-        """
-        Provides access to the max_size property.
-        """
-        return self._max_size
-    
-    @max_size.setter
-    def max_size(self, new_max_size: int) -> None:
-        """
-        Sets a new maximum size for the conversation history.
-        """
-        if new_max_size <= 0:
-            raise ValueError("max_size must be greater than 0.")
-        self._max_size = new_max_size
-
-    def add_message(self, message: IMessage):
-        """
-        Adds a message to the conversation history and ensures history does not exceed the max size.
-        """
-        if isinstance(message, SystemMessage):
-            raise ValueError(f"System context cannot be set through this method on {self.__class_name__}.")
-        else:
-            super().add_message(message)
-        self._enforce_max_size_limit()
-        
-    def _enforce_max_size_limit(self):
-        """
-        Remove messages from the beginning of the conversation history if the limit is exceeded.
-        """
-        while len(self._history) + 1 > self._max_size:
-            self._history.pop(0)
-
-    @property
-    def system_context(self) -> Union[SystemMessage, None]:
-        """Get the system context message. Raises an error if it's not set."""
-        if self._system_context is None:
-            raise ValueError("System context has not been set.")
-        return self._system_context
-
-
-    @system_context.setter
-    def system_context(self, new_system_message: Union[SystemMessage, str]) -> None:
-        """
-        Set a new system context message. The new system message can be a string or 
-        an instance of SystemMessage. If it's a string, it converts it to a SystemMessage.
-        """
-        if isinstance(new_system_message, SystemMessage):
-            self._system_context = new_system_message
-        elif isinstance(new_system_message, str):
-            self._system_context = SystemMessage(new_system_message)
-        else:
-            raise ValueError("System context must be a string or a SystemMessage instance.")
+from typing import Optional, Union, List
+from ....core.messages.IMessage import IMessage
+from ....core.conversations.IMaxSize import IMaxSize
+from ..base.ConversationBase import ConversationBase
+from ..base.SystemContextBase import SystemContextBase
+from ...messages.concrete.SystemMessage import SystemMessage
+
+class LimitedSystemContextConversation(ConversationBase, SystemContextBase, IMaxSize):
+    def __init__(self, max_size: int, system_message_content: Optional[SystemMessage] = None):
+        """
+        Initializes the conversation with a system context message and a maximum history size.
+        
+        Parameters:
+            max_size (int): The maximum number of messages allowed in the conversation history.
+            system_message_content (Optional[str], optional): The initial system message content. Can be a string.
+        """
+        ConversationBase.__init__(self)  # Initialize the base Conversation
+        SystemContextBase.__init__(self, system_message_content=system_message_content if system_message_content else "")  # Initialize SystemContext with a SystemMessage
+        self._max_size = max_size  # Set the maximum size
+    
+    @property
+    def history(self) -> List[IMessage]:
+        """
+        Provides read-only access to the conversation history.
+        """
+        
+        
+        res = [] 
+        res.append(self.system_context)
+        res.extend(self._history)
+        return res
+        
+        
+    @property
+    def max_size(self) -> int:
+        """
+        Provides access to the max_size property.
+        """
+        return self._max_size
+    
+    @max_size.setter
+    def max_size(self, new_max_size: int) -> None:
+        """
+        Sets a new maximum size for the conversation history.
+        """
+        if new_max_size <= 0:
+            raise ValueError("max_size must be greater than 0.")
+        self._max_size = new_max_size
+
+    def add_message(self, message: IMessage):
+        """
+        Adds a message to the conversation history and ensures history does not exceed the max size.
+        """
+        if isinstance(message, SystemMessage):
+            raise ValueError(f"System context cannot be set through this method on {self.__class_name__}.")
+        else:
+            super().add_message(message)
+        self._enforce_max_size_limit()
+        
+    def _enforce_max_size_limit(self):
+        """
+        Remove messages from the beginning of the conversation history if the limit is exceeded.
+        """
+        while len(self._history) + 1 > self._max_size:
+            self._history.pop(0)
+
+    @property
+    def system_context(self) -> Union[SystemMessage, None]:
+        """Get the system context message. Raises an error if it's not set."""
+        if self._system_context is None:
+            raise ValueError("System context has not been set.")
+        return self._system_context
+
+
+    @system_context.setter
+    def system_context(self, new_system_message: Union[SystemMessage, str]) -> None:
+        """
+        Set a new system context message. The new system message can be a string or 
+        an instance of SystemMessage. If it's a string, it converts it to a SystemMessage.
+        """
+        if isinstance(new_system_message, SystemMessage):
+            self._system_context = new_system_message
+        elif isinstance(new_system_message, str):
+            self._system_context = SystemMessage(new_system_message)
+        else:
+            raise ValueError("System context must be a string or a SystemMessage instance.")
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/conversations/concrete/SharedConversation.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/concrete/SharedConversation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,115 @@
-import inspect
-from threading import Lock
-from typing import Optional, Dict, List, Tuple
-from swarmauri.core.messages.IMessage import IMessage
-from swarmauri.standard.conversations.base.ConversationBase import ConversationBase
-from swarmauri.standard.messages.concrete.HumanMessage import HumanMessage
-from swarmauri.standard.messages.concrete.SystemMessage import SystemMessage
-
-class SharedConversation(ConversationBase):
-    """
-    A thread-safe conversation class that supports individual system contexts for each SwarmAgent.
-    """
-    def __init__(self):
-        super().__init__()
-        self._lock = Lock()  # A lock to ensure thread safety
-        self._agent_system_contexts: Dict[str, SystemMessage] = {}  # Store system contexts for each agent
-        self._history: List[Tuple[str, IMessage]] = []  # Stores tuples of (sender_id, IMessage)
-
-
-    @property
-    def history(self):
-        history = []
-        for each in self._history:
-            history.append((each[0], each[1]))
-        return history
-
-    def add_message(self, message: IMessage, sender_id: str):
-        with self._lock:
-            self._history.append((sender_id, message))
-
-    def reset_messages(self) -> None:
-        self._history = []
-        
-
-    def _get_caller_name(self) -> Optional[str]:
-        for frame_info in inspect.stack():
-            # Check each frame for an instance with a 'name' attribute in its local variables
-            local_variables = frame_info.frame.f_locals
-            for var_name, var_value in local_variables.items():
-                if hasattr(var_value, 'name'):
-                    # Found an instance with a 'name' attribute. Return its value.
-                    return getattr(var_value, 'name')
-        # No suitable caller found
-        return None
-
-    def as_dict(self) -> List[Dict]:
-        caller_name = self._get_caller_name()
-        history = []
-
-        with self._lock:
-            # If Caller is not one of the agents, then give history
-            if caller_name not in self._agent_system_contexts.keys():
-                for sender_id, message in self._history:
-                    history.append((sender_id, message.as_dict()))
-                
-                
-            else:
-                system_context = self.get_system_context(caller_name)
-                #print(caller_name, system_context, type(system_context))
-                if type(system_context) == str:
-                    history.append(SystemMessage(system_context).as_dict())
-                else:
-                    history.append(system_context.as_dict())
-                    
-                for sender_id, message in self._history:
-                    #print(caller_name, sender_id, message, type(message))
-                    if sender_id == caller_name:
-                        if message.__class__.__name__ == 'AgentMessage' or 'FunctionMessage':
-                            # The caller is the sender; treat as AgentMessage
-                            history.append(message.as_dict())
-                            
-                            # Print to see content that is empty.
-                            #if not message.content:
-                                #print('\n\t\t\t=>', message, message.content)
-                    else:
-                        if message.content:
-                            # The caller is not the sender; treat as HumanMessage
-                            history.append(HumanMessage(message.content).as_dict())
-        return history
-    
-    def get_last(self) -> IMessage:
-        with self._lock:
-            return super().get_last()
-
-
-    def clear_history(self):
-        with self._lock:
-            super().clear_history()
-
-
-        
-
-    def set_system_context(self, agent_id: str, context: SystemMessage):
-        """
-        Sets the system context for a specific agent.
-
-        Args:
-            agent_id (str): Unique identifier for the agent.
-            context (SystemMessage): The context message to be set for the agent.
-        """
-        with self._lock:
-            self._agent_system_contexts[agent_id] = context
-
-    def get_system_context(self, agent_id: str) -> Optional[SystemMessage]:
-        """
-        Retrieves the system context for a specific agent.
-
-        Args:
-            agent_id (str): Unique identifier for the agent.
-
-        Returns:
-            Optional[SystemMessage]: The context message of the agent, or None if not found.
-        """
+import inspect
+from threading import Lock
+from typing import Optional, Dict, List, Tuple
+from swarmauri.core.messages.IMessage import IMessage
+from swarmauri.standard.conversations.base.ConversationBase import ConversationBase
+from swarmauri.standard.messages.concrete.HumanMessage import HumanMessage
+from swarmauri.standard.messages.concrete.SystemMessage import SystemMessage
+from swarmauri.standard.messages.concrete.AgentMessage import AgentMessage
+
+class SharedConversation(ConversationBase):
+    """
+    A thread-safe conversation class that supports individual system contexts for each SwarmAgent.
+    """
+    def __init__(self):
+        super().__init__()
+        self._lock = Lock()  # A lock to ensure thread safety
+        self._agent_system_contexts: Dict[str, SystemMessage] = {}  # Store system contexts for each agent
+        self._history: List[Tuple[str, IMessage]] = []  # Stores tuples of (sender_id, IMessage)
+
+
+    @property
+    def history(self):
+        history = []
+        for each in self._history:
+            history.append((each[0], each[1]))
+        return history
+
+    def add_message(self, message: IMessage, sender_id: str):
+        with self._lock:
+            self._history.append((sender_id, message))
+
+    def reset_messages(self) -> None:
+        self._history = []
+        
+
+    def _get_caller_name(self) -> Optional[str]:
+        for frame_info in inspect.stack():
+            # Check each frame for an instance with a 'name' attribute in its local variables
+            local_variables = frame_info.frame.f_locals
+            for var_name, var_value in local_variables.items():
+                if hasattr(var_value, 'name'):
+                    # Found an instance with a 'name' attribute. Return its value.
+                    return getattr(var_value, 'name')
+        # No suitable caller found
+        return None
+
+    def as_dict(self) -> List[Dict]:
+        caller_name = self._get_caller_name()
+        history = []
+
+        with self._lock:
+            # If Caller is not one of the agents, then give history
+            if caller_name not in self._agent_system_contexts.keys():
+                for sender_id, message in self._history:
+                    history.append((sender_id, message.as_dict()))
+                
+                
+            else:
+                system_context = self.get_system_context(caller_name)
+                #print(caller_name, system_context, type(system_context))
+                if type(system_context) == str:
+                    history.append(SystemMessage(system_context).as_dict())
+                else:
+                    history.append(system_context.as_dict())
+                    
+                for sender_id, message in self._history:
+                    #print(caller_name, sender_id, message, type(message))
+                    if sender_id == caller_name:
+                        if message.__class__.__name__ == 'AgentMessage' or 'FunctionMessage':
+                            # The caller is the sender; treat as AgentMessage
+                            history.append(message.as_dict())
+                            
+                            # Print to see content that is empty.
+                            #if not message.content:
+                                #print('\n\t\t\t=>', message, message.content)
+                    else:
+                        if message.content:
+                            # The caller is not the sender; treat as HumanMessage
+                            history.append(HumanMessage(message.content).as_dict())
+        return history
+    
+    def get_last(self) -> IMessage:
+        with self._lock:
+            return super().get_last()
+
+
+    def clear_history(self):
+        with self._lock:
+            super().clear_history()
+
+
+        
+
+    def set_system_context(self, agent_id: str, context: SystemMessage):
+        """
+        Sets the system context for a specific agent.
+
+        Args:
+            agent_id (str): Unique identifier for the agent.
+            context (SystemMessage): The context message to be set for the agent.
+        """
+        with self._lock:
+            self._agent_system_contexts[agent_id] = context
+
+    def get_system_context(self, agent_id: str) -> Optional[SystemMessage]:
+        """
+        Retrieves the system context for a specific agent.
+
+        Args:
+            agent_id (str): Unique identifier for the agent.
+
+        Returns:
+            Optional[SystemMessage]: The context message of the agent, or None if not found.
+        """
         return self._agent_system_contexts.get(agent_id, None)
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/distances/concrete/ChiSquaredDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/ChebyshevDistance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,47 @@
-from typing import List
-from swarmauri.core.distances.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-class ChiSquaredDistance(IDistanceSimilarity):
-    """
-    Implementation of the IDistanceSimilarity interface using Chi-squared distance metric.
-    """
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Chi-squared distance between two vectors.
-        """
-        if len(vector_a.data) != len(vector_b.data):
-            raise ValueError("Vectors must have the same dimensionality.")
-
-        chi_squared_distance = 0
-        for a, b in zip(vector_a.data, vector_b.data):
-            if (a + b) != 0:
-                chi_squared_distance += (a - b) ** 2 / (a + b)
-
-        return 0.5 * chi_squared_distance
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Compute the similarity between two vectors based on the Chi-squared distance.
-        """
-        return 1 / (1 + self.distance(vector_a, vector_b))
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
+from typing import List
+from swarmauri.core.vectors.IVector import IVector
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+
+class ChebyshevDistance(IDistanceSimilarity):
+    """
+    Concrete implementation of the IDistanceSimiliarity interface using the Chebyshev distance metric.
+    Chebyshev distance is the maximum absolute distance between two vectors' elements.
+    """
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Chebyshev distance between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector in the comparison.
+            vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+            float: The computed Chebyshev distance between vector_a and vector_b.
+        """
+        max_distance = 0
+        for a, b in zip(vector_a.data, vector_b.data):
+            max_distance = max(max_distance, abs(a - b))
+        return max_distance
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the similarity between two vectors based on the Chebyshev distance.
+
+        Args:
+            vector_a (IVector): The first vector.
+            vector_b (IVector): The second vector.
+
+        Returns:
+            float: The similarity score between the two vectors.
+        """
+
+        return 1 / (1 + self.distance(vector_a, vector_b))
+    
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
         return similarities
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/distances/concrete/EuclideanDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-from math import sqrt
-from typing import List
-from swarmauri.core.distances.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-
-class EuclideanDistance(IDistanceSimilarity):
-    """
-    Class to compute the Euclidean distance between two vectors.
-    Implements the IDistanceSimiliarity interface.
-    """
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Euclidean distance between two vectors.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            float: The computed Euclidean distance between vector_a and vector_b.
-        """
-        if len(vector_a.data) != len(vector_b.data):
-            raise ValueError("Vectors do not have the same dimensionality.")
-        
-        distance = sqrt(sum((a - b) ** 2 for a, b in zip(vector_a.data, vector_b.data)))
-        return distance
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the similarity score as the inverse of the Euclidean distance between two vectors.
-
-        Args:
-            vector_a (IVector): The first vector in the comparison.
-            vector_b (IVector): The second vector in the comparison.
-
-        Returns:
-            float: The similarity score between vector_a and vector_b.
-        """
-        distance = self.distance(vector_a, vector_b)
-        return 1 / (1 + distance)
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
-        return similarities
+from typing import List
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+class SquaredEuclideanDistance(IDistanceSimilarity):
+    """
+    A concrete class for computing the squared Euclidean distance between two vectors.
+    """
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the squared Euclidean distance between vectors `vector_a` and `vector_b`.
+
+        Parameters:
+        - vector_a (IVector): The first vector in the comparison.
+        - vector_b (IVector): The second vector in the comparison.
+
+        Returns:
+        - float: The computed squared Euclidean distance between vector_a and vector_b.
+        """
+        if vector_a.dimensions != vector_b.dimensions:
+            raise ValueError("Vectors must be of the same dimensionality.")
+
+        squared_distance = sum((a - b) ** 2 for a, b in zip(vector_a.data, vector_b.data))
+        return squared_distance
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Squared Euclidean distance is not used for calculating similarity.
+        
+        Parameters:
+        - vector_a (IVector): The first vector.
+        - vector_b (IVector): The second vector.
+
+        Raises:
+        - NotImplementedError: Indicates that similarity calculation is not implemented.
+        """
+        raise NotImplementedError("Similarity calculation is not implemented for Squared Euclidean distance.")
+        
+        
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        raise NotImplementedError("Similarity calculation is not implemented for Squared Euclidean distance.")
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/distances/concrete/JaccardIndexDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/JaccardIndexDistance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from typing import List
-from swarmauri.core.distances.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-class JaccardIndexDistance(IDistanceSimilarity):
-    """
-    A class implementing Jaccard Index as a similarity and distance metric between two vectors.
-    """
-
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Jaccard distance between two vectors.
-
-        The Jaccard distance, which is 1 minus the Jaccard similarity,
-        measures dissimilarity between sample sets. It's defined as
-        1 - (the intersection of the sets divided by the union of the sets).
-
-        Args:
-            vector_a (IVector): The first vector.
-            vector_b (IVector): The second vector.
-
-        Returns:
-            float: The Jaccard distance between vector_a and vector_b.
-        """
-        set_a = set(vector_a.data)
-        set_b = set(vector_b.data)
-
-        # Calculate the intersection and union of the two sets.
-        intersection = len(set_a.intersection(set_b))
-        union = len(set_a.union(set_b))
-
-        # In the special case where the union is zero, return 1.0 which implies complete dissimilarity.
-        if union == 0:
-            return 1.0
-
-        # Compute Jaccard similarity and then return the distance as 1 - similarity.
-        jaccard_similarity = intersection / union
-        return 1 - jaccard_similarity
-
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Computes the Jaccard similarity between two vectors.
-
-        Args:
-            vector_a (IVector): The first vector.
-            vector_b (IVector): The second vector.
-
-        Returns:
-            float: Jaccard similarity score between vector_a and vector_b.
-        """
-        set_a = set(vector_a.data)
-        set_b = set(vector_b.data)
-
-        # Calculate the intersection and union of the two sets.
-        intersection = len(set_a.intersection(set_b))
-        union = len(set_a.union(set_b))
-
-        # In case the union is zero, which means both vectors have no elements, return 1.0 implying identical sets.
-        if union == 0:
-            return 1.0
-
-        # Compute and return Jaccard similarity.
-        return intersection / union
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
+from typing import List
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+class JaccardIndexDistance(IDistanceSimilarity):
+    """
+    A class implementing Jaccard Index as a similarity and distance metric between two vectors.
+    """
+
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Jaccard distance between two vectors.
+
+        The Jaccard distance, which is 1 minus the Jaccard similarity,
+        measures dissimilarity between sample sets. It's defined as
+        1 - (the intersection of the sets divided by the union of the sets).
+
+        Args:
+            vector_a (IVector): The first vector.
+            vector_b (IVector): The second vector.
+
+        Returns:
+            float: The Jaccard distance between vector_a and vector_b.
+        """
+        set_a = set(vector_a.data)
+        set_b = set(vector_b.data)
+
+        # Calculate the intersection and union of the two sets.
+        intersection = len(set_a.intersection(set_b))
+        union = len(set_a.union(set_b))
+
+        # In the special case where the union is zero, return 1.0 which implies complete dissimilarity.
+        if union == 0:
+            return 1.0
+
+        # Compute Jaccard similarity and then return the distance as 1 - similarity.
+        jaccard_similarity = intersection / union
+        return 1 - jaccard_similarity
+
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Computes the Jaccard similarity between two vectors.
+
+        Args:
+            vector_a (IVector): The first vector.
+            vector_b (IVector): The second vector.
+
+        Returns:
+            float: Jaccard similarity score between vector_a and vector_b.
+        """
+        set_a = set(vector_a.data)
+        set_b = set(vector_b.data)
+
+        # Calculate the intersection and union of the two sets.
+        intersection = len(set_a.intersection(set_b))
+        union = len(set_a.union(set_b))
+
+        # In case the union is zero, which means both vectors have no elements, return 1.0 implying identical sets.
+        if union == 0:
+            return 1.0
+
+        # Compute and return Jaccard similarity.
+        return intersection / union
+    
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
         return similarities
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/distances/concrete/LevenshteinDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/LevenshteinDistance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from typing import List
-import numpy as np
-from swarmauri.core.distances.IDistanceSimilarity import IDistanceSimilarity
-from swarmauri.core.vectors.IVector import IVector
-
-class LevenshteinDistance(IDistanceSimilarity):
-    """
-    Implements the IDistance interface to calculate the Levenshtein distance between two vectors.
-    The Levenshtein distance between two strings is given by the minimum number of operations needed to transform
-    one string into the other, where an operation is an insertion, deletion, or substitution of a single character.
-    """
-    
-    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
-        """
-        Compute the Levenshtein distance between two vectors.
-
-        Note: Since Levenshtein distance is typically calculated between strings,
-        it is assumed that the vectors represent strings where each element of the
-        vector corresponds to the ASCII value of a character in the string.
-
-        Args:
-            vector_a (List[float]): The first vector in the comparison.
-            vector_b (List[float]): The second vector in the comparison.
-
-        Returns:
-           float: The computed Levenshtein distance between vector_a and vector_b.
-        """
-        string_a = ''.join([chr(int(round(value))) for value in vector_a.data])
-        string_b = ''.join([chr(int(round(value))) for value in vector_b.data])
-        
-        return self.levenshtein(string_a, string_b)
-    
-    def levenshtein(self, seq1: str, seq2: str) -> float:
-        """
-        Calculate the Levenshtein distance between two strings.
-        
-        Args:
-            seq1 (str): The first string.
-            seq2 (str): The second string.
-        
-        Returns:
-            float: The Levenshtein distance between seq1 and seq2.
-        """
-        size_x = len(seq1) + 1
-        size_y = len(seq2) + 1
-        matrix = np.zeros((size_x, size_y))
-        
-        for x in range(size_x):
-            matrix[x, 0] = x
-        for y in range(size_y):
-            matrix[0, y] = y
-
-        for x in range(1, size_x):
-            for y in range(1, size_y):
-                if seq1[x-1] == seq2[y-1]:
-                    matrix[x, y] = min(matrix[x-1, y] + 1, matrix[x-1, y-1], matrix[x, y-1] + 1)
-                else:
-                    matrix[x, y] = min(matrix[x-1, y] + 1, matrix[x-1, y-1] + 1, matrix[x, y-1] + 1)
-        
-        return matrix[size_x - 1, size_y - 1]
-    
-    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
-        string_a = ''.join([chr(int(round(value))) for value in vector_a.data])
-        string_b = ''.join([chr(int(round(value))) for value in vector_b.data])
-        return 1 - self.levenshtein(string_a, string_b) / max(len(vector_a), len(vector_b))
-    
-    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
-        return distances
-    
-    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
-        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
+from typing import List
+import numpy as np
+from swarmauri.core.vector_stores.IDistanceSimilarity import IDistanceSimilarity
+from swarmauri.core.vectors.IVector import IVector
+
+class LevenshteinDistance(IDistanceSimilarity):
+    """
+    Implements the IDistance interface to calculate the Levenshtein distance between two vectors.
+    The Levenshtein distance between two strings is given by the minimum number of operations needed to transform
+    one string into the other, where an operation is an insertion, deletion, or substitution of a single character.
+    """
+    
+    def distance(self, vector_a: IVector, vector_b: IVector) -> float:
+        """
+        Compute the Levenshtein distance between two vectors.
+
+        Note: Since Levenshtein distance is typically calculated between strings,
+        it is assumed that the vectors represent strings where each element of the
+        vector corresponds to the ASCII value of a character in the string.
+
+        Args:
+            vector_a (List[float]): The first vector in the comparison.
+            vector_b (List[float]): The second vector in the comparison.
+
+        Returns:
+           float: The computed Levenshtein distance between vector_a and vector_b.
+        """
+        string_a = ''.join([chr(int(round(value))) for value in vector_a.data])
+        string_b = ''.join([chr(int(round(value))) for value in vector_b.data])
+        
+        return self.levenshtein(string_a, string_b)
+    
+    def levenshtein(self, seq1: str, seq2: str) -> float:
+        """
+        Calculate the Levenshtein distance between two strings.
+        
+        Args:
+            seq1 (str): The first string.
+            seq2 (str): The second string.
+        
+        Returns:
+            float: The Levenshtein distance between seq1 and seq2.
+        """
+        size_x = len(seq1) + 1
+        size_y = len(seq2) + 1
+        matrix = np.zeros((size_x, size_y))
+        
+        for x in range(size_x):
+            matrix[x, 0] = x
+        for y in range(size_y):
+            matrix[0, y] = y
+
+        for x in range(1, size_x):
+            for y in range(1, size_y):
+                if seq1[x-1] == seq2[y-1]:
+                    matrix[x, y] = min(matrix[x-1, y] + 1, matrix[x-1, y-1], matrix[x, y-1] + 1)
+                else:
+                    matrix[x, y] = min(matrix[x-1, y] + 1, matrix[x-1, y-1] + 1, matrix[x, y-1] + 1)
+        
+        return matrix[size_x - 1, size_y - 1]
+    
+    def similarity(self, vector_a: IVector, vector_b: IVector) -> float:
+        string_a = ''.join([chr(int(round(value))) for value in vector_a.data])
+        string_b = ''.join([chr(int(round(value))) for value in vector_b.data])
+        return 1 - self.levenshtein(string_a, string_b) / max(len(vector_a), len(vector_b))
+    
+    def distances(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        distances = [self.distance(vector_a, vector_b) for vector_b in vectors_b]
+        return distances
+    
+    def similarities(self, vector_a: IVector, vectors_b: List[IVector]) -> List[float]:
+        similarities = [self.similarity(vector_a, vector_b) for vector_b in vectors_b]
         return similarities
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/messages/base/MessageBase.py` & `swarmauri-0.1.9/swarmauri/standard/messages/base/MessageBase.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from abc import ABC, abstractmethod
-from swarmauri.core.messages.IMessage import IMessage
-
-class MessageBase(IMessage, ABC):
-    
-    @abstractmethod
-    def __init__(self, role: str, content: str):
-        self._role = role
-        self._content = content
-    
-    @property
-    def role(self) -> str:
-        return self._role
-    
-    @property
-    def content(self) -> str:
-        return self._content
-
-    
-    def as_dict(self) -> dict:
-        """
-        Dynamically return a dictionary representation of the object,
-        including all properties.
-        """
-        result_dict = {}
-        # Iterate over all attributes
-        for attr in dir(self):
-            # Skip private attributes and anything not considered a property
-            if attr.startswith("_") or callable(getattr(self, attr)):
-                continue
-            result_dict[attr] = getattr(self, attr)
-            
-        return result_dict
-
-    def __repr__(self) -> str:
-        """
-        Return the string representation of the ConcreteMessage.
-        """
-        return f"{self.__class__.__name__}(role='{self.role}')"
-    
-    def __getattr__(self, name):
-        """
-        Return the value of the named attribute of the instance.
-        """
-        try:
-            return self.__dict__[name]
-        except KeyError:
-            raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'")
-
-    
-    def __setattr__(self, name, value):
-        """
-        Set the value of the named attribute of the instance.
-        """
+from abc import ABC, abstractmethod
+from ....core.messages.IMessage import IMessage
+
+class MessageBase(IMessage, ABC):
+    
+    @abstractmethod
+    def __init__(self, role: str, content: str):
+        self._role = role
+        self._content = content
+    
+    @property
+    def role(self) -> str:
+        return self._role
+    
+    @property
+    def content(self) -> str:
+        return self._content
+
+    
+    def as_dict(self) -> dict:
+        """
+        Dynamically return a dictionary representation of the object,
+        including all properties.
+        """
+        result_dict = {}
+        # Iterate over all attributes
+        for attr in dir(self):
+            # Skip private attributes and anything not considered a property
+            if attr.startswith("_") or callable(getattr(self, attr)):
+                continue
+            result_dict[attr] = getattr(self, attr)
+            
+        return result_dict
+
+    def __repr__(self) -> str:
+        """
+        Return the string representation of the ConcreteMessage.
+        """
+        return f"{self.__class__.__name__}(role='{self.role}')"
+    
+    def __getattr__(self, name):
+        """
+        Return the value of the named attribute of the instance.
+        """
+        try:
+            return self.__dict__[name]
+        except KeyError:
+            raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'")
+
+    
+    def __setattr__(self, name, value):
+        """
+        Set the value of the named attribute of the instance.
+        """
         self.__dict__[name] = value
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/messages/concrete/FunctionMessage.py` & `swarmauri-0.1.9/swarmauri/standard/messages/concrete/FunctionMessage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from swarmauri.standard.messages.base.MessageBase import MessageBase
-
-
-class FunctionMessage(MessageBase):
-    """
-    Represents a message created by a human user.
-
-    This class extends the `Message` class to specifically represent messages that
-    are input by human users in a conversational interface. It contains the message
-    content and assigns the type "HumanMessage" to distinguish it from other types
-    of messages.
-
-    Attributes:
-        content (str): The text content of the message.
-
-    Methods:
-        display: Returns a dictionary representation of the message for display,
-                 tagging it with the role "user".
-    """
-
-    def __init__(self, content, name, tool_call_id):
-        super().__init__(role='tool', content=content)
-        self.name = name
-        self.tool_call_id = tool_call_id
+from ..base.MessageBase import MessageBase
+
+
+class FunctionMessage(MessageBase):
+    """
+    Represents a message created by a human user.
+
+    This class extends the `Message` class to specifically represent messages that
+    are input by human users in a conversational interface. It contains the message
+    content and assigns the type "HumanMessage" to distinguish it from other types
+    of messages.
+
+    Attributes:
+        content (str): The text content of the message.
+
+    Methods:
+        display: Returns a dictionary representation of the message for display,
+                 tagging it with the role "user".
+    """
+
+    def __init__(self, content, name, tool_call_id):
+        super().__init__(role='tool', content=content)
+        self.name = name
+        self.tool_call_id = tool_call_id
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/messages/concrete/HumanMessage.py` & `swarmauri-0.1.9/swarmauri/standard/messages/concrete/HumanMessage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from swarmauri.standard.messages.base.MessageBase import MessageBase
-
-class HumanMessage(MessageBase):
-    """
-    Represents a message created by a human user.
-
-    Extends the `Message` class to specifically represent messages input by human users in a conversational
-    interface. It contains the message content and assigns the type "HumanMessage" to distinguish it from
-    other types of messages.
-    """
-
-    def __init__(self, content, name=None):
-        """
-        Initializes a new instance of HumanMessage with specified content.
-
-        Args:
-            content (str): The text content of the human-created message.
-            name (str, optional): The name of the human sender.
-        """
-        super().__init__(role='user', content=content)
-
+from ..base.MessageBase import MessageBase
+
+class HumanMessage(MessageBase):
+    """
+    Represents a message created by a human user.
+
+    Extends the `Message` class to specifically represent messages input by human users in a conversational
+    interface. It contains the message content and assigns the type "HumanMessage" to distinguish it from
+    other types of messages.
+    """
+
+    def __init__(self, content, name=None):
+        """
+        Initializes a new instance of HumanMessage with specified content.
+
+        Args:
+            content (str): The text content of the human-created message.
+            name (str, optional): The name of the human sender.
+        """
+        super().__init__(role='user', content=content)
+
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/messages/concrete/SystemMessage.py` & `swarmauri-0.1.9/swarmauri/standard/messages/concrete/SystemMessage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from swarmauri.standard.messages.base.MessageBase import MessageBase
-
-class SystemMessage(MessageBase):
-    """
-    SystemMessage class represents a message generated by the system. 
-    
-    This type of message is used to communicate system-level information such as 
-    errors, notifications, or updates to the user. Inherits from the Message base class.
-    
-    Attributes:
-        content (str): The content of the system message.
-    """
-    
-    def __init__(self, content):
-        super().__init__(role='system', content=content)
-    
+from ..base.MessageBase import MessageBase
+
+class SystemMessage(MessageBase):
+    """
+    SystemMessage class represents a message generated by the system. 
+    
+    This type of message is used to communicate system-level information such as 
+    errors, notifications, or updates to the user. Inherits from the Message base class.
+    
+    Attributes:
+        content (str): The content of the system message.
+    """
+    
+    def __init__(self, content):
+        super().__init__(role='system', content=content)
+
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/models/base/ModelBase.py` & `swarmauri-0.1.9/swarmauri/standard/models/base/ModelBase.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from abc import ABC, abstractmethod
-from typing import Any
-from ....core.models.IModel import IModel
-
-class ModelBase(IModel, ABC):
-    """
-    Concrete implementation of the IModel abstract base class.
-    This version includes managing the model name through a property and a setter.
-    """
-    @abstractmethod
-    def __init__(self, model_name: str):
-        self._model_name = model_name
-    
-    @property
-    def model_name(self):
-        return self._model_name
-    
-    @model_name.setter
-    def model_name(self, value: str) -> None:
-        """
-        Property setter that sets the name of the model.
-
-        Parameters:
-        - value (str): The new name of the model.
-        """
-        self._model_name = value
-       
-    
+from abc import ABC, abstractmethod
+from typing import Any
+from ....core.models.IModel import IModel
+
+class ModelBase(IModel, ABC):
+    """
+    Concrete implementation of the IModel abstract base class.
+    This version includes managing the model name through a property and a setter.
+    """
+    @abstractmethod
+    def __init__(self, model_name: str):
+        self._model_name = model_name
+    
+    @property
+    def model_name(self):
+        return self._model_name
+    
+    @model_name.setter
+    def model_name(self, value: str) -> None:
+        """
+        Property setter that sets the name of the model.
+
+        Parameters:
+        - value (str): The new name of the model.
+        """
+        self._model_name = value
+       
+
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/models/concrete/AzureGPT.py` & `swarmauri-0.1.9/swarmauri/standard/models/concrete/AzureGPT.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import json
-from openai import AzureOpenAI
-from ..base.ModelBase import ModelBase
-from ....core.models.IPredict import IPredict
-
-class AzureGPT(ModelBase, IPredict):
-    def __init__(self, azure_endpoint: str, api_key: str, api_version: str, model_name: str):
-        """
-        Initialize the Azure model with an API key.
-
-        Parameters:
-        - api_key (str): Your OpenAI API key.
-        """
-        self.azure_endpoint = azure_endpoint
-        self.api_key = api_key
-        self.api_version = api_version
-        self.client = AzureOpenAI(
-                azure_endpoint = azure_endpoint, 
-                api_key = api_key,  
-                api_version = api_version
-            )
-        super().__init__(model_name)
-       
-
-    
-    def predict(self, messages, temperature=0.7, max_tokens=256, enable_json=True):
-        """
-        Generate predictions using the OpenAI model.
-
-        Parameters:
-        - messages: Input data/messages for the model.
-        - temperature (float): Sampling temperature.
-        - max_tokens (int): Maximum number of tokens to generate.
-        - enable_json (bool): Format response as JSON.
-        
-        Returns:
-        - The generated message content.
-        """
-        if self.client is None:
-            raise Exception("OpenAI client is not initialized. Call 'load_model' first.")
-        
-        if enable_json:
-            response = self.client.chat.completions.create(
-                model=self.model_name,
-                messages=messages,
-                temperature=temperature,
-                response_format={ "type": "json_object" },
-                max_tokens=max_tokens,
-                top_p=1,
-                frequency_penalty=0,
-                presence_penalty=0,
-                stop=None
-            )
-        else:
-            response = self.client.chat.completions.create(
-                model=self.model_name,
-                messages=messages,
-                temperature=temperature,
-                max_tokens=max_tokens,
-                top_p=1,
-                frequency_penalty=0,
-                presence_penalty=0,
-                stop=None
-            )
-        
-        result = response.json()
-        message_content = json.loads(result['choices'][0]['message']['content'])
-        
+import json
+from openai import AzureOpenAI
+from ..base.ModelBase import ModelBase
+from ....core.models.IPredict import IPredict
+
+class AzureGPT(ModelBase, IPredict):
+    def __init__(self, azure_endpoint: str, api_key: str, api_version: str, model_name: str):
+        """
+        Initialize the Azure model with an API key.
+
+        Parameters:
+        - api_key (str): Your OpenAI API key.
+        """
+        self.azure_endpoint = azure_endpoint
+        self.api_key = api_key
+        self.api_version = api_version
+        self.client = AzureOpenAI(
+                azure_endpoint = azure_endpoint, 
+                api_key = api_key,  
+                api_version = api_version
+            )
+        super().__init__(model_name)
+       
+
+    
+    def predict(self, messages, temperature=0.7, max_tokens=256, enable_json=True):
+        """
+        Generate predictions using the OpenAI model.
+
+        Parameters:
+        - messages: Input data/messages for the model.
+        - temperature (float): Sampling temperature.
+        - max_tokens (int): Maximum number of tokens to generate.
+        - enable_json (bool): Format response as JSON.
+        
+        Returns:
+        - The generated message content.
+        """
+        if self.client is None:
+            raise Exception("OpenAI client is not initialized. Call 'load_model' first.")
+        
+        if enable_json:
+            response = self.client.chat.completions.create(
+                model=self.model_name,
+                messages=messages,
+                temperature=temperature,
+                response_format={ "type": "json_object" },
+                max_tokens=max_tokens,
+                top_p=1,
+                frequency_penalty=0,
+                presence_penalty=0,
+                stop=None
+            )
+        else:
+            response = self.client.chat.completions.create(
+                model=self.model_name,
+                messages=messages,
+                temperature=temperature,
+                max_tokens=max_tokens,
+                top_p=1,
+                frequency_penalty=0,
+                presence_penalty=0,
+                stop=None
+            )
+        
+        result = response.json()
+        message_content = json.loads(result['choices'][0]['message']['content'])
+        
         return message_content
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/models/concrete/OpenAIToolModel.py` & `swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIToolModel.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from openai import OpenAI
-from swarmauri.standard.models.base.ModelBase import ModelBase
-from swarmauri.core.models.IPredict import IPredict
-
-class OpenAIToolModel(ModelBase, IPredict):
-    def __init__(self, api_key: str, model_name: str = "gpt-3.5-turbo-0125"):
-        self.client = OpenAI(api_key=api_key)
-        super().__init__(model_name)
-
-    def predict(self, messages, tools=None, tool_choice=None, temperature=0.7, max_tokens=1024):
-        if tools and not tool_choice:
-            tool_choice = "auto"
-        response = self.client.chat.completions.create(
-            model=self.model_name,
-            messages=messages,
-            temperature=temperature,
-            max_tokens=max_tokens,
-            tools=tools,
-            tool_choice=tool_choice,
-        )
+from openai import OpenAI
+from swarmauri.standard.models.base.ModelBase import ModelBase
+from swarmauri.core.models.IPredict import IPredict
+
+class OpenAIToolModel(ModelBase, IPredict):
+    def __init__(self, api_key: str, model_name: str = "gpt-3.5-turbo-0125"):
+        self.client = OpenAI(api_key=api_key)
+        super().__init__(model_name)
+
+    def predict(self, messages, tools=None, tool_choice=None, temperature=0.7, max_tokens=1024):
+        if tools and not tool_choice:
+            tool_choice = "auto"
+        response = self.client.chat.completions.create(
+            model=self.model_name,
+            messages=messages,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            tools=tools,
+            tool_choice=tool_choice,
+        )
         return response
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from typing import List, Union, Any
-from transformers import BertTokenizer, BertModel
-import torch
-from swarmauri.core.parsers.IParser import IParser
-from swarmauri.core.documents.IDocument import IDocument
-from swarmauri.standard.documents.concrete.Document import Document
-
-class BERTEmbeddingParser(IParser):
-    """
-    A parser that transforms input text into document embeddings using BERT.
-    
-    This parser tokenizes the input text, passes it through a pre-trained BERT model,
-    and uses the resulting embeddings as the document content.
-    """
-
-    def __init__(self, model_name: str = 'bert-base-uncased'):
-        """
-        Initializes the BERTEmbeddingParser with a specific BERT model.
-        
-        Parameters:
-        - model_name (str): The name of the pre-trained BERT model to use.
-        """
-        self.tokenizer = BertTokenizer.from_pretrained(model_name)
-        self.model = BertModel.from_pretrained(model_name)
-        self.model.eval()  # Set model to evaluation mode
-
-    
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Tokenizes input data and generates embeddings using a BERT model.
-
-        Parameters:
-        - data (Union[str, Any]): Input data, expected to be a single string or batch of strings.
-
-        Returns:
-        - List[IDocument]: A list containing a single IDocument instance with BERT embeddings as content.
-        """
-        
-        # Tokenization
-        inputs = self.tokenizer(data, return_tensors='pt', padding=True, truncation=True, max_length=512)
-
-        # Generate embeddings
-        with torch.no_grad():
-            outputs = self.model(**inputs)
-
-        # Use the last hidden state as document embeddings (batch_size, sequence_length, hidden_size)
-        embeddings = outputs.last_hidden_state
-        
-        # Convert to list of numpy arrays
-        embeddings = embeddings.detach().cpu().numpy()
-        
-        # For simplicity, let's consider the mean of embeddings across tokens to represent the document
-        doc_embeddings = embeddings.mean(axis=1)
-        
-        # Creating document object(s)
-        documents = [Document(doc_id=str(i), content=emb, metadata={"source": "BERTEmbeddingParser"}) for i, emb in enumerate(doc_embeddings)]
-        
+from typing import List, Union, Any
+from transformers import BertTokenizer, BertModel
+import torch
+from swarmauri.core.parsers.IParser import IParser
+from swarmauri.core.documents.IDocument import IDocument
+from swarmauri.standard.documents.concrete.Document import Document
+
+class BERTEmbeddingParser(IParser):
+    """
+    A parser that transforms input text into document embeddings using BERT.
+    
+    This parser tokenizes the input text, passes it through a pre-trained BERT model,
+    and uses the resulting embeddings as the document content.
+    """
+
+    def __init__(self, model_name: str = 'bert-base-uncased'):
+        """
+        Initializes the BERTEmbeddingParser with a specific BERT model.
+        
+        Parameters:
+        - model_name (str): The name of the pre-trained BERT model to use.
+        """
+        self.tokenizer = BertTokenizer.from_pretrained(model_name)
+        self.model = BertModel.from_pretrained(model_name)
+        self.model.eval()  # Set model to evaluation mode
+
+    
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Tokenizes input data and generates embeddings using a BERT model.
+
+        Parameters:
+        - data (Union[str, Any]): Input data, expected to be a single string or batch of strings.
+
+        Returns:
+        - List[IDocument]: A list containing a single IDocument instance with BERT embeddings as content.
+        """
+        
+        # Tokenization
+        inputs = self.tokenizer(data, return_tensors='pt', padding=True, truncation=True, max_length=512)
+
+        # Generate embeddings
+        with torch.no_grad():
+            outputs = self.model(**inputs)
+
+        # Use the last hidden state as document embeddings (batch_size, sequence_length, hidden_size)
+        embeddings = outputs.last_hidden_state
+        
+        # Convert to list of numpy arrays
+        embeddings = embeddings.detach().cpu().numpy()
+        
+        # For simplicity, let's consider the mean of embeddings across tokens to represent the document
+        doc_embeddings = embeddings.mean(axis=1)
+        
+        # Creating document object(s)
+        documents = [Document(doc_id=str(i), content=emb, metadata={"source": "BERTEmbeddingParser"}) for i, emb in enumerate(doc_embeddings)]
+        
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/CSVParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/CSVParser.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import csv
-from io import StringIO
-from typing import List, Union, Any
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class CSVParser(IParser):
-    """
-    Concrete implementation of IParser for parsing CSV formatted text into Document instances.
-
-    The parser can handle input as a CSV formatted string or from a file, with each row
-    represented as a separate Document. Assumes the first row is the header which will
-    be used as keys for document metadata.
-    """
-
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses the given CSV data into a list of Document instances.
-
-        Parameters:
-        - data (Union[str, Any]): The input data to parse, either as a CSV string or file path.
-
-        Returns:
-        - List[IDocument]: A list of documents parsed from the CSV data.
-        """
-        # Prepare an in-memory string buffer if the data is provided as a string
-        if isinstance(data, str):
-            data_stream = StringIO(data)
-        else:
-            raise ValueError("Data provided is not a valid CSV string")
-
-        # Create a list to hold the parsed documents
-        documents: List[IDocument] = []
-
-        # Read CSV content row by row
-        reader = csv.DictReader(data_stream)
-        for row in reader:
-            # Each row represents a document, where the column headers are metadata fields
-            document = Document(doc_id=row.get('id', None), 
-                                        content=row.get('content', ''), 
-                                        metadata=row)
-            documents.append(document)
-
+import csv
+from io import StringIO
+from typing import List, Union, Any
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class CSVParser(IParser):
+    """
+    Concrete implementation of IParser for parsing CSV formatted text into Document instances.
+
+    The parser can handle input as a CSV formatted string or from a file, with each row
+    represented as a separate Document. Assumes the first row is the header which will
+    be used as keys for document metadata.
+    """
+
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses the given CSV data into a list of Document instances.
+
+        Parameters:
+        - data (Union[str, Any]): The input data to parse, either as a CSV string or file path.
+
+        Returns:
+        - List[IDocument]: A list of documents parsed from the CSV data.
+        """
+        # Prepare an in-memory string buffer if the data is provided as a string
+        if isinstance(data, str):
+            data_stream = StringIO(data)
+        else:
+            raise ValueError("Data provided is not a valid CSV string")
+
+        # Create a list to hold the parsed documents
+        documents: List[IDocument] = []
+
+        # Read CSV content row by row
+        reader = csv.DictReader(data_stream)
+        for row in reader:
+            # Each row represents a document, where the column headers are metadata fields
+            document = Document(doc_id=row.get('id', None), 
+                                        content=row.get('content', ''), 
+                                        metadata=row)
+            documents.append(document)
+
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import spacy
-from typing import List, Union, Any
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class EntityRecognitionParser(IParser):
-    """
-    EntityRecognitionParser leverages NER capabilities to parse text and 
-    extract entities with their respective tags such as PERSON, LOCATION, ORGANIZATION, etc.
-    """
-
-    def __init__(self):
-        # Load a SpaCy model. The small model is used for demonstration; larger models provide improved accuracy.
-        self.nlp = spacy.load("en_core_web_sm")
-    
-    def parse(self, text: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses the input text, identifies entities, and returns a list of documents with entities tagged.
-
-        Parameters:
-        - text (Union[str, Any]): The input text to be parsed and analyzed for entities.
-
-        Returns:
-        - List[IDocument]: A list of IDocument instances representing the identified entities in the text.
-        """
-        # Ensure the input is a string type before processing
-        if not isinstance(text, str):
-            text = str(text)
-        
-        # Apply the NER model
-        doc = self.nlp(text)
-
-        # Compile identified entities into documents
-        entities_docs = []
-        for ent in doc.ents:
-            # Create a document for each entity with metadata carrying entity type
-            entity_doc = Document(doc_id=ent.text, content=ent.text, metadata={"entity_type": ent.label_})
-            entities_docs.append(entity_doc)
-        
+import spacy
+from typing import List, Union, Any
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class EntityRecognitionParser(IParser):
+    """
+    EntityRecognitionParser leverages NER capabilities to parse text and 
+    extract entities with their respective tags such as PERSON, LOCATION, ORGANIZATION, etc.
+    """
+
+    def __init__(self):
+        # Load a SpaCy model. The small model is used for demonstration; larger models provide improved accuracy.
+        self.nlp = spacy.load("en_core_web_sm")
+    
+    def parse(self, text: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses the input text, identifies entities, and returns a list of documents with entities tagged.
+
+        Parameters:
+        - text (Union[str, Any]): The input text to be parsed and analyzed for entities.
+
+        Returns:
+        - List[IDocument]: A list of IDocument instances representing the identified entities in the text.
+        """
+        # Ensure the input is a string type before processing
+        if not isinstance(text, str):
+            text = str(text)
+        
+        # Apply the NER model
+        doc = self.nlp(text)
+
+        # Compile identified entities into documents
+        entities_docs = []
+        for ent in doc.ents:
+            # Create a document for each entity with metadata carrying entity type
+            entity_doc = Document(doc_id=ent.text, content=ent.text, metadata={"entity_type": ent.label_})
+            entities_docs.append(entity_doc)
+        
         return entities_docs
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import yake
-from typing import List, Union, Any
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class KeywordExtractorParser(IParser):
-    """
-    Extracts keywords from text using the YAKE keyword extraction library.
-    """
-
-    def __init__(self, lang: str = 'en', num_keywords: int = 10):
-        """
-        Initialize the keyword extractor with specified language and number of keywords.
-
-        Parameters:
-        - lang (str): The language of the text for keyword extraction. Default is 'en' for English.
-        - num_keywords (int): The number of top keywords to extract. Default is 10.
-        """
-        self.lang = lang
-        self.num_keywords = num_keywords
-        # Initialize YAKE extractor with specified parameters
-        self.kw_extractor = yake.KeywordExtractor(lan=lang, n=3, dedupLim=0.9, dedupFunc='seqm', windowsSize=1, top=num_keywords, features=None)
-
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Extract keywords from input text and return as list of IDocument instances containing keyword information.
-
-        Parameters:
-        - data (Union[str, Any]): The input text from which to extract keywords.
-
-        Returns:
-        - List[IDocument]: A list of IDocument instances, each containing information about an extracted keyword.
-        """
-        # Ensure data is in string format for analysis
-        text = str(data) if not isinstance(data, str) else data
-
-        # Extract keywords using YAKE
-        keywords = self.kw_extractor.extract_keywords(text)
-
-        # Create Document instances for each keyword
-        documents = [Document(doc_id=str(index), content=keyword, metadata={"score": score}) for index, (keyword, score) in enumerate(keywords)]
-        
+import yake
+from typing import List, Union, Any
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class KeywordExtractorParser(IParser):
+    """
+    Extracts keywords from text using the YAKE keyword extraction library.
+    """
+
+    def __init__(self, lang: str = 'en', num_keywords: int = 10):
+        """
+        Initialize the keyword extractor with specified language and number of keywords.
+
+        Parameters:
+        - lang (str): The language of the text for keyword extraction. Default is 'en' for English.
+        - num_keywords (int): The number of top keywords to extract. Default is 10.
+        """
+        self.lang = lang
+        self.num_keywords = num_keywords
+        # Initialize YAKE extractor with specified parameters
+        self.kw_extractor = yake.KeywordExtractor(lan=lang, n=3, dedupLim=0.9, dedupFunc='seqm', windowsSize=1, top=num_keywords, features=None)
+
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Extract keywords from input text and return as list of IDocument instances containing keyword information.
+
+        Parameters:
+        - data (Union[str, Any]): The input text from which to extract keywords.
+
+        Returns:
+        - List[IDocument]: A list of IDocument instances, each containing information about an extracted keyword.
+        """
+        # Ensure data is in string format for analysis
+        text = str(data) if not isinstance(data, str) else data
+
+        # Extract keywords using YAKE
+        keywords = self.kw_extractor.extract_keywords(text)
+
+        # Create Document instances for each keyword
+        documents = [Document(doc_id=str(index), content=keyword, metadata={"score": score}) for index, (keyword, score) in enumerate(keywords)]
+        
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/MarkdownParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/MarkdownParser.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import re
-from markdown import markdown
-from bs4 import BeautifulSoup
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class MarkdownParser(IParser):
-    """
-    A concrete implementation of the IParser interface that parses Markdown text.
-    
-    This parser takes Markdown formatted text, converts it to HTML using Python's
-    markdown library, and then uses BeautifulSoup to extract plain text content. The
-    resulting plain text is then wrapped into IDocument instances.
-    """
-    
-    def parse(self, data: str) -> list[IDocument]:
-        """
-        Parses the input Markdown data into a list of IDocument instances.
-        
-        Parameters:
-        - data (str): The input Markdown formatted text to be parsed.
-        
-        Returns:
-        - list[IDocument]: A list containing a single IDocument instance with the parsed text content.
-        """
-        # Convert Markdown to HTML
-        html_content = markdown(data)
-        
-        # Use BeautifulSoup to extract text content from HTML
-        soup = BeautifulSoup(html_content, features="html.parser")
-        plain_text = soup.get_text(separator=" ", strip=True)
-        
-        # Generate a document ID
-        doc_id = "1"  # For this implementation, a simple fixed ID is used. 
-                      # A more complex system might generate unique IDs for each piece of text.
-
-        # Create and return a list containing the single extracted plain text document
-        document = Document(doc_id=doc_id, content=plain_text, metadata={"source_format": "markdown"})
+import re
+from markdown import markdown
+from bs4 import BeautifulSoup
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class MarkdownParser(IParser):
+    """
+    A concrete implementation of the IParser interface that parses Markdown text.
+    
+    This parser takes Markdown formatted text, converts it to HTML using Python's
+    markdown library, and then uses BeautifulSoup to extract plain text content. The
+    resulting plain text is then wrapped into IDocument instances.
+    """
+    
+    def parse(self, data: str) -> list[IDocument]:
+        """
+        Parses the input Markdown data into a list of IDocument instances.
+        
+        Parameters:
+        - data (str): The input Markdown formatted text to be parsed.
+        
+        Returns:
+        - list[IDocument]: A list containing a single IDocument instance with the parsed text content.
+        """
+        # Convert Markdown to HTML
+        html_content = markdown(data)
+        
+        # Use BeautifulSoup to extract text content from HTML
+        soup = BeautifulSoup(html_content, features="html.parser")
+        plain_text = soup.get_text(separator=" ", strip=True)
+        
+        # Generate a document ID
+        doc_id = "1"  # For this implementation, a simple fixed ID is used. 
+                      # A more complex system might generate unique IDs for each piece of text.
+
+        # Create and return a list containing the single extracted plain text document
+        document = Document(doc_id=doc_id, content=plain_text, metadata={"source_format": "markdown"})
         return [document]
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import List, Union, Any
-import yaml
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class OpenAPISpecParser(IParser):
-    """
-    A parser that processes OpenAPI Specification files (YAML or JSON format)
-    and extracts information into structured Document instances. 
-    This is useful for building documentation, APIs inventory, or analyzing the API specification.
-    """
-
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses an OpenAPI Specification from a YAML or JSON string into a list of Document instances.
-
-        Parameters:
-        - data (Union[str, Any]): The OpenAPI specification in YAML or JSON format as a string.
-
-        Returns:
-        - List[IDocument]: A list of Document instances representing the parsed information.
-        """
-        try:
-            # Load the OpenAPI spec into a Python dictionary
-            spec_dict = yaml.safe_load(data)
-        except yaml.YAMLError as e:
-            raise ValueError(f"Failed to parse the OpenAPI specification: {e}")
-        
-        documents = []
-        # Iterate over paths in the OpenAPI spec to extract endpoint information
-        for path, path_item in spec_dict.get("paths", {}).items():
-            for method, operation in path_item.items():
-                # Create a Document instance for each operation
-                doc_id = f"{path}_{method}"
-                content = yaml.dump(operation)
-                metadata = {
-                    "path": path,
-                    "method": method.upper(),
-                    "operationId": operation.get("operationId", "")
-                }
-                document = Document(doc_id=doc_id, content=content, metadata=metadata)
-                documents.append(document)
-
+from typing import List, Union, Any
+import yaml
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class OpenAPISpecParser(IParser):
+    """
+    A parser that processes OpenAPI Specification files (YAML or JSON format)
+    and extracts information into structured Document instances. 
+    This is useful for building documentation, APIs inventory, or analyzing the API specification.
+    """
+
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses an OpenAPI Specification from a YAML or JSON string into a list of Document instances.
+
+        Parameters:
+        - data (Union[str, Any]): The OpenAPI specification in YAML or JSON format as a string.
+
+        Returns:
+        - List[IDocument]: A list of Document instances representing the parsed information.
+        """
+        try:
+            # Load the OpenAPI spec into a Python dictionary
+            spec_dict = yaml.safe_load(data)
+        except yaml.YAMLError as e:
+            raise ValueError(f"Failed to parse the OpenAPI specification: {e}")
+        
+        documents = []
+        # Iterate over paths in the OpenAPI spec to extract endpoint information
+        for path, path_item in spec_dict.get("paths", {}).items():
+            for method, operation in path_item.items():
+                # Create a Document instance for each operation
+                doc_id = f"{path}_{method}"
+                content = yaml.dump(operation)
+                metadata = {
+                    "path": path,
+                    "method": method.upper(),
+                    "operationId": operation.get("operationId", "")
+                }
+                document = Document(doc_id=doc_id, content=content, metadata=metadata)
+                documents.append(document)
+
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import re
-from typing import List, Union, Any
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class PhoneNumberExtractorParser(IParser):
-    """
-    A parser that extracts phone numbers from the input text.
-    Utilizes regular expressions to identify phone numbers in various formats.
-    """
-
-    def __init__(self):
-        """
-        Initializes the PhoneNumberExtractorParser.
-        """
-        super().__init__()
-
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses the input data, looking for phone numbers employing a regular expression.
-        Each phone number found is contained in a separate IDocument instance.
-
-        Parameters:
-        - data (Union[str, Any]): The input text to be parsed for phone numbers.
-
-        Returns:
-        - List[IDocument]: A list of IDocument instances, each containing a phone number.
-        """
-        # Define a regular expression for phone numbers.
-        # This is a simple example and might not capture all phone number formats accurately.
-        phone_regex = r'\+?\d[\d -]{8,}\d'
-
-        # Find all occurrences of phone numbers in the text
-        phone_numbers = re.findall(phone_regex, str(data))
-
-        # Create a new IDocument for each phone number found
-        documents = [Document(doc_id=str(index), content=phone_number, metadata={}) for index, phone_number in enumerate(phone_numbers)]
-
+import re
+from typing import List, Union, Any
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class PhoneNumberExtractorParser(IParser):
+    """
+    A parser that extracts phone numbers from the input text.
+    Utilizes regular expressions to identify phone numbers in various formats.
+    """
+
+    def __init__(self):
+        """
+        Initializes the PhoneNumberExtractorParser.
+        """
+        super().__init__()
+
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses the input data, looking for phone numbers employing a regular expression.
+        Each phone number found is contained in a separate IDocument instance.
+
+        Parameters:
+        - data (Union[str, Any]): The input text to be parsed for phone numbers.
+
+        Returns:
+        - List[IDocument]: A list of IDocument instances, each containing a phone number.
+        """
+        # Define a regular expression for phone numbers.
+        # This is a simple example and might not capture all phone number formats accurately.
+        phone_regex = r'\+?\d[\d -]{8,}\d'
+
+        # Find all occurrences of phone numbers in the text
+        phone_numbers = re.findall(phone_regex, str(data))
+
+        # Create a new IDocument for each phone number found
+        documents = [Document(doc_id=str(index), content=phone_number, metadata={}) for index, phone_number in enumerate(phone_numbers)]
+
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/PythonParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PythonParser.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from typing import List, Union, Any
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-import ast
-import uuid
-
-class PythonParser(IParser):
-    """
-    A parser that processes Python source code to extract structural elements
-    such as functions, classes, and their docstrings.
-    
-    This parser utilizes the `ast` module to parse the Python code into an abstract syntax tree (AST)
-    and then walks the tree to extract relevant information.
-    """
-    
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses the given Python source code to extract structural elements.
-
-        Args:
-            data (Union[str, Any]): The input Python source code as a string.
-
-        Returns:
-            List[IDocument]: A list of IDocument objects, each representing a structural element 
-                             extracted from the code along with its metadata.
-        """
-        if not isinstance(data, str):
-            raise ValueError("PythonParser expects a string input.")
-        
-        documents = []
-        tree = ast.parse(data)
-        
-        for node in ast.walk(tree):
-            if isinstance(node, ast.FunctionDef) or isinstance(node, ast.ClassDef):
-                element_name = node.name
-                docstring = ast.get_docstring(node)
-                
-                # Generate a unique ID for each element
-                doc_id = str(uuid.uuid4())
-                
-                # Create a metadata dictionary
-                metadata = {
-                    "type": "function" if isinstance(node, ast.FunctionDef) else "class",
-                    "name": element_name,
-                    "docstring": docstring
-                }
-                
-                # Create a Document for each structural element
-                document = Document(doc_id=doc_id, content=docstring, metadata=metadata)
-                documents.append(document)
-                
+from typing import List, Union, Any
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+import ast
+import uuid
+
+class PythonParser(IParser):
+    """
+    A parser that processes Python source code to extract structural elements
+    such as functions, classes, and their docstrings.
+    
+    This parser utilizes the `ast` module to parse the Python code into an abstract syntax tree (AST)
+    and then walks the tree to extract relevant information.
+    """
+    
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses the given Python source code to extract structural elements.
+
+        Args:
+            data (Union[str, Any]): The input Python source code as a string.
+
+        Returns:
+            List[IDocument]: A list of IDocument objects, each representing a structural element 
+                             extracted from the code along with its metadata.
+        """
+        if not isinstance(data, str):
+            raise ValueError("PythonParser expects a string input.")
+        
+        documents = []
+        tree = ast.parse(data)
+        
+        for node in ast.walk(tree):
+            if isinstance(node, ast.FunctionDef) or isinstance(node, ast.ClassDef):
+                element_name = node.name
+                docstring = ast.get_docstring(node)
+                
+                # Generate a unique ID for each element
+                doc_id = str(uuid.uuid4())
+                
+                # Create a metadata dictionary
+                metadata = {
+                    "type": "function" if isinstance(node, ast.FunctionDef) else "class",
+                    "name": element_name,
+                    "docstring": docstring
+                }
+                
+                # Create a Document for each structural element
+                document = Document(doc_id=doc_id, content=docstring, metadata=metadata)
+                documents.append(document)
+                
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/TFIDFParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TfidfParser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from sklearn.feature_extraction.text import TfidfVectorizer
-from swarmauri.core.parsers.IParser import IParser
-from swarmauri.core.documents.IDocument import IDocument
-from swarmauri.standard.documents.concrete.Document import Document
-
-class TFIDFParser(IParser):
-    def __init__(self):
-        self.vectorizer = TfidfVectorizer()
-        super().__init__()
-
-    def parse(self, data):
-        # Assuming `data` is a list of strings (documents)
-        tfidf_matrix = self.vectorizer.fit_transform(data)
-        # Depending on how you want to use the output, you could return Document objects
-        # For demonstration, let's return a list of IDocument with vectorized content
-        documents = [Document(doc_id=str(i), content=vector, metadata={}) for i, vector in enumerate(tfidf_matrix.toarray())]
+from sklearn.feature_extraction.text import TfidfVectorizer
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class TfidfParser(IParser):
+    def __init__(self):
+        self.vectorizer = TfidfVectorizer()
+        super().__init__()
+
+    def parse(self, data):
+        # Assuming `data` is a list of strings (documents)
+        tfidf_matrix = self.vectorizer.fit_transform(data)
+        # Depending on how you want to use the output, you could return Document objects
+        # For demonstration, let's return a list of IDocument with vectorized content
+        documents = [Document(doc_id=str(i), content=vector, metadata={}) for i, vector in enumerate(tfidf_matrix.toarray())]
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/TextBlobNounParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobNounParser.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import List, Union, Any
-from textblob import TextBlob
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class TextBlobNounParser(IParser):
-    """
-    A concrete implementation of IParser using TextBlob for Natural Language Processing tasks.
-    
-    This parser leverages TextBlob's functionalities such as noun phrase extraction, 
-    sentiment analysis, classification, language translation, and more for parsing texts.
-    """
-    
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses the input data using TextBlob to perform basic NLP tasks 
-        and returns a list of documents with the parsed information.
-        
-        Parameters:
-        - data (Union[str, Any]): The input data to parse, expected to be text data for this parser.
-        
-        Returns:
-        - List[IDocument]: A list of documents with metadata generated from the parsing process.
-        """
-        # Ensure the data is a string
-        if not isinstance(data, str):
-            raise ValueError("TextBlobParser expects a string as input data.")
-        
-        # Use TextBlob for NLP tasks
-        blob = TextBlob(data)
-        
-        # Extracts noun phrases to demonstrate one of TextBlob's capabilities. 
-        # In practice, this parser could be expanded to include more sophisticated processing.
-        noun_phrases = list(blob.noun_phrases)
-        
-        # Example: Wrap the extracted noun phrases into an IDocument instance
-        # In real scenarios, you might want to include more details, like sentiment, POS tags, etc.
-        document = Document(doc_id="0", content=data, metadata={"noun_phrases": noun_phrases})
-        
+from typing import List, Union, Any
+from textblob import TextBlob
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class TextBlobNounParser(IParser):
+    """
+    A concrete implementation of IParser using TextBlob for Natural Language Processing tasks.
+    
+    This parser leverages TextBlob's functionalities such as noun phrase extraction, 
+    sentiment analysis, classification, language translation, and more for parsing texts.
+    """
+    
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses the input data using TextBlob to perform basic NLP tasks 
+        and returns a list of documents with the parsed information.
+        
+        Parameters:
+        - data (Union[str, Any]): The input data to parse, expected to be text data for this parser.
+        
+        Returns:
+        - List[IDocument]: A list of documents with metadata generated from the parsing process.
+        """
+        # Ensure the data is a string
+        if not isinstance(data, str):
+            raise ValueError("TextBlobParser expects a string as input data.")
+        
+        # Use TextBlob for NLP tasks
+        blob = TextBlob(data)
+        
+        # Extracts noun phrases to demonstrate one of TextBlob's capabilities. 
+        # In practice, this parser could be expanded to include more sophisticated processing.
+        noun_phrases = list(blob.noun_phrases)
+        
+        # Example: Wrap the extracted noun phrases into an IDocument instance
+        # In real scenarios, you might want to include more details, like sentiment, POS tags, etc.
+        document = Document(doc_id="0", content=data, metadata={"noun_phrases": noun_phrases})
+        
         return [document]
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from textblob import TextBlob
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-from typing import List, Union, Any
-
-class TextBlobParser(IParser):
-    """
-    A parser that leverages TextBlob to break text into sentences.
-
-    This parser uses the natural language processing capabilities of TextBlob
-    to accurately identify sentence boundaries within large blocks of text.
-    """
-
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses the input text into sentence-based document chunks using TextBlob.
-
-        Args:
-            data (Union[str, Any]): The input text to be parsed.
-
-        Returns:
-            List[IDocument]: A list of IDocument instances, each representing a sentence.
-        """
-        # Ensure the input is a string
-        if not isinstance(data, str):
-            data = str(data)
-
-        # Utilize TextBlob for sentence tokenization
-        blob = TextBlob(data)
-        sentences = blob.sentences
-
-        # Create a document instance for each sentence
-        documents = [
-            Document(doc_id=str(index), content=str(sentence), metadata={'parser': 'TextBlobParser'})
-            for index, sentence in enumerate(sentences)
-        ]
-
+from textblob import TextBlob
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+from typing import List, Union, Any
+
+class TextBlobParser(IParser):
+    """
+    A parser that leverages TextBlob to break text into sentences.
+
+    This parser uses the natural language processing capabilities of TextBlob
+    to accurately identify sentence boundaries within large blocks of text.
+    """
+
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses the input text into sentence-based document chunks using TextBlob.
+
+        Args:
+            data (Union[str, Any]): The input text to be parsed.
+
+        Returns:
+            List[IDocument]: A list of IDocument instances, each representing a sentence.
+        """
+        # Ensure the input is a string
+        if not isinstance(data, str):
+            data = str(data)
+
+        # Utilize TextBlob for sentence tokenization
+        blob = TextBlob(data)
+        sentences = blob.sentences
+
+        # Create a document instance for each sentence
+        documents = [
+            Document(doc_id=str(index), content=str(sentence), metadata={'parser': 'TextBlobParser'})
+            for index, sentence in enumerate(sentences)
+        ]
+
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/URLExtractorParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/URLExtractorParser.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import List, Union, Any
-from urllib.parse import urlparse
-import re
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class URLExtractorParser(IParser):
-    """
-    A concrete implementation of IParser that extracts URLs from text.
-    
-    This parser scans the input text for any URLs and creates separate
-    documents for each extracted URL. It utilizes regular expressions
-    to identify URLs within the given text.
-    """
-
-    def __init__(self):
-        """
-        Initializes the URLExtractorParser.
-        """
-        super().__init__()
-    
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parse input data (string) and extract URLs, each URL is then represented as a document.
-        
-        Parameters:
-        - data (Union[str, Any]): The input data to be parsed for URLs.
-        
-        Returns:
-        - List[IDocument]: A list of documents, each representing an extracted URL.
-        """
-        if not isinstance(data, str):
-            raise ValueError("URLExtractorParser expects input data to be of type str.")
-
-        # Regular expression for finding URLs
-        url_regex = r"https?://(?:[-\w.]|(?:%[\da-fA-F]{2}))+"
-        
-        # Find all matches in the text
-        urls = re.findall(url_regex, data)
-        
-        # Create a document for each extracted URL
-        documents = [Document(doc_id=str(i), content=url, metadata={"source": "URLExtractor"}) for i, url in enumerate(urls)]
-        
+from typing import List, Union, Any
+from urllib.parse import urlparse
+import re
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class URLExtractorParser(IParser):
+    """
+    A concrete implementation of IParser that extracts URLs from text.
+    
+    This parser scans the input text for any URLs and creates separate
+    documents for each extracted URL. It utilizes regular expressions
+    to identify URLs within the given text.
+    """
+
+    def __init__(self):
+        """
+        Initializes the URLExtractorParser.
+        """
+        super().__init__()
+    
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parse input data (string) and extract URLs, each URL is then represented as a document.
+        
+        Parameters:
+        - data (Union[str, Any]): The input data to be parsed for URLs.
+        
+        Returns:
+        - List[IDocument]: A list of documents, each representing an extracted URL.
+        """
+        if not isinstance(data, str):
+            raise ValueError("URLExtractorParser expects input data to be of type str.")
+
+        # Regular expression for finding URLs
+        url_regex = r"https?://(?:[-\w.]|(?:%[\da-fA-F]{2}))+"
+        
+        # Find all matches in the text
+        urls = re.findall(url_regex, data)
+        
+        # Create a document for each extracted URL
+        documents = [Document(doc_id=str(i), content=url, metadata={"source": "URLExtractor"}) for i, url in enumerate(urls)]
+        
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/parsers/concrete/XMLParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/XMLParser.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import xml.etree.ElementTree as ET
-from typing import List, Union, Any
-from ....core.parsers.IParser import IParser
-from ....core.documents.IDocument import IDocument
-from ....standard.documents.concrete.Document import Document
-
-class XMLParser(IParser):
-    """
-    A parser that extracts information from XML data and converts it into IDocument objects.
-    This parser assumes a simple use-case where each targeted XML element represents a separate document.
-    """
-
-    def __init__(self, element_tag: str):
-        """
-        Initialize the XMLParser with the tag name of the XML elements to be extracted as documents.
-
-        Parameters:
-        - element_tag (str): The tag name of XML elements to parse into documents.
-        """
-        self.element_tag = element_tag
-
-    def parse(self, data: Union[str, Any]) -> List[IDocument]:
-        """
-        Parses XML data and converts elements with the specified tag into IDocument instances.
-
-        Parameters:
-        - data (Union[str, Any]): The XML data as a string to be parsed.
-
-        Returns:
-        - List[IDocument]: A list of IDocument instances created from the XML elements.
-        """
-        if isinstance(data, str):
-            root = ET.fromstring(data)  # Parse the XML string into an ElementTree element
-        else:
-            raise TypeError("Data for XMLParser must be a string containing valid XML.")
-
-        documents = []
-        for element in root.findall(self.element_tag):
-            # Extracting content and metadata from each element
-            content = "".join(element.itertext())  # Get text content
-            metadata = {child.tag: child.text for child in element}  # Extract child elements as metadata
-
-            # Create a Document instance for each element
-            doc = Document(doc_id=None, content=content, metadata=metadata)
-            documents.append(doc)
-
+import xml.etree.ElementTree as ET
+from typing import List, Union, Any
+from ....core.parsers.IParser import IParser
+from ....core.documents.IDocument import IDocument
+from ....standard.documents.concrete.Document import Document
+
+class XMLParser(IParser):
+    """
+    A parser that extracts information from XML data and converts it into IDocument objects.
+    This parser assumes a simple use-case where each targeted XML element represents a separate document.
+    """
+
+    def __init__(self, element_tag: str):
+        """
+        Initialize the XMLParser with the tag name of the XML elements to be extracted as documents.
+
+        Parameters:
+        - element_tag (str): The tag name of XML elements to parse into documents.
+        """
+        self.element_tag = element_tag
+
+    def parse(self, data: Union[str, Any]) -> List[IDocument]:
+        """
+        Parses XML data and converts elements with the specified tag into IDocument instances.
+
+        Parameters:
+        - data (Union[str, Any]): The XML data as a string to be parsed.
+
+        Returns:
+        - List[IDocument]: A list of IDocument instances created from the XML elements.
+        """
+        if isinstance(data, str):
+            root = ET.fromstring(data)  # Parse the XML string into an ElementTree element
+        else:
+            raise TypeError("Data for XMLParser must be a string containing valid XML.")
+
+        documents = []
+        for element in root.findall(self.element_tag):
+            # Extracting content and metadata from each element
+            content = "".join(element.itertext())  # Get text content
+            metadata = {child.tag: child.text for child in element}  # Extract child elements as metadata
+
+            # Create a Document instance for each element
+            doc = Document(doc_id=None, content=content, metadata=metadata)
+            documents.append(doc)
+
         return documents
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/prompts/concrete/Prompt.py` & `swarmauri-0.1.9/swarmauri/standard/prompts/concrete/Prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from swarmauri.core.prompts.IPrompt import IPrompt
-
-class Prompt(IPrompt):
-    """
-    The ChatPrompt class represents a simple, chat-like prompt system where a 
-    message can be set and retrieved as needed. It's particularly useful in 
-    applications involving conversational agents, chatbots, or any system that 
-    requires dynamic text-based interactions.
-    """
-
-    def __init__(self, prompt: str = ""):
-        """
-        Initializes an instance of ChatPrompt with an optional initial message.
-        
-        Parameters:
-        - message (str, optional): The initial message for the prompt. Defaults to an empty string.
-        """
-        self.prompt = prompt
-
-    def __call__(self, prompt):
-        """
-        Enables the instance to be callable, allowing direct retrieval of the message. 
-        This method facilitates intuitive access to the prompt's message, mimicking callable 
-        behavior seen in functional programming paradigms.
-        
-        Returns:
-        - str: The current message stored in the prompt.
-        """
-        return self.prompt
-
-    def set_prompt(self, prompt: str):
-        """
-        Updates the internal message of the chat prompt. This method provides a way to change 
-        the content of the prompt dynamically, reflecting changes in the conversational context 
-        or user inputs.
-        
-        Parameters:
-        - message (str): The new message to set for the prompt.
-        """
-        self.prompt = prompt
+from ....core.prompts.IPrompt import IPrompt
+
+class Prompt(IPrompt):
+    """
+    The ChatPrompt class represents a simple, chat-like prompt system where a 
+    message can be set and retrieved as needed. It's particularly useful in 
+    applications involving conversational agents, chatbots, or any system that 
+    requires dynamic text-based interactions.
+    """
+
+    def __init__(self, prompt: str = ""):
+        """
+        Initializes an instance of ChatPrompt with an optional initial message.
+        
+        Parameters:
+        - message (str, optional): The initial message for the prompt. Defaults to an empty string.
+        """
+        self.prompt = prompt
+
+    def __call__(self, prompt):
+        """
+        Enables the instance to be callable, allowing direct retrieval of the message. 
+        This method facilitates intuitive access to the prompt's message, mimicking callable 
+        behavior seen in functional programming paradigms.
+        
+        Returns:
+        - str: The current message stored in the prompt.
+        """
+        return self.prompt
+
+    def set_prompt(self, prompt: str):
+        """
+        Updates the internal message of the chat prompt. This method provides a way to change 
+        the content of the prompt dynamically, reflecting changes in the conversational context 
+        or user inputs.
+        
+        Parameters:
+        - message (str): The new message to set for the prompt.
+        """
+        self.prompt = prompt
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/prompts/concrete/PromptTemplate.py` & `swarmauri-0.1.9/swarmauri/standard/prompts/concrete/PromptTemplate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,58 @@
-from typing import Dict, List
-from swarmauri.core.prompts.IPrompt import IPrompt
-from swarmauri.core.prompts.ITemplate import ITemplate
-
-class PromptTemplate(IPrompt, ITemplate):
-    """
-    A class for generating prompts based on a template and variables.
-    Implements the IPrompt for generating prompts and ITemplate for template manipulation.
-    """
-
-    def __init__(self, template: str = "", variables: List[Dict[str, str]] = []):
-        self._template = template
-        self._variables_list = variables
-
-    @property
-    def template(self) -> str:
-        """
-        Get the current prompt template.
-        """
-        return self._template
-
-    @template.setter
-    def template(self, value: str) -> None:
-        """
-        Set a new template string for the prompt.
-        """
-        self._template = value
-
-    @property
-    def variables(self) -> List[Dict[str, str]]:
-        """
-        Get the current set of variables for the template.
-        """
-        return self._variables_list 
-
-    @variables.setter
-    def variables(self, value: List[Dict[str, str]]) -> None:
-        if not isinstance(value, list):
-            raise ValueError("Variables must be a list of dictionaries.")
-        self._variables_list = value
-
-    def set_template(self, template: str) -> None:
-        """
-        Sets or updates the current template string.
-        """
-        self._template = template
-
-    def set_variables(self, variables: Dict[str, str]) -> None:
-        """
-        Sets or updates the variables to be substituted into the template.
-        """
-        self._variables_list = variables
-
-    def generate_prompt(self, variables: List[Dict[str, str]] = None) -> str:
-        variables = variables.pop(0) or (self._variables_list.pop(0) if self._variables_list else {})
-        return self._template.format(**variables)
-
-    def __call__(self, variables: List[Dict[str, str]]) -> str:
-        """
-        Generates a prompt using the current template and provided keyword arguments for substitution.
-        """
-        return self.generate_prompt(variables)
+from typing import Dict
+from ....core.prompts.IPrompt import IPrompt
+
+class PromptTemplate(IPrompt):
+    """
+    A class that represents a template for generating prompts, 
+    allowing dynamic content insertion into pre-defined template slots.
+
+    Attributes:
+        template (str): A string template with placeholders for content insertion.
+        variables (Dict[str, str]): A dictionary mapping placeholder names in the template to their content.
+    """
+
+    def __init__(self, template: str = "", variables: Dict[str, str] = {}):
+        """
+        Initializes a new instance of the PromptTemplate class.
+
+        Args:
+            template (str): The string template for the prompt.
+            variables (Dict[str, str]): A dictionary mapping variables in the template to their values.
+        """
+        self.template = template
+        self.variables = variables
+
+    def __call__(self, variables: Dict[str, str] = {}):
+        """
+        Generates the prompt string by substituting variables into the template.
+
+        Returns:
+            str: The generated prompt with variables substituted.
+        """
+        variables = variables or self.variables
+        formatted_prompt = self.template.format(**variables)
+        return formatted_prompt
+
+    def set_template(self, template: str):
+        """
+        Sets a new template string for the prompt.
+
+        Args:
+            template (str): The new string template to use.
+        """
+        self.template = template
+
+    def set_variables(self, variables: Dict[str, str]):
+        """
+        Sets the variables to be substituted into the template.
+
+        Args:
+            variables (Dict[str, str]): A dictionary of variables to be substituted into the template.
+        
+        Raises:
+            TypeError: If the provided variables argument is not a dictionary.
+        """
+        if isinstance(variables, dict):
+            self.variables = variables
+        else:
+            raise TypeError("Invalid type. Expected dict for variables.")
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/swarms/base/SwarmComponentBase.py` & `swarmauri-0.1.9/swarmauri/standard/swarms/base/SwarmComponentBase.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from swarmauri.core.swarms.ISwarmComponent import ISwarmComponent
-
-class SwarmComponentBase(ISwarmComponent):
-    """
-    Interface for defining basics of any component within the swarm system.
-    """
-    def __init__(self, key: str, name: str, superclass: str, module: str, class_name: str, args=None, kwargs=None):
-        self.key = key
-        self.name = name
-        self.superclass = superclass
-        self.module = module
-        self.class_name = class_name
-        self.args = args or []
-        self.kwargs = kwargs or {}
+from swarmauri.core.swarms.ISwarmComponent import ISwarmComponent
+
+class SwarmComponentBase(ISwarmComponent):
+    """
+    Interface for defining basics of any component within the swarm system.
+    """
+    def __init__(self, key: str, name: str, superclass: str, module: str, class_name: str, args=None, kwargs=None):
+        self.key = key
+        self.name = name
+        self.superclass = superclass
+        self.module = module
+        self.class_name = class_name
+        self.args = args or []
+        self.kwargs = kwargs or {}
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/toolkits/base/ToolkitBase.py` & `swarmauri-0.1.9/swarmauri/standard/toolkits/base/ToolkitBase.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from abc import ABC, abstractmethod
-from typing import Dict
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.tools.ITool import ITool  
-
-class ToolkitBase(IToolkit, ABC):
-    """
-    A class representing a toolkit used by Swarm Agents.
-    Tools are maintained in a dictionary keyed by the tool's name.
-    """
-
-    @abstractmethod
-    def __init__(self, initial_tools: Dict[str, ITool] = None):
-        """
-        Initialize the Toolkit with an optional dictionary of initial tools.
-        """
-        # If initial_tools is provided, use it; otherwise, use an empty dictionary
-        self._tools = initial_tools if initial_tools is not None else {}
-
-    @property
-    def tools(self) -> Dict[str, ITool]:
-        return [self._tools[tool].as_dict() for tool in self._tools]
-
-    def add_tools(self, tools: Dict[str, ITool]):
-        """
-        Add multiple tools to the toolkit.
-
-        Parameters:
-            tools (Dict[str, Tool]): A dictionary of tool objects keyed by their names.
-        """
-        self._tools.update(tools)
-
-    def add_tool(self, tool: ITool):
-        """
-        Add a single tool to the toolkit.
-
-        Parameters:
-            tool (Tool): The tool instance to be added to the toolkit.
-        """
-        self._tools[tool.function['name']] = tool
-
-    def remove_tool(self, tool_name: str):
-        """
-        Remove a tool from the toolkit by name.
-
-        Parameters:
-            tool_name (str): The name of the tool to be removed from the toolkit.
-        """
-        if tool_name in self._tools:
-            del self._tools[tool_name]
-        else:
-            raise ValueError(f"Tool '{tool_name}' not found in the toolkit.")
-
-    def get_tool_by_name(self, tool_name: str) -> ITool:
-        """
-        Get a tool from the toolkit by name.
-
-        Parameters:
-            tool_name (str): The name of the tool to retrieve.
-
-        Returns:
-            Tool: The tool instance with the specified name.
-        """
-        if tool_name in self._tools:
-            return self._tools[tool_name]
-        else:
-            raise ValueError(f"Tool '{tool_name}' not found in the toolkit.")
-
-    def __len__(self) -> int:
-        """
-        Returns the number of tools in the toolkit.
-
-        Returns:
-            int: The number of tools in the toolkit.
-        """
+from abc import ABC, abstractmethod
+from typing import Dict
+from ....core.toolkits.IToolkit import IToolkit
+from ....core.tools.ITool import ITool  
+
+class ToolkitBase(IToolkit, ABC):
+    """
+    A class representing a toolkit used by Swarm Agents.
+    Tools are maintained in a dictionary keyed by the tool's name.
+    """
+
+    @abstractmethod
+    def __init__(self, initial_tools: Dict[str, ITool] = None):
+        """
+        Initialize the Toolkit with an optional dictionary of initial tools.
+        """
+        # If initial_tools is provided, use it; otherwise, use an empty dictionary
+        self._tools = initial_tools if initial_tools is not None else {}
+
+    @property
+    def tools(self) -> Dict[str, ITool]:
+        return [self._tools[tool].as_dict() for tool in self._tools]
+
+    def add_tools(self, tools: Dict[str, ITool]):
+        """
+        Add multiple tools to the toolkit.
+
+        Parameters:
+            tools (Dict[str, Tool]): A dictionary of tool objects keyed by their names.
+        """
+        self._tools.update(tools)
+
+    def add_tool(self, tool: ITool):
+        """
+        Add a single tool to the toolkit.
+
+        Parameters:
+            tool (Tool): The tool instance to be added to the toolkit.
+        """
+        self._tools[tool.function['name']] = tool
+
+    def remove_tool(self, tool_name: str):
+        """
+        Remove a tool from the toolkit by name.
+
+        Parameters:
+            tool_name (str): The name of the tool to be removed from the toolkit.
+        """
+        if tool_name in self._tools:
+            del self._tools[tool_name]
+        else:
+            raise ValueError(f"Tool '{tool_name}' not found in the toolkit.")
+
+    def get_tool_by_name(self, tool_name: str) -> ITool:
+        """
+        Get a tool from the toolkit by name.
+
+        Parameters:
+            tool_name (str): The name of the tool to retrieve.
+
+        Returns:
+            Tool: The tool instance with the specified name.
+        """
+        if tool_name in self._tools:
+            return self._tools[tool_name]
+        else:
+            raise ValueError(f"Tool '{tool_name}' not found in the toolkit.")
+
+    def __len__(self) -> int:
+        """
+        Returns the number of tools in the toolkit.
+
+        Returns:
+            int: The number of tools in the toolkit.
+        """
         return len(self._tools)
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/tools/concrete/Parameter.py` & `swarmauri-0.1.9/swarmauri/standard/tools/concrete/Parameter.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from typing import Optional, List, Any
-import json
-from ....core.tools.IParameter import IParameter
-
-class Parameter(IParameter):
-    """
-    A class to represent a parameter for a tool.
-
-    Attributes:
-        name (str): Name of the parameter.
-        type (str): Data type of the parameter (e.g., 'int', 'str', 'float').
-        description (str): A brief description of the parameter.
-        required (bool): Whether the parameter is required or optional.
-        enum (Optional[List[any]]): A list of acceptable values for the parameter, if any.
-    """
-
-    def __init__(self, name: str, type: str, description: str, required: bool = True, enum: Optional[List[Any]] = None):
-        """
-        Initializes a new instance of the Parameter class.
-
-        Args:
-            name (str): The name of the parameter.
-            type (str): The type of the parameter.
-            description (str): A brief description of what the parameter is used for.
-            required (bool, optional): Specifies if the parameter is required. Defaults to True.
-            enum (Optional[List[Any]], optional): A list of acceptable values for the parameter. Defaults to None.
-        """
-        self._name = name
-        self._type = type
-        self._description = description
-        self._required = required
-        self._enum = enum
-        
-    @property
-    def name(self) -> str:
-        """
-        Abstract property for getting the name of the parameter.
-        """
-        return self._name
-
-    @name.setter
-    def name(self, value: str):
-        """
-        Abstract setter for setting the name of the parameter.
-        """
-        self._name = value
-
-    @property
-    def type(self) -> str:
-        """
-        Abstract property for getting the type of the parameter.
-        """
-        return self._type
-
-    @type.setter
-    def type(self, value: str):
-        """
-        Abstract setter for setting the type of the parameter.
-        """
-        self._type = value
-
-    @property
-    def description(self) -> str:
-        """
-        Abstract property for getting the description of the parameter.
-        """
-        return self._description
-
-    @description.setter
-    def description(self, value: str):
-        """
-        Abstract setter for setting the description of the parameter.
-        """
-        self._description = value
-
-    @property
-    def required(self) -> bool:
-        """
-        Abstract property for getting the required status of the parameter.
-        """
-        return self._required
-
-    @required.setter
-    def required(self, value: bool):
-        """
-        Abstract setter for setting the required status of the parameter.
-        """
-        self._required = value
-
-    @property
-    def enum(self) -> Optional[List[Any]]:
-        """
-        Abstract property for getting the enum list of the parameter.
-        """
-        return self._enum
-
-    @enum.setter
-    def enum(self, value: Optional[List[Any]]):
-        """
-        Abstract setter for setting the enum list of the parameter.
-        """
+from typing import Optional, List, Any
+import json
+from ....core.tools.IParameter import IParameter
+
+class Parameter(IParameter):
+    """
+    A class to represent a parameter for a tool.
+
+    Attributes:
+        name (str): Name of the parameter.
+        type (str): Data type of the parameter (e.g., 'int', 'str', 'float').
+        description (str): A brief description of the parameter.
+        required (bool): Whether the parameter is required or optional.
+        enum (Optional[List[any]]): A list of acceptable values for the parameter, if any.
+    """
+
+    def __init__(self, name: str, type: str, description: str, required: bool = True, enum: Optional[List[Any]] = None):
+        """
+        Initializes a new instance of the Parameter class.
+
+        Args:
+            name (str): The name of the parameter.
+            type (str): The type of the parameter.
+            description (str): A brief description of what the parameter is used for.
+            required (bool, optional): Specifies if the parameter is required. Defaults to True.
+            enum (Optional[List[Any]], optional): A list of acceptable values for the parameter. Defaults to None.
+        """
+        self._name = name
+        self._type = type
+        self._description = description
+        self._required = required
+        self._enum = enum
+        
+    @property
+    def name(self) -> str:
+        """
+        Abstract property for getting the name of the parameter.
+        """
+        return self._name
+
+    @name.setter
+    def name(self, value: str):
+        """
+        Abstract setter for setting the name of the parameter.
+        """
+        self._name = value
+
+    @property
+    def type(self) -> str:
+        """
+        Abstract property for getting the type of the parameter.
+        """
+        return self._type
+
+    @type.setter
+    def type(self, value: str):
+        """
+        Abstract setter for setting the type of the parameter.
+        """
+        self._type = value
+
+    @property
+    def description(self) -> str:
+        """
+        Abstract property for getting the description of the parameter.
+        """
+        return self._description
+
+    @description.setter
+    def description(self, value: str):
+        """
+        Abstract setter for setting the description of the parameter.
+        """
+        self._description = value
+
+    @property
+    def required(self) -> bool:
+        """
+        Abstract property for getting the required status of the parameter.
+        """
+        return self._required
+
+    @required.setter
+    def required(self, value: bool):
+        """
+        Abstract setter for setting the required status of the parameter.
+        """
+        self._required = value
+
+    @property
+    def enum(self) -> Optional[List[Any]]:
+        """
+        Abstract property for getting the enum list of the parameter.
+        """
+        return self._enum
+
+    @enum.setter
+    def enum(self, value: Optional[List[Any]]):
+        """
+        Abstract setter for setting the enum list of the parameter.
+        """
         self._enum = value
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/tracing/concrete/CallableTracer.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/CallableTracer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import functools
-from swarmauri.standard.tracing.concrete.SimpleTracer import SimpleTracer  # Import SimpleTracer from the previously defined path
-
-# Initialize the global tracer object
-tracer = SimpleTracer()
-
-def CallableTracer(func):
-    """
-    A decorator to trace function or method calls, capturing inputs, outputs, and the caller.
-    """
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        # Trying to automatically identify the caller details; practical implementations 
-        # might need to adjust based on specific requirements or environment.
-        caller_info = f"{func.__module__}.{func.__name__}"
-        
-        # Start a new trace context for this callable
-        trace_context = tracer.start_trace(name=caller_info, initial_attributes={'args': args, 'kwargs': kwargs})
-        
-        try:
-            # Call the actual function/method
-            result = func(*args, **kwargs)
-            tracer.annotate_trace(key="result", value=result)
-            return result
-        except Exception as e:
-            # Optionally annotate the trace with the exception details
-            tracer.annotate_trace(key="exception", value=str(e))
-            raise  # Re-raise the exception to not interfere with the program's flow
-        finally:
-            # End the trace after the function call is complete
-            tracer.end_trace()
+import functools
+from swarmauri.standard.tracing.concrete.SimpleTracer import SimpleTracer  # Import SimpleTracer from the previously defined path
+
+# Initialize the global tracer object
+tracer = SimpleTracer()
+
+def CallableTracer(func):
+    """
+    A decorator to trace function or method calls, capturing inputs, outputs, and the caller.
+    """
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        # Trying to automatically identify the caller details; practical implementations 
+        # might need to adjust based on specific requirements or environment.
+        caller_info = f"{func.__module__}.{func.__name__}"
+        
+        # Start a new trace context for this callable
+        trace_context = tracer.start_trace(name=caller_info, initial_attributes={'args': args, 'kwargs': kwargs})
+        
+        try:
+            # Call the actual function/method
+            result = func(*args, **kwargs)
+            tracer.annotate_trace(key="result", value=result)
+            return result
+        except Exception as e:
+            # Optionally annotate the trace with the exception details
+            tracer.annotate_trace(key="exception", value=str(e))
+            raise  # Re-raise the exception to not interfere with the program's flow
+        finally:
+            # End the trace after the function call is complete
+            tracer.end_trace()
     return wrapper
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/tracing/concrete/ChainTracer.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/ChainTracer.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from swarmauri.core.tracing.IChainTracer import IChainTracer
-from typing import Callable, List, Tuple, Dict, Any   
-        
-class ChainTracer(IChainTracer):
-    def __init__(self):
-        self.traces = []
-
-    def process_chain(self, chain: List[Tuple[Callable[..., Any], List[Any], Dict[str, Any]]]) -> "ChainTracer":
-        """
-        Processes each item in the operation chain by executing the specified external function
-        with its args and kwargs. Logs starting, annotating, and ending the trace based on tuple position.
-
-        Args:
-            chain (List[Tuple[Callable[..., Any], List[Any], Dict[str, Any]]]): A list where each tuple contains:
-                - An external function to execute.
-                - A list of positional arguments for the function.
-                - A dictionary of keyword arguments for the function.
-        """
-        for i, (func, args, kwargs) in enumerate(chain):
-            # Infer operation type and log
-            
-            if i == 0:
-                operation = "Start"
-                self.start_trace(*args, **kwargs)
-            elif i == len(chain) - 1:
-                operation = "End"
-                self.end_trace(*args, **kwargs)
-            else:
-                operation = "Annotate"
-                self.annotate_trace(*args, **kwargs)
-                
-            # For the actual external function call
-            result = func(*args, **kwargs)
-            print(f"Function '{func.__name__}' executed with result: {result}")
-
-            self.traces.append((operation, func, args, kwargs, result))
-
-        return self
-
-    def start_trace(self, *args, **kwargs) -> None:
-        print(f"Starting trace with args: {args}, kwargs: {kwargs}")
-        
-    def annotate_trace(self, *args, **kwargs) -> None:
-        print(f"Annotating trace with args: {args}, kwargs: {kwargs}")
-
-    def end_trace(self, *args, **kwargs) -> None:
-        print(f"Ending trace with args: {args}, kwargs: {kwargs}")
-
-    def show(self) -> None:
-        for entry in self.traces:
+from swarmauri.core.tracing.IChainTracer import IChainTracer
+from typing import Callable, List, Tuple, Dict, Any   
+        
+class ChainTracer(IChainTracer):
+    def __init__(self):
+        self.traces = []
+
+    def process_chain(self, chain: List[Tuple[Callable[..., Any], List[Any], Dict[str, Any]]]) -> "ChainTracer":
+        """
+        Processes each item in the operation chain by executing the specified external function
+        with its args and kwargs. Logs starting, annotating, and ending the trace based on tuple position.
+
+        Args:
+            chain (List[Tuple[Callable[..., Any], List[Any], Dict[str, Any]]]): A list where each tuple contains:
+                - An external function to execute.
+                - A list of positional arguments for the function.
+                - A dictionary of keyword arguments for the function.
+        """
+        for i, (func, args, kwargs) in enumerate(chain):
+            # Infer operation type and log
+            
+            if i == 0:
+                operation = "Start"
+                self.start_trace(*args, **kwargs)
+            elif i == len(chain) - 1:
+                operation = "End"
+                self.end_trace(*args, **kwargs)
+            else:
+                operation = "Annotate"
+                self.annotate_trace(*args, **kwargs)
+                
+            # For the actual external function call
+            result = func(*args, **kwargs)
+            print(f"Function '{func.__name__}' executed with result: {result}")
+
+            self.traces.append((operation, func, args, kwargs, result))
+
+        return self
+
+    def start_trace(self, *args, **kwargs) -> None:
+        print(f"Starting trace with args: {args}, kwargs: {kwargs}")
+        
+    def annotate_trace(self, *args, **kwargs) -> None:
+        print(f"Annotating trace with args: {args}, kwargs: {kwargs}")
+
+    def end_trace(self, *args, **kwargs) -> None:
+        print(f"Ending trace with args: {args}, kwargs: {kwargs}")
+
+    def show(self) -> None:
+        for entry in self.traces:
             print(entry)
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/tracing/concrete/SimpleTraceContext.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/SimpleTraceContext.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from datetime import datetime
-from typing import Dict, Any, Optional
-
-from swarmauri.core.tracing.ITraceContext import ITraceContext
-
-class SimpleTraceContext(ITraceContext):
-    def __init__(self, trace_id: str, name: str, initial_attributes: Optional[Dict[str, Any]] = None):
-        self.trace_id = trace_id
-        self.name = name
-        self.attributes = initial_attributes if initial_attributes else {}
-        self.start_time = datetime.now()
-        self.end_time = None
-
-    def get_trace_id(self) -> str:
-        return self.trace_id
-
-    def add_attribute(self, key: str, value: Any):
-        self.attributes[key] = value
-
-    def close(self):
+from datetime import datetime
+from typing import Dict, Any, Optional
+
+from swarmauri.core.tracing.ITraceContext import ITraceContext
+
+class SimpleTraceContext(ITraceContext):
+    def __init__(self, trace_id: str, name: str, initial_attributes: Optional[Dict[str, Any]] = None):
+        self.trace_id = trace_id
+        self.name = name
+        self.attributes = initial_attributes if initial_attributes else {}
+        self.start_time = datetime.now()
+        self.end_time = None
+
+    def get_trace_id(self) -> str:
+        return self.trace_id
+
+    def add_attribute(self, key: str, value: Any):
+        self.attributes[key] = value
+
+    def close(self):
         self.end_time = datetime.now()
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/tracing/concrete/TracedVariable.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/TracedVariable.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Any
-from swarmauri.standard.tracing.concrete.SimpleTracer import SimpleTracer  # Assuming this is the path to the tracer
-
-class TracedVariable:
-    """
-    Wrapper class to trace multiple changes to a variable within the context manager.
-    """
-    def __init__(self, name: str, value: Any, tracer: SimpleTracer):
-        self.name = name
-        self._value = value
-        self._tracer = tracer
-        self._changes = []  # Initialize an empty list to track changes
-
-    @property
-    def value(self) -> Any:
-        return self._value
-
-    @value.setter
-    def value(self, new_value: Any):
-        # Record the change before updating the variable's value
-        change_annotation = {"from": self._value, "to": new_value}
-        self._changes.append(change_annotation)
-        
-        # Update the trace by appending the latest change to the list under a single key
-        # Note that the key is now constant and does not change with each update
-        self._tracer.annotate_trace(key=f"{self.name}_changes", value=self._changes)
-        
+from typing import Any
+from swarmauri.standard.tracing.concrete.SimpleTracer import SimpleTracer  # Assuming this is the path to the tracer
+
+class TracedVariable:
+    """
+    Wrapper class to trace multiple changes to a variable within the context manager.
+    """
+    def __init__(self, name: str, value: Any, tracer: SimpleTracer):
+        self.name = name
+        self._value = value
+        self._tracer = tracer
+        self._changes = []  # Initialize an empty list to track changes
+
+    @property
+    def value(self) -> Any:
+        return self._value
+
+    @value.setter
+    def value(self, new_value: Any):
+        # Record the change before updating the variable's value
+        change_annotation = {"from": self._value, "to": new_value}
+        self._changes.append(change_annotation)
+        
+        # Update the trace by appending the latest change to the list under a single key
+        # Note that the key is now constant and does not change with each update
+        self._tracer.annotate_trace(key=f"{self.name}_changes", value=self._changes)
+        
         self._value = new_value
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/tracing/concrete/VariableTracer.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/VariableTracer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from contextlib import contextmanager
-
-from swarmauri.standard.tracing.concrete.TracedVariable import TracedVariable
-from swarmauri.standard.tracing.concrete.SimpleTracer import SimpleTracer
-
-# Initialize a global instance of SimpleTracer for use across the application
-global_tracer = SimpleTracer()
-
-@contextmanager
-def VariableTracer(name: str, initial_value=None):
-    """
-    Context manager for tracing the declaration, modification, and usage of a variable.
-    """
-    trace_context = global_tracer.start_trace(name=f"Variable: {name}", initial_attributes={"initial_value": initial_value})
-    traced_variable = TracedVariable(name, initial_value, global_tracer)
-    
-    try:
-        yield traced_variable
-    finally:
-        # Optionally record any final value or state of the variable before it goes out of scope
-        global_tracer.annotate_trace(key=f"{name}_final", value={"final_value": traced_variable.value})
-        # End the trace, marking the variable's lifecycle
+from contextlib import contextmanager
+
+from swarmauri.standard.tracing.concrete.TracedVariable import TracedVariable
+from swarmauri.standard.tracing.concrete.SimpleTracer import SimpleTracer
+
+# Initialize a global instance of SimpleTracer for use across the application
+global_tracer = SimpleTracer()
+
+@contextmanager
+def VariableTracer(name: str, initial_value=None):
+    """
+    Context manager for tracing the declaration, modification, and usage of a variable.
+    """
+    trace_context = global_tracer.start_trace(name=f"Variable: {name}", initial_attributes={"initial_value": initial_value})
+    traced_variable = TracedVariable(name, initial_value, global_tracer)
+    
+    try:
+        yield traced_variable
+    finally:
+        # Optionally record any final value or state of the variable before it goes out of scope
+        global_tracer.annotate_trace(key=f"{name}_final", value={"final_value": traced_variable.value})
+        # End the trace, marking the variable's lifecycle
         global_tracer.end_trace()
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py` & `swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/TFIDFDocumentStore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,56 @@
-from typing import List, Union
-from swarmauri.core.documents.IDocument import IDocument
-from swarmauri.standard.documents.concrete.EmbeddedDocument import EmbeddedDocument
-from swarmauri.standard.vectorizers.concrete.Doc2VecVectorizer import Doc2VecVectorizer
-from swarmauri.standard.distances.concrete.CosineDistance import CosineDistance
-from swarmauri.standard.vector_stores.base.VectorDocumentStoreRetrieveBase import VectorDocumentStoreRetrieveBase
-from swarmauri.standard.vector_stores.base.SaveLoadStoreBase import SaveLoadStoreBase    
-
-
-class Doc2VecVectorStore(VectorDocumentStoreRetrieveBase, SaveLoadStoreBase):
-    def __init__(self):
-        self.vectorizer = Doc2VecVectorizer()
-        self.metric = CosineDistance()
-        self.documents = []      
-        SaveLoadStoreBase.__init__(self, self.vectorizer, self.documents)
-
-    def add_document(self, document: IDocument) -> None:
-        self.documents.append(document)
-        self._recalculate_embeddings()
-
-    def add_documents(self, documents: List[IDocument]) -> None:
-        self.documents.extend(documents)
-        self._recalculate_embeddings()
-
-    def get_document(self, doc_id: str) -> Union[EmbeddedDocument, None]:
-        for document in self.documents:
-            if document.id == doc_id:
-                return document
-        return None
-
-    def get_all_documents(self) -> List[EmbeddedDocument]:
-        return self.documents
-
-    def delete_document(self, doc_id: str) -> None:
-        self.documents = [doc for doc in self.documents if doc.id != doc_id]
-        self._recalculate_embeddings()
-
-    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
-        for i, document in enumerate(self.documents):
-            if document.id == doc_id:
-                self.documents[i] = updated_document
-                break
-        self._recalculate_embeddings()
-
-    def _recalculate_embeddings(self):
-        # Recalculate document embeddings for the current set of documents
-        documents_text = [_d.content for _d in self.documents if _d.content]
-        embeddings = self.vectorizer.fit_transform(documents_text)
-
-        embedded_documents = [EmbeddedDocument(id=_d.id, 
-            content=_d.content, 
-            metadata=_d.metadata, 
-            embedding=embeddings[_count]) for _count, _d in enumerate(self.documents)
-            if _d.content]
-
-        self.documents = embedded_documents
-
-    def retrieve(self, query: str, top_k: int = 5) -> List[IDocument]:
-        query_vector = self.vectorizer.infer_vector(query)
-        document_vectors = [_d.embedding for _d in self.documents if _d.content]
-
-        distances = self.metric.distances(query_vector, document_vectors)
-
-        # Get the indices of the top_k least distant (most similar) documents
-        top_k_indices = sorted(range(len(distances)), key=lambda i: distances[i])[:top_k]
-        
-        return [self.documents[i] for i in top_k_indices]
+from typing import List, Union
+from swarmauri.core.documents.IDocument import IDocument
+from swarmauri.core.document_stores.IDocumentStore import IDocumentStore
+from swarmauri.core.retrievers.IRetriever import IRetriever
+from swarmauri.standard.vectorizers.concrete.TFIDFVectorizer import TFIDFVectorizer
+from swarmauri.standard.vector_stores.concrete.CosineDistance import CosineDistance
+
+class TFIDFDocumentStore(IDocumentStore, IRetriever):
+    def __init__(self):
+        self.vectorizer = TFIDFVectorizer()
+        self.metric = CosineDistance()
+        self.documents = []
+        self.tfidf_matrix = None        
+
+    def add_document(self, document: IDocument) -> None:
+        self.documents.append(document)
+        # Recalculate TF-IDF matrix for the current set of documents
+        self.tfidf_matrix = self.vectorizer.fit([doc.content for doc in self.documents])
+
+    def add_documents(self, documents: List[IDocument]) -> None:
+        self.documents.extend(documents)
+        # Recalculate TF-IDF matrix for the current set of documents
+        self.tfidf_matrix = self.vectorizer.fit([doc.content for doc in self.documents])
+
+    def get_document(self, doc_id: str) -> Union[IDocument, None]:
+        for document in self.documents:
+            if document.id == doc_id:
+                return document
+        return None
+
+    def get_all_documents(self) -> List[IDocument]:
+        return self.documents
+
+    def delete_document(self, doc_id: str) -> None:
+        self.documents = [doc for doc in self.documents if doc.id != doc_id]
+        # Recalculate TF-IDF matrix for the current set of documents
+        self.tfidf_matrix = self.vectorizer.fit([doc.content for doc in self.documents])
+
+    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
+        for i, document in enumerate(self.documents):
+            if document.id == doc_id:
+                self.documents[i] = updated_document
+                break
+        # Recalculate TF-IDF matrix for the current set of documents
+        self.tfidf_matrix = self.vectorizer.fit([doc.content for doc in self.documents])
+
+    def retrieve(self, query: str, top_k: int = 5) -> List[IDocument]:
+        documents = [doc.content for doc in self.documents]
+        documents.append(query)
+        tmp_tfidf_matrix = self.vectorizer.transform(documents)
+        query_vector = tmp_tfidf_matrix[-1]
+    
+        distances = self.metric.distances(query_vector, tmp_tfidf_matrix[:-1])  # Calculate similarities
+        # Get the indices of the top_k most similar (least distant) documents
+        top_k_indices = sorted(range(len(distances)), key=lambda i: distances[i])[:top_k]
+        return [self.documents[i] for i in top_k_indices]
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py` & `swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,56 @@
-from typing import List, Union, Any
-import joblib
-from sklearn.feature_extraction.text import TfidfVectorizer as SklearnTfidfVectorizer
-from swarmauri.core.vectorizers.IVectorize import IVectorize
-from swarmauri.core.vectorizers.IFeature import IFeature
-from swarmauri.core.vectors.IVector import IVector
-from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
-from swarmauri.core.vectorizers.ISaveModel import ISaveModel
-
-
-class TFIDFVectorizer(IVectorize, IFeature, ISaveModel):
-    def __init__(self):
-        # Using scikit-learn's TfidfVectorizer as the underlying mechanism
-        self.model = SklearnTfidfVectorizer()
-        super().__init__()
-        
-    def extract_features(self):
-        return self.model.get_feature_names_out()
-
-    def fit(self, data: Union[str, Any]) -> List[IVector]:
-        """
-        Vectorizes the input data using the TF-IDF scheme.
-
-        Parameters:
-        - data (Union[str, Any]): The input data to be vectorized. Expected to be a single string (document)
-                                  or a list of strings (corpus).
-
-        Returns:
-        - List[IVector]: A list containing IVector instances, each representing a document's TF-IDF vector.
-        """
-        if isinstance(data, str):
-            data = [data]  # Convert a single string into a list for the vectorizer
-        
-        self.fit_matrix = self.model.fit_transform(data)
-
-        # Convert the sparse matrix rows into SimpleVector instances
-        vectors = [SimpleVector(vector.toarray().flatten()) for vector in self.fit_matrix]
-
-        return vectors
-
-    def fit_transform(self, data: Union[str, Any], documents) -> List[IVector]:
-        documents = [doc.content for doc in documents]
-        if isinstance(data, str):
-            data = [data]  # Convert a single string into a list for the vectorizer
-        documents.extend(data)
-
-        transform_matrix = self.model.fit_transform(documents)
-
-        # Convert the sparse matrix rows into SimpleVector instances
-        vectors = [SimpleVector(vector.toarray().flatten()) for vector in transform_matrix]
-        return vectors
-    
-    def transform(self, data: Union[str, Any], documents) -> List[IVector]:
-        raise NotImplementedError('Transform not implemented on TFIDFVectorizer.')
-
-    def infer_vector(self, data: str, documents) -> IVector:
-        documents = [doc.content for doc in documents]
-        documents.append(data)
-        tmp_tfidf_matrix = self.transform(documents)
-        query_vector = tmp_tfidf_matrix[-1]
-        return query_vector
-
-    def save_model(self, path: str) -> None:
-        """
-        Saves the TF-IDF model to the specified path using joblib.
-        """
-        joblib.dump(self.model, path)
-    
-    def load_model(self, path: str) -> None:
-        """
-        Loads a TF-IDF model from the specified path using joblib.
-        """
-        self.model = joblib.load(path)
+from sklearn.feature_extraction.text import TfidfVectorizer as SklearnTfidfVectorizer
+from typing import List, Union, Any
+from swarmauri.core.vectorizers.IVectorize import IVectorize
+from swarmauri.core.vectors.IVector import IVector
+from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
+
+class TFIDFVectorizer(IVectorize):
+    def __init__(self):
+        # Using scikit-learn's TfidfVectorizer as the underlying mechanism
+        self.tfidf_vectorizer = SklearnTfidfVectorizer()
+        super().__init__()
+        
+    def extract_features(self):
+        return self.tfidf_vectorizer.get_feature_names_out()
+
+    def fit(self, data: Union[str, Any]) -> List[IVector]:
+        """
+        Vectorizes the input data using the TF-IDF scheme.
+
+        Parameters:
+        - data (Union[str, Any]): The input data to be vectorized. Expected to be a single string (document)
+                                  or a list of strings (corpus).
+
+        Returns:
+        - List[IVector]: A list containing IVector instances, each representing a document's TF-IDF vector.
+        """
+        if isinstance(data, str):
+            data = [data]  # Convert a single string into a list for the vectorizer
+        
+        tfidf_matrix = self.tfidf_vectorizer.fit_transform(data)
+
+        # Convert the sparse matrix rows into SimpleVector instances
+        vectors = [SimpleVector(vector.toarray().flatten()) for vector in tfidf_matrix]
+
+        return vectors
+    
+    def transform(self, data: Union[str, Any]) -> List[IVector]:
+        """
+        Vectorizes the input data using the TF-IDF scheme.
+
+        Parameters:
+        - data (Union[str, Any]): The input data to be vectorized. Expected to be a single string (document)
+                                  or a list of strings (corpus).
+
+        Returns:
+        - List[IVector]: A list containing IVector instances, each representing a document's TF-IDF vector.
+        """
+        if isinstance(data, str):
+            data = [data]  # Convert a single string into a list for the vectorizer
+        
+        tfidf_matrix = self.tfidf_vectorizer.fit_transform(data)
+
+        # Convert the sparse matrix rows into SimpleVector instances
+        vectors = [SimpleVector(vector.toarray().flatten()) for vector in tfidf_matrix]
+
+        return vectors
```

### Comparing `swarmauri-0.1.80/swarmauri/standard/vectors/concrete/VectorProduct.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/VectorProduct.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import numpy as np
-from typing import List
-
-from swarmauri.core.vectors.IVector import IVector
-from swarmauri.core.vectors.IVectorProduct import IVectorProduct
-from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
-
-class VectorProduct(IVectorProduct):
-    def dot_product(self, vector_a: IVector, vector_b: IVector) -> float:
-        a = np.array(vector_a.data).flatten()
-        b = np.array(vector_b.data).flatten()
-        return np.dot(a, b)
-    
-    def cross_product(self, vector_a: IVector, vector_b: IVector) -> IVector:
-        if len(vector_a.data) != 3 or len(vector_b.data) != 3:
-            raise ValueError("Cross product is only defined for 3-dimensional vectors")
-        a = np.array(vector_a.data)
-        b = np.array(vector_b.data)
-        cross = np.cross(a, b)
-        return SimpleVector(cross.tolist())
-    
-    def vector_triple_product(self, vector_a: IVector, vector_b: IVector, vector_c: IVector) -> IVector:
-        a = np.array(vector_a.data)
-        b = np.array(vector_b.data)
-        c = np.array(vector_c.data)
-        result = np.cross(a, np.cross(b, c))
-        return SimpleVector(result.tolist())
-    
-    def scalar_triple_product(self, vector_a: IVector, vector_b: IVector, vector_c: IVector) -> float:
-        a = np.array(vector_a.data)
-        b = np.array(vector_b.data)
-        c = np.array(vector_c.data)
+import numpy as np
+from typing import List
+
+from swarmauri.core.vectors.IVector import IVector
+from swarmauri.core.vector_stores.IVectorProduct import IVectorProduct
+from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
+
+class VectorProduct(IVectorProduct):
+    def dot_product(self, vector_a: IVector, vector_b: IVector) -> float:
+        a = np.array(vector_a.data)
+        b = np.array(vector_b.data)
+        return np.dot(a, b)
+    
+    def cross_product(self, vector_a: IVector, vector_b: IVector) -> IVector:
+        if len(vector_a.data) != 3 or len(vector_b.data) != 3:
+            raise ValueError("Cross product is only defined for 3-dimensional vectors")
+        a = np.array(vector_a.data)
+        b = np.array(vector_b.data)
+        cross = np.cross(a, b)
+        return SimpleVector(cross.tolist())
+    
+    def vector_triple_product(self, vector_a: IVector, vector_b: IVector, vector_c: IVector) -> IVector:
+        a = np.array(vector_a.data)
+        b = np.array(vector_b.data)
+        c = np.array(vector_c.data)
+        result = np.cross(a, np.cross(b, c))
+        return SimpleVector(result.tolist())
+    
+    def scalar_triple_product(self, vector_a: IVector, vector_b: IVector, vector_c: IVector) -> float:
+        a = np.array(vector_a.data)
+        b = np.array(vector_b.data)
+        c = np.array(vector_c.data)
         return np.dot(a, np.cross(b, c))
```

### Comparing `swarmauri-0.1.80/swarmauri.egg-info/SOURCES.txt` & `swarmauri-0.1.9/swarmauri.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -20,116 +20,94 @@
 swarmauri/community/tools/concrete/DownloadPdfTool.py
 swarmauri/community/tools/concrete/EntityRecognitionTool.py
 swarmauri/community/tools/concrete/GmailReadTool.py
 swarmauri/community/tools/concrete/GmailSendTool.py
 swarmauri/community/tools/concrete/PaCMAP.py
 swarmauri/community/tools/concrete/SentimentAnalysisTool.py
 swarmauri/community/tools/concrete/WebScrapingTool.py
-swarmauri/community/tools/concrete/ZapierHookTool.py
 swarmauri/community/tools/concrete/__init__.py
 swarmauri/core/__init__.py
 swarmauri/core/agent_apis/IAgentCommands.py
 swarmauri/core/agent_apis/IAgentRouterCRUD.py
 swarmauri/core/agent_apis/__init__.py
-swarmauri/core/agent_factories/IAgentFactory.py
-swarmauri/core/agent_factories/IExportConf.py
-swarmauri/core/agent_factories/__init__.py
-swarmauri/core/agents/IAgent.py
 swarmauri/core/agents/IAgentConversation.py
+swarmauri/core/agents/IAgentDocument.py
 swarmauri/core/agents/IAgentName.py
 swarmauri/core/agents/IAgentParser.py
 swarmauri/core/agents/IAgentRetriever.py
 swarmauri/core/agents/IAgentToolkit.py
-swarmauri/core/agents/IAgentVectorStore.py
+swarmauri/core/agents/ISwarmAgent.py
 swarmauri/core/agents/__init__.py
 swarmauri/core/chains/ICallableChain.py
 swarmauri/core/chains/IChain.py
-swarmauri/core/chains/IChainFactory.py
 swarmauri/core/chains/IChainStep.py
 swarmauri/core/chains/__init__.py
 swarmauri/core/chunkers/IChunker.py
 swarmauri/core/chunkers/__init__.py
 swarmauri/core/conversations/IConversation.py
 swarmauri/core/conversations/IMaxSize.py
 swarmauri/core/conversations/ISystemContext.py
 swarmauri/core/conversations/__init__.py
-swarmauri/core/distances/IDistanceSimilarity.py
-swarmauri/core/distances/__init__.py
-swarmauri/core/document_stores/IDocumentRetrieve.py
 swarmauri/core/document_stores/IDocumentStore.py
 swarmauri/core/document_stores/__init__.py
 swarmauri/core/documents/IDocument.py
 swarmauri/core/documents/IEmbed.py
-swarmauri/core/documents/IExperimentDocument.py
 swarmauri/core/documents/__init__.py
-swarmauri/core/experiment_stores/IExperimentStore.py
-swarmauri/core/experiment_stores/__init__.py
 swarmauri/core/messages/IMessage.py
 swarmauri/core/messages/__init__.py
-swarmauri/core/metrics/IAggMeasurements.py
-swarmauri/core/metrics/ICalculateMetric.py
-swarmauri/core/metrics/IMetric.py
-swarmauri/core/metrics/IThreshold.py
-swarmauri/core/metrics/__init__.py
 swarmauri/core/models/IFit.py
 swarmauri/core/models/IModel.py
 swarmauri/core/models/IPredict.py
 swarmauri/core/models/__init__.py
 swarmauri/core/parsers/IParser.py
 swarmauri/core/parsers/__init__.py
 swarmauri/core/prompts/IPrompt.py
-swarmauri/core/prompts/ITemplate.py
 swarmauri/core/prompts/__init__.py
-swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
+swarmauri/core/retrievers/IRetriever.py
+swarmauri/core/retrievers/__init__.py
+swarmauri/core/swarm_apis/IAgentRegistration.py
 swarmauri/core/swarm_apis/ISwarmAPI.py
 swarmauri/core/swarm_apis/__init__.py
 swarmauri/core/swarms/ISwarm.py
-swarmauri/core/swarms/ISwarmAgentRegistration.py
-swarmauri/core/swarms/ISwarmChainCRUD.py
 swarmauri/core/swarms/ISwarmComponent.py
-swarmauri/core/swarms/ISwarmConfigurationExporter.py
-swarmauri/core/swarms/ISwarmFactory.py
 swarmauri/core/swarms/__init__.py
 swarmauri/core/toolkits/IToolkit.py
 swarmauri/core/toolkits/__init__.py
 swarmauri/core/tools/IParameter.py
 swarmauri/core/tools/ITool.py
 swarmauri/core/tools/__init__.py
 swarmauri/core/tracing/IChainTracer.py
 swarmauri/core/tracing/ITraceContext.py
 swarmauri/core/tracing/ITracer.py
 swarmauri/core/tracing/__init__.py
 swarmauri/core/utils/ITransactional.py
 swarmauri/core/utils/__init__.py
 swarmauri/core/vector_stores/IAngleBetweenVectors.py
 swarmauri/core/vector_stores/IDecompose.py
+swarmauri/core/vector_stores/IDistanceSimilarity.py
 swarmauri/core/vector_stores/IDivergence.py
 swarmauri/core/vector_stores/IGradient.py
 swarmauri/core/vector_stores/IOrthogonalProject.py
 swarmauri/core/vector_stores/IProject.py
 swarmauri/core/vector_stores/IReflect.py
-swarmauri/core/vector_stores/ISaveLoadStore.py
 swarmauri/core/vector_stores/ISimilarity.py
 swarmauri/core/vector_stores/ISimiliarityQuery.py
 swarmauri/core/vector_stores/IVectorArithmetic.py
 swarmauri/core/vector_stores/IVectorBasisCheck.py
 swarmauri/core/vector_stores/IVectorLinearCombination.py
 swarmauri/core/vector_stores/IVectorNorm.py
-swarmauri/core/vector_stores/IVectorRetrieve.py
+swarmauri/core/vector_stores/IVectorProduct.py
 swarmauri/core/vector_stores/IVectorRotate.py
 swarmauri/core/vector_stores/IVectorSpan.py
 swarmauri/core/vector_stores/IVectorStore.py
 swarmauri/core/vector_stores/__init__.py
-swarmauri/core/vectorizers/IFeature.py
-swarmauri/core/vectorizers/ISaveModel.py
 swarmauri/core/vectorizers/IVectorize.py
 swarmauri/core/vectorizers/__init__.py
 swarmauri/core/vectors/IVector.py
 swarmauri/core/vectors/IVectorMeta.py
-swarmauri/core/vectors/IVectorProduct.py
 swarmauri/core/vectors/IVectorTransform.py
 swarmauri/core/vectors/__init__.py
 swarmauri/experimental/__init__.py
 swarmauri/experimental/chains/ChainOrderStrategy.py
 swarmauri/experimental/chains/ChainOrderStrategyBase.py
 swarmauri/experimental/chains/ChainProcessingStrategy.py
 swarmauri/experimental/chains/ChainProcessingStrategyBase.py
@@ -138,85 +116,64 @@
 swarmauri/experimental/chains/MatrixOrderStrategy.py
 swarmauri/experimental/chains/MatrixProcessingStrategy.py
 swarmauri/experimental/chains/TypeAgnosticCallableChain.py
 swarmauri/experimental/chains/__init__.py
 swarmauri/experimental/conversations/ConsensusBuildingConversation.py
 swarmauri/experimental/conversations/SemanticConversation.py
 swarmauri/experimental/conversations/__init__.py
-swarmauri/experimental/distances/CanberraDistance.py
-swarmauri/experimental/distances/ChebyshevDistance.py
-swarmauri/experimental/distances/HaversineDistance.py
-swarmauri/experimental/distances/ManhattanDistance.py
-swarmauri/experimental/distances/MinkowskiDistance.py
-swarmauri/experimental/distances/SSASimilarity.py
-swarmauri/experimental/distances/SSIVSimilarity.py
-swarmauri/experimental/distances/ScannVectorStore.py
-swarmauri/experimental/distances/SorensenDiceDistance.py
-swarmauri/experimental/distances/SquaredEuclideanDistance.py
-swarmauri/experimental/distances/__init__.py
-swarmauri/experimental/document_stores/TriplesDocumentStore.py
-swarmauri/experimental/document_stores/Word2VecDocumentStore.py
-swarmauri/experimental/document_stores/__init__.py
 swarmauri/experimental/models/HierarchicalAttentionModel.py
 swarmauri/experimental/models/SageMaker.py
 swarmauri/experimental/models/__init__.py
 swarmauri/experimental/parsers/PDFToTextParser.py
 swarmauri/experimental/parsers/__init__.py
 swarmauri/experimental/tools/CypherQueryTool.py
 swarmauri/experimental/tools/FileDownloaderTool.py
 swarmauri/experimental/tools/LinkedInArticleTool.py
 swarmauri/experimental/tools/OutlookSendMailTool.py
 swarmauri/experimental/tools/SQLite3QueryTool.py
 swarmauri/experimental/tools/TwitterPostTool.py
 swarmauri/experimental/tools/__init__.py
-swarmauri/experimental/tracing/RemoteTrace.py
-swarmauri/experimental/tracing/__init__.py
 swarmauri/experimental/utils/ISerializable.py
 swarmauri/experimental/utils/__init__.py
 swarmauri/experimental/utils/get_last_frame.py
-swarmauri/experimental/utils/log_prompt_response.py
 swarmauri/experimental/utils/save_schema.py
-swarmauri/experimental/vector_stores/TriplesDocumentStore.py
-swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
+swarmauri/experimental/vector_stores/CanberraDistance.py
+swarmauri/experimental/vector_stores/ChebyshevDistance.py
+swarmauri/experimental/vector_stores/HaversineDistance.py
+swarmauri/experimental/vector_stores/ManhattanDistance.py
+swarmauri/experimental/vector_stores/MinkowskiDistance.py
+swarmauri/experimental/vector_stores/SSASimilarity.py
+swarmauri/experimental/vector_stores/SSIVSimilarity.py
+swarmauri/experimental/vector_stores/ScannVectorStore.py
+swarmauri/experimental/vector_stores/SorensenDiceDistance.py
+swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py
 swarmauri/experimental/vector_stores/__init__.py
-swarmauri/experimental/vectorizers/DGLVectorizer.py
-swarmauri/experimental/vectorizers/__init__.py
 swarmauri/standard/__init__.py
-swarmauri/standard/agent_factories/__init__.py
-swarmauri/standard/agent_factories/base/__init__.py
-swarmauri/standard/agent_factories/concrete/AgentFactory.py
-swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
-swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
-swarmauri/standard/agent_factories/concrete/__init__.py
 swarmauri/standard/agents/__init__.py
 swarmauri/standard/agents/base/AgentBase.py
 swarmauri/standard/agents/base/ConversationAgentBase.py
 swarmauri/standard/agents/base/NamedAgentBase.py
 swarmauri/standard/agents/base/ToolAgentBase.py
-swarmauri/standard/agents/base/VectorStoreAgentBase.py
 swarmauri/standard/agents/base/__init__.py
 swarmauri/standard/agents/concrete/ChatSwarmAgent.py
-swarmauri/standard/agents/concrete/GenerativeRagAgent.py
 swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
 swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
-swarmauri/standard/agents/concrete/RagAgent.py
 swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
 swarmauri/standard/agents/concrete/SingleCommandAgent.py
 swarmauri/standard/agents/concrete/ToolAgent.py
 swarmauri/standard/agents/concrete/__init__.py
 swarmauri/standard/apis/__init__.py
 swarmauri/standard/apis/base/__init__.py
 swarmauri/standard/apis/concrete/__init__.py
 swarmauri/standard/chains/__init__.py
 swarmauri/standard/chains/base/ChainBase.py
 swarmauri/standard/chains/base/ChainStepBase.py
 swarmauri/standard/chains/base/__init__.py
 swarmauri/standard/chains/concrete/CallableChain.py
-swarmauri/standard/chains/concrete/ChainStep.py
-swarmauri/standard/chains/concrete/StateChain.py
+swarmauri/standard/chains/concrete/Chain.py
 swarmauri/standard/chains/concrete/__init__.py
 swarmauri/standard/chunkers/__init__.py
 swarmauri/standard/chunkers/base/__init__.py
 swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
 swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
 swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
 swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
@@ -227,26 +184,20 @@
 swarmauri/standard/conversations/base/SystemContextBase.py
 swarmauri/standard/conversations/base/__init__.py
 swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
 swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
 swarmauri/standard/conversations/concrete/SharedConversation.py
 swarmauri/standard/conversations/concrete/SimpleConversation.py
 swarmauri/standard/conversations/concrete/__init__.py
-swarmauri/standard/distances/__init__.py
-swarmauri/standard/distances/base/__init__.py
-swarmauri/standard/distances/concrete/ChiSquaredDistance.py
-swarmauri/standard/distances/concrete/CosineDistance.py
-swarmauri/standard/distances/concrete/EuclideanDistance.py
-swarmauri/standard/distances/concrete/JaccardIndexDistance.py
-swarmauri/standard/distances/concrete/LevenshteinDistance.py
-swarmauri/standard/distances/concrete/__init__.py
 swarmauri/standard/document_stores/__init__.py
 swarmauri/standard/document_stores/base/DocumentStoreBase.py
-swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
 swarmauri/standard/document_stores/base/__init__.py
+swarmauri/standard/document_stores/concrete/Doc2VecDocumentStore.py
+swarmauri/standard/document_stores/concrete/TFIDFDocumentStore.py
+swarmauri/standard/document_stores/concrete/Word2VecDocumentStore.py
 swarmauri/standard/document_stores/concrete/__init__.py
 swarmauri/standard/documents/__init__.py
 swarmauri/standard/documents/base/DocumentBase.py
 swarmauri/standard/documents/base/EmbeddedBase.py
 swarmauri/standard/documents/base/__init__.py
 swarmauri/standard/documents/concrete/Document.py
 swarmauri/standard/documents/concrete/EmbeddedDocument.py
@@ -255,31 +206,14 @@
 swarmauri/standard/messages/base/MessageBase.py
 swarmauri/standard/messages/base/__init__.py
 swarmauri/standard/messages/concrete/AgentMessage.py
 swarmauri/standard/messages/concrete/FunctionMessage.py
 swarmauri/standard/messages/concrete/HumanMessage.py
 swarmauri/standard/messages/concrete/SystemMessage.py
 swarmauri/standard/messages/concrete/__init__.py
-swarmauri/standard/metrics/__init__.py
-swarmauri/standard/metrics/base/AggregateMetricBase.py
-swarmauri/standard/metrics/base/CalculateMetricBase.py
-swarmauri/standard/metrics/base/MetricBase.py
-swarmauri/standard/metrics/base/ThresholdMetricBase.py
-swarmauri/standard/metrics/base/__init__.py
-swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
-swarmauri/standard/metrics/concrete/HitRateAtK.py
-swarmauri/standard/metrics/concrete/ImpressionAtK.py
-swarmauri/standard/metrics/concrete/MeanMetric.py
-swarmauri/standard/metrics/concrete/StaticValueMetric.py
-swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
-swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
-swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
-swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
-swarmauri/standard/metrics/concrete/ZeroMetric.py
-swarmauri/standard/metrics/concrete/__init__.py
 swarmauri/standard/models/__init__.py
 swarmauri/standard/models/base/ModelBase.py
 swarmauri/standard/models/base/__init__.py
 swarmauri/standard/models/concrete/AzureGPT.py
 swarmauri/standard/models/concrete/OpenAIImageGenerator.py
 swarmauri/standard/models/concrete/OpenAIModel.py
 swarmauri/standard/models/concrete/OpenAIToolModel.py
@@ -292,33 +226,35 @@
 swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
 swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
 swarmauri/standard/parsers/concrete/MarkdownParser.py
 swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
 swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
 swarmauri/standard/parsers/concrete/PythonParser.py
 swarmauri/standard/parsers/concrete/RegExParser.py
-swarmauri/standard/parsers/concrete/TFIDFParser.py
 swarmauri/standard/parsers/concrete/TextBlobNounParser.py
 swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
+swarmauri/standard/parsers/concrete/TfidfParser.py
 swarmauri/standard/parsers/concrete/URLExtractorParser.py
 swarmauri/standard/parsers/concrete/XMLParser.py
 swarmauri/standard/parsers/concrete/__init__.py
 swarmauri/standard/prompts/__init__.py
 swarmauri/standard/prompts/base/__init__.py
 swarmauri/standard/prompts/concrete/Prompt.py
-swarmauri/standard/prompts/concrete/PromptGenerator.py
 swarmauri/standard/prompts/concrete/PromptTemplate.py
 swarmauri/standard/prompts/concrete/__init__.py
+swarmauri/standard/retrievers/__init__.py
+swarmauri/standard/retrievers/base/DocumentRetrieverBase.py
+swarmauri/standard/retrievers/base/__init__.py
+swarmauri/standard/retrievers/concrete/__init__.py
 swarmauri/standard/states/__init__.py
 swarmauri/standard/states/base/__init__.py
 swarmauri/standard/states/concrete/__init__.py
 swarmauri/standard/swarms/__init__.py
 swarmauri/standard/swarms/base/SwarmComponentBase.py
 swarmauri/standard/swarms/base/__init__.py
-swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
 swarmauri/standard/swarms/concrete/__init__.py
 swarmauri/standard/toolkits/__init__.py
 swarmauri/standard/toolkits/base/ToolkitBase.py
 swarmauri/standard/toolkits/base/__init__.py
 swarmauri/standard/toolkits/concrete/Toolkit.py
 swarmauri/standard/toolkits/concrete/__init__.py
 swarmauri/standard/tools/__init__.py
@@ -335,32 +271,28 @@
 swarmauri/standard/tracing/concrete/ChainTracer.py
 swarmauri/standard/tracing/concrete/SimpleTraceContext.py
 swarmauri/standard/tracing/concrete/SimpleTracer.py
 swarmauri/standard/tracing/concrete/TracedVariable.py
 swarmauri/standard/tracing/concrete/VariableTracer.py
 swarmauri/standard/tracing/concrete/__init__.py
 swarmauri/standard/utils/__init__.py
-swarmauri/standard/utils/load_documents_from_json.py
 swarmauri/standard/vector_stores/__init__.py
-swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
-swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
-swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
 swarmauri/standard/vector_stores/base/__init__.py
-swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
-swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
-swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
-swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
+swarmauri/standard/vector_stores/concrete/ChiSquaredDistance.py
+swarmauri/standard/vector_stores/concrete/CosineDistance.py
+swarmauri/standard/vector_stores/concrete/EuclideanDistance.py
+swarmauri/standard/vector_stores/concrete/FaissVectorStore.py
+swarmauri/standard/vector_stores/concrete/JaccardIndexDistance.py
+swarmauri/standard/vector_stores/concrete/LevenshteinDistance.py
+swarmauri/standard/vector_stores/concrete/VectorProduct.py
+swarmauri/standard/vector_stores/concrete/WeaviateVectorStore.py
 swarmauri/standard/vector_stores/concrete/__init__.py
 swarmauri/standard/vectorizers/__init__.py
 swarmauri/standard/vectorizers/base/__init__.py
-swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
-swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
-swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
-swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
+swarmauri/standard/vectorizers/concrete/BERTEmbeddingVectorizer.py
 swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
 swarmauri/standard/vectorizers/concrete/__init__.py
 swarmauri/standard/vectors/__init__.py
 swarmauri/standard/vectors/base/VectorBase.py
 swarmauri/standard/vectors/base/__init__.py
 swarmauri/standard/vectors/concrete/SimpleVector.py
-swarmauri/standard/vectors/concrete/VectorProduct.py
 swarmauri/standard/vectors/concrete/__init__.py
```


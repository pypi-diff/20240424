# Comparing `tmp/athena_intelligence-0.1.45.tar.gz` & `tmp/athena_intelligence-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.45.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.49.tar", max compression
```

## Comparing `athena_intelligence-0.1.45.tar` & `athena_intelligence-0.1.49.tar`

### file list

```diff
@@ -1,59 +1,65 @@
--rw-r--r--   0        0        0     4235 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/README.md
--rw-r--r--   0        0        0      435 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/pyproject.toml
--rw-r--r--   0        0        0     1389 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/__init__.py
--rw-r--r--   0        0        0     5416 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/base_client.py
--rw-r--r--   0        0        0      159 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/__init__.py
--rw-r--r--   0        0        0     8333 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/client.py
--rw-r--r--   0        0        0      187 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/types/__init__.py
--rw-r--r--   0        0        0     2203 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/types/structured_parse_in_parsing_model.py
--rw-r--r--   0        0        0     3576 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7515 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    13328 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/tools/client.py
--rw-r--r--   0        0        0     1450 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/dataset.py
--rw-r--r--   0        0        0      895 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1021 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1128 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      989 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      865 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     3180 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/report.py
--rw-r--r--   0        0        0     1126 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      905 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1829 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/tool_models.py
--rw-r--r--   0        0        0     1422 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/tools.py
--rw-r--r--   0        0        0      893 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/url_result.py
--rw-r--r--   0        0        0      992 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/README.md
+-rw-r--r--   0        0        0      603 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/pyproject.toml
+-rw-r--r--   0        0        0     1547 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/__init__.py
+-rw-r--r--   0        0        0     6860 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0     8026 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/chain/client.py
+-rw-r--r--   0        0        0     3576 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/client.py
+-rw-r--r--   0        0        0      853 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1495 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12498 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6338 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6623 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/tasks/__init__.py
+-rw-r--r--   0        0        0     8214 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/tasks/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    20114 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1722 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/__init__.py
+-rw-r--r--   0        0        0      994 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1061 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/document.py
+-rw-r--r--   0        0        0      875 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1001 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1143 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      969 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      969 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      953 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      919 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0     4101 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/llm_model.py
+-rw-r--r--   0        0        0      845 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1031 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2991 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/model.py
+-rw-r--r--   0        0        0     1034 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/plan_execute_out.py
+-rw-r--r--   0        0        0      926 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/report.py
+-rw-r--r--   0        0        0     1106 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      880 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      885 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1829 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/tool_models.py
+-rw-r--r--   0        0        0     1422 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/tools.py
+-rw-r--r--   0        0        0      873 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      972 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-24 19:01:27.054424 athena_intelligence-0.1.49/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       87 2024-04-24 19:01:27.058424 athena_intelligence-0.1.49/src/athena/version.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.49/PKG-INFO
```

### Comparing `athena_intelligence-0.1.45/README.md` & `athena_intelligence-0.1.49/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/__init__.py` & `athena_intelligence-0.1.49/src/athena/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Dataset,
+    Document,
     ExcecuteToolFirstWorkflowOut,
     FirecrawlScrapeUrlDataReponseDto,
     FirecrawlScrapeUrlMetadata,
     GetDatasetsResponse,
     GetSnippetsResponse,
     HttpValidationError,
+    LangchainDocumentsRequestOut,
+    LlmModel,
     MessageOut,
     MessageOutDto,
     Model,
+    PlanExecuteOut,
     Report,
     Snippet,
     SqlResults,
     StatusEnum,
     StructuredParseResult,
     ToolModels,
     Tools,
     UrlResult,
     ValidationError,
     ValidationErrorLocItem,
 )
 from .errors import UnprocessableEntityError
-from . import chain, dataset, message, query, report, search, snippet, tools
-from .chain import StructuredParseInParsingModel
+from . import chain, dataset, message, query, report, search, snippet, tasks, tools
 from .environment import AthenaEnvironment
+from .version import __version__
 
 __all__ = [
     "AthenaEnvironment",
     "Dataset",
+    "Document",
     "ExcecuteToolFirstWorkflowOut",
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
+    "LangchainDocumentsRequestOut",
+    "LlmModel",
     "MessageOut",
     "MessageOutDto",
     "Model",
+    "PlanExecuteOut",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
-    "StructuredParseInParsingModel",
     "StructuredParseResult",
     "ToolModels",
     "Tools",
     "UnprocessableEntityError",
     "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
+    "__version__",
     "chain",
     "dataset",
     "message",
     "query",
     "report",
     "search",
     "snippet",
+    "tasks",
     "tools",
 ]
```

### Comparing `athena_intelligence-0.1.45/src/athena/base_client.py` & `athena_intelligence-0.1.49/src/athena/base_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .dataset.client import AsyncDatasetClient, DatasetClient
 from .environment import AthenaEnvironment
 from .message.client import AsyncMessageClient, MessageClient
 from .query.client import AsyncQueryClient, QueryClient
 from .report.client import AsyncReportClient, ReportClient
 from .search.client import AsyncSearchClient, SearchClient
 from .snippet.client import AsyncSnippetClient, SnippetClient
+from .tasks.client import AsyncTasksClient, TasksClient
 from .tools.client import AsyncToolsClient, ToolsClient
 
 
 class BaseAthena:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
@@ -25,15 +26,17 @@
 
         - environment: AthenaEnvironment. The environment to use for requests from the client. from .environment import AthenaEnvironment
 
                                           Defaults to AthenaEnvironment.DEFAULT
 
         - api_key: str.
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds.
+        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
         - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
     ---
     from athena.client import Athena
 
     client = Athena(
         api_key="YOUR_API_KEY",
@@ -42,30 +45,38 @@
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: AthenaEnvironment = AthenaEnvironment.DEFAULT,
         api_key: str,
-        timeout: typing.Optional[float] = 60,
+        timeout: typing.Optional[float] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None
     ):
+        _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
-            httpx_client=httpx.Client(timeout=timeout) if httpx_client is None else httpx_client,
+            httpx_client=httpx_client
+            if httpx_client is not None
+            else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
+            if follow_redirects is not None
+            else httpx.Client(timeout=_defaulted_timeout),
+            timeout=_defaulted_timeout,
         )
         self.message = MessageClient(client_wrapper=self._client_wrapper)
         self.dataset = DatasetClient(client_wrapper=self._client_wrapper)
         self.snippet = SnippetClient(client_wrapper=self._client_wrapper)
         self.report = ReportClient(client_wrapper=self._client_wrapper)
         self.query = QueryClient(client_wrapper=self._client_wrapper)
         self.search = SearchClient(client_wrapper=self._client_wrapper)
         self.chain = ChainClient(client_wrapper=self._client_wrapper)
         self.tools = ToolsClient(client_wrapper=self._client_wrapper)
+        self.tasks = TasksClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseAthena:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
@@ -73,15 +84,17 @@
 
         - environment: AthenaEnvironment. The environment to use for requests from the client. from .environment import AthenaEnvironment
 
                                           Defaults to AthenaEnvironment.DEFAULT
 
         - api_key: str.
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds.
+        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
         - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
     ---
     from athena.client import AsyncAthena
 
     client = AsyncAthena(
         api_key="YOUR_API_KEY",
@@ -90,30 +103,38 @@
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: AthenaEnvironment = AthenaEnvironment.DEFAULT,
         api_key: str,
-        timeout: typing.Optional[float] = 60,
+        timeout: typing.Optional[float] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
+        _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
-            httpx_client=httpx.AsyncClient(timeout=timeout) if httpx_client is None else httpx_client,
+            httpx_client=httpx_client
+            if httpx_client is not None
+            else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
+            if follow_redirects is not None
+            else httpx.AsyncClient(timeout=_defaulted_timeout),
+            timeout=_defaulted_timeout,
         )
         self.message = AsyncMessageClient(client_wrapper=self._client_wrapper)
         self.dataset = AsyncDatasetClient(client_wrapper=self._client_wrapper)
         self.snippet = AsyncSnippetClient(client_wrapper=self._client_wrapper)
         self.report = AsyncReportClient(client_wrapper=self._client_wrapper)
         self.query = AsyncQueryClient(client_wrapper=self._client_wrapper)
         self.search = AsyncSearchClient(client_wrapper=self._client_wrapper)
         self.chain = AsyncChainClient(client_wrapper=self._client_wrapper)
         self.tools = AsyncToolsClient(client_wrapper=self._client_wrapper)
+        self.tasks = AsyncTasksClient(client_wrapper=self._client_wrapper)
 
 
 def _get_base_url(*, base_url: typing.Optional[str] = None, environment: AthenaEnvironment) -> str:
     if base_url is not None:
         return base_url
     elif environment is not None:
         return environment.value
```

### Comparing `athena_intelligence-0.1.45/src/athena/chain/client.py` & `athena_intelligence-0.1.49/src/athena/chain/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,95 +3,92 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
+from ..types.llm_model import LlmModel
 from ..types.structured_parse_result import StructuredParseResult
-from .types.structured_parse_in_parsing_model import StructuredParseInParsingModel
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ChainClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def structured_parse(
         self,
         *,
         text_input: str,
         custom_type_dict: typing.Dict[str, typing.Any],
-        parsing_model: typing.Optional[StructuredParseInParsingModel] = OMIT,
+        model: LlmModel,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> StructuredParseResult:
         """
         Parameters:
             - text_input: str. The text input to be parsed.
 
             - custom_type_dict: typing.Dict[str, typing.Any]. A dictionary of field names and their default values.
 
-            - parsing_model: typing.Optional[StructuredParseInParsingModel]. The model to be used for parsing.
+            - model: LlmModel.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import StructuredParseInParsingModel
+        from athena import LlmModel
         from athena.client import Athena
 
-        client = Athena(api_key="YOUR_API_KEY", )
-        client.chain.structured_parse(text_input='Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows
-                        by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot,
-                        allowing you to hand over controls to her for autonomous execution with confidence."
-
-                        Give me all of the modes Athena provides.', custom_type_dict={"modes": {}}, parsing_model=StructuredParseInParsingModel.GPT_4_TURBO, )
+        client = Athena(
+            api_key="YOUR_API_KEY",
+        )
+        client.chain.structured_parse(
+            text_input='Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows \n                by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, \n                allowing you to hand over controls to her for autonomous execution with confidence." \n                \n                Give me all of the modes Athena provides.',
+            custom_type_dict={"modes": {}},
+            model=LlmModel.GPT_35_TURBO,
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"text_input": text_input, "custom_type_dict": custom_type_dict}
-        if parsing_model is not OMIT:
-            _request["parsing_model"] = parsing_model
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -100,68 +97,69 @@
         self._client_wrapper = client_wrapper
 
     async def structured_parse(
         self,
         *,
         text_input: str,
         custom_type_dict: typing.Dict[str, typing.Any],
-        parsing_model: typing.Optional[StructuredParseInParsingModel] = OMIT,
+        model: LlmModel,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> StructuredParseResult:
         """
         Parameters:
             - text_input: str. The text input to be parsed.
 
             - custom_type_dict: typing.Dict[str, typing.Any]. A dictionary of field names and their default values.
 
-            - parsing_model: typing.Optional[StructuredParseInParsingModel]. The model to be used for parsing.
+            - model: LlmModel.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from athena import StructuredParseInParsingModel
+        from athena import LlmModel
         from athena.client import AsyncAthena
 
-        client = AsyncAthena(api_key="YOUR_API_KEY", )
-        await client.chain.structured_parse(text_input='Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows
-                        by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot,
-                        allowing you to hand over controls to her for autonomous execution with confidence."
-
-                        Give me all of the modes Athena provides.', custom_type_dict={"modes": {}}, parsing_model=StructuredParseInParsingModel.GPT_4_TURBO, )
+        client = AsyncAthena(
+            api_key="YOUR_API_KEY",
+        )
+        await client.chain.structured_parse(
+            text_input='Athena is an AI-native analytics platform and artificial employee built to accelerate analytics workflows \n                by offering enterprise teams co-pilot and auto-pilot modes. Athena learns your workflow as a co-pilot, \n                allowing you to hand over controls to her for autonomous execution with confidence." \n                \n                Give me all of the modes Athena provides.',
+            custom_type_dict={"modes": {}},
+            model=LlmModel.GPT_35_TURBO,
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"text_input": text_input, "custom_type_dict": custom_type_dict}
-        if parsing_model is not OMIT:
-            _request["parsing_model"] = parsing_model
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/structured-parse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
+            json=jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(_request),
+                **jsonable_encoder({"text_input": text_input, "custom_type_dict": custom_type_dict, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(StructuredParseResult, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/client.py` & `athena_intelligence-0.1.49/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/core/__init__.py` & `athena_intelligence-0.1.49/src/athena/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 from .api_error import ApiError
 from .client_wrapper import AsyncClientWrapper, BaseClientWrapper, SyncClientWrapper
 from .datetime_utils import serialize_datetime
 from .file import File, convert_file_dict_to_httpx_tuples
 from .http_client import AsyncHttpClient, HttpClient
 from .jsonable_encoder import jsonable_encoder
+from .pydantic_utilities import pydantic_v1
 from .remove_none_from_dict import remove_none_from_dict
 from .request_options import RequestOptions
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
     "AsyncHttpClient",
     "BaseClientWrapper",
     "File",
     "HttpClient",
     "RequestOptions",
     "SyncClientWrapper",
     "convert_file_dict_to_httpx_tuples",
     "jsonable_encoder",
+    "pydantic_v1",
     "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `athena_intelligence-0.1.45/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.49/src/athena/core/client_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,34 +4,42 @@
 
 import httpx
 
 from .http_client import AsyncHttpClient, HttpClient
 
 
 class BaseClientWrapper:
-    def __init__(self, *, api_key: str, base_url: str):
+    def __init__(self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None):
         self.api_key = api_key
         self._base_url = base_url
+        self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.45",
+            "X-Fern-SDK-Version": "0.1.49",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
 
+    def get_timeout(self) -> typing.Optional[float]:
+        return self._timeout
+
 
 class SyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, base_url: str, httpx_client: httpx.Client):
-        super().__init__(api_key=api_key, base_url=base_url)
+    def __init__(
+        self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None, httpx_client: httpx.Client
+    ):
+        super().__init__(api_key=api_key, base_url=base_url, timeout=timeout)
         self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, base_url: str, httpx_client: httpx.AsyncClient):
-        super().__init__(api_key=api_key, base_url=base_url)
+    def __init__(
+        self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None, httpx_client: httpx.AsyncClient
+    ):
+        super().__init__(api_key=api_key, base_url=base_url, timeout=timeout)
         self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `athena_intelligence-0.1.45/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.49/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/core/file.py` & `athena_intelligence-0.1.49/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/core/http_client.py` & `athena_intelligence-0.1.49/src/athena/core/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import asyncio
 import email.utils
 import re
 import time
 import typing
+from contextlib import asynccontextmanager, contextmanager
 from functools import wraps
 from random import random
 
 import httpx
 
 INITIAL_RETRY_DELAY_SECONDS = 0.5
 MAX_RETRY_DELAY_SECONDS = 10
@@ -94,16 +95,18 @@
         if _should_retry(response=response):
             if max_retries > retries:
                 time.sleep(_retry_timeout(response=response, retries=retries))
                 return self.request(max_retries=max_retries, retries=retries + 1, *args, **kwargs)
         return response
 
     @wraps(httpx.Client.stream)
+    @contextmanager
     def stream(self, *args: typing.Any, max_retries: int = 0, retries: int = 0, **kwargs: typing.Any) -> typing.Any:
-        return self.httpx_client.stream(*args, **kwargs)
+        with self.httpx_client.stream(*args, **kwargs) as stream:
+            yield stream
 
 
 class AsyncHttpClient:
     def __init__(self, *, httpx_client: httpx.AsyncClient):
         self.httpx_client = httpx_client
 
     # Ensure that the signature of the `request` method is the same as the `httpx.Client.request` method
@@ -114,12 +117,14 @@
         response = await self.httpx_client.request(*args, **kwargs)
         if _should_retry(response=response):
             if max_retries > retries:
                 await asyncio.sleep(_retry_timeout(response=response, retries=retries))
                 return await self.request(max_retries=max_retries, retries=retries + 1, *args, **kwargs)
         return response
 
-    @wraps(httpx.AsyncClient.request)
+    @wraps(httpx.AsyncClient.stream)
+    @asynccontextmanager
     async def stream(
         self, *args: typing.Any, max_retries: int = 0, retries: int = 0, **kwargs: typing.Any
     ) -> typing.Any:
-        return self.httpx_client.stream(*args, **kwargs)
+        async with self.httpx_client.stream(*args, **kwargs) as stream:
+            yield stream
```

### Comparing `athena_intelligence-0.1.45/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.49/src/athena/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic.json.ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, pydantic.BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -61,18 +57,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
@@ -80,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in pydantic.json.ENCODERS_BY_TYPE:
-        return pydantic.json.ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `athena_intelligence-0.1.45/src/athena/core/request_options.py` & `athena_intelligence-0.1.49/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/dataset/client.py` & `athena_intelligence-0.1.49/src/athena/dataset/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.get_datasets_response import GetDatasetsResponse
 from ..types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class DatasetClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(
         self,
@@ -42,16 +38,16 @@
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
         client.dataset.get()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/datasets"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/datasets"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page": page,
                         "page_size": page_size,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -67,22 +63,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetDatasetsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(GetDatasetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -109,16 +107,16 @@
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
         await client.dataset.get()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/datasets"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/datasets"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page": page,
                         "page_size": page_size,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -134,20 +132,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetDatasetsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(GetDatasetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/message/client.py` & `athena_intelligence-0.1.49/src/athena/message/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,24 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.message_out import MessageOut
 from ..types.message_out_dto import MessageOutDto
 from ..types.model import Model
 from ..types.tools import Tools
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class MessageClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -71,16 +67,16 @@
         if tools is not OMIT:
             _request["tools"] = tools
         if conversation_id is not OMIT:
             _request["conversation_id"] = conversation_id
         if conversation_name is not OMIT:
             _request["conversation_name"] = conversation_name
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/message"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/message"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -92,22 +88,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageOut, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(MessageOut, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> MessageOutDto:
@@ -123,37 +121,41 @@
             api_key="YOUR_API_KEY",
         )
         client.message.get(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v0/message/{jsonable_encoder(id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v0/message/{jsonable_encoder(id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageOutDto, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(MessageOutDto, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -203,16 +205,16 @@
         if tools is not OMIT:
             _request["tools"] = tools
         if conversation_id is not OMIT:
             _request["conversation_id"] = conversation_id
         if conversation_name is not OMIT:
             _request["conversation_name"] = conversation_name
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/message"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/message"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -224,22 +226,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageOut, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(MessageOut, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> MessageOutDto:
@@ -255,35 +259,39 @@
             api_key="YOUR_API_KEY",
         )
         await client.message.get(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v0/message/{jsonable_encoder(id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v0/message/{jsonable_encoder(id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageOutDto, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(MessageOutDto, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/polling_message_client.py` & `athena_intelligence-0.1.49/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/query/client.py` & `athena_intelligence-0.1.49/src/athena/query/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.sql_results import SqlResults
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class QueryClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -44,16 +40,16 @@
         )
         client.query.execute(
             sql_command="sql_command",
             database_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
@@ -65,22 +61,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SqlResults, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(SqlResults, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -106,16 +104,16 @@
         )
         await client.query.execute(
             sql_command="sql_command",
             database_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/execute-sql"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder({"sql_command": sql_command, "database_id": database_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"sql_command": sql_command, "database_id": database_id}),
@@ -127,20 +125,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SqlResults, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(SqlResults, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/report/client.py` & `athena_intelligence-0.1.49/src/athena/report/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.report import Report
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ReportClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -50,16 +46,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
         if workspace_access is not OMIT:
             _request["workspace_access"] = workspace_access
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -71,22 +67,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Report, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(Report, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -118,16 +116,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
         if workspace_access is not OMIT:
             _request["workspace_access"] = workspace_access
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/report"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -139,20 +137,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Report, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(Report, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/search/client.py` & `athena_intelligence-0.1.49/src/athena/search/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.url_result import UrlResult
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class SearchClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -68,16 +64,16 @@
         if country_code is not OMIT:
             _request["country_code"] = country_code
         if country_restrict is not OMIT:
             _request["country_restrict"] = country_restrict
         if site is not OMIT:
             _request["site"] = site
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/search/get-urls"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/search/get-urls"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -89,22 +85,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UrlResult, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(UrlResult, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -154,16 +152,16 @@
         if country_code is not OMIT:
             _request["country_code"] = country_code
         if country_restrict is not OMIT:
             _request["country_restrict"] = country_restrict
         if site is not OMIT:
             _request["site"] = site
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/search/get-urls"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/search/get-urls"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -175,20 +173,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UrlResult, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(UrlResult, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/snippet/client.py` & `athena_intelligence-0.1.49/src/athena/snippet/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.get_snippets_response import GetSnippetsResponse
 from ..types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class SnippetClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(
         self,
@@ -42,16 +38,16 @@
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
         client.snippet.get()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page": page,
                         "page_size": page_size,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -67,22 +63,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -109,16 +107,16 @@
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
         await client.snippet.get()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/snippets"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "page": page,
                         "page_size": page_size,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -134,20 +132,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(GetSnippetsResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/tools/client.py` & `athena_intelligence-0.1.49/src/athena/tools/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from ..types.firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from ..types.http_validation_error import HttpValidationError
+from ..types.langchain_documents_request_out import LangchainDocumentsRequestOut
 from ..types.tool_models import ToolModels
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ToolsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -52,16 +49,90 @@
             url="https://athenaintelligence.ai",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"url": url}
         if params is not OMIT:
             _request["params"] = params
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/firecrawl/scrape-url"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/firecrawl/scrape-url"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic_v1.parse_obj_as(FirecrawlScrapeUrlDataReponseDto, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def langchain_documents(
+        self,
+        *,
+        document_id: str,
+        pagination_limit: typing.Optional[int] = OMIT,
+        pagination_offset: typing.Optional[int] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> LangchainDocumentsRequestOut:
+        """
+        Parameters:
+            - document_id: str.
+
+            - pagination_limit: typing.Optional[int].
+
+            - pagination_offset: typing.Optional[int].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from athena.client import Athena
+
+        client = Athena(
+            api_key="YOUR_API_KEY",
+        )
+        client.tools.langchain_documents(
+            document_id="doc_9249292-d118-42d3-95b4-00eccfe0754f",
+            pagination_limit=250,
+            pagination_offset=0,
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"document_id": document_id}
+        if pagination_limit is not OMIT:
+            _request["pagination_limit"] = pagination_limit
+        if pagination_offset is not OMIT:
+            _request["pagination_offset"] = pagination_offset
+        _response = self._client_wrapper.httpx_client.request(
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/file/langchain-documents"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -73,22 +144,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(FirecrawlScrapeUrlDataReponseDto, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(LangchainDocumentsRequestOut, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def tool_first_workflow(
@@ -127,16 +200,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {"tool_name": tool_name, "content": content}
         if model is not OMIT:
             _request["model"] = model
         if tool_kwargs is not OMIT:
             _request["tool_kwargs"] = tool_kwargs
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/first-agent"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/first-agent"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -148,22 +221,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExcecuteToolFirstWorkflowOut, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ExcecuteToolFirstWorkflowOut, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -195,16 +270,90 @@
             url="https://athenaintelligence.ai",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"url": url}
         if params is not OMIT:
             _request["params"] = params
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/firecrawl/scrape-url"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/firecrawl/scrape-url"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic_v1.parse_obj_as(FirecrawlScrapeUrlDataReponseDto, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def langchain_documents(
+        self,
+        *,
+        document_id: str,
+        pagination_limit: typing.Optional[int] = OMIT,
+        pagination_offset: typing.Optional[int] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> LangchainDocumentsRequestOut:
+        """
+        Parameters:
+            - document_id: str.
+
+            - pagination_limit: typing.Optional[int].
+
+            - pagination_offset: typing.Optional[int].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from athena.client import AsyncAthena
+
+        client = AsyncAthena(
+            api_key="YOUR_API_KEY",
+        )
+        await client.tools.langchain_documents(
+            document_id="doc_9249292-d118-42d3-95b4-00eccfe0754f",
+            pagination_limit=250,
+            pagination_offset=0,
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"document_id": document_id}
+        if pagination_limit is not OMIT:
+            _request["pagination_limit"] = pagination_limit
+        if pagination_offset is not OMIT:
+            _request["pagination_offset"] = pagination_offset
+        _response = await self._client_wrapper.httpx_client.request(
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/file/langchain-documents"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -216,22 +365,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(FirecrawlScrapeUrlDataReponseDto, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(LangchainDocumentsRequestOut, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def tool_first_workflow(
@@ -270,16 +421,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {"tool_name": tool_name, "content": content}
         if model is not OMIT:
             _request["model"] = model
         if tool_kwargs is not OMIT:
             _request["tool_kwargs"] = tool_kwargs
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/first-agent"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/first-agent"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -291,20 +442,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExcecuteToolFirstWorkflowOut, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ExcecuteToolFirstWorkflowOut, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/__init__.py` & `athena_intelligence-0.1.49/src/athena/types/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .dataset import Dataset
+from .document import Document
 from .excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from .firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from .firecrawl_scrape_url_metadata import FirecrawlScrapeUrlMetadata
 from .get_datasets_response import GetDatasetsResponse
 from .get_snippets_response import GetSnippetsResponse
 from .http_validation_error import HttpValidationError
+from .langchain_documents_request_out import LangchainDocumentsRequestOut
+from .llm_model import LlmModel
 from .message_out import MessageOut
 from .message_out_dto import MessageOutDto
 from .model import Model
+from .plan_execute_out import PlanExecuteOut
 from .report import Report
 from .snippet import Snippet
 from .sql_results import SqlResults
 from .status_enum import StatusEnum
 from .structured_parse_result import StructuredParseResult
 from .tool_models import ToolModels
 from .tools import Tools
 from .url_result import UrlResult
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "Dataset",
+    "Document",
     "ExcecuteToolFirstWorkflowOut",
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
+    "LangchainDocumentsRequestOut",
+    "LlmModel",
     "MessageOut",
     "MessageOutDto",
     "Model",
+    "PlanExecuteOut",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "StructuredParseResult",
     "ToolModels",
     "Tools",
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/dataset.py` & `athena_intelligence-0.1.49/src/athena/types/report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Dataset(pydantic.BaseModel):
+class Report(pydantic_v1.BaseModel):
     id: str
     name: typing.Optional[str] = None
-    description: typing.Optional[str] = None
-    database_id: int
-    schema_details: typing.Optional[str] = None
+    workspace_access: bool
+    created_at: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.49/src/athena/types/get_datasets_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .dataset import Dataset
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ExcecuteToolFirstWorkflowOut(pydantic.BaseModel):
-    output_message: str
+class GetDatasetsResponse(pydantic_v1.BaseModel):
+    datasets: typing.List[Dataset]
+    total: int
+    page: int
+    page_size: int
+    pages: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.49/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .firecrawl_scrape_url_metadata import FirecrawlScrapeUrlMetadata
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FirecrawlScrapeUrlDataReponseDto(pydantic.BaseModel):
-    content: str
-    markdown: str
-    metadata: FirecrawlScrapeUrlMetadata
+class ExcecuteToolFirstWorkflowOut(pydantic_v1.BaseModel):
+    output_message: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.49/src/athena/types/message_out_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .status_enum import StatusEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FirecrawlScrapeUrlMetadata(pydantic.BaseModel):
-    title: typing.Optional[str] = None
-    description: typing.Optional[str] = None
-    language: typing.Optional[str] = None
-    source_url: typing.Optional[str] = pydantic.Field(alias="sourceURL", default=None)
+class MessageOutDto(pydantic_v1.BaseModel):
+    id: str
+    conversation_id: str
+    logs: typing.Optional[str] = None
+    content: typing.Optional[str] = None
+    created_at: str
+    status: StatusEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.49/src/athena/types/langchain_documents_request_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .dataset import Dataset
+from ..core.pydantic_utilities import pydantic_v1
+from .document import Document
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetDatasetsResponse(pydantic.BaseModel):
-    datasets: typing.List[Dataset]
-    total: int
-    page: int
-    page_size: int
-    pages: int
+class LangchainDocumentsRequestOut(pydantic_v1.BaseModel):
+    documents: typing.List[Document]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.49/src/athena/types/get_snippets_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .snippet import Snippet
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetSnippetsResponse(pydantic.BaseModel):
+class GetSnippetsResponse(pydantic_v1.BaseModel):
     snippets: typing.List[Snippet]
     total: int
     page: int
     page_size: int
     pages: int
 
     def json(self, **kwargs: typing.Any) -> str:
@@ -26,8 +22,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.49/src/athena/types/http_validation_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .validation_error import ValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class HttpValidationError(pydantic.BaseModel):
+class HttpValidationError(pydantic_v1.BaseModel):
     detail: typing.Optional[typing.List[ValidationError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.49/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .status_enum import StatusEnum
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class MessageOutDto(pydantic.BaseModel):
-    id: str
-    conversation_id: str
-    logs: typing.Optional[str] = None
-    content: typing.Optional[str] = None
-    created_at: str
-    status: StatusEnum
+class FirecrawlScrapeUrlMetadata(pydantic_v1.BaseModel):
+    title: typing.Optional[str] = None
+    description: typing.Optional[str] = None
+    language: typing.Optional[str] = None
+    source_url: typing.Optional[str] = pydantic_v1.Field(alias="sourceURL", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/model.py` & `athena_intelligence-0.1.49/src/athena/types/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     GPT_35_TURBO = "gpt-3.5-turbo"
     GPT_4_TURBO = "gpt-4-turbo"
     GPT_4_TURBO_PREVIEW = "gpt-4-turbo-preview"
     GPT_4 = "gpt-4"
     MIXTRAL_SMALL_8_X_7_B_0211 = "mixtral-small-8x7b-0211"
     MISTRAL_LARGE_0224 = "mistral-large-0224"
     MIXTRAL_8_X_22_B_INSTRUCT = "mixtral-8x22b-instruct"
-    LLAMA_V_270_B_CHAT = "llama-v2-70b-chat"
     LLAMA_V_370_B_INSTRUCT = "llama-v3-70b-instruct"
     LLAMA_V_38_B_INSTRUCT = "llama-v3-8b-instruct"
     CLAUDE_3_OPUS_20240229 = "claude-3-opus-20240229"
     CLAUDE_3_SONNET_20240229 = "claude-3-sonnet-20240229"
     CLAUDE_3_HAIKU_20240307 = "claude-3-haiku-20240307"
     GOOGLE_GEMINI_10_PRO_LATEST = "google-gemini-1.0-pro-latest"
     DATABRICKS_DBRX = "databricks-dbrx"
@@ -32,15 +31,14 @@
         gpt_35_turbo: typing.Callable[[], T_Result],
         gpt_4_turbo: typing.Callable[[], T_Result],
         gpt_4_turbo_preview: typing.Callable[[], T_Result],
         gpt_4: typing.Callable[[], T_Result],
         mixtral_small_8_x_7_b_0211: typing.Callable[[], T_Result],
         mistral_large_0224: typing.Callable[[], T_Result],
         mixtral_8_x_22_b_instruct: typing.Callable[[], T_Result],
-        llama_v_270_b_chat: typing.Callable[[], T_Result],
         llama_v_370_b_instruct: typing.Callable[[], T_Result],
         llama_v_38_b_instruct: typing.Callable[[], T_Result],
         claude_3_opus_20240229: typing.Callable[[], T_Result],
         claude_3_sonnet_20240229: typing.Callable[[], T_Result],
         claude_3_haiku_20240307: typing.Callable[[], T_Result],
         google_gemini_10_pro_latest: typing.Callable[[], T_Result],
         databricks_dbrx: typing.Callable[[], T_Result],
@@ -55,16 +53,14 @@
             return gpt_4()
         if self is Model.MIXTRAL_SMALL_8_X_7_B_0211:
             return mixtral_small_8_x_7_b_0211()
         if self is Model.MISTRAL_LARGE_0224:
             return mistral_large_0224()
         if self is Model.MIXTRAL_8_X_22_B_INSTRUCT:
             return mixtral_8_x_22_b_instruct()
-        if self is Model.LLAMA_V_270_B_CHAT:
-            return llama_v_270_b_chat()
         if self is Model.LLAMA_V_370_B_INSTRUCT:
             return llama_v_370_b_instruct()
         if self is Model.LLAMA_V_38_B_INSTRUCT:
             return llama_v_38_b_instruct()
         if self is Model.CLAUDE_3_OPUS_20240229:
             return claude_3_opus_20240229()
         if self is Model.CLAUDE_3_SONNET_20240229:
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/report.py` & `athena_intelligence-0.1.49/src/athena/types/validation_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from .validation_error_loc_item import ValidationErrorLocItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Report(pydantic.BaseModel):
-    id: str
-    name: typing.Optional[str] = None
-    workspace_access: bool
-    created_at: str
+class ValidationError(pydantic_v1.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/snippet.py` & `athena_intelligence-0.1.49/src/athena/types/snippet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Snippet(pydantic.BaseModel):
+class Snippet(pydantic_v1.BaseModel):
     id: str
     title: typing.Optional[str] = None
     description: typing.Optional[str] = None
     content: typing.Optional[str] = None
     language: typing.Optional[str] = None
     created_at: str
     dependencies: typing.Optional[typing.Dict[str, typing.List[str]]] = None
@@ -27,8 +23,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/sql_results.py` & `athena_intelligence-0.1.49/src/athena/types/message_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SqlResults(pydantic.BaseModel):
-    result: typing.Optional[typing.Any] = None
+class MessageOut(pydantic_v1.BaseModel):
+    id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/status_enum.py` & `athena_intelligence-0.1.49/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.49/src/athena/types/document.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class Document(pydantic_v1.BaseModel):
+    """
+    Class for storing a piece of text and associated metadata.
+    """
 
-class StructuredParseResult(pydantic.BaseModel):
-    result: typing.Dict[str, typing.Any]
+    page_content: str
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
+    type: typing.Optional[typing.Literal["Document"]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/tool_models.py` & `athena_intelligence-0.1.49/src/athena/types/tool_models.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/types/tools.py` & `athena_intelligence-0.1.49/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.45/src/athena/types/url_result.py` & `athena_intelligence-0.1.49/src/athena/types/url_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UrlResult(pydantic.BaseModel):
+class UrlResult(pydantic_v1.BaseModel):
     result: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/src/athena/types/validation_error.py` & `athena_intelligence-0.1.49/src/athena/types/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .validation_error_loc_item import ValidationErrorLocItem
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ValidationError(pydantic.BaseModel):
-    loc: typing.List[ValidationErrorLocItem]
-    msg: str
-    type: str
+class Dataset(pydantic_v1.BaseModel):
+    id: str
+    name: typing.Optional[str] = None
+    description: typing.Optional[str] = None
+    database_id: int
+    schema_details: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `athena_intelligence-0.1.45/PKG-INFO` & `athena_intelligence-0.1.49/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.45
+Version: 0.1.49
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

